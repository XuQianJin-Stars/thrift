#
# Licensed to the Apache Software Foundation (ASF) under one
# or more contributor license agreements. See the NOTICE file
# distributed with this work for additional information
# regarding copyright ownership. The ASF licenses this file
# to you under the Apache License, Version 2.0 (the
# "License"); you may not use this file except in compliance
# with the License. You may obtain a copy of the License at
#
#   http://www.apache.org/licenses/LICENSE-2.0
#
# Unless required by applicable law or agreed to in writing,
# software distributed under the License is distributed on an
# "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
# KIND, either express or implied. See the License for the
# specific language governing permissions and limitations
# under the License.
#

SUBDIRS = . 

all-local:
	$(DOTNETCORE) build

clean-local:
	$(RM) Interfaces.dll
	$(RM) -r Client/bin
	$(RM) -r Client/obj
	$(RM) -r Server/bin
	$(RM) -r Server/obj
	$(RM) -r Interfaces/bin
	$(RM) -r Interfaces/obj

dist-hook:
	$(RM) $(distdir)/Interfaces.dll
	$(RM) -r $(distdir)/Client/bin
	$(RM) -r $(distdir)/Client/obj
	$(RM) -r $(distdir)/Server/bin
	$(RM) -r $(distdir)/Server/obj
	$(RM) -r $(distdir)/Interfaces/bin
	$(RM) -r $(distdir)/Interfaces/obj

EXTRA_DIST = \
	Client \
	Interfaces \
	README.md \
	Server \
	Tutorial.sln \
	build.cmd \
	build.sh
			 

#
# Copyright 2008 Google Inc.
#
# Licensed under the Apache License, Version 2.0 (the "License");
# you may not use this file except in compliance with the License.
# You may obtain a copy of the License at
#
#      http://www.apache.org/licenses/LICENSE-2.0
#
# Unless required by applicable law or agreed to in writing, software
# distributed under the License is distributed on an "AS IS" BASIS,
# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
# See the License for the specific language governing permissions and
# limitations under the License.

EXTRA_DIST = CMakeLists.txt

if GGL_BUILD_QT_EDIT_ELEMENT

INCLUDES		= -I$(top_builddir) \
			  -I$(top_srcdir)

noinst_HEADERS		= qt_edit_element.h

extension_LTLIBRARIES	= qt-edit-element.la
extensiondir		= $(GGL_MODULE_DIR)

qt_edit_element_la_SOURCES = \
			  qt_edit_element.cc

qt_edit_element_la_CXXFLAGS = \
			  $(DEFAULT_COMPILE_FLAGS)

qt_edit_element_la_CPPFLAGS = \
			  $(QT4_CFLAGS) \
			  $(PREDEFINED_MACROS)

qt_edit_element_la_LIBADD = \
			  $(QT4_LIBS) \
			  $(top_builddir)/ggadget/libggadget@GGL_EPOCH@.la \
			  $(top_builddir)/ggadget/qt/libggadget-qt@GGL_EPOCH@.la

qt_edit_element_la_LDFLAGS = \
			  -no-undefined \
			  -avoid-version \
			  -module
endif

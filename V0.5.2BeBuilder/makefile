## BeOS Generic Makefile v2.0 ##

## Fill in this file to specify the project being created, and the referenced
## makefile-engine will do all of the hard work for you.  This handles both
## Intel and PowerPC builds of the BeOS.

## Application Specific Settings ---------------------------------------------

# specify the name of the binary
NAME= BeBuilder

# specify the type of binary
#	APP:	Application
#	SHARED:	Shared library or add-on
#	STATIC:	Static library archive
#	DRIVER: Kernel Driver
TYPE= APP

#	specify the source files to use
#	full paths or paths relative to the makefile can be included
# 	all files, regardless of directory, will have their object
#	files created in the common object directory.
#	Note that this means this makefile will not work correctly
#	if two source files with the same name (source.c or source.cpp)
#	are included from different directories.  Also note that spaces
#	in folder names do not work well with this makefile.
SRCS= 	BeBuilder.cpp \
		AddOnManager.cpp \
		CodeGenerator.cpp \
		Component.cpp \
		ComponentKindaView.cpp \
		ComponentList.cpp \
		Property.cpp \
		PropertyList.cpp \
		../Kernel/FileReader.cpp \
		../Kernel/FileWriter.cpp \
		../Kernel/FileRW.cpp \
		../Kernel/BGeneralWindow.cpp \
		../Kernel/BGeneralWindowOption.cpp \
		../Kernel/BOption.cpp \
		../Kernel/GeneralOutlineList.cpp \
		../Kernel/JerFiles.cpp \
		../Kernel/StringList.cpp \
		BuilderWindow.cpp \
		BuilderMenu.cpp \
		../Kernel/Global.cpp \
		../Kernel/GeneralException.cpp \
		../Kernel/Object.cpp \
		../Kernel/OpenDir.cpp \
		BuilderView.cpp \
		ToolView.cpp \
		ToolWindow.cpp \
		ComponentItem.cpp \
		Parser.cpp \
		CodeFile.cpp \
		CodeLine.cpp \
		ToolBar.cpp \
		ToolBarView.cpp \
		BeBuilderOption.cpp \
		EditorOption.cpp \
		WindowOption.cpp \
		ViewOption.cpp \
		./PropertyEditor/PropertyEditorView.cpp \
		./PropertyEditor/PropertyEditorWindow.cpp \
		./PropertyEditor/MenuPropertyEditorChoice.cpp \
		./PropertyEditor/PropertyEditorChoice.cpp \
		./PropertyEditor/PropertyEditorChoiceView.cpp \
		./PropertyEditor/PropertyEditorMultiChoice.cpp \
		./PropertyEditor/PropertyEditorMultiChoiceView.cpp \
		./PropertyEditor/PropertyEditorStandardView.cpp \
		./PropertyEditor/PropertyEditorStandard.cpp \
		./Component/WindowComponent.cpp \
		./Component/ViewComponent.cpp \
		./Component/ButtonComponent.cpp \
		./Component/ProjectComponent.cpp \
		./CodeGenerator/WindowCodeGenerator.cpp \
		./CodeGenerator/ViewCodeGenerator.cpp \
		./CodeGenerator/ProjectCodeGenerator.cpp \
		./CodeGenerator/ButtonCodeGenerator.cpp \
		./Component/TextControlComponent.cpp \
		./CodeGenerator/TextControlCodeGenerator.cpp \
		./Component/CheckBoxComponent.cpp \
		./CodeGenerator/CheckBoxCodeGenerator.cpp \
		./Component/RadioButtonComponent.cpp \
		./CodeGenerator/RadioButtonCodeGenerator.cpp \
		./Component/MenuComponent.cpp \
		./CodeGenerator/MenuCodeGenerator.cpp \
		./CodeGenerator/MenuBarCodeGenerator.cpp \
		./Component/MenuBarComponent.cpp \
		./CodeGenerator/MenuItemCodeGenerator.cpp \
		./CodeGenerator/MenuSeparatorCodeGenerator.cpp \
		./Component/MenuItemComponent.cpp \
		./Component/MenuSeparatorComponent.cpp \
		./Component/MenuFieldComponent.cpp \
		./CodeGenerator/MenuFieldCodeGenerator.cpp \
		./Component/BoxComponent.cpp \
		./CodeGenerator/BoxCodeGenerator.cpp \
		./Component/SliderComponent.cpp \
		./CodeGenerator/SliderCodeGenerator.cpp 

		
#	specify the resource files to use
#	full path or a relative path to the resource file can be used.
RSRCS= bebuilder.rsrc \
		./Resources/ViewResource.rsrc \
		./Resources/WindowResource.rsrc

#	specify additional libraries to link against
#	there are two acceptable forms of library specifications
#	-	if your library follows the naming pattern of:
#		libXXX.so or libXXX.a you can simply specify XXX
#		library: libbe.so entry: be
#		
#	- 	if your library does not follow the standard library
#		naming scheme you need to specify the path to the library
#		and it's name
#		library: my_lib.a entry: my_lib.a or path/my_lib.a
LIBS=	be \
		translation \
		stdc++.r4 \
		tracker \
		root
		
#	specify additional paths to directories following the standard
#	libXXX.so or libXXX.a naming scheme.  You can specify full paths
#	or paths relative to the makefile.  The paths included may not
#	be recursive, so include all of the paths where libraries can
#	be found.  Directories where source files are found are
#	automatically included.
LIBPATHS= 

#	additional paths to look for system headers
#	thes use the form: #include <header>
#	source file directories are NOT auto-included here
SYSTEM_INCLUDE_PATHS = 

#	additional paths to look for local headers
#	thes use the form: #include "header"
#	source file directories are automatically included
LOCAL_INCLUDE_PATHS = 
#../Kernel \
#					./PropertyEditor \
#					./CodeGenerator \
#					./Component		

#	specify the level of optimization that you desire
#	NONE, SOME, FULL
OPTIMIZE= NONE

#	specify any preprocessor symbols to be defined.  The symbols
#	will be set to a value of 1.  For example specify DEBUG if you want
#	DEBUG=1 to be set when compiling.
DEFINES= 

#	specify special warning levels
#	if unspecified default warnings will be used
#	NONE = supress all warnings
#	ALL = enable all warnings
WARNINGS = ALL

#	specify whether image symbols will be created
#	so that stack crawls in the debugger are meaningful
#	if TRUE symbols will be created
SYMBOLS = 

#	specify debug settings
#	if TRUE will allow application to be run from
#	a source-level debugger
DEBUGGER = 

#	specify additional compiler flags for all files
COMPILER_FLAGS =

#	specify additional linker flags
LINKER_FLAGS =


## include the makefile-engine
DEVEL_DIRECTORY := \
        $(shell findpaths -r "makefile_engine" B_FIND_PATH_DEVELOP_DIRECTORY)

include $(DEVEL_DIRECTORY)/etc/makefile-engine


KEY_FILE=$(top_srcdir)/mono-addins.snk
ASSEMBLY_COMPILER_COMMAND = gmcs
ASSEMBLY_COMPILER_FLAGS =  -keyfile:$(KEY_FILE) -noconfig -codepage:utf8 -warn:4 -debug -d:DEBUG
ASSEMBLY = ../bin/Mono.Addins.dll
ASSEMBLY_NAME=Mono.Addins
COMPILE_TARGET = exe
PC_FILES_IN = mono-addins.pc.in
PROJECT_REFERENCES = 
BUILD_DIR = ../bin

	
all: $(ASSEMBLY)

FILES =  \
	AssemblyInfo.cs \
	Mono.Addins.Database/AddinDatabase.cs \
	Mono.Addins.Database/AddinFileSystemExtension.cs \
	Mono.Addins.Database/AddinHostIndex.cs \
	Mono.Addins.Database/AddinScanFolderInfo.cs \
	Mono.Addins.Database/AddinScanner.cs \
	Mono.Addins.Database/AddinScanResult.cs \
	Mono.Addins.Database/AddinUpdateData.cs \
	Mono.Addins.Database/DatabaseConfiguration.cs \
	Mono.Addins.Database/DefaultAssemblyReflector.cs \
	Mono.Addins.Database/FileDatabase.cs \
	Mono.Addins.Database/IAssemblyReflector.cs \
	Mono.Addins.Database/ISetupHandler.cs \
	Mono.Addins.Database/ProcessProgressStatus.cs \
	Mono.Addins.Database/SetupDomain.cs \
	Mono.Addins.Database/SetupLocal.cs \
	Mono.Addins.Database/SetupProcess.cs \
	Mono.Addins.Database/Util.cs \
	Mono.Addins.Description/AddinDependency.cs \
	Mono.Addins.Description/AddinDescription.cs \
	Mono.Addins.Description/AddinFlags.cs \
	Mono.Addins.Description/AddinProperty.cs \
	Mono.Addins.Description/AddinPropertyCollection.cs \
	Mono.Addins.Description/AssemblyDependency.cs \
	Mono.Addins.Description/ConditionTypeDescription.cs \
	Mono.Addins.Description/ConditionTypeDescriptionCollection.cs \
	Mono.Addins.Description/Dependency.cs \
	Mono.Addins.Description/DependencyCollection.cs \
	Mono.Addins.Description/Extension.cs \
	Mono.Addins.Description/ExtensionCollection.cs \
	Mono.Addins.Description/ExtensionNodeDescription.cs \
	Mono.Addins.Description/ExtensionNodeDescriptionCollection.cs \
	Mono.Addins.Description/ExtensionNodeSet.cs \
	Mono.Addins.Description/ExtensionNodeSetCollection.cs \
	Mono.Addins.Description/ExtensionNodeType.cs \
	Mono.Addins.Description/ExtensionNodeTypeCollection.cs \
	Mono.Addins.Description/ExtensionPoint.cs \
	Mono.Addins.Description/ExtensionPointCollection.cs \
	Mono.Addins.Description/ModuleDescription.cs \
	Mono.Addins.Description/ModuleDescriptionCollection.cs \
	Mono.Addins.Description/NativeDependency.cs \
	Mono.Addins.Description/NodeTypeAttribute.cs \
	Mono.Addins.Description/NodeTypeAttributeCollection.cs \
	Mono.Addins.Description/ObjectDescription.cs \
	Mono.Addins.Description/ObjectDescriptionCollection.cs \
	Mono.Addins.Localization/GettextDomain.cs \
	Mono.Addins.Localization/GettextLocalizer.cs \
	Mono.Addins.Localization/IAddinLocalizer.cs \
	Mono.Addins.Localization/IAddinLocalizerFactory.cs \
	Mono.Addins.Localization/IPluralAddinLocalizer.cs \
	Mono.Addins.Localization/NullLocalizer.cs \
	Mono.Addins.Localization/StringResourceLocalizer.cs \
	Mono.Addins.Localization/StringTableLocalizer.cs \
	Mono.Addins.Serialization/BinaryXmlReader.cs \
	Mono.Addins.Serialization/BinaryXmlTypeMap.cs \
	Mono.Addins.Serialization/BinaryXmlWriter.cs \
	Mono.Addins.Serialization/IBinaryXmlElement.cs \
	Mono.Addins/Addin.cs \
	Mono.Addins/AddinAttribute.cs \
	Mono.Addins/AddinAuthorAttribute.cs \
	Mono.Addins/AddinDependencyAttribute.cs \
	Mono.Addins/AddinDescriptionAttribute.cs \
	Mono.Addins/AddinEngine.cs \
	Mono.Addins/AddinErrorEventArgs.cs \
	Mono.Addins/AddinEventArgs.cs \
	Mono.Addins/AddinInfo.cs \
	Mono.Addins/AddinLocalizer.cs \
	Mono.Addins/AddinLocalizerGettextAttribute.cs \
	Mono.Addins/AddinManager.cs \
	Mono.Addins/AddinModuleAttribute.cs \
	Mono.Addins/AddinNameAttribute.cs \
	Mono.Addins/AddinPropertyAttribute.cs \
	Mono.Addins/AddinRegistry.cs \
	Mono.Addins/AddinRootAttribute.cs \
	Mono.Addins/ConditionType.cs \
	Mono.Addins/ConsoleProgressStatus.cs \
	Mono.Addins/ContentType.cs \
	Mono.Addins/CustomExtensionAttribute.cs \
	Mono.Addins/ExtensionAttribute.cs \
	Mono.Addins/ExtensionAttributeAttribute.cs \
	Mono.Addins/ExtensionContext.cs \
	Mono.Addins/ExtensionNode.cs \
	Mono.Addins/ExtensionNodeAttribute.cs \
	Mono.Addins/ExtensionNodeChildAttribute.cs \
	Mono.Addins/ExtensionNodeList.cs \
	Mono.Addins/ExtensionPointAttribute.cs \
	Mono.Addins/ExtensionTree.cs \
	Mono.Addins/GettextCatalog.cs \
	Mono.Addins/IAddinInstaller.cs \
	Mono.Addins/ImportAddinAssemblyAttribute.cs \
	Mono.Addins/ImportAddinFileAttribute.cs \
	Mono.Addins/InstanceExtensionNode.cs \
	Mono.Addins/IProgressStatus.cs \
	Mono.Addins/MissingDependencyException.cs \
	Mono.Addins/NodeAttributeAttribute.cs \
	Mono.Addins/NodeElement.cs \
	Mono.Addins/RuntimeAddin.cs \
	Mono.Addins/TreeNode.cs \
	Mono.Addins/TreeNodeCollection.cs \
	Mono.Addins/TypeExtensionNode.cs \
	Mono.Addins/TypeExtensionPointAttribute.cs 

DATA_FILES = 

RESOURCES = 

EXTRAS = 

REFERENCES =  \
	-r:System \
	-r:System.Core \
	-r:System.Xml

DLL_REFERENCES = 

$(ASSEMBLY).mdb: $(ASSEMBLY)

$(ASSEMBLY): $(build_sources) $(build_resources) $(build_datafiles) $(POLICY_ASSEMBLIES)
	mkdir -p $(dir $(ASSEMBLY))		
	$(ASSEMBLY_COMPILER_COMMAND) $(ASSEMBLY_COMPILER_FLAGS) -out:$@ -target:$(COMPILE_TARGET) $(build_sources) $(build_resources_embed) $(build_references_ref)

install-data-local: gac-install

uninstall-local: gac-uninstall

include $(top_srcdir)/Makefile.include

CLEANFILES += $(POLICY_ASSEMBLIES) $(POLICY_CONFIGS)

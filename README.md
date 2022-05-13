# pipelinetools
 Azure Pipeline Tools in template format using self hosted agents

There is a Library names "Build Variables" with the following defaults (modify as needed and override as needed)

ArtifactName			drop
Build_Server			myserver.mydomain.prv
Builds_base_path		s:\Builds
Builds_release_path		S:\Release_Files
company					YourCompany
CompileJobPool			AgentPool
DefaultEnvironment		SQA
CertificatePW			*****************  (Secure)
emailCCList
eMailConditionConfig	Always
emailtoList
FlattenArtifactContents	false
GatherDirectory			.\
InnoExe					C:\dev\tools\Inno Setup 5\iscc.exe
NugetPackagesToPack		**/*.nuspec
NugetPackagesToPush		$(build.artifactstagingdirectory)/**/*.nupkg;**/*.nupkg;*.nupkg;!**/packages/**/*.nupkg;!$(build.artifactstagingdirectory)/**/*.symbols.nupkg;!**/*.symbols.nupkg
nugetVersion			6.0.0
PublishDirectiveToShare	true
PublishFilesContents	**
PublishJobPool			DomainPool
PublishToShare			true
RunSettingFile
UniversalSourceFolder	$(Build.ArtifactStagingDirectory)
VersionINIFile			InstallDirective.ini
VsBuildVersion			16.0
VsTestVersion			16.0
VSTSToken				*****************  (Secure)
Windows SDK				10.0.17763.0
year					2022
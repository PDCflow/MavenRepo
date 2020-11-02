To add a jar to the repo.
execute the following from the MavenRepo project directory.
{GrougId} - Group Id you want to use in the pom.xml
{ArtifactId} - Artifact id you want to use in the pom.xml
{Version} - Version # you want to use in the pom.xml
{File} - full path / filename of the jar file being added to the repo

mvn install:install-file -DgroupId={GroupId} -DartifactId={ArtifactId} -Dversion={Version} -Dfile={File} -Dpackaging=jar -DgeneratePom=true -DlocalRepositoryPath=.  -DcreateChecksum=true
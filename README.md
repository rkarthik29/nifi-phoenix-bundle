# nifi-phoenix-bundle

git clone this in you nifi/nifi-nar-bundle folder.

do mvn clean package , this will use the default versions for hbase,nifi and phoenix mentioned in the root pom.xml.

To build against a specific version of nifi,hbase or phoenix , build as

mvn clean package -Dnifi.version=<version> -Dhbase.version=<version> -Dphoenix.version=<>

cd nifi-phoenix-bundle/nifi-phoenix-service-nar/target

copy .nar and deploy to nifi/lib.

Right now it only does thick, though i have an option to add for thin if needed.

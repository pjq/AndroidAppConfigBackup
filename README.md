AndroidAppConfigBackup
======================


Description
=====================
I want to make a common lib to backup/recovery the Android App data.

The data path mostly is:/data/data/app.packagename/.

Backup the data to the sdcard

 
Feature in mind
=====================
1.Create a lib that will be used in another Android project.

2.The backup data will be stored/parsed with XML format.

3.Support file encryption.

4.Support file compress with zip format.


Backup config XML
=====================

doc/config_backup_example.xml

<code>
<root>
	<app_info>
		<app_name> your app name </app_name>
		<package_name>me.pjq.app</package_name>
		<app_version_name>2.1.1</app_version_name>
		<app_version_code>40</app_version_code>
	</app_info>
	<device_info>
		<model>Galaxy Nexus</model>
		<sdk_version>4.1.1</sdk_version>
		<api_level>15</api_level>
	</device_info>
	<backup_info>
		<origin>/data/data/me.pjq.app/</origin>
		<backup_time>timestamp</backup_time>
		<dest>/sdcard/backup/me.pjq.app/time/</dest>
	</backup_info>	
</root>
</code>





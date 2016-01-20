1.

https://www.npmjs.com/package/cordova-plugin-media
https://github.com/apache/cordova-plugin-media

2.

plugin.xml

    <platform name="android">
        <config-file target="res/xml/config.xml" parent="/*">
            <feature name="Media" >
                <param name="android-package" value="org.apache.cordova.media.AudioHandler"/>
            </feature>
        </config-file>
        
        <config-file target="AndroidManifest.xml" parent="/*">
<!--		
            <uses-permission android:name="android.permission.RECORD_AUDIO" />
            <uses-permission android:name="android.permission.MODIFY_AUDIO_SETTINGS" />
            <uses-permission android:name="android.permission.WRITE_EXTERNAL_STORAGE" />
            <uses-permission android:name="android.permission.READ_PHONE_STATE" />
-->			
        </config-file>
        
        <source-file src="src/android/AudioHandler.java" target-dir="src/org/apache/cordova/media" />
        <source-file src="src/android/AudioPlayer.java" target-dir="src/org/apache/cordova/media" />
        <source-file src="src/android/FileHelper.java" target-dir="src/org/apache/cordova/media" />
     </platform>
	 
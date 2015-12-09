## faralot-app
Ist eine eigenständige Applikation zur Darstellung von einer einzelnen Geolocation-Plattform.
 Basiert auf dem Framework **faralot-core** ([GitHub-Projekt](https://github.com/bestog/faralot-core)) und ist das Skeleton zum Entwickeln.
 
Weitere Informationen unter [faralot.com](https//faralot.com)

#### Demo
*findplaces* ([GitHub](https://github.com/bestog/findplaces)) ([apk](https://github.com/bestog/findplaces/releases/latest))

<img src="http://faralot.com/assets/faralot/login.png" height="200px" style="padding: 5px;">
<img src="http://faralot.com/assets/faralot/profile.png" height="200px" style="padding: 5px;">
<img src="http://faralot.com/assets/faralot/list.png" height="200px" style="padding: 5px;">
<img src="http://faralot.com/assets/faralot/map.png" height="200px" style="padding: 5px;"><br>
<img src="http://faralot.com/assets/faralot/detail-1.png" height="200px" style="padding: 5px;">
<img src="http://faralot.com/assets/faralot/detail-2.png" height="200px" style="padding: 5px;">
<img src="http://faralot.com/assets/faralot/drawer.png" height="200px" style="padding: 5px;">
<img src="http://faralot.com/assets/faralot/crop.png" height="200px" style="padding: 5px;">
<img src="http://faralot.com/assets/faralot/search.png" height="200px" style="padding: 5px;">

### Verwendung
Durch wenige Schritte kann eine neue funktionsfähige und eigenständige Applikation angefertigt werden:
* Ein eigener API-Applikation-Name (*API_APP*) muss für die neue Art der Locations im Server angelegt werden, dies kann nur der Administrator des faralot-Servers einrichten.
* Die Konfiguration der API, die von den Clients immer als erstes geladen wird bevor die Applikation startet, muss ebenfalls der Administrator manuell einstellen.
* Der Package-Name muss auf einen Eigenen geändert werden. Zu beachten ist, dass sowohl die Ordnerstruktur als auch in den Java Dateien die `import`-Namen geändert werden muss. Des weiteren sind die Einstellungen im `build.gradle` wichtig und müssen ebenfalls angepasst werden. Damit wird verhindert, dass bei dem Hochladen zum Google Play-Store die Applikation nicht abgelehnt wird. Da der Package-Name für jede Applikation eindeutig sein muss. 

*Weitere Informationen, wie Kontakt-Adresse zum faralot-Administrator oder Farbbeschreibung, sind unter [faralot.com](https//faralot.com) zu finden.*

### Konfigurationsmöglichkeiten
* **res/values/values.xml**: Die Farben und der Name der Applikation und deren Darstellung.
* **LaunchActivity.java**: *com.faralot.core.App* `setRest(<app_name>)` - beinhaltet den Api-Applikation-Namen für eine erfolgreiche Verbindung zur REST-API.
* **res/drawable/app_logo.png**: ist das Logo, welches beim Einloggen oberhalb angezeigt wird. Dies kann mit einem eigenen Bild ersetzt werden.
* **res/mipmap-***: beinhaltet das Applikation-Icon, welches mit dem neuen Logo ersetzt werden muss.
* Die Server-Konfiguration aus der REST-API kann nur durch den Administrator geändert werden, ist aber nur in einem gewissen Umfang erlaubt.

### Externe Bibliotheken
	(name: 'osmbonuspack_v5.5', ext: 'aar')
 	'com.android.support:support-v4:23.1.1'
	'com.android.support:appcompat-v7:23.1.1'
	'com.android.support:recyclerview-v7:23.1.1'
	'com.android.support:cardview-v7:23.1.1'
	'com.android.support:design:23.1.1'
	'com.baoyz.pullrefreshlayout:library:1.2.0'
	'com.daimajia.slider:library:1.1.5@aar'
	'com.github.dmytrodanylyk.android-process-button:library:1.0.4'
	'com.github.jorgecastilloprz:fabprogresscircle:1.01@aar'
	'com.google.code.gson:gson:2.4'
	'com.isseiaoki:simplecropview:1.0.9'
	'com.miguelcatalan:materialsearchview:1.3.0'
	'com.nineoldandroids:library:2.4.0'
	'com.orhanobut:dialogplus:1.10@aar'
	'com.squareup.okhttp:okhttp:2.5.0'
	'com.squareup.okhttp:okhttp-urlconnection:2.5.0'
	'com.squareup.picasso:picasso:2.5.2'
	'com.squareup.retrofit:converter-gson:2.0.0-beta2'
	'com.squareup.retrofit:retrofit:2.0.0-beta2'
	'de.hdodenhof:circleimageview:2.0.0'
	'io.paperdb:paperdb:1.1'
	'org.apache.commons:commons-lang3:3.3.2'
	'org.osmdroid:osmdroid-android:5.0.1@aar'
	'org.parceler:parceler:1.0.4'

### License
The components inside this GitHub project are under LGPL v3 licence, with an important simplification: 
The constraints described in Section 5.d and 5.e of the [LGPL LICENCE](https://github.com/bestog/faralot-core/blob/master/LICENSE) are DISCARDED. 

This means that you are allowed to convey a Combined Work without providing the user any way to recombine or relink the application, and without providing any shared library mechanism. 

In other terms, you are allowed to include the faralot-app in your Android application, without making your application open source. 


#Android Library 發佈到 jcenter

## 準備
***
<<<<<<< HEAD
 * 註冊帳號：[JFrog Bintray](https://bintray.com/bintray/jcenter) 
 * 取得API key 
 * Gradle : Version >=2.4
=======
 * 註冊帳號：到[JFrog Bintray](https://bintray.com/bintray/jcenter) 
 * ,取得API key 
 * Gradle : Version >=2.4,
>>>>>>> c1849d39e638dd8ed28b570aa0d27dc37d3b440b
 
##如何使用
***

 * 建立一個要上傳的Android Library Project
 
 * 在local.properties中加入
 
 ```
 bintray.apikey = 你的API key
 bintray.user=你註冊的使用者名稱
 ```
 * 修改Project主目錄的build.gradle ,
 
 ```
 buildscript {
    repositories {
        jcenter()
    }
    dependencies {
<<<<<<< HEAD
        classpath "com.android.tools.build:gradle:1.3.0"     
=======
        classpath "com.android.tools.build:gradle:1.3.0" <span style="color:red;">     
>>>>>>> c1849d39e638dd8ed28b570aa0d27dc37d3b440b
        //新增以下兩行
		classpath "com.jfrog.bintray.gradle:gradle-bintray-plug:1.0"
		classpath "com.github.dcendents:android-maven-gradle-plu</span>gin:1.3"
    }
}
allprojects {
    repositories {
        jcenter()
    }
}

 ```
<<<<<<< HEAD
 * 修改library module中的build.gradle
 
 ```
 
 ```

=======
* 修改library module中的build.gradle
>>>>>>> c1849d39e638dd8ed28b570aa0d27dc37d3b440b

 
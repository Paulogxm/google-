allprojects {
        repositories {
            google()
            jcenter()
        }
    } 


    dependencies {
        def lifecycle_version = "2.2.0"
        implementation "androidx.lifecycle:lifecycle-livedata-ktx:$lifecycle_version"
        implementation "androidx.lifecycle:lifecycle-viewmodel-ktx:$lifecycle_version"
        ...
    dependencies {
  def work_version = "2.4.0"

    // (Java only)
    implementation "androidx.work:work-runtime:$work_version"

    // Kotlin + coroutines
    implementation "androidx.work:work-runtime-ktx:$work_version"

    // optional - RxJava2 support
    implementation "androidx.work:work-rxjava2:$work_version"

    // optional - GCMNetworkManager support
    implementation "androidx.work:work-gcm:$work_version"

    // optional - Test helpers
    androidTestImplementation "androidx.work:work-testing:$work_version"
  }

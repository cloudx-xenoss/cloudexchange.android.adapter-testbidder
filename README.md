## 🚀 CloudX TestBidder Adapter Installation Guide

### 📦 Compatibility

#### 🧩 Language Compatibility
- **Kotlin version**: Built with `1.9.22`
    - Host apps should use Kotlin `1.9.0+`
- **Java compatibility**: Compiled to Java 8 bytecode (`jvmTarget = 1.8`)
    - Fully compatible with Java-based host apps (no Kotlin required)

#### 📱 Android Compatibility
- **Minimum SDK version**: `21`
- **Compile SDK version**: `35`
    - Host apps must set `minSdkVersion >= 21` to use the adapter.

#### 🛠️ Build Compatibility
- **Gradle version**: `8.5`
- **Android Gradle Plugin**: `8.2.2`
    - Host apps using AGP `8.0+` and Gradle `8.5+` are fully supported.

---

### 1. Add Maven Central Repository

In your project’s `settings.gradle` or `settings.gradle.kts`  
(You likely already have this by default):

```kotlin
dependencyResolutionManagement {
    repositoriesMode.set(RepositoriesMode.FAIL_ON_PROJECT_REPOS)
    repositories {
        google()
        mavenCentral()
    }
}
```

---

### 2. Add Adapter Dependency

In your app/module `build.gradle` or `build.gradle.kts`:

```kotlin
dependencies {
    implementation("io.cloudx:adapter-testbidder:<latest-version>")
}
```

> Replace `<latest-version>` with the version you want to use (e.g., `0.0.1.27`).

---

### 3. Sync and Build

* Sync your project in Android Studio.
* The CloudX TestBidder adapter will be downloaded automatically from Maven Central.

✅ **That’s it! You’re ready to use the CloudX TestBidder Adapter.**

---

### ➕ Related Adapters

You may also integrate other CloudX Adapters:

- [CloudX Adapter](https://github.com/cloudx-xenoss/cloudexchange.android.adapter-cloudx)
- [Google Adapter](https://github.com/cloudx-xenoss/cloudexchange.android.adapter-google)
- [Mintegral Adapter](https://github.com/cloudx-xenoss/cloudexchange.android.adapter-mintegral)
- [Meta Adapter](https://github.com/cloudx-xenoss/cloudexchange.android.adapter-meta)

> Visit each link for setup guides and available versions.

---

## License

This software is licensed under the Elastic License 2.0.  
See the [LICENSE](./LICENSE) file for details.

# Paper-Template
This repository contains a template for paper plugins.

## Installation
#### 1. Clone this repository:
```sh
git clone https://github.com/Vaycore-Network/paper-template
```
and open it in the IDE of your choice.

<br>

#### 2. Create the testing server
To create a local server for testing, run the `runServer` gradle task:
```sh
./gradlew runServer
```

<br>

#### 3. Accept Server EULA
Accept the minecraft server eula in `run/eula.txt`.

<br>

#### 4. Customize Metadata
It is recommended to
- Change the project name in the `settings.gradle.kts`
- Customize the plugin data in the `build.gradle.kts`
- Rename the root path from `de.c4vxl.papertemplate` to your own group id

<br>

### Download the Vaycore-API
- Either download it from the [latest release](https://github.com/Vaycore-Network/VaycoreAPI/releases/latest) manually
- or run the setup script to download it automatically:
   ```sh
  sh setup.sh
   ```

<br>

#### 5. Reinitializing the git repo
1. Delete the old repo:<br>
   On Windows:
    ```sh
   rmdir /s /q .git
    ```

   On linux/mac:
    ```sh
   rm -rf .git
    ```

2. Initialize a new one:
    ```sh
   git init
   git add .
    ```

3. Push an initial commit:
    ```sh
   git commit -am "Initial Commit"
   git remote add origin "<your repo url>"
   git checkout -b main
   git push origin main
   ```

### That's it.


## Testing locally
For testing your plugin locally use the `runServer`-gradle task:
```sh
./gradlew runServer
```
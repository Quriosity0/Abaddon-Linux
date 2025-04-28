# I am not the author of Abaddon. Its original page can be found [here](https://github.com/uowuo/abaddon)


### Abaddon-Linux
An alternative Discord client with voice support made with C++ and GTK 3 for linux

## If you want to build it manually
1. Install dependencies
    * On Ubuntu 22.04 (Jammy)/Debian 12 (bookworm) and newer:
      ```Shell
      $ sudo apt install g++ cmake libgtkmm-3.0-dev libcurl4-gnutls-dev libsqlite3-dev libssl-dev nlohmann-json3-dev libhandy-1-dev libsecret-1-dev libopus-dev libsodium-dev libspdlog-dev
      ```
    * On Arch Linux
      ```Shell
      $ sudo pacman -S gcc cmake gtkmm3 libcurl-gnutls lib32-sqlite lib32-openssl nlohmann-json libhandy opus libsodium spdlog
      ```
    * On Fedora Linux:
      ```Shell
      $ sudo dnf install g++ cmake gtkmm3.0-devel libcurl-devel sqlite-devel openssl-devel json-devel libsecret-devel libhandy-devel opus-devel libsodium-devel spdlog-devel
      ```
      > **Note:** On older versions of fedora you might need to install gtkmm30-devel instead of gtkmm3.0-devel.
      Use `dnf search gtkmm3` to see available packages.
2. `git clone https://github.com/uowuo/abaddon --recurse-submodules="subprojects" && cd abaddon`
3. `mkdir build && cd build`
4. `cmake ..`
5. `make`
6. Copy `res` and `css` folders to the compiled executable and run it

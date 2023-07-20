cmake_minimum_required(VERSION 3.5)

project(long-sddm-theme)

set(CMAKE_INCLUDE_CURRENT_DIR ON)
set(CMAKE_AUTOMOC ON)
set(CMAKE_AUTOUIC ON)
set(CMAKE_AUTORCC ON)

install(FILES Main.qml DESTINATION /usr/share/sddm/themes/long)
install(FILES SessionMenu.qml DESTINATION /usr/share/sddm/themes/long)
install(FILES UserView.qml DESTINATION /usr/share/sddm/themes/long)
install(FILES LongUIMenu.qml DESTINATION /usr/share/sddm/themes/long)
install(FILES LongUIMenuItem.qml DESTINATION /usr/share/sddm/themes/long)
install(FILES system-shutdown-symbolic.svg DESTINATION /usr/share/sddm/themes/long)

install(FILES theme.conf DESTINATION /usr/share/sddm/themes/long)
install(FILES hidpi.conf DESTINATION /etc/sddm.conf.d/)
install(FILES sddm.conf DESTINATION /etc/)

# install(FILES "faces/.face.icon" DESTINATION /usr/share/sddm/faces/)

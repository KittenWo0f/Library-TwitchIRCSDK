add_library(TwitchIRCSDK STATIC
    src/clientIRC.cpp
    src/twitchirc.cpp
    src/message.cpp
    src/user.cpp
    src/commandManager.cpp
    src/event.cpp
    src/eventManager.cpp
)

target_include_directories(TwitchIRCSDK PUBLIC include)

target_link_libraries(TwitchIRCSDK PRIVATE asio)
# 3rd Party ImGui backedn

The ImGui backend within these 2 files is mostly the same as the original, however there are some significant modifications to support MDI. In particular the backend has been modified to not store its state in the form of static globals. Instead, there is a state struct which can be used to reset the backend state when needed.

This allows for multiple instances of ImGuiRenderer running simoultaneously.

Main changes have been marged with `SPEECH_GRAPHICS` comments.

# kitty


## Install

```bash
sudo apt install kitty
```

## Settings

```bash
# nvim ~/.config/kitty/kitty.conf

# ============================================================
# KITTY — POWER USER CONFIG
# Kitty + tmux + LazyVim
# ============================================================


# ============================================================
# WINDOW
# ============================================================

# Start fullscreen
fullscreen yes

# Window padding
window_padding_width 8

# Remove the OS title bar
hide_window_decorations yes

# Remember window dimensions when not fullscreen
remember_window_size yes

# Prevent Kitty from resizing itself
resize_in_steps yes


# ============================================================
# BACKGROUND
# ============================================================

# Deep Cyberdream-style background
background #0b0e14

# Slight transparency
background_opacity 0.94

# Allow opacity to be changed dynamically
dynamic_background_opacity yes

# Background image (enable if desired)
background_image ~/.config/kitty/background/1.jpg
background_image_layout scaled
background_image_linear yes
background_tint 0.30


# ============================================================
# FONT
# ============================================================

# Nerd Font — good for LazyVim / Starship / tmux
font_family ComicShannsMono Nerd Font

font_size 13.0

# Slightly tighter spacing
modify_font cell_height 0px
modify_font cell_width 0px


# ============================================================
# CURSOR
# ============================================================

cursor #ffffff
cursor_text_color #0b0e14

# Cursor style
cursor_shape beam

# Cursor blinking
cursor_blink_interval 0.6

# Stop blinking after inactivity
cursor_stop_blinking_after 15


# ============================================================
# SELECTION
# ============================================================

selection_foreground #ffffff
selection_background #30363d


# ============================================================
# SCROLLBACK
# ============================================================

scrollback_lines 10000

# Mouse wheel scrolling
wheel_scroll_multiplier 3.0


# ============================================================
# URLS
# ============================================================

url_color #5ccfe6
url_style curly

# Open URLs with Ctrl+Click
open_url_with ctrl+shift+u


# ============================================================
# TAB BAR
# ============================================================

tab_bar_edge top

tab_bar_style powerline

tab_powerline_style slanted

tab_title_template "{index}: {title}"

active_tab_font_style bold-italic
inactive_tab_font_style normal

active_tab_foreground #ffffff
inactive_tab_foreground #7d8590


# ============================================================
# MOUSE
# ============================================================

mouse_map left click ungrabbed mouse_selection normal

# Ctrl + click URL
mouse_map ctrl+left click ungrabbed mouse_handle_click selection


# ============================================================
# COPY / PASTE
# ============================================================

# Linux-friendly shortcuts
map ctrl+shift+c copy_to_clipboard
map ctrl+shift+v paste_from_clipboard

# Primary selection
map shift+insert paste_from_selection


# ============================================================
# FULLSCREEN
# ============================================================

# F11 = fullscreen toggle
map f11 toggle_fullscreen


# ============================================================
# FONT SIZE
# ============================================================

map ctrl+equal change_font_size all +1.0
map ctrl+minus change_font_size all -1.0
map ctrl+0 change_font_size all 13.0


# ============================================================
# OPACITY
# ============================================================

# Increase / decrease transparency
map ctrl+shift+equal change_background_opacity +0.05
map ctrl+shift+minus change_background_opacity -0.05

# Reset opacity
map ctrl+shift+0 set_background_opacity 0.94


# ============================================================
# KITTY MANAGEMENT
# ============================================================

# Reload configuration
map ctrl+shift+f5 load_config_file

# Debug keyboard input
# Run externally:
# kitty --debug-input


# ============================================================
# PERFORMANCE
# ============================================================

# Don't animate unnecessarily
repaint_delay 10

# Reduce input latency
input_delay 0

# Sync rendering
sync_to_monitor yes


# ============================================================
# TERMINAL BEHAVIOR
# ============================================================

# Shell integration
shell_integration enabled

# Allow applications to change the terminal title
set_tab_title "{title}"


# ============================================================
# BELL
# ============================================================

enable_audio_bell no
visual_bell_duration 0.0

# No annoying window flashing
window_alert_on_bell no


# ============================================================
# LINUX / WAYLAND
# ============================================================

linux_display_server auto

# Disable remote control unless explicitly needed
allow_remote_control no


# ============================================================
# ADVANCED
# ============================================================

# Use extended keyboard protocol
kitty_mod ctrl+shift

# Keep terminal clean
confirm_os_window_close 0
```

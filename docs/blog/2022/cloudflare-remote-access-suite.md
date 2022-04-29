---
title: Cloudflare Remote Access Suite
tags:
  - internet
  - network
  - selfhosted
---

...

## 1. Existing Solutions

## 2. The Cloudflare Replacement Suite

## 3. Wishlist, Development, and the Competition


```lua title="wezterm.lua"

local wezterm = require("wezterm")

return {
  font = wezterm.font("Fira Code"),
  font_size = 15.0,

  window_close_confirmation = "NeverPrompt",

  -- ANCHOR Tab Bar
  hide_tab_bar_if_only_one_tab = true,

  window_background_opacity = 1.0,

  window_padding = {
    left = 25,
    right = 25,
    top = 25,
    bottom = 25,
  },

  -- SECTION Colors
  color_scheme = "Horizon Dark",
  
  color_schemes = {
    ["Horizon Dark"] = {
        -- The default text color
        foreground = "#FDF0ED",
        -- The default background color
        background = "#1C1E26",

        -- Overrides the cell background color when the current cell is occupied by the
        -- cursor and the cursor style is set to Block
        cursor_bg = "#FCEf0C",
        -- Overrides the text color when the current cell is occupied by the cursor
        cursor_fg = "black",
        -- Specifies the border color of the cursor when the cursor style is set to Block,
        -- or the color of the vertical or horizontal bar when the cursor style is set to
        -- Bar or Underline.
        cursor_border = "#52ad70",

        -- the foreground color of selected text
        selection_fg = "#FFF27D",
        -- the background color of selected text
        selection_bg = "#4D504C",

        -- The color of the scrollbar "thumb"; the portion that represents the current viewport
        scrollbar_thumb = "#222222",

        -- The color of the split lines between panes
        split = "#444444",

        ansi = {"#131519", "#E95678", "#FFF27D", "#689D6A", "#6C6F93", "#EE64AE", "#59E3E3", "#689D6A"},
        brights = {"#686868", "#e06783", "#0af29d", "#FBC3A7", "#3FC6DE", "#F075B7", "#E95678", "#F2F2F2"},

        -- Arbitrary colors of the palette in the range from 16 to 255
        indexed = {[136] = "#af8700"},

        -- Since: 20220319-142410-0fcdea07
        -- When the IME, a dead key or a leader key are being processed and are effectively
        -- holding input pending the result of input composition, change the cursor
        -- to this color to give a visual cue about the compose state.
        compose_cursor = "orange",
    }
  }
     -- !SECTION
}

```
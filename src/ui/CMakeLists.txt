# Aseprite UI Library
# Copyright (C) 2019-2025  Igara Studio S.A.
# Copyright (C) 2001-2018  David Capello

if(WIN32)
  add_definitions(-D_CRT_SECURE_NO_WARNINGS)
endif()

add_library(ui-lib
  alert.cpp
  app_state.cpp
  box.cpp
  button.cpp
  combobox.cpp
  component.cpp
  cursor.cpp
  display.cpp
  entry.cpp
  event.cpp
  fit_bounds.cpp
  graphics.cpp
  grid.cpp
  image_view.cpp
  int_entry.cpp
  intern.cpp
  label.cpp
  layer.cpp
  link_label.cpp
  listbox.cpp
  listitem.cpp
  manager.cpp
  menu.cpp
  message.cpp
  message_loop.cpp
  move_region.cpp
  paint.cpp
  paint_event.cpp
  panel.cpp
  popup_window.cpp
  property.cpp
  register_message.cpp
  resize_event.cpp
  scroll_bar.cpp
  scroll_helper.cpp
  separator.cpp
  shortcut.cpp
  size_hint_event.cpp
  slider.cpp
  splitter.cpp
  style.cpp
  system.cpp
  textbox.cpp
  theme.cpp
  timer.cpp
  tooltips.cpp
  view.cpp
  viewport.cpp
  widget.cpp
  window.cpp)

target_link_libraries(ui-lib
  laf-os
  laf-text
  laf-gfx
  laf-base
  obs
  fmt)

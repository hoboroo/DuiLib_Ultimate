add_definitions(-DUNICODE -D_UNICODE)
add_definitions(-DUILIB_STATIC)

set(_SOURCE_FILES
  # Root
  "StdAfx.cpp"
  "UILib.cpp"

  # Control
  "Control/UIActiveX.cpp"
  "Control/UIFadeButton.cpp"
  "Control/UILabel.cpp"
  "Control/UIRollText.cpp"
  "Control/UIAnimation.cpp"
  "Control/UIFlash.cpp"
  "Control/UIList.cpp"
  "Control/UIScrollBar.cpp"
  "Control/UIButton.cpp"
  "Control/UIGifAnim.cpp"
  "Control/UIListEx.cpp"
  "Control/UISlider.cpp"
  "Control/UIColorPalette.cpp"
  "Control/UIGifAnimEx.cpp"
  "Control/UIMenu.cpp"
  "Control/UIText.cpp"
  "Control/UICombo.cpp"
  "Control/UIGroupBox.cpp"
  "Control/UIOption.cpp"
  "Control/UITreeView.cpp"
  "Control/UIComboBox.cpp"
  "Control/UIHotKey.cpp"
  "Control/UIProgress.cpp"
  "Control/UIWebBrowser.cpp"
  "Control/UIDateTime.cpp"
  "Control/UIIPAddress.cpp"
  "Control/UIRichEdit.cpp"
  "Control/UIEdit.cpp"
  "Control/UIIPAddressEx.cpp"
  "Control/UIRing.cpp"

  # Core
  "Core/ControlFactory.cpp"
  "Core/UIContainer.cpp"
  "Core/UIDlgBuilder.cpp"
  "Core/UIMarkup.cpp"
  "Core/UIResourceManager.cpp"
  "Core/UIBase.cpp"
  "Core/UIControl.cpp"
  "Core/UIManager.cpp"
  "Core/UIRender.cpp"

  # Layout
  "Layout/UIAnimationTabLayout.cpp"
  "Layout/UIHorizontalLayout.cpp"
  "Layout/UITileLayout.cpp"
  "Layout/UIChildLayout.cpp"
  "Layout/UITabLayout.cpp"
  "Layout/UIVerticalLayout.cpp"

  # Utils
  "Utils/DPI.cpp"
  "Utils/TrayIcon.cpp"
  "Utils/UIShadow.cpp"
  "Utils/WinImplBase.cpp"
  "Utils/DragDropImpl.cpp"
  "Utils/UIDelegate.cpp"
  "Utils/Utils.cpp"
  "Utils/unzip.cpp"
)

add_library(duilib STATIC ${_SOURCE_FILES})
target_include_directories(duilib PUBLIC ${CMAKE_CURRENT_SOURCE_DIR})

# OS
Windows

# AutoHotkey v2.0
https://www.autohotkey.com/

# key
| Key | Code |
| ---- | ---- |
| Win | # |
| Alt | ! |
| Ctrl | ^ |
| Shift | + |

# Function
| Group | Function | Note | Default Hotkey |
| - | - | - | - |
| APP | Suspend | Suspend Hotkey |  Ctrl+F3 |
|  | ExitApp | Exit APP | Ctrl+F4 |
|  | Reload | Reload APP | Ctrl+F5 |
| Show | showVersion() | Show Version | Ctrl+Alt+Y |
|  | getMonitorInfo() | Show Monitor Info | Ctrl+Alt+N |
| HotGUI | guiHot("key") | Hotkey GUI to update Hotkeys | Ctrl+Alt+K |
|  | guiHot("str") | Hotstring GUI to update Hotstrings | Ctrl+Alt+H |
| TTS | ttsSpeak() | TTS Speech selection | Ctrl+Alt+1 |
|  | ttsPause() | TTS Pause | Ctrl+Alt+2 |
|  | ttsResume() | TTS Resume | Ctrl+Alt+3 |
| Web | search(browserPath) | Google Search selection with browser | Ctrl+Alt+G |
|  | translate(browserPath) | Google translate selection with browser | Ctrl+Alt+J |
|  | url(browserPath) | Open selected URL with browser | Ctrl+Alt+U |
| Date | date() | then press Delimiter(d) h(hyphen)/s(slash)/else("") in yyyy(d)MM(d)dd. Send Date | Ctrl+Alt+D |
|  | time() | Send time(HH:mm:ss) |  |
| Text | reInput() | reInput selection (after changing input mode from english to 注音) | Ctrl+Alt+R |
|  | caseText() | then press l(lowercase)/u(uppercase)/t(title case)/k(kebab-case)/c(CamelCase)/s(snake_case). Convert selection to case and Send | Ctrl+Alt+S |
|  | replace() | use InputBox to input find and replace string. Replace selection and Send | Ctrl+Alt+T |
|  | trimSpace() | Trim selection and Send | Ctrl+Alt+Space |
|  | indent() | then press i(increase)/d(decrease) indent(`"  "`). Change indent of selection and Send | Ctrl+Alt+I |
|  | mdTable() | use InputBox to input row and col. Send markdown table | Ctrl+Alt+B |
| File | RUN ::{645FF040-5081-101B-9F08-00AA002F954E} | Open Recycle Bin | Ctrl+Alt+X |
|  | copy() | Copy and sleep 100 ms |  |
|  | copyFileCase() | then press t(copy setting file)/else(InputBox) to copy folder | Ctrl+Alt+F |
|  | createShortcut(linkName, linkPath) | Create Shortcut | Ctrl+Alt+L |
| Window | WinSetAlwaysOnTop -1, "A" | Selected Window Always on top | Ctrl+F1 |
|  | Send "!{Tab}" | Switch window | LButton+RButton |
|  | Send "#d" | Show Desktop | RButton+LButton |
|  | setTrans() | then press 1~9(transparent alpha)/else(non-transparent) to change transparency of window | Ctrl+Alt+Q |
|  | moveApp(alias, x, y, width, height) | Move window to (x, y) and set (width, height) |  |
|  | moveToDesktop("left"/"right") | Move window to last/next virtual desktop | Ctrl+Alt+Left/Right |
| OCR | ocrText() | OCR & save to clipboard | Ctrl+Alt+C |

## copy setting file
settings\copy.txt\
old folder, new folder, ignore folder
```
D:\repos\old,D:\repos\new,log file
```

# Add your script
1. new directory named Lib"
2. add your script in directory "Lib"
3. include your script in Includes.ahk
4. add function in your script with Hotkey GUI

# Version
Major_Version_Number.Minor_Version_Number(.Revision_Number.Build_Number)\
主版號：當你做了不相容的 API 修改\
次版號：當你做了向下相容的功能性新增\
修訂號：當你做了向下相容的問題修正\
編譯號

| Date | Version | Type | Note | Reference |
| ---- | ---- | ---- | ---- | ---- |
| 2023-08-16 | 2.1.0 | Feature | search(), translate(), reInput() |  |
| 2023-08-23 | 2.2.0 | Feature | caseText() |  |
| 2023-08-31 | 2.2.0 | Feature | moveApp() |  |
| 2023-09-13 | 2.3.0 | Feature | mdTable(), indent() |  |
| 2023-09-13 | 2.3.1 | Fix | search(), translate() with filePath |  |
| 2023-09-25 | 2.3.2 | Fix | caseText() fix kebab-case/CamelCase/snake_case |  |
| 2023-09-28 | 2.4.0 | Feature | transparent window |  |
| 2023-10-13 | 2.5.0 | Feature | hotkey/hotstr GUI, version |  |
| 2023-10-16 | 2.5.1 | Fix | mouse over tray icon show gui with hotkeys |  |
| 2023-10-27 | 2.5.2 | Fix | modify date() |  |
| 2023-11-02 | 2.6.0 | Feature | moveToDesktop() |  |
| 2023-11-03 | 2.6.0 | Feature | getMonitorInfo() |  |
| 2023-11-09 | 2.6.0 | Feature | url() |  |
| 2023-11-30 | 2.6.0 | Feature | copyFileCase() |  |
| 2023-12-01 | 2.6.0 | Feature | create shortcut |  |
| 2023-03-10 | 2.6.1 | Fix | fix HotGUI |  |
| 2024-04-01 | 2.7.0 | Feature | TTS |  |


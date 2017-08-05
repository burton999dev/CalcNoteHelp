# CalcNotePlugin for GoogleDrive
[CalcNotePlugin for GoogleDrive](https://play.google.com/store/apps/details?id=com.burton999.notecal.plugin.gdrive) allows you to automatically backup your files to GoogleDrive. This [Plugin](https://play.google.com/store/apps/details?id=com.burton999.notecal.plugin.gdrive) can be used with CalcNote and CalcNotePro v2.4.14 or later.

## How to setup
1. Launch the `CalcNotePlugin for GoogleDrive`.
1. Allow CalcNote to access your contacts. **This plugin needs to access your Google account (via Contacts).**
1. Enable `Sync with your Google Drive`.
1. Select your google account to use.
1. Then the automatic backup feature is enabled. You don't need to setup on CalcNote.
<br/>
<br/>
<img src="https://raw.githubusercontent.com/burton999dev/CalcNoteHelp/master/images/en/google_drive_plugin.png">

## Mechanism
[CalcNotePlugin for GoogleDrive](https://play.google.com/store/apps/details?id=com.burton999.notecal.plugin.gdrive) creates `__calcnote__` folder to your google drive root folder. All of your files and drafts are saved in this folder.
Also plugin creates `trash` folder in the `__calcnote__` folder. All for your deleted files and drafts are saved in the `trash` folder.

## Specification
1. All files and drafts are backuped automatically.
1. When you use on multiple devices, A file created by device A are automatically synchronized to device B. File updates and deletes are also synchronized.
1. This plugin is intended to provide automatic backup. It does not provide accurate synchronization function.
1. Plugin resolves an update conflict based on device time. So if the time of the device is not accurate, it will result in unintended consequences.
1. A file created by another application is not synchronized. If you create text file using GoogleDrive app and save file in `__calcnote__` folder, file is ignored by plugin.
1. Plugin does not delete deleted files in `trash` folder. So you need to delete deleted files manually if need.

<br><br>
[HOME](index.md)　[How to use](how2use.md)　[Grammar](http://burton999dev.github.io/CalcNoteHelp/grammar_en.html)　[Operators and Functions](operator_and_function.md)　[Unit Converter](unit_converter.md)　[Currency Converter](currency_converter.md)　[Floating Widget](floating_widget.md)　[Settings](settings.md)　[Customizing Keypad](customizing_keypad.md)　[Custom Extension](custom_extension.md)　[FAQ](faq.md)　[Customization Example](example4theme.md)  

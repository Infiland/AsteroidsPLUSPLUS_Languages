This repository is a sub-module of Asteroids ++, containing all translations
Please fork this repository and make a pull request to make updates.

# Adding a New Language

To add a new language to the game, follow these steps:

1.  **Create a new language file:**
    *   Duplicate an existing language file (e.g., `english.lang`).
    *   Rename the duplicated file to the name of the new language (e.g., `spanish.lang`, `french.lang`). Ensure the file extension remains `.lang`.

2.  **Edit the language file:**
    *   Open the new language file in a text editor.
    *   Each line in the file represents a key-value pair, where the key is the identifier used in the game's code, and the value is the translated text.
    *   Translate the text for each key into the new language.
    *   **Important:** Do not change the keys. Only modify the text after the `=` sign.
    *   Example:
        ```
        7=Start
        8=Continue
        9=Settings
        10=Online Levels
        11=Extras
        12=Quit
        ```
        Should become (for German):
        ```
        7=Start
        8=Fortfahren
        9=Einstellungen
        10=Online-Level
        11=Extras
        12=Beenden
        ```

3.  **Integrate the new language into the game (if necessary):**
    *   The actual game repository uses this module repository for translations, so the localization system scans this directory for `.lang` files.

# EE Translation Repository  
This repository is dedicated to the translation work for the game **"Emerjency Exit"**.  

## Translation Steps  
1. **Fork this repository** and clone it locally.  
2. **Create a new branch** for your work, whether adding a new language or revising an existing one. Perform all changes in this branch.  
3. Use the game files in the repository to **test your translations** at any time.  
4. After completing your work, **submit a pull request**. In the pull request description, clearly outline the changes you made.  

---

## Translation Dictionaries  

### Language Files  
- Language files have the `.lng` extension and are located in the `lang` folder. Each language corresponds to one `.lng` file.  
- Format:  
  ```  
  key1=value1  
  key2=value2  
  ...  
  ```  
- **To add a new language**:  
  1. Duplicate an existing `.lng` file (e.g., `chn.lng`).  
  2. Translate only the **values** (text after the `=`). Do **not** modify the keys (text before the `=`).  
  3. Preserve `%x` placeholders, which will be dynamically replaced in the game. Handle them carefully.  

### Subtitle Files  
- Subtitle files are placed in the **same folder** as their corresponding audio files.  
- Naming convention:  
  ```  
  <audio_filename_without_extension>_sub_<language_code>.txt  
  ```  
  Example: For an audio file `sounds/items/fzt/1.ogg`, the Chinese subtitle file should be named `1_sub_chn.txt`.  

- Format:  
  ```  
  <timestamp_in_milliseconds>:Subtitle text  
  ```  
- **Guidelines**:  
  - If adding a new subtitle file, duplicate an existing one and modify it.  
  - **Do not alter timestamps** unless absolutely necessary. If changes are required, notify the repository maintainer.  
  - Note: Audio files are **not included** in the repository.  

---


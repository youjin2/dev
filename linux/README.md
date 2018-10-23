# Linux commands
* chown
  - change group permission
  ``` bash
  $ chown {owner}:{group} {file_or_directory}
  # recursive for sub directories
  $ chown -R {owner}:{group} {file_or_directory}
  ```


* Slack
    - External link opened as blank tab in new browser in Chrome
    ```
    $ cd /home/`user`/.local/share/applications
    $ vim google-chrome.desktop
    # add space and %U as below and save
    # Exec=/opt/google/chrome/chrome %U
    ```

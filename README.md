How to use
==========

Production Pack
---------------

1. Add follow lines to '/edx/app/edx_ansible/server-vars.yml' (create if it doesn't exist):<br/>
  **Warning!** If you use seperate file/custom ansible-book, feel free to add these lines there (and update your system).
  * edx_platform_repo: https://github.com/epam-mooc/edx-platform.git
  * edx_platform_version: master
  * edxapp_use_custom_theme: true
  * edxapp_theme_name: stanford
  * edxapp_theme_source_repo: https://github.com/epam-mooc/edx-theme.git
  * edxapp_theme_version: master
2. Execute update command:
  * sudo /edx/bin/update edx-platform master
3. If in the end of execution you see 0 errors, it execute normally, otherwise I'm sorry - in this case you can find log files here: '/edx/var/log' and try to fix it.

License
=======

The code in this repo is licensed under the Apache 2.0 License.
See [LICENSE.txt](LICENSE.txt) for more info.

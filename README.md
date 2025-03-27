<h2 align="center"><a href="#wrench-installation"><img src="https://user-images.githubusercontent.com/61329159/204102654-0e414196-bea2-4147-9e1e-aeb8b4190893.png" width="20" height="20" /></a> Firefox Mod Blur - Modular (Installer Fork)</h2>

<p align="center"><i>This fork adds an installer that helps manage mods/themes.</i></p>

> [!NOTE]
> I'll keep maintaining this fork until the upstream author
> finishes the feature of toggling extra mods/themes in `about:config`.
> -- Alan Kuan
>
> Please go to https://github.com/datguypiko/Firefox-Mod-Blur for more information.

<p align="center"> <img alt="FirefoxCss" src="https://i.imgur.com/ChlWHFp.png"> </p>
<h6 align="center"> :wrench: Version 3.0 - Working on functionality overhaul. Responsive oneliner, toggling extra mods through about:config and other adjustments. </h6>

<p align="center"><h6 align="center" href="https://github.com/datguypiko/Firefox-Mod-Blur/issues/129">Preview v 3.0 https://github.com/datguypiko/Firefox-Mod-Blur/issues/129</h6></p>

<h2>:wrench: Installation</h2>

> [!IMPORTANT]
> ##### 1. In `about:config` set `toolkit.legacyUserProfileCustomizations.stylesheets` to "True" for your custom themes to work.
> ##### 2. Clone the repo with the latest or your preferred version.
> ##### 3. You can find your profile folder by writing `about:support` in URL bar and using `Open folder` in `Profile folder` section.
> ##### 4. Follow the instructions below.

<h3>:page_with_curl: Installer Script</h3>

> [!WARNING]
> Since the original file organization is modified in this fork,
> the installer does not work in the upstream repo.
> For example, the mod that pops out/push bookmarks bar on hover is placed at `EXTRA_MODS/Auto hide Mods`.

<h4>Prerequisites</h4>
Install a Python package with the following command:

```sh
pip install -r requirements.txt
```

<h4>Usage</h4>

```sh
./installer.py [-h] [-e] DIRECTORY
```

| Arguments | Description |
| :--- | :--- |
| DIRECTORY | The path to Firefox profile directory; if '-e', '--exact' flag is enabled, this should be the path to the exact directory where the files are installed. |

| Options | Description |
| :--- | :--- |
| -h, --help | Show help messages. |
| -e, --exact | Whether the given directory is exactly where the files are installed. It will be useful if you wrap 'Firefox Mod Blur' in your own 'chrome' directory with a different name. |

Examples:
```sh
./installer.py ~/.mozilla/firefox/x0x0x0x0.default-release
```

```sh
./installer.py -e ~/.mozilla/firefox/x0x0x0x0.default-release/chrome/Firefox-Mod-Blur
```

> [!IMPORTANT]
> You should run `git pull` by yourself before executing "Update" with the script.

> [!NOTE]
> You should run the script with `python3 ./installer.py ...` on Windows.

<h4>Screenshots</h4>

- First time to install:
  ![image](https://github.com/Alan-Kuan/Firefox-Mod-Blur/assets/24734750/e42d8bcb-bf7e-4a95-8a59-b68e22d08838)
- Run the script after installed:
  ![image](https://github.com/Alan-Kuan/Firefox-Mod-Blur/assets/24734750/328953d1-3ca4-4109-adef-fb8dc5e4250a)
- Manage Mods:
  ![image](https://github.com/Alan-Kuan/Firefox-Mod-Blur/assets/24734750/e958649c-3c70-4961-b512-0b4bac854eef)
- Manage Themes:
  ![image](https://github.com/Alan-Kuan/Firefox-Mod-Blur/assets/24734750/46110517-57bc-4a4f-97c7-cf0c6f49f4c8)
- Update Mods/Theme:
  ![image](https://github.com/Alan-Kuan/Firefox-Mod-Blur/assets/24734750/c6e0e946-4a3b-475c-bb8c-9cd72e4d6372)
- List Installed Mods/Theme:
  ![image](https://github.com/Alan-Kuan/Firefox-Mod-Blur/assets/24734750/fea31d07-cbaa-4a46-8290-d5c58abbdd44)
- Uninstall:
  ![image](https://github.com/Alan-Kuan/Firefox-Mod-Blur/assets/24734750/93183b15-bc1b-4ee9-b88c-29c8892abe41)

# Установка VSX / VisionCore / Installation

## Русский

**Требования:** Windows 11 x64, права администратора Windows, не менее 1 ГБ для установки и отдельное место для архива. Для подключения камер нужен доступ к ним по сети. Видеокарта и интернет для установки не обязательны.

1. Скачайте `install.exe` и `install.sha256` из одного выпуска в **Releases**.
2. В папке загрузки выполните в PowerShell: `Get-FileHash -Algorithm SHA256 .\install.exe`. Если результат не совпадает с `install.sha256`, не запускайте установщик. Контрольная сумма не заменяет цифровую подпись.
3. Закройте VSX, запустите установщик от имени администратора и примите лицензию. Автопоиск камер через брандмауэр включайте только в доверенной частной сети. Для ручного подключения он не нужен.
4. При первом запуске сервера создайте администратора VSX — готового логина и пароля нет. Выберите локальную папку архива, добавьте камеру и проверьте оба потока перед включением записи. На рабочем месте подключитесь к серверу под своей учётной записью VSX.

**Обновление:** сделайте резервную копию и установите новую версию поверх старой. Копия локального профиля не заменяет копию серверных данных. Не удаляйте вручную `C:\ProgramData\VisionCore`.

**Удаление:** используйте «Параметры → Приложения → Установленные приложения». Удаление очищает пользователей, сохранённые пароли, камеры и настройки. Видеозаписи, экспорт и внешние резервные копии не удаляются. После повторной установки администратора нужно создать заново.

## English

**Requirements:** Windows 11 x64, Windows administrator privileges, at least 1 GB for installation, and separate space for the video archive. Cameras must be reachable over the network. A GPU and an internet connection are not required for installation.

1. Download `install.exe` and `install.sha256` from the same release under **Releases**.
2. In the download folder, run `Get-FileHash -Algorithm SHA256 .\install.exe` in PowerShell. If the hash differs from `install.sha256`, do not run the installer. A checksum does not replace a digital signature.
3. Close VSX, run the installer as administrator, and accept the license. Allow camera discovery through the firewall only on a trusted private network. Manual camera setup does not require discovery.
4. On the server’s first launch, create a VSX administrator account. There are no default credentials. Choose a local archive folder, add a camera, and test both streams before enabling recording. On a workstation, connect to the server with your VSX account.

**Updating:** back up your data and install the new version over the existing one. A local profile backup does not replace a server backup. Do not manually delete `C:\ProgramData\VisionCore`.

**Uninstalling:** use **Settings → Apps → Installed apps**. Uninstalling clears users, saved passwords, cameras, and settings. Recordings, exports, and external backups are not removed. Create a new administrator account after reinstalling.

## Тихая установка / Silent installation

Указывайте `/ACCEPTEULA=YES` только если принимаете лицензию. Учётные записи автоматически не создаются.  
Use `/ACCEPTEULA=YES` only if you accept the license. User accounts are not created automatically.

```bat
install.exe /VERYSILENT /SUPPRESSMSGBOXES /NORESTART /ACCEPTEULA=YES
```

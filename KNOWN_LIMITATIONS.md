# Известные ограничения / Known limitations

## Русский

- **Установка.** Статус подписи и проверок на чистой Windows 11 смотрите в описании выпуска. Неподписанный установщик может вызвать предупреждение Windows. Перед обновлением сделайте резервную копию; не удаляйте рабочую установку ради обновления.
- **Камеры и нагрузка.** Каталог до 128 камер не гарантирует длительную работу 128 потоков одновременно. Плавность сетки и видеостен нужно проверить на своём оборудовании. Для больших сеток используйте обычное качество, высокое — для развёрнутой камеры.
- **Совместимость.** Поиск, профили, поворот и события ONVIF зависят от модели камеры. Если ONVIF недоступен, попробуйте ручное подключение по RTSP.
- **Аналитика.** Распознавание номеров не поддерживается. Аналитика на многих камерах повышает нагрузку; пользовательские модели принимаются только в совместимых пакетах, прошедших локальную проверку. Произвольные внешние источники событий через интерфейс не подключаются.
- **Сеть и обслуживание.** Нет мобильного приложения, облачного кабинета и доступа через браузер. Обновления устанавливаются из локального файла. VSX использует системное время Windows и не меняет часы.

**Перед эксплуатацией** проверьте обе передачи каждой камеры, запись и воспроизведение, поведение при заполнении диска, восстановление из копии и автозапуск после перезагрузки. Убедитесь, что видеонаблюдение и сроки хранения соответствуют применимым требованиям.

Об ошибках пишите на [vsx.core@mail.ru](mailto:vsx.core@mail.ru). Не прикладывайте пароли или рабочие базы данных.

## English

- **Installation.** Check the release notes for signing status and clean Windows 11 test results. An unsigned installer may trigger a Windows warning. Back up your data before upgrading; do not uninstall a working installation just to upgrade.
- **Cameras and performance.** A catalog of up to 128 cameras does not guarantee sustained operation of 128 simultaneous streams. Test grid and video wall performance on your hardware. Use standard quality for large grids and high quality for an expanded camera.
- **Compatibility.** ONVIF discovery, profiles, PTZ, and events depend on the camera model. If ONVIF is unavailable, try connecting manually via RTSP.
- **Analytics.** License plate recognition is not supported. Analytics across many cameras increases load. Custom models require a compatible package that passes local validation. Arbitrary external event sources cannot be configured through the interface.
- **Network and maintenance.** There is no mobile app, cloud portal, or browser access. Updates are installed from local files. VSX uses Windows system time without changing the clock.

**Before deployment**, test both streams from each camera, recording and playback, low-disk behavior, backup restoration, and automatic startup after reboot. Check that surveillance and retention comply with applicable requirements.

Report issues to [vsx.core@mail.ru](mailto:vsx.core@mail.ru). Do not attach passwords or production databases.

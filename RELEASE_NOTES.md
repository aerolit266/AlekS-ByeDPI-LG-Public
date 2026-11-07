# 0.6.32 Public Beta — release notes / Описание выпуска

## Русский

Первая отдельная публичная сборка на основе проверенной частной версии 0.6.31.

**Добавлено/сохранено:** единый IPK ARMv7/ARM64, локальный R656, автоматический выбор IP/LAN, отдельные служебный и видеомаршрут, R296 — подключение DNS к Cobalt после его запуска, журнал состояния и откат.

**Удалено:** два встроенных адреса VPS, исключение для домена частной инфраструктуры, весь отдельный модуль телеметрии и его автозапуск. В интерфейсе и манифестах версия 0.6.32.

**Ограничение:** эта сборка не проверена на настоящем ТВ; рабочая 0.6.31 сохранена без изменений. Не установлен автозапуск. Root и Homebrew обязательны. Не гарантируется запуск YouTube во всех сетях.

## English

First separate public beta derived from the user-confirmed private 0.6.31 baseline.

**Retained:** ARMv7/ARM64 one-file IPK, local R656 controller, automatic LAN IPv4 detection, separate control/media routes, R296 post-launch Cobalt DNS binding, status diagnostics and rollback.

**Removed:** two embedded private VPS IP literals, private infrastructure domain exclusion, entire opt-in telemetry module and its launch path. App, package and installer versions are consistently 0.6.32.

**Important:** This exact public build has **not** been hardware-tested. The working private 0.6.31 baseline is untouched. No persistent boot hook is installed. Root and Homebrew privileges are required, and YouTube is not guaranteed to work on every ISP/TV.

# <a name="automaticupdatemode-enum-type"></a>Тип перечисления automaticUpdateMode

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Возможные значения для режима автоматического обновления.
## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|userDefined|0|User Defined, значение по умолчанию, без цели.|
|notifyDownload|1|Уведомите при загрузке.|
|autoInstallAtMaintenanceTime|2|Автоматическая установка с во время обслуживания.|
|autoInstallAndRebootAtMaintenanceTime|3|Установить и перезагрузите во время обслуживания.|
|autoInstallAndRebootAtScheduledTime|4|Установить и перезагрузите компьютер в запланированное время.|
|autoInstallAndRebootWithoutEndUserControl|5|Установить и перезапустите без управления конечных пользователей|




# <a name="windows10teamgeneralconfiguration-resource-type"></a>Тип ресурса windows10TeamGeneralConfiguration

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

В этой статье описаны объявляемые методы, свойства и связи, которые предоставляются ресурсом windows10TeamGeneralConfiguration.

Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Перечисление объектов windows10TeamGeneralConfiguration](../api/intune_deviceconfig_windows10teamgeneralconfiguration_list.md)|Коллекция [windows10TeamGeneralConfiguration](../resources/intune_deviceconfig_windows10teamgeneralconfiguration.md)|Перечисление свойств и связей объектов [windows10TeamGeneralConfiguration](../resources/intune_deviceconfig_windows10teamgeneralconfiguration.md).|
|[Получение объекта windows10TeamGeneralConfiguration](../api/intune_deviceconfig_windows10teamgeneralconfiguration_get.md)|[windows10TeamGeneralConfiguration](../resources/intune_deviceconfig_windows10teamgeneralconfiguration.md)|Чтение свойств и связей объекта [windows10TeamGeneralConfiguration](../resources/intune_deviceconfig_windows10teamgeneralconfiguration.md).|
|[Создание объекта windows10TeamGeneralConfiguration](../api/intune_deviceconfig_windows10teamgeneralconfiguration_create.md)|[windows10TeamGeneralConfiguration](../resources/intune_deviceconfig_windows10teamgeneralconfiguration.md)|Создание объекта [windows10TeamGeneralConfiguration](../resources/intune_deviceconfig_windows10teamgeneralconfiguration.md).|
|[Удаление объекта windows10TeamGeneralConfiguration](../api/intune_deviceconfig_windows10teamgeneralconfiguration_delete.md)|Нет|Удаление объекта [windows10TeamGeneralConfiguration](../resources/intune_deviceconfig_windows10teamgeneralconfiguration.md).|
|[Обновление объекта windows10TeamGeneralConfiguration](../api/intune_deviceconfig_windows10teamgeneralconfiguration_update.md)|[windows10TeamGeneralConfiguration](../resources/intune_deviceconfig_windows10teamgeneralconfiguration.md)|Обновление свойств объекта [windows10TeamGeneralConfiguration](../resources/intune_deviceconfig_windows10teamgeneralconfiguration.md).|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|ид|Строка|Ключ объекта. Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта. Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|createdDateTime|DateTimeOffset|Дата и время создания объекта. Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|описание|Строка|Указанное администратором описание конфигурации устройства. Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|displayName|Строка|Указанное администратором имя конфигурации устройства. Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|версия|Int32|Версия конфигурации устройства. Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|azureOperationalInsightsBlockTelemetry|Логический|Указывает, следует ли заблокировать оперативную аналитику Azure.|
|azureOperationalInsightsWorkspaceId|Строка|Идентификатор рабочей области оперативной аналитики Azure.|
|azureOperationalInsightsWorkspaceKey|Строка|Ключ рабочей области оперативной аналитики Azure.|
|connectAppBlockAutoLaunch|Логический|Указывает, следует ли автоматически запускать приложение Connect, когда начинается проекция.|
|maintenanceWindowBlocked|Логический|Указывает, следует ли запретить устанавливать период обслуживания для обновлений устройства.|
|maintenanceWindowDurationInHours|Int32|Длительность периода обслуживания для обновлений устройства. Допустимые значения: от 0 до 5|
|maintenanceWindowStartTime|TimeOfDay|Начало периода обслуживания для обновлений устройства.|
|miracastChannel|[miracastChannel](../resources/intune_deviceconfig_miracastchannel.md)|Канал. Возможные значения: `userDefined`, `one`, `two`, `three`, `four`, `five`, `six`, `seven`, `eight`, `nine`, `ten`, `eleven`, `thirtySix`, `forty`, `fortyFour`, `fortyEight`, `oneHundredFortyNine`, `oneHundredFiftyThree`, `oneHundredFiftySeven`, `oneHundredSixtyOne`, `oneHundredSixtyFive`.|
|miracastBlocked|Логический|Указывает, следует ли заблокировать беспроводное проецирование.|
|miracastRequirePin|Логический|Указывает, обязательно ли использовать ПИН-код для беспроводного проецирования.|
|settingsBlockMyMeetingsAndFiles|Логический|Указывает, следует ли отключить функцию "Мои встречи и файлы" в меню "Пуск", которая показывает собрания и файлы вошедшего пользователя из Office 365.|
|settingsBlockSessionResume|Логический|Указывает, следует ли разрешить возобновление сеанса после истечения времени.|
|settingsBlockSigninSuggestions|Логический|Указывает, следует ли отключить автоматическое добавление в диалоговое окно входа приглашенных из запланированных собраний.|
|settingsDefaultVolume|Int32|Задает объем нового сеанса по умолчанию. Допустимые значения: от 0 до 100. Значение по умолчанию — 45. Допустимые значения: от 0 до 100|
|settingsScreenTimeoutInMinutes|Int32|Определяет время до отключения экрана Центра (в минутах).|
|settingsSessionTimeoutInMinutes|Int32|Определяет время до истечения времени сеанса (в минутах).|
|settingsSleepTimeoutInMinutes|Int32|Определяет время до перехода Центра в спящий режим (в минутах).|
|welcomeScreenBlockAutomaticWakeUp|Логический|Указывает, следует ли заблокировать автоматический вывод экрана приветствия из спящего режима, когда кто-то входит в комнату.|
|welcomeScreenBackgroundImageUrl|Строка|URL-адрес фонового изображения экрана приветствия. URL-адрес должен начинаться с протокола HTTPS и возвращать PNG-изображение.|
|welcomeScreenMeetingInformation|[welcomeScreenMeetingInformation](../resources/intune_deviceconfig_welcomescreenmeetinginformation.md)|Информация о собраниях, показываемая на экране приветствия. Возможные значения: `userDefined`, `showOrganizerAndTimeOnly`, `showOrganizerAndTimeAndSubject`.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|задания|Коллекция [deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md)|Список назначений для профиля конфигурации устройства. Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|deviceStatuses|Коллекция [deviceConfigurationDeviceStatus](../resources/intune_deviceconfig_deviceconfigurationdevicestatus.md)|Состояние установки конфигурации для каждого устройства. Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|userStatuses|Коллекция [deviceConfigurationUserStatus](../resources/intune_deviceconfig_deviceconfigurationuserstatus.md)|Состояние установки конфигурации устройства пользователем. Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune_deviceconfig_deviceconfigurationdeviceoverview.md)|Обзор состояния конфигурации по устройствам. Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune_deviceconfig_deviceconfigurationuseroverview.md)|Обзор состояния конфигурации устройств по пользователям. Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|deviceSettingStateSummaries|Коллекция [settingStateDeviceSummary](../resources/intune_deviceconfig_settingstatedevicesummary.md)|Обзор состояния параметров конфигурации устройств по пользователям. Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.deviceConfiguration",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windows10TeamGeneralConfiguration"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.windows10TeamGeneralConfiguration",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "version": 1024,
  "azureOperationalInsightsBlockTelemetry": true,
  "azureOperationalInsightsWorkspaceId": "String",
  "azureOperationalInsightsWorkspaceKey": "String",
  "connectAppBlockAutoLaunch": true,
  "maintenanceWindowBlocked": true,
  "maintenanceWindowDurationInHours": 1024,
  "maintenanceWindowStartTime": "String (time of day)",
  "miracastChannel": "String",
  "miracastBlocked": true,
  "miracastRequirePin": true,
  "settingsBlockMyMeetingsAndFiles": true,
  "settingsBlockSessionResume": true,
  "settingsBlockSigninSuggestions": true,
  "settingsDefaultVolume": 1024,
  "settingsScreenTimeoutInMinutes": 1024,
  "settingsSessionTimeoutInMinutes": 1024,
  "settingsSleepTimeoutInMinutes": 1024,
  "welcomeScreenBlockAutomaticWakeUp": true,
  "welcomeScreenBackgroundImageUrl": "String",
  "welcomeScreenMeetingInformation": "String"
}
```









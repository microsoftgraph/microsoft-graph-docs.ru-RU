---
title: Тип ресурса windows10TeamGeneralConfiguration
description: В этой статье описаны объявляемые методы, свойства и связи, которые предоставляются ресурсом windows10TeamGeneralConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 8051df445b10887d79a88c2c17f8d845776f5a1d
ms.sourcegitcommit: 7bc623e73fdfb970dbd0a62154d10bb2863afaf7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/07/2022
ms.locfileid: "66671207"
---
# <a name="windows10teamgeneralconfiguration-resource-type"></a>Тип ресурса windows10TeamGeneralConfiguration

Пространство имен: microsoft.graph

> **Важно:** API Microsoft Graph в версии /beta могут быть изменены; использование в рабочей области не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

В этой статье описаны объявляемые методы, свойства и связи, которые предоставляются ресурсом windows10TeamGeneralConfiguration.


Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Перечисление объектов windows10TeamGeneralConfiguration](../api/intune-deviceconfig-windows10teamgeneralconfiguration-list.md)|Коллекция [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md)|Перечисление свойств и связей объектов [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md).|
|[Получение объекта windows10TeamGeneralConfiguration](../api/intune-deviceconfig-windows10teamgeneralconfiguration-get.md)|[windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md)|Чтение свойств и связей объекта [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md).|
|[Создание объекта windows10TeamGeneralConfiguration](../api/intune-deviceconfig-windows10teamgeneralconfiguration-create.md)|[windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md)|Создание объекта [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md).|
|[Удаление объекта windows10TeamGeneralConfiguration](../api/intune-deviceconfig-windows10teamgeneralconfiguration-delete.md)|Нет|Удаление объекта [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md).|
|[Обновление объекта windows10TeamGeneralConfiguration](../api/intune-deviceconfig-windows10teamgeneralconfiguration-update.md)|[windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md)|Обновление свойств объекта [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md).|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|Идентификаторы roleScopeTagId|Коллекция String|Список тегов области для этого экземпляра сущности. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|supportsScopeTags|Логическое|Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области. Назначение свойству ScopeTags не допускается, если это значение имеет значение false и сущности не будут видны пользователям с заданной областью. Это происходит для устаревших политик, созданных в Silverlight, и их можно устранить, удалив и повторно создав политику на портале Azure. Это свойство доступно только для чтения. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|deviceManagementApplicabilityRuleOsEdition|[deviceManagementApplicabilityRuleOsEdition](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|Применимость выпуска ОС для этой политики. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|deviceManagementApplicabilityRuleOsVersion|[deviceManagementApplicabilityRuleOsVersion](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|Правило применимости версии ОС для этой политики. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|deviceManagementApplicabilityRuleDeviceMode|[deviceManagementApplicabilityRuleDeviceMode](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|Правило применимости режима устройства для этой политики. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|createdDateTime|DateTimeOffset|Дата и время создания объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|description|String|Указанное администратором описание конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|displayName|String|Указанное администратором имя конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|version|Int32|Версия конфигурации устройства. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|azureOperationalInsightsBlockTelemetry|Boolean|Указывает, следует ли заблокировать оперативную аналитику Azure.|
|azureOperationalInsightsWorkspaceId|String|Идентификатор рабочей области оперативной аналитики Azure.|
|azureOperationalInsightsWorkspaceKey|String|Ключ рабочей области оперативной аналитики Azure.|
|connectAppBlockAutoLaunch|Boolean|Указывает, следует ли автоматически запускать приложение Connect, когда начинается проекция.|
|maintenanceWindowBlocked|Boolean|Указывает, следует ли запретить устанавливать период обслуживания для обновлений устройства.|
|maintenanceWindowDurationInHours|Int32|Длительность периода обслуживания для обновлений устройства. Допустимые значения: от 0 до 5|
|maintenanceWindowStartTime|TimeOfDay|Начало периода обслуживания для обновлений устройства.|
|miracastChannel|[miracastChannel](../resources/intune-deviceconfig-miracastchannel.md)|Канал. Возможные значения: `userDefined`, `one`, `two`, `three`, `four`, `five`, `six`, `seven`, `eight`, `nine`, `ten`, `eleven`, `thirtySix`, `forty`, `fortyFour`, `fortyEight`, `oneHundredFortyNine`, `oneHundredFiftyThree`, `oneHundredFiftySeven`, `oneHundredSixtyOne`, `oneHundredSixtyFive`.|
|miracastBlocked|Boolean|Указывает, следует ли заблокировать беспроводное проецирование.|
|miracastRequirePin|Boolean|Указывает, обязательно ли использовать ПИН-код для беспроводного проецирования.|
|settingsBlockMyMeetingsAndFiles|Boolean|Указывает, следует ли отключить функцию "Мои встречи и файлы" в меню "Пуск", которая показывает собрания и файлы вошедшего пользователя из Office 365.|
|settingsBlockSessionResume|Boolean|Указывает, следует ли разрешить возобновление сеанса после истечения времени.|
|settingsBlockSigninSuggestions|Boolean|Указывает, следует ли отключить автоматическое добавление в диалоговое окно входа приглашенных из запланированных собраний.|
|settingsDefaultVolume|Int32|Задает объем нового сеанса по умолчанию. Допустимые значения: от 0 до 100. Значение по умолчанию — 45. Допустимые значения: от 0 до 100|
|settingsScreenTimeoutInMinutes|Int32|Определяет время до отключения экрана Центра (в минутах).|
|settingsSessionTimeoutInMinutes|Int32|Определяет время до истечения времени сеанса (в минутах).|
|settingsSleepTimeoutInMinutes|Int32|Определяет время до перехода Центра в спящий режим (в минутах).|
|welcomeScreenBlockAutomaticWakeUp|Boolean|Указывает, следует ли заблокировать автоматический вывод экрана приветствия из спящего режима, когда кто-то входит в комнату.|
|welcomeScreenBackgroundImageUrl|String|URL-адрес фонового изображения экрана приветствия. URL-адрес должен начинаться с протокола HTTPS и возвращать PNG-изображение.|
|welcomeScreenMeetingInformation|[welcomeScreenMeetingInformation](../resources/intune-deviceconfig-welcomescreenmeetinginformation.md)|Информация о собраниях, показываемая на экране приветствия. Возможные значения: `userDefined`, `showOrganizerAndTimeOnly`, `showOrganizerAndTimeAndSubject`.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|groupAssignments|[Коллекция deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)|Список назначений групп для профиля конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|assignments|Коллекция [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|Список назначений для профиля конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|deviceStatuses|Коллекция [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md)|Состояние установки конфигурации для каждого устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|userStatuses|Коллекция [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md)|Состояние установки конфигурации устройства по пользователю. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|Обзор состояния конфигурации устройств. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|Обзор состояния конфигурации устройств для пользователей. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|deviceSettingStateSummaries|Коллекция [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)|Сводка данных о состоянии настройки конфигурации устройств. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windows10TeamGeneralConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windows10TeamGeneralConfiguration",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "roleScopeTagIds": [
    "String"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "String"
    ],
    "name": "String",
    "ruleType": "String"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "String",
    "maxOSVersion": "String",
    "name": "String",
    "ruleType": "String"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "String",
    "name": "String",
    "ruleType": "String"
  },
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





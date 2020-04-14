---
title: Тип ресурса Виндовсделиверйоптимизатионконфигуратион
description: Конфигурация оптимизации доставки Windows
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 833e674c720cb774b794c54e55fc672ed174ac8e
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43473638"
---
# <a name="windowsdeliveryoptimizationconfiguration-resource-type"></a>Тип ресурса Виндовсделиверйоптимизатионконфигуратион

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Конфигурация оптимизации доставки Windows


Наследуется от [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Виндовсделиверйоптимизатионконфигуратионс](../api/intune-deviceconfig-windowsdeliveryoptimizationconfiguration-list.md)|Коллекция [виндовсделиверйоптимизатионконфигуратион](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md)|Список свойств и связей объектов [виндовсделиверйоптимизатионконфигуратион](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md) .|
|[Получение Виндовсделиверйоптимизатионконфигуратион](../api/intune-deviceconfig-windowsdeliveryoptimizationconfiguration-get.md)|[виндовсделиверйоптимизатионконфигуратион](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md)|Чтение свойств и связей объекта [виндовсделиверйоптимизатионконфигуратион](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md) .|
|[Создание Виндовсделиверйоптимизатионконфигуратион](../api/intune-deviceconfig-windowsdeliveryoptimizationconfiguration-create.md)|[виндовсделиверйоптимизатионконфигуратион](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md)|Создание нового объекта [виндовсделиверйоптимизатионконфигуратион](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md) .|
|[Удаление Виндовсделиверйоптимизатионконфигуратион](../api/intune-deviceconfig-windowsdeliveryoptimizationconfiguration-delete.md)|Нет|Удаляет объект [виндовсделиверйоптимизатионконфигуратион](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md).|
|[Обновление Виндовсделиверйоптимизатионконфигуратион](../api/intune-deviceconfig-windowsdeliveryoptimizationconfiguration-update.md)|[виндовсделиверйоптимизатионконфигуратион](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md)|Обновление свойств объекта [виндовсделиверйоптимизатионконфигуратион](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|roleScopeTagIds|Коллекция String|Список тегов областей для этого экземпляра сущности. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|суппортсскопетагс|Boolean|Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области. Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия. Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure. Это свойство доступно только для чтения. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|deviceManagementApplicabilityRuleOsEdition|[deviceManagementApplicabilityRuleOsEdition](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|Применимость выпусков ОС для этой политики. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|deviceManagementApplicabilityRuleOsVersion|[deviceManagementApplicabilityRuleOsVersion](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|Правило применимости версии ОС для этой политики. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|deviceManagementApplicabilityRuleDeviceMode|[deviceManagementApplicabilityRuleDeviceMode](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|Правило применимости режима устройства для этой политики. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|createdDateTime|DateTimeOffset|Дата и время создания объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|description|String|Указанное администратором описание конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|displayName|Строка|Указанное администратором имя конфигурации устройства. Наследуется от [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|version|Int32|Версия конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|deliveryOptimizationMode|[виндовсделиверйоптимизатионмоде](../resources/intune-deviceconfig-windowsdeliveryoptimizationmode.md)|Указывает метод загрузки, который можно использовать для управления пропускной способностью сети для сценариев распространения большого контента. Возможные значения: `userDefined`, `httpOnly`, `httpWithPeeringNat`, `httpWithPeeringPrivateGroup`, `httpWithInternetPeering`, `simpleDownload`, `bypassMode`.|
|рестриктпирселектионби|[deliveryOptimizationRestrictPeerSelectionByOptions](../resources/intune-deviceconfig-deliveryoptimizationrestrictpeerselectionbyoptions.md)|Задает ограничение выбора однорангового узла с помощью выбранного параметра.
Вариант 1 (маска подсети) применяется только к режимам оптимизации доставки LAN (1) и Group (2). Возможные значения: `notConfigured`, `subnetMask`.|
|граупидсаурце|[deliveryOptimizationGroupIdSource](../resources/intune-deviceconfig-deliveryoptimizationgroupidsource.md)|Задает ограничение выбора однорангового узла для источника получать.
Параметры, заданные в этой политике, применяются только к режиму загрузки группы режима оптимизации доставки (2). Если группа (2) не установлена в режиме загрузки, эта политика будет игнорироваться. Для варианта 3 — идентификатор параметра DHCP клиент будет запрашивать параметр DHCP с ИДЕНТИФИКАТОРом 234 и использовать возвращенное значение GUID в качестве идентификатора группы.|
|бандвидсмоде|[deliveryOptimizationBandwidth](../resources/intune-deviceconfig-deliveryoptimizationbandwidth.md)|Указывает фоновую и фоновую пропускную способность при использовании процентных значений, абсолютных или часов.|
|баккграунддовнлоадфромхттпделайинсекондс|Int64|Указывает время в секундах, в течение которого HTTP-источник задерживается в фоновой загрузке, для которого разрешено использование однорангового подключения. Допустимые значения — от 0 до 4294967295|
|фореграунддовнлоадфромхттпделайинсекондс|Int64|Указывает время (в секундах), в течение которого источник HTTP загружается в фоновом режиме загрузки, для которого разрешено использование одноранговой сети (0-86400). Допустимые значения — от 0 до 86400
Значение 0 задает оптимизацию доставки для управления этим параметром с помощью облачной службы. Допустимые значения — от 0 до 86400|
|минимумрамалловедтопирингигабитес|Int32|Указывает минимальный размер ОЗУ в ГБ для использования однорангового кэширования (1-100000). Допустимые значения — от 1 до 100000|
|минимумдисксизеалловедтопирингигабитес|Int32|Указывает минимальный размер диска в ГБ для использования однорангового кэширования (1-100000). Допустимые значения — от 1 до 100000
Рекомендуемые значения: 64 ГБ до 256 ГБ. Допустимые значения — от 1 до 100000|
|минимумфилесизетокачеинмегабитес|Int32|Указывает минимальный размер файла контента в МЕГАБАЙТах, поддерживающий одноранговое кэширование (1-100000). Допустимые значения — от 1 до 100000
Рекомендуемые значения: от 1 МБ до 100 000 МБ. Допустимые значения — от 1 до 100000|
|минимумбаттериперцентажеалловедтауплоад|Int32|Указывает минимальный процент батареи, позволяющий устройству отправлять данные (0-100). Допустимые значения: от 0 до 100
Значение по умолчанию равно 0. Значение 0 (ноль) означает "не ограничено", будет использоваться значение по умолчанию для облачной службы. Допустимые значения: от 0 до 100|
|модификачелокатион|String|Указывает диск, который должна использовать оптимизация доставки для своего кэша.|
|максимумкачеажеиндайс|Int32|Указывает максимальное время (в днях), в течение которого каждый файл хранится в кэше оптимизации доставки после успешного скачивания (0-3650). Допустимые значения — от 0 до 3650|
|максимумкачесизе|[deliveryOptimizationMaxCacheSize](../resources/intune-deviceconfig-deliveryoptimizationmaxcachesize.md)|Задает максимальный размер кэша для оптимизации доставки: в процентах или в ГБ.|
|впнпиркачинг|[Включение](../resources/intune-shared-enablement.md)|Указывает, разрешено ли устройству принимать участие в одноранговом кэшировании при подключении через VPN к доменной сети. Возможные значения: `notConfigured`, `enabled`, `disabled`.|
|качесерверхостнамес|Коллекция String|Указывает имена узлов серверов кэша.|
|качесерверфореграунддовнлоадфаллбакктохттпделайинсекондс|Int32|Указывает время (в секундах), по истечении которого откладывается обратное сообщение от серверов кэша к источнику HTTP для загрузки переднего плана. Допустимые значения: от 0 до 2592000.|
|качесервербаккграунддовнлоадфаллбакктохттпделайинсекондс|Int32|Указывает время (в секундах), по истечении которого будет возвращаться обратно от серверов кэша к источнику HTTP для загрузки в фоновом режиме. Допустимые значения: от 0 до 2592000.|

## <a name="relationships"></a>Отношения
|Связь|Тип|Описание|
|:---|:---|:---|
|groupAssignments|Коллекция [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)|Список назначений групп для профиля конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|assignments|Коллекция [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|Список назначений для профиля конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|deviceStatuses|Коллекция [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md)|Состояние установки конфигурации для каждого устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|userStatuses|Коллекция [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md)|Состояние установки конфигурации устройств пользователем. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|Обзор состояния конфигурации устройств. Наследуется от [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|Обзор состояния конфигурации устройств для пользователей. Наследуется от [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|deviceSettingStateSummaries|Коллекция [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)|Сводка данных о состоянии настройки конфигурации устройств. Наследуется от [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsDeliveryOptimizationConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsDeliveryOptimizationConfiguration",
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
  "deliveryOptimizationMode": "String",
  "restrictPeerSelectionBy": "String",
  "groupIdSource": {
    "@odata.type": "microsoft.graph.deliveryOptimizationGroupIdSource"
  },
  "bandwidthMode": {
    "@odata.type": "microsoft.graph.deliveryOptimizationBandwidth"
  },
  "backgroundDownloadFromHttpDelayInSeconds": 1024,
  "foregroundDownloadFromHttpDelayInSeconds": 1024,
  "minimumRamAllowedToPeerInGigabytes": 1024,
  "minimumDiskSizeAllowedToPeerInGigabytes": 1024,
  "minimumFileSizeToCacheInMegabytes": 1024,
  "minimumBatteryPercentageAllowedToUpload": 1024,
  "modifyCacheLocation": "String",
  "maximumCacheAgeInDays": 1024,
  "maximumCacheSize": {
    "@odata.type": "microsoft.graph.deliveryOptimizationMaxCacheSize"
  },
  "vpnPeerCaching": "String",
  "cacheServerHostNames": [
    "String"
  ],
  "cacheServerForegroundDownloadFallbackToHttpDelayInSeconds": 1024,
  "cacheServerBackgroundDownloadFallbackToHttpDelayInSeconds": 1024
}
```




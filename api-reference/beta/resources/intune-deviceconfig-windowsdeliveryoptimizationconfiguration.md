---
title: Тип ресурса Виндовсделиверйоптимизатионконфигуратион
description: Конфигурация оптимизации доставки Windows
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 62fef7e874f004c28f71287895e84005c93905b4
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30162092"
---
# <a name="windowsdeliveryoptimizationconfiguration-resource-type"></a>Тип ресурса Виндовсделиверйоптимизатионконфигуратион

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Конфигурация оптимизации доставки Windows


Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Виндовсделиверйоптимизатионконфигуратионс](../api/intune-deviceconfig-windowsdeliveryoptimizationconfiguration-list.md)|Коллекция [виндовсделиверйоптимизатионконфигуратион](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md)|Список свойств и связей объектов [виндовсделиверйоптимизатионконфигуратион](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md) .|
|[Получение Виндовсделиверйоптимизатионконфигуратион](../api/intune-deviceconfig-windowsdeliveryoptimizationconfiguration-get.md)|[Виндовсделиверйоптимизатионконфигуратион](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md)|Чтение свойств и связей объекта [виндовсделиверйоптимизатионконфигуратион](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md) .|
|[Создание Виндовсделиверйоптимизатионконфигуратион](../api/intune-deviceconfig-windowsdeliveryoptimizationconfiguration-create.md)|[Виндовсделиверйоптимизатионконфигуратион](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md)|Создание нового объекта [виндовсделиверйоптимизатионконфигуратион](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md) .|
|[Удаление Виндовсделиверйоптимизатионконфигуратион](../api/intune-deviceconfig-windowsdeliveryoptimizationconfiguration-delete.md)|Нет|Удаляет объект [виндовсделиверйоптимизатионконфигуратион](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md).|
|[Обновление Виндовсделиверйоптимизатионконфигуратион](../api/intune-deviceconfig-windowsdeliveryoptimizationconfiguration-update.md)|[Виндовсделиверйоптимизатионконфигуратион](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md)|Обновление свойств объекта [виндовсделиверйоптимизатионконфигуратион](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|roleScopeTagIds|Коллекция строк|Список тегов областей для этого экземпляра сущности. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|Суппортсскопетагс|Логический|Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области. Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия. Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure. Это свойство доступно только для чтения. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|createdDateTime|DateTimeOffset|Дата и время создания объекта. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|description|String|Указанное администратором описание конфигурации устройства. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|displayName|String|Указанное администратором имя конфигурации устройства. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|version|Int32|Версия конфигурации устройства. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|deliveryOptimizationMode|[Виндовсделиверйоптимизатионмоде](../resources/intune-deviceconfig-windowsdeliveryoptimizationmode.md)|Указывает метод загрузки, который можно использовать для управления пропускной способностью сети для сценариев распространения большого контента. Возможные значения: `userDefined`, `httpOnly`, `httpWithPeeringNat`, `httpWithPeeringPrivateGroup`, `httpWithInternetPeering`, `simpleDownload`, `bypassMode`.|
|Рестриктпирселектионби|[deliveryOptimizationRestrictPeerSelectionByOptions](../resources/intune-deviceconfig-deliveryoptimizationrestrictpeerselectionbyoptions.md)|Задает ограничение выбора однорангового узла с помощью выбранного параметра.
Вариант 1 (маска подСети) применяется только к режимам оптимизации доставки LAN (1) и Group (2). Возможные значения: `notConfigured`, `subnetMask`.|
|Граупидсаурце|[deliveryOptimizationGroupIdSource](../resources/intune-deviceconfig-deliveryoptimizationgroupidsource.md)|Задает ограничение выбора однорангового узла для источника получать.
Параметры, заданные в этой политике, применяются только к режиму загрузки группы режима оптимизации доставки (2). Если группа (2) не установлена в режиме загрузки, эта политика будет игнорироваться. Для варианта 3 — идентификатор параметра DHCP клиент будет запрашивать параметр DHCP с ИДЕНТИФИКАТОРом 234 и использовать возвращенное значение GUID в качестве идентификатора группы.|
|Бандвидсмоде|[deliveryOptimizationBandwidth](../resources/intune-deviceconfig-deliveryoptimizationbandwidth.md)|Указывает фоновую и фоновую пропускную способность при использовании процентных значений, абсолютных или часов.|
|Баккграунддовнлоадфромхттпделайинсекондс|Int64|Указывает время в секундах, в течение которого HTTP-источник задерживается в фоновой загрузке, для которого разрешено использование однорангового подключения. Допустимые значения — от 0 до 4294967295|
|Фореграунддовнлоадфромхттпделайинсекондс|Int64|Указывает время (в секундах), в течение которого источник HTTP загружается в фоновом режиме загрузки, для которого разрешено использование одноранговой сети (0-86400). Допустимые значения — от 0 до 86400
Значение 0 задает оптимизацию доставки для управления этим параметром с помощью облачной службы. Допустимые значения — от 0 до 86400|
|Минимумрамалловедтопирингигабитес|Int32|Указывает минимальный размер ОЗУ в ГБ для использования одноРангового кэширования (1-100000). Допустимые значения — от 1 до 100000|
|Минимумдисксизеалловедтопирингигабитес|Int32|Указывает минимальный размер диска в ГБ для использования одноРангового кэширования (1-100000). Допустимые значения — от 1 до 100000
Рекомендуемые значения: 64 ГБ до 256 ГБ. Допустимые значения — от 1 до 100000|
|Минимумфилесизетокачеинмегабитес|Int32|Указывает минимальный размер файла контента в МЕГАБАЙТах, поддерживающий одноранговое кэширование (1-100000). Допустимые значения — от 1 до 100000
Рекомендуемые значения: от 1 МБ до 100 000 МБ. Допустимые значения — от 1 до 100000|
|Минимумбаттериперцентажеалловедтауплоад|Int32|Указывает минимальный процент батареи, позволяющий устройству отправлять данные (0-100). Допустимые значения: от 0 до 100
Значение по умолчанию равно 0. Значение 0 (ноль) означает "не ограничено", будет использоваться значение по умолчанию для облачной службы. Допустимые значения: от 0 до 100|
|Модификачелокатион|String|Указывает диск, который должна использовать оптимизация доставки для своего кэша.|
|Максимумкачеажеиндайс|Int32|Указывает максимальное время (в днях), в течение которого каждый файл хранится в кэше оптимизации доставки после успешного скачивания (0-49710). Допустимые значения — от 0 до 49710|
|Максимумкачесизе|[deliveryOptimizationMaxCacheSize](../resources/intune-deviceconfig-deliveryoptimizationmaxcachesize.md)|Задает максимальный размер кэша для оптимизации доставки: в процентах или в ГБ.|
|Впнпиркачинг|[Включение](../resources/intune-shared-enablement.md)|Указывает, разрешено ли устройству принимать участие в одноранговом кэшировании при подключении через VPN к доменной сети. Возможные значения: `notConfigured`, `enabled`, `disabled`.|

## <a name="relationships"></a>Связи
|Отношение|Тип|Описание|
|:---|:---|:---|
|groupAssignments|Коллекция [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)|Список назначений групп для профиля конфигурации устройства. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|assignments|Коллекция [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|Список назначений для профиля конфигурации устройства. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|deviceStatuses|Коллекция [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md)|Состояние установки конфигурации для каждого устройства. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|userStatuses|Коллекция [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md)|Состояние установки конфигурации устройств пользователем. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|Обзор состояния конфигурации по устройствам. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|Обзор состояния конфигурации устройств по пользователям. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|deviceSettingStateSummaries|Коллекция [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)|Обзор состояния параметров конфигурации устройств по пользователям. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|

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
  "vpnPeerCaching": "String"
}
```





---
title: Тип ресурса iosWiFiConfiguration
description: Предоставляя конфигурации в этом профиле, вы можете указать устройству iOS подключаться к необходимой конечной точке Wi-Fi. Указав способ проверки подлинности и типы безопасности, ожидаемые конечной точкой Wi-Fi, вы можете сделать Wi-Fi подключение неполноценным для конечного пользователя. Этот профиль предоставляет ограниченные и простые типы безопасности, чем корпоративный Wi-Fi профиль.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 3f03ac6c6e110cea72a0574f0c9ea226e8089ddf
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48701531"
---
# <a name="ioswificonfiguration-resource-type"></a>Тип ресурса iosWiFiConfiguration

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Предоставляя конфигурации в этом профиле, вы можете указать устройству iOS подключаться к необходимой конечной точке Wi-Fi. Указав способ проверки подлинности и типы безопасности, ожидаемые конечной точкой Wi-Fi, вы можете сделать Wi-Fi подключение неполноценным для конечного пользователя. Этот профиль предоставляет ограниченные и простые типы безопасности, чем корпоративный Wi-Fi профиль.


Наследуется от [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Иосвификонфигуратионс](../api/intune-deviceconfig-ioswificonfiguration-list.md)|Коллекция [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)|Список свойств и связей объектов [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md) .|
|[Получение iosWiFiConfiguration](../api/intune-deviceconfig-ioswificonfiguration-get.md)|[iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)|Чтение свойств и связей объекта [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md) .|
|[Создание iosWiFiConfiguration](../api/intune-deviceconfig-ioswificonfiguration-create.md)|[iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)|Создание нового объекта [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md) .|
|[Удаление iosWiFiConfiguration](../api/intune-deviceconfig-ioswificonfiguration-delete.md)|Нет|Удаляет объект [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md).|
|[Обновление iosWiFiConfiguration](../api/intune-deviceconfig-ioswificonfiguration-update.md)|[iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)|Обновление свойств объекта [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Ключ объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|roleScopeTagIds|Коллекция строк|Список тегов областей для этого экземпляра сущности. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|суппортсскопетагс|Логический|Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области. Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия. Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure. Это свойство доступно только для чтения. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|deviceManagementApplicabilityRuleOsEdition|[deviceManagementApplicabilityRuleOsEdition](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|Применимость выпусков ОС для этой политики. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|deviceManagementApplicabilityRuleOsVersion|[deviceManagementApplicabilityRuleOsVersion](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|Правило применимости версии ОС для этой политики. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|deviceManagementApplicabilityRuleDeviceMode|[deviceManagementApplicabilityRuleDeviceMode](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|Правило применимости режима устройства для этой политики. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|createdDateTime|DateTimeOffset|Дата и время создания объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|description|Строка|Указанное администратором описание конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|displayName|Строка|Указанное администратором имя конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|version|Int32|Версия конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|нетворкнаме|Строка|Сетевое имя|
|SSID|Строка|Это имя Wi-Fiной сети, которая отправляется на все устройства.|
|коннектаутоматикалли|Логический|Подключаться автоматически, если сеть находится в диапазоне. Если задать для этого параметра значение true, запрос пользователя будет пропущен и устройство будет автоматически подключено к Wi-Fi сети.|
|коннектвхеннетворкнамеишидден|Логический|Подключаться, если сеть не ведет вещание своего имени (SSID). Если задано значение true, этот профиль заставляет устройство подключаться к сети, на которой не выполняется трансляция идентификатора SSID на все устройства.|
|вифисекурититипе|[вифисекурититипе](../resources/intune-deviceconfig-wifisecuritytype.md)|Указывает, использует ли конечная точка Wi-Fi тип безопасности на основе EAP. Возможные значения: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.|
|proxySettings|[вифипроксисеттинг](../resources/intune-deviceconfig-wifiproxysetting.md)|Тип прокси-сервера для этого подключения Wi-Fi. Возможные значения: `none`, `manual`, `automatic`.|
|проксимануаладдресс|Строка|IP-адрес или DNS-имя узла прокси-сервера при выборе конфигурации вручную.|
|проксимануалпорт|Int32|Порт прокси-сервера при выборе конфигурации вручную.|
|проксяутоматикконфигуратионурл|Строка|URL-адрес скрипта автоматической настройки прокси-сервера при выборе параметра Автоматическая настройка. Обычно это URL-адрес файла PAC (Автонастройка прокси-сервера).|
|дисаблемакаддрессрандомизатион|Логический|Если задано значение true, устройства, подключающиеся с помощью данного профиля Wi-Fi, предоставляют свои фактические Wi-Fi MAC-адреса вместо случайного MAC-адреса. Применяется к iOS 14 и более поздних версий.|
|preSharedKey|Строка|Это предварительно общий ключ для сети WPA Personal Wi-Fi.|

## <a name="relationships"></a>Связи
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
  "@odata.type": "microsoft.graph.iosWiFiConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosWiFiConfiguration",
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
  "networkName": "String",
  "ssid": "String",
  "connectAutomatically": true,
  "connectWhenNetworkNameIsHidden": true,
  "wiFiSecurityType": "String",
  "proxySettings": "String",
  "proxyManualAddress": "String",
  "proxyManualPort": 1024,
  "proxyAutomaticConfigurationUrl": "String",
  "disableMacAddressRandomization": true,
  "preSharedKey": "String"
}
```






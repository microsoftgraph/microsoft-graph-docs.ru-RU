---
title: Тип ресурса Макосвпнконфигуратион
description: Предоставляя конфигурации в этом профиле, вы можете указать Mac-устройству подключаться к необходимой конечной точке VPN. Указав способ проверки подлинности и типы безопасности, ожидаемые конечной точкой VPN, вы можете сделать VPN-подключение неполноценным для конечного пользователя.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2dd5626ea0129b87a36c1fcb823d57dd8e5fa3e8
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30147686"
---
# <a name="macosvpnconfiguration-resource-type"></a>Тип ресурса Макосвпнконфигуратион

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Предоставляя конфигурации в этом профиле, вы можете указать Mac-устройству подключаться к необходимой конечной точке VPN. Указав способ проверки подлинности и типы безопасности, ожидаемые конечной точкой VPN, вы можете сделать VPN-подключение неполноценным для конечного пользователя.


НаСледуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Макосвпнконфигуратионс](../api/intune-deviceconfig-macosvpnconfiguration-list.md)|Коллекция [макосвпнконфигуратион](../resources/intune-deviceconfig-macosvpnconfiguration.md)|Список свойств и связей объектов [макосвпнконфигуратион](../resources/intune-deviceconfig-macosvpnconfiguration.md) .|
|[Получение Макосвпнконфигуратион](../api/intune-deviceconfig-macosvpnconfiguration-get.md)|[Макосвпнконфигуратион](../resources/intune-deviceconfig-macosvpnconfiguration.md)|Чтение свойств и связей объекта [макосвпнконфигуратион](../resources/intune-deviceconfig-macosvpnconfiguration.md) .|
|[Создание Макосвпнконфигуратион](../api/intune-deviceconfig-macosvpnconfiguration-create.md)|[Макосвпнконфигуратион](../resources/intune-deviceconfig-macosvpnconfiguration.md)|Создание нового объекта [макосвпнконфигуратион](../resources/intune-deviceconfig-macosvpnconfiguration.md) .|
|[Удаление Макосвпнконфигуратион](../api/intune-deviceconfig-macosvpnconfiguration-delete.md)|Нет|Удаляет объект [макосвпнконфигуратион](../resources/intune-deviceconfig-macosvpnconfiguration.md).|
|[Обновление Макосвпнконфигуратион](../api/intune-deviceconfig-macosvpnconfiguration-update.md)|[Макосвпнконфигуратион](../resources/intune-deviceconfig-macosvpnconfiguration.md)|Обновление свойств объекта [макосвпнконфигуратион](../resources/intune-deviceconfig-macosvpnconfiguration.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|roleScopeTagIds|Коллекция строк|Список тегов областей для этого экземпляра сущности. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|Суппортсскопетагс|Логический|Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области. Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия. Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure. Это свойство доступно только для чтения. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|createdDateTime|DateTimeOffset|Дата и время создания объекта. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|description|String|Указанное администратором описание конфигурации устройства. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|displayName|String|Указанное администратором имя конфигурации устройства. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|version|Int32|Версия конфигурации устройства. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|Коннектионнаме|String|Имя подключения, отображаемое для пользователя. НаСледуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)|
|connectionType|[Апплевпнконнектионтипе](../resources/intune-deviceconfig-applevpnconnectiontype.md)|Тип подключения. НаСледуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md). Возможные значения: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `customVpn`, `ciscoIPSec`, `citrix`, `ciscoAnyConnectV2`, `paloAltoGlobalProtect`, `zscalerPrivateAccess`, `f5Access2018`, `citrixSso`,. `paloAltoGlobalProtectV2`|
|Логинграупордомаин|String|Группа входа или домен, когда для параметра Тип подключения установлено мобильное подключение Dell Сониквалл. НаСледуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)|
|role|String|Роль, когда для типа подключения задано значение Secure Pulse. НаСледуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)|
|область|String|Область, когда для параметра Тип подключения задано значение Secure Pulse. НаСледуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)|
|сервер|[Vpnserver.](../resources/intune-deviceconfig-vpnserver.md)|VPN-сервер в сети. Убедитесь, что конечные пользователи имеют доступ к этому сетевому расположению. НаСледуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)|
|идентификатор|String|Идентификатор, предоставленный поставщиком VPN, если для параметра Тип подключения задано значение пользовательская сеть VPN. Например: Cisco Аниконнект использует идентификатор формы com. Cisco. аниконнект. апплевпн. подключаемый модуль, наСледуемый от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)|
|Пользовательские|Коллекция [keyValue](../resources/intune-deviceconfig-keyvalue.md)|Пользовательские данные, когда для параметра Тип подключения задано значение Custom VPN. Используйте это поле, чтобы включить функции, не поддерживаемые Intune, но доступные в решении VPN. Обратитесь к поставщику услуг VPN, чтобы узнать, как добавить эти пары "ключ-значение". Эта коллекция может содержать не более 25 элементов. НаСледуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)|
|customKeyValueData|Коллекция [keyValuePair](../resources/intune-shared-keyvaluepair.md)|Пользовательские данные, когда для параметра Тип подключения задано значение Custom VPN. Используйте это поле, чтобы включить функции, не поддерживаемые Intune, но доступные в решении VPN. Обратитесь к поставщику услуг VPN, чтобы узнать, как добавить эти пары "ключ-значение". Эта коллекция может содержать не более 25 элементов. НаСледуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)|
|Енаблесплиттуннелинг|Логический|Отправлять весь сетевой трафик через VPN. НаСледуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)|
|Параметр authenticationmethod|[Впнаусентикатионмесод](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|Способ проверки поДлинности для этого VPN-подключения. НаСледуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md). Возможные значения: `certificate`, `usernameAndPassword`.|
|Енаблеперапп|Логический|Если задать для этого параметра значение true, будут создаваться полезные данные VPN для каждого приложения, которые позже могут быть связаны с приложениями, которые могут активировать эту ВИРТУАЛЬную сеть VPN коннеЦитон на устройстве iOS конечного пользователя. НаСледуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)|
|Сафаридомаинс|Коллекция строк|Домены Safari при включении этого параметра VPN для каждого приложения. Кроме приложений, связанных с этой ВИРТУАЛЬНОЙ частной сети, домены Safari, указанные здесь, также смогут инициировать это VPN-подключение. НаСледуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)|
|Ондемандрулес|Коллекция [впнондемандруле](../resources/intune-deviceconfig-vpnondemandrule.md)|Правила по запросу. Эта коллекция может содержать не более 500 элементов. НаСледуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)|
|проксисервер|[Впнпроксисервер](../resources/intune-deviceconfig-vpnproxyserver.md)|Прокси-сервер. НаСледуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)|
|Оптинтодевицеидшаринг|Логический|Предоставление доступа к идентификатору устройства сторонним VPN-клиентам для использования во время проверки управления доступом к сети. НаСледуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)|

## <a name="relationships"></a>Отношения
|Связь|Тип|Описание|
|:---|:---|:---|
|groupAssignments|Коллекция [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)|Список назначений групп для профиля конфигурации устройства. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|assignments|Коллекция [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|Список назначений для профиля конфигурации устройства. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|deviceStatuses|Коллекция [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md)|Состояние установки конфигурации для каждого устройства. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|userStatuses|Коллекция [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md)|Состояние установки конфигурации устройств пользователем. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|Обзор состояния конфигурации по устройствам. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|Обзор состояния конфигурации устройств по пользователям. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|deviceSettingStateSummaries|Коллекция [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)|Обзор состояния параметров конфигурации устройств по пользователям. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|Identitycertificate (|[Макосцертификатепрофилебасе](../resources/intune-deviceconfig-macoscertificateprofilebase.md)|Сертификат удостоверения для проверки подлинности клиента при использовании метода проверки подлинности Certificate.|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.macOSVpnConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSVpnConfiguration",
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
  "connectionName": "String",
  "connectionType": "String",
  "loginGroupOrDomain": "String",
  "role": "String",
  "realm": "String",
  "server": {
    "@odata.type": "microsoft.graph.vpnServer",
    "description": "String",
    "address": "String",
    "isDefaultServer": true
  },
  "identifier": "String",
  "customData": [
    {
      "@odata.type": "microsoft.graph.keyValue",
      "key": "String",
      "value": "String"
    }
  ],
  "customKeyValueData": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "String",
      "value": "String"
    }
  ],
  "enableSplitTunneling": true,
  "authenticationMethod": "String",
  "enablePerApp": true,
  "safariDomains": [
    "String"
  ],
  "onDemandRules": [
    {
      "@odata.type": "microsoft.graph.vpnOnDemandRule",
      "ssids": [
        "String"
      ],
      "dnsSearchDomains": [
        "String"
      ],
      "probeUrl": "String",
      "action": "String",
      "domainAction": "String",
      "domains": [
        "String"
      ],
      "probeRequiredUrl": "String"
    }
  ],
  "proxyServer": {
    "@odata.type": "microsoft.graph.vpnProxyServer",
    "automaticConfigurationScriptUrl": "String",
    "address": "String",
    "port": 1024
  },
  "optInToDeviceIdSharing": true
}
```





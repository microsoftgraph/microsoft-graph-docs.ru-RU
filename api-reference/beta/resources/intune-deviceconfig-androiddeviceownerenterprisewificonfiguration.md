---
title: Тип ресурса Андроиддевицеовнерентерприсевификонфигуратион
description: Предоставляя конфигурации в этом профиле, вы можете указать устройству владельца устройства Android подключаться к желаемой конечной точке Wi/Fi. Указав способ проверки подлинности и типы безопасности, ожидаемые конечной точкой Wi/Fi, можно легко установить соединение Wi/Fi для конечного пользователя.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 760a69c27fb3600881c6b4d623e8ae2ddcca0b4c
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36336597"
---
# <a name="androiddeviceownerenterprisewificonfiguration-resource-type"></a>Тип ресурса Андроиддевицеовнерентерприсевификонфигуратион

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Предоставляя конфигурации в этом профиле, вы можете указать устройству владельца устройства Android подключаться к желаемой конечной точке Wi/Fi. Указав способ проверки подлинности и типы безопасности, ожидаемые конечной точкой Wi/Fi, можно легко установить соединение Wi/Fi для конечного пользователя.


Наследуется от [андроиддевицеовнервификонфигуратион](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Андроиддевицеовнерентерприсевификонфигуратионс](../api/intune-deviceconfig-androiddeviceownerenterprisewificonfiguration-list.md)|Коллекция [андроиддевицеовнерентерприсевификонфигуратион](../resources/intune-deviceconfig-androiddeviceownerenterprisewificonfiguration.md)|Список свойств и связей объектов [андроиддевицеовнерентерприсевификонфигуратион](../resources/intune-deviceconfig-androiddeviceownerenterprisewificonfiguration.md) .|
|[Получение Андроиддевицеовнерентерприсевификонфигуратион](../api/intune-deviceconfig-androiddeviceownerenterprisewificonfiguration-get.md)|[андроиддевицеовнерентерприсевификонфигуратион](../resources/intune-deviceconfig-androiddeviceownerenterprisewificonfiguration.md)|Чтение свойств и связей объекта [андроиддевицеовнерентерприсевификонфигуратион](../resources/intune-deviceconfig-androiddeviceownerenterprisewificonfiguration.md) .|
|[Создание Андроиддевицеовнерентерприсевификонфигуратион](../api/intune-deviceconfig-androiddeviceownerenterprisewificonfiguration-create.md)|[андроиддевицеовнерентерприсевификонфигуратион](../resources/intune-deviceconfig-androiddeviceownerenterprisewificonfiguration.md)|Создание нового объекта [андроиддевицеовнерентерприсевификонфигуратион](../resources/intune-deviceconfig-androiddeviceownerenterprisewificonfiguration.md) .|
|[Удаление Андроиддевицеовнерентерприсевификонфигуратион](../api/intune-deviceconfig-androiddeviceownerenterprisewificonfiguration-delete.md)|Нет|Удаляет объект [андроиддевицеовнерентерприсевификонфигуратион](../resources/intune-deviceconfig-androiddeviceownerenterprisewificonfiguration.md).|
|[Обновление Андроиддевицеовнерентерприсевификонфигуратион](../api/intune-deviceconfig-androiddeviceownerenterprisewificonfiguration-update.md)|[андроиддевицеовнерентерприсевификонфигуратион](../resources/intune-deviceconfig-androiddeviceownerenterprisewificonfiguration.md)|Обновление свойств объекта [андроиддевицеовнерентерприсевификонфигуратион](../resources/intune-deviceconfig-androiddeviceownerenterprisewificonfiguration.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|roleScopeTagIds|Коллекция строк|Список тегов областей для этого экземпляра сущности. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|суппортсскопетагс|Boolean|Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области. Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия. Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure. Это свойство доступно только для чтения. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|deviceManagementApplicabilityRuleOsEdition|[deviceManagementApplicabilityRuleOsEdition](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|Применимость выпусков ОС для этой политики. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|deviceManagementApplicabilityRuleOsVersion|[deviceManagementApplicabilityRuleOsVersion](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|Правило применимости версии ОС для этой политики. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|девицеманажементаппликабилитируледевицемоде|[девицеманажементаппликабилитируледевицемоде](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|Правило применимости режима устройства для этой политики. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|createdDateTime|DateTimeOffset|Дата и время создания объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|description|String|Указанное администратором описание конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|displayName|Строка|Указанное администратором имя конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|version|Int32|Версия конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|нетворкнаме|String|Сетевое имя, унаследованное от [андроиддевицеовнервификонфигуратион](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)|
|SSID|String|Это имя сети Wi-Fi, которая отправляется на все устройства. Наследуется от [андроиддевицеовнервификонфигуратион](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)|
|коннектаутоматикалли|Boolean|Подключаться автоматически, если сеть находится в диапазоне. Если задать для этого параметра значение true, запрос пользователя будет пропущен и автоматически подключено устройство к сети Wi/Fi. Наследуется от [андроиддевицеовнервификонфигуратион](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)|
|коннектвхеннетворкнамеишидден|Boolean|Если задано значение true, этот профиль заставляет устройство подключаться к сети, на которой не выполняется трансляция идентификатора SSID на все устройства. Наследуется от [андроиддевицеовнервификонфигуратион](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)|
|вифисекурититипе|[androidDeviceOwnerWiFiSecurityType](../resources/intune-deviceconfig-androiddeviceownerwifisecuritytype.md)|Указывает, использует ли конечная точка Wi/Fi тип безопасности на основе EAP. Наследуется от [андроиддевицеовнервификонфигуратион](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md). Возможные значения: `open`, `wep`, `wpaPersonal`, `wpaEnterprise`.|
|preSharedKey|String|Это предварительно общий ключ для частной сети Wi-Fi WPA. Наследуется от [андроиддевицеовнервификонфигуратион](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)|
|прешаредкэйиссет|Boolean|Это предварительно общий ключ для частной сети Wi-Fi WPA. Наследуется от [андроиддевицеовнервификонфигуратион](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)|
|еаптипе|[андроидеаптипе](../resources/intune-deviceconfig-androideaptype.md)|Указывает тип протокола EAP, установленный для конечной точки Wi-Fi (маршрутизатора). Возможные значения: `eapTls`, `eapTtls`, `peap`.|
|Параметр authenticationmethod|[вифиаусентикатионмесод](../resources/intune-deviceconfig-wifiauthenticationmethod.md)|Указывает метод проверки подлинности, который должен использоваться клиентом (устройством), если тип EAP настроен для протокола PEAP или EAP-TTLS. Возможные значения: `certificate`, `usernameAndPassword`, `derivedCredential`.|
|Свойства innerauthenticationprotocolforeapttls|[нонеапаусентикатионмесодфореапттлстипе](../resources/intune-deviceconfig-noneapauthenticationmethodforeapttlstype.md)|Метод проверки подлинности (внутреннее удостоверение), не относящийся к EAP, если тип EAP — EAP-TTLS, а параметр authenticationmethod — имя пользователя и пароль. Возможные значения: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.|
|innerAuthenticationProtocolForPeap|[nonEapAuthenticationMethodForPeap](../resources/intune-deviceconfig-noneapauthenticationmethodforpeap.md)|Метод проверки подлинности, отличный от EAP (внутреннее удостоверение), если тип EAP — PEAP, а параметр authenticationmethod — имя пользователя и пароль. Возможные значения: `none`, `microsoftChapVersionTwo`.|
|outerIdentityPrivacyTemporaryValue|String|Включите конфиденциальность удостоверений (внешнее удостоверение), если тип EAP настроен для EAP-TTLS или PEAP. Приведенная здесь строка используется для маскирования имени пользователя отдельных пользователей при попытке подключения к сети Wi-Fi.|

## <a name="relationships"></a>Отношения
|Отношение|Тип|Описание|
|:---|:---|:---|
|groupAssignments|Коллекция [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)|Список назначений групп для профиля конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|assignments|Коллекция [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|Список назначений для профиля конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|deviceStatuses|Коллекция [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md)|Состояние установки конфигурации для каждого устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|userStatuses|Коллекция [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md)|Состояние установки конфигурации устройств пользователем. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|Обзор состояния конфигурации устройств. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|Обзор состояния конфигурации устройств для пользователей. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|deviceSettingStateSummaries|Коллекция [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)|Сводка данных о состоянии настройки конфигурации устройств. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|рутцертификатефорсервервалидатион|[андроиддевицеовнертрустедрутцертификате](../resources/intune-deviceconfig-androiddeviceownertrustedrootcertificate.md)|Доверенный корневой сертификат для проверки сервера, если тип EAP настроен для EAP-TLS, EAP-TTLS или PEAP. Это сертификат, представленный конечной точкой Wi-Fi, когда устройство пытается подключиться к конечной точке Wi-Fi. Для продолжения попытки подключения устройство (или пользователь) должно принять этот сертификат.|
|идентитицертификатефорклиентаусентикатион|[андроиддевицеовнерцертификатепрофилебасе](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md)|Сертификат удостоверения для проверки подлинности клиента, если тип EAP настроен для EAP-TLS, EAP-TTLS (с проверкой подлинности с помощью сертификата) или PEAP (с проверкой подлинности сертификата). Это сертификат, представленный клиентом конечной точке Wi-Fi. Сервер проверки подлинности, который находится за конечной точкой Wi/Fi, должен принять этот сертификат для успешной установки подключения Wi/Fi.|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.androidDeviceOwnerEnterpriseWiFiConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerEnterpriseWiFiConfiguration",
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
  "preSharedKey": "String",
  "preSharedKeyIsSet": true,
  "eapType": "String",
  "authenticationMethod": "String",
  "innerAuthenticationProtocolForEapTtls": "String",
  "innerAuthenticationProtocolForPeap": "String",
  "outerIdentityPrivacyTemporaryValue": "String"
}
```




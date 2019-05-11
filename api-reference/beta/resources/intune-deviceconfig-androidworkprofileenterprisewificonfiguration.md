---
title: Тип ресурса Андроидворкпрофилинтерприсевификонфигуратион
description: Предоставляя конфигурации в этом профиле, вы можете указать устройству рабочего профиля Android подключаться к желаемой конечной точке Wi/Fi. Указав способ проверки подлинности и типы безопасности, ожидаемые конечной точкой Wi/Fi, можно легко установить соединение Wi/Fi для конечного пользователя.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4382a44dc976af7f0d7882bc1d68907642f1e14b
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33947780"
---
# <a name="androidworkprofileenterprisewificonfiguration-resource-type"></a>Тип ресурса Андроидворкпрофилинтерприсевификонфигуратион

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Предоставляя конфигурации в этом профиле, вы можете указать устройству рабочего профиля Android подключаться к желаемой конечной точке Wi/Fi. Указав способ проверки подлинности и типы безопасности, ожидаемые конечной точкой Wi/Fi, можно легко установить соединение Wi/Fi для конечного пользователя.


Наследуется от [андроидворкпрофилевификонфигуратион](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Андроидворкпрофилинтерприсевификонфигуратионс](../api/intune-deviceconfig-androidworkprofileenterprisewificonfiguration-list.md)|Коллекция [андроидворкпрофилинтерприсевификонфигуратион](../resources/intune-deviceconfig-androidworkprofileenterprisewificonfiguration.md)|Список свойств и связей объектов [андроидворкпрофилинтерприсевификонфигуратион](../resources/intune-deviceconfig-androidworkprofileenterprisewificonfiguration.md) .|
|[Получение Андроидворкпрофилинтерприсевификонфигуратион](../api/intune-deviceconfig-androidworkprofileenterprisewificonfiguration-get.md)|[androidWorkProfileEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofileenterprisewificonfiguration.md)|Чтение свойств и связей объекта [андроидворкпрофилинтерприсевификонфигуратион](../resources/intune-deviceconfig-androidworkprofileenterprisewificonfiguration.md) .|
|[Создание Андроидворкпрофилинтерприсевификонфигуратион](../api/intune-deviceconfig-androidworkprofileenterprisewificonfiguration-create.md)|[androidWorkProfileEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofileenterprisewificonfiguration.md)|Создание нового объекта [андроидворкпрофилинтерприсевификонфигуратион](../resources/intune-deviceconfig-androidworkprofileenterprisewificonfiguration.md) .|
|[Удаление Андроидворкпрофилинтерприсевификонфигуратион](../api/intune-deviceconfig-androidworkprofileenterprisewificonfiguration-delete.md)|Нет|Удаляет объект [андроидворкпрофилинтерприсевификонфигуратион](../resources/intune-deviceconfig-androidworkprofileenterprisewificonfiguration.md).|
|[Обновление Андроидворкпрофилинтерприсевификонфигуратион](../api/intune-deviceconfig-androidworkprofileenterprisewificonfiguration-update.md)|[androidWorkProfileEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofileenterprisewificonfiguration.md)|Обновление свойств объекта [андроидворкпрофилинтерприсевификонфигуратион](../resources/intune-deviceconfig-androidworkprofileenterprisewificonfiguration.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|roleScopeTagIds|Коллекция строк|Список тегов областей для этого экземпляра сущности. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|Суппортсскопетагс|Логический|Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области. Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия. Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure. Это свойство доступно только для чтения. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|createdDateTime|DateTimeOffset|Дата и время создания объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|description|String|Указанное администратором описание конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|displayName|Строка|Указанное администратором имя конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|version|Int32|Версия конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|Нетворкнаме|Строка|Сетевое имя, унаследованное от [андроидворкпрофилевификонфигуратион](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)|
|SSID|Строка|Это имя сети Wi-Fi, которая отправляется на все устройства. Наследуется от [андроидворкпрофилевификонфигуратион](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)|
|Коннектаутоматикалли|Логический|Подключаться автоматически, если сеть находится в диапазоне. Если задать для этого параметра значение true, запрос пользователя будет пропущен и автоматически подключено устройство к сети Wi/Fi. Наследуется от [андроидворкпрофилевификонфигуратион](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)|
|Коннектвхеннетворкнамеишидден|Логический|Если задано значение true, этот профиль заставляет устройство подключаться к сети, на которой не выполняется трансляция идентификатора SSID на все устройства. Наследуется от [андроидворкпрофилевификонфигуратион](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)|
|Вифисекурититипе|[Андроидвифисекурититипе](../resources/intune-deviceconfig-androidwifisecuritytype.md)|Указывает, использует ли конечная точка Wi/Fi тип безопасности на основе EAP. Наследуется от [андроидворкпрофилевификонфигуратион](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md). Возможные значения: `open`, `wpaEnterprise`.|
|Еаптипе|[Андроидеаптипе](../resources/intune-deviceconfig-androideaptype.md)|Указывает тип протокола EAP, установленный для конечной точки Wi-Fi (маршрутизатора). Возможные значения: `eapTls`, `eapTtls`, `peap`.|
|Параметр authenticationmethod|[Вифиаусентикатионмесод](../resources/intune-deviceconfig-wifiauthenticationmethod.md)|Указывает метод проверки подлинности, который должен использоваться клиентом (устройством), если тип EAP настроен для протокола PEAP или EAP-TTLS. Возможные значения: `certificate`, `usernameAndPassword`, `derivedCredential`.|
|Свойства innerauthenticationprotocolforeapttls|[Нонеапаусентикатионмесодфореапттлстипе](../resources/intune-deviceconfig-noneapauthenticationmethodforeapttlstype.md)|Метод проверки подлинности (внутреннее удостоверение), не относящийся к EAP, если тип EAP — EAP-TTLS, а параметр authenticationmethod — имя пользователя и пароль. Возможные значения: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.|
|innerAuthenticationProtocolForPeap|[nonEapAuthenticationMethodForPeap](../resources/intune-deviceconfig-noneapauthenticationmethodforpeap.md)|Метод проверки подлинности, отличный от EAP (внутреннее удостоверение), если тип EAP — PEAP, а параметр authenticationmethod — имя пользователя и пароль. Возможные значения: `none`, `microsoftChapVersionTwo`.|
|outerIdentityPrivacyTemporaryValue|Строка|Включите конфиденциальность удостоверений (внешнее удостоверение), если тип EAP настроен для EAP-TTLS или PEAP. Приведенная здесь строка используется для маскирования имени пользователя отдельных пользователей при попытке подключения к сети Wi-Fi.|

## <a name="relationships"></a>Связи
|Отношение|Тип|Описание|
|:---|:---|:---|
|groupAssignments|Коллекция [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)|Список назначений групп для профиля конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|assignments|Коллекция [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|Список назначений для профиля конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|deviceStatuses|Коллекция [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md)|Состояние установки конфигурации для каждого устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|userStatuses|Коллекция [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md)|Состояние установки конфигурации устройств пользователем. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|Обзор состояния конфигурации устройств. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|Обзор состояния конфигурации устройств для пользователей. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|deviceSettingStateSummaries|Коллекция [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)|Сводка данных о состоянии настройки конфигурации устройств. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|Рутцертификатефорсервервалидатион|[androidWorkProfileTrustedRootCertificate](../resources/intune-deviceconfig-androidworkprofiletrustedrootcertificate.md)|Доверенный корневой сертификат для проверки сервера, если тип EAP настроен для EAP-TLS, EAP-TTLS или PEAP. Это сертификат, представленный конечной точкой Wi-Fi, когда устройство пытается подключиться к конечной точке Wi-Fi. Для продолжения попытки подключения устройство (или пользователь) должно принять этот сертификат.|
|Идентитицертификатефорклиентаусентикатион|[androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md)|Сертификат удостоверения для проверки подлинности клиента, если тип EAP настроен для EAP-TLS, EAP-TTLS (с проверкой подлинности с помощью сертификата) или PEAP (с проверкой подлинности сертификата). Это сертификат, представленный клиентом конечной точке Wi-Fi. Сервер проверки подлинности, который находится за конечной точкой Wi/Fi, должен принять этот сертификат для успешной установки подключения Wi/Fi.|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.androidWorkProfileEnterpriseWiFiConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidWorkProfileEnterpriseWiFiConfiguration",
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
  "networkName": "String",
  "ssid": "String",
  "connectAutomatically": true,
  "connectWhenNetworkNameIsHidden": true,
  "wiFiSecurityType": "String",
  "eapType": "String",
  "authenticationMethod": "String",
  "innerAuthenticationProtocolForEapTtls": "String",
  "innerAuthenticationProtocolForPeap": "String",
  "outerIdentityPrivacyTemporaryValue": "String"
}
```





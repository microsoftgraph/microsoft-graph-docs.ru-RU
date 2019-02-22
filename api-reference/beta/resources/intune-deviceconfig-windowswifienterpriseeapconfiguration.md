---
title: Тип ресурса Виндовсвифиентерприсиапконфигуратион
description: Эта сущность предоставляет описания объявляемых методов, свойств и связей, предоставляемых CSP WiFi.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4394a927f413ce311c6b371140ab69a7f14109f3
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30159775"
---
# <a name="windowswifienterpriseeapconfiguration-resource-type"></a>Тип ресурса Виндовсвифиентерприсиапконфигуратион

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Эта сущность предоставляет описания объявляемых методов, свойств и связей, предоставляемых CSP WiFi.


НаСледуется от [виндовсвификонфигуратион](../resources/intune-deviceconfig-windowswificonfiguration.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Виндовсвифиентерприсиапконфигуратионс](../api/intune-deviceconfig-windowswifienterpriseeapconfiguration-list.md)|Коллекция [виндовсвифиентерприсиапконфигуратион](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md)|Список свойств и связей объектов [виндовсвифиентерприсиапконфигуратион](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) .|
|[Получение Виндовсвифиентерприсиапконфигуратион](../api/intune-deviceconfig-windowswifienterpriseeapconfiguration-get.md)|[Виндовсвифиентерприсиапконфигуратион](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md)|Чтение свойств и связей объекта [виндовсвифиентерприсиапконфигуратион](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) .|
|[Создание Виндовсвифиентерприсиапконфигуратион](../api/intune-deviceconfig-windowswifienterpriseeapconfiguration-create.md)|[Виндовсвифиентерприсиапконфигуратион](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md)|Создание нового объекта [виндовсвифиентерприсиапконфигуратион](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) .|
|[Удаление Виндовсвифиентерприсиапконфигуратион](../api/intune-deviceconfig-windowswifienterpriseeapconfiguration-delete.md)|Нет|Удаляет объект [виндовсвифиентерприсиапконфигуратион](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md).|
|[Обновление Виндовсвифиентерприсиапконфигуратион](../api/intune-deviceconfig-windowswifienterpriseeapconfiguration-update.md)|[Виндовсвифиентерприсиапконфигуратион](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md)|Обновление свойств объекта [виндовсвифиентерприсиапконфигуратион](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) .|

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
|preSharedKey|String|Это предварительно общий ключ для частной сети Wi-Fi WPA. НаСледуется от [виндовсвификонфигуратион](../resources/intune-deviceconfig-windowswificonfiguration.md)|
|Вифисекурититипе|[Вифисекурититипе](../resources/intune-deviceconfig-wifisecuritytype.md)|Укажите тип безопасности Wi-Fi. НаСледуется от [виндовсвификонфигуратион](../resources/intune-deviceconfig-windowswificonfiguration.md). Возможные значения: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.|
|Метередконнектионлимит|[meteredConnectionLimitType](../resources/intune-deviceconfig-meteredconnectionlimittype.md)|Указать тип лимита межлимитного подключения для подключения WiFi. НаСледуется от [виндовсвификонфигуратион](../resources/intune-deviceconfig-windowswificonfiguration.md). Возможные значения: `unrestricted`, `fixed`, `variable`.|
|SSID|String|Укажите идентификатор SSID подключения WiFi. НаСледуется от [виндовсвификонфигуратион](../resources/intune-deviceconfig-windowswificonfiguration.md)|
|Нетворкнаме|String|Укажите имя конфигурации сети. НаСледуется от [виндовсвификонфигуратион](../resources/intune-deviceconfig-windowswificonfiguration.md)|
|Коннектаутоматикалли|Логический|Указывает, должно ли подключение WiFi автоматически подключаться к сети в пределах диапазона. НаСледуется от [виндовсвификонфигуратион](../resources/intune-deviceconfig-windowswificonfiguration.md)|
|Коннекттопреферреднетворк|Логический|Укажите, должно ли подключение WiFi подключаться к более предпочтительным сетям, если оно уже подключено к этому.  Необходимо, чтобы Коннектаутоматикалли был true. НаСледуется от [виндовсвификонфигуратион](../resources/intune-deviceconfig-windowswificonfiguration.md)|
|Коннектвхеннетворкнамеишидден|Логический|Укажите, должно ли подключение WiFi автоматически подключаться, даже если идентификатор SSID не является широковещательным. НаСледуется от [виндовсвификонфигуратион](../resources/intune-deviceconfig-windowswificonfiguration.md)|
|Проксисеттинг|[Вифипроксисеттинг](../resources/intune-deviceconfig-wifiproxysetting.md)|Укажите параметры прокси-сервера для конфигурации Wi-Fi, наСледуемой от [виндовсвификонфигуратион](../resources/intune-deviceconfig-windowswificonfiguration.md). Возможные значения: `none`, `manual`, `automatic`.|
|Проксимануаладдресс|String|Укажите IP-адрес прокси-сервера. НаСледуется от [виндовсвификонфигуратион](../resources/intune-deviceconfig-windowswificonfiguration.md)|
|Проксимануалпорт|Int32|Укажите порт прокси-сервера. НаСледуется от [виндовсвификонфигуратион](../resources/intune-deviceconfig-windowswificonfiguration.md)|
|Проксяутоматикконфигуратионурл|String|Укажите URL-адрес скрипта настройки прокси-сервера. НаСледуется от [виндовсвификонфигуратион](../resources/intune-deviceconfig-windowswificonfiguration.md)|
|Форцефипскомплианце|Логический|Укажите, следует ли применять соответствие требованиям FIPS. НаСледуется от [виндовсвификонфигуратион](../resources/intune-deviceconfig-windowswificonfiguration.md)|
|Нетворксинглесигнон|[Нетворксинглесигнонтипе](../resources/intune-deviceconfig-networksinglesignontype.md)|Укажите тип единого входа в сеть. Возможные значения: `disabled`, `prelogon`, `postlogon`.|
|Максимумаусентикатионтимеаутинсекондс|Int32|Укажите максимальное время ожидания проверки подлинности (в секундах).  Допустимый диапазон: 1-120|
|Промптфораддитионалаусентикатионкредентиалс|Логический|Укажите, должно ли подключение Wi-Fi запрашивать дополнительные учетные данные проверки подлинности.|
|Енаблепаирвисемастеркэйкачинг|Логический|Укажите, следует ли включить кэширование парных главных ключей в подключении Wi-Fi.|
|Максимумпаирвисемастеркэйкачетимеинминутес|Int32|Указать максимальное время кэширования парных главных ключей (в минутах).  Допустимый диапазон: 5-1440|
|Максимумнумберофпаирвисемастеркэйсинкаче|Int32|Укажите максимальное число парных главных ключей в кэше.  Допустимый диапазон: 1-255|
|Енаблепреаусентикатион|Логический|Укажите, следует ли включить предварительную проверку подлинности.|
|Максимумпреаусентикатионаттемптс|Int32|Указать максимальное количество попыток перед проверкой подлинности.  Допустимый диапазон: 1-16|
|Еаптипе|[Еаптипе](../resources/intune-deviceconfig-eaptype.md)|Протокол расширенной проверки поДлинности (EAP). Указывает тип протокола EAP, установленный для конечной точки Wi-Fi (маршрутизатора). Возможные значения: `eapTls`, `leap`, `eapSim`, `eapTtls`, `peap`, `eapFast`.|
|Трустедсерверцертификатенамес|Коллекция строк|Укажите имена сертификатов доверенного сервера.|
|Параметр authenticationmethod|[Вифиаусентикатионмесод](../resources/intune-deviceconfig-wifiauthenticationmethod.md)|Укажите метод проверки подлинности. Возможные значения: `certificate`, `usernameAndPassword`.|
|Свойства innerauthenticationprotocolforeapttls|[Нонеапаусентикатионмесодфореапттлстипе](../resources/intune-deviceconfig-noneapauthenticationmethodforeapttlstype.md)|Укажите внутренний протокол проверки подлинности для EAP TTLS. Возможные значения: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.|
|outerIdentityPrivacyTemporaryValue|String|Укажите строку для замены имен пользователей для обеспечения конфиденциальности при использовании EAP TTLS или PEAP.|

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
|Рутцертификатесфорсервервалидатион|Коллекция [windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md)|Укажите корневой сертификат для проверки сервера.|
|Идентитицертификатефорклиентаусентикатион|[windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)|Укажите сертификат удостоверения для проверки подлинности клиента.|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsWifiEnterpriseEAPConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsWifiEnterpriseEAPConfiguration",
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
  "preSharedKey": "String",
  "wifiSecurityType": "String",
  "meteredConnectionLimit": "String",
  "ssid": "String",
  "networkName": "String",
  "connectAutomatically": true,
  "connectToPreferredNetwork": true,
  "connectWhenNetworkNameIsHidden": true,
  "proxySetting": "String",
  "proxyManualAddress": "String",
  "proxyManualPort": 1024,
  "proxyAutomaticConfigurationUrl": "String",
  "forceFIPSCompliance": true,
  "networkSingleSignOn": "String",
  "maximumAuthenticationTimeoutInSeconds": 1024,
  "promptForAdditionalAuthenticationCredentials": true,
  "enablePairwiseMasterKeyCaching": true,
  "maximumPairwiseMasterKeyCacheTimeInMinutes": 1024,
  "maximumNumberOfPairwiseMasterKeysInCache": 1024,
  "enablePreAuthentication": true,
  "maximumPreAuthenticationAttempts": 1024,
  "eapType": "String",
  "trustedServerCertificateNames": [
    "String"
  ],
  "authenticationMethod": "String",
  "innerAuthenticationProtocolForEAPTTLS": "String",
  "outerIdentityPrivacyTemporaryValue": "String"
}
```





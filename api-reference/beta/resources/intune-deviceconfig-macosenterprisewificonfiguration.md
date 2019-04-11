---
title: Тип ресурса macOSEnterpriseWiFiConfiguration
description: Профиль конфигурации WPA-предприятие/WPA2-предприятие MacOS Wi-Fi WPA.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f4643a8004bc5835cabdc5fdb19e2ddb2ea7fd34
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31803040"
---
# <a name="macosenterprisewificonfiguration-resource-type"></a>Тип ресурса macOSEnterpriseWiFiConfiguration

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Профиль конфигурации WPA-предприятие/WPA2-предприятие MacOS Wi-Fi WPA.


НаСледуется от [макосвификонфигуратион](../resources/intune-deviceconfig-macoswificonfiguration.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Макосентерприсевификонфигуратионс](../api/intune-deviceconfig-macosenterprisewificonfiguration-list.md)|Коллекция [macOSEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-macosenterprisewificonfiguration.md)|Список свойств и связей объектов [macOSEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-macosenterprisewificonfiguration.md) .|
|[Получение macOSEnterpriseWiFiConfiguration](../api/intune-deviceconfig-macosenterprisewificonfiguration-get.md)|[macOSEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-macosenterprisewificonfiguration.md)|Чтение свойств и связей объекта [macOSEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-macosenterprisewificonfiguration.md) .|
|[Создание macOSEnterpriseWiFiConfiguration](../api/intune-deviceconfig-macosenterprisewificonfiguration-create.md)|[macOSEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-macosenterprisewificonfiguration.md)|Создание нового объекта [macOSEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-macosenterprisewificonfiguration.md) .|
|[Удаление macOSEnterpriseWiFiConfiguration](../api/intune-deviceconfig-macosenterprisewificonfiguration-delete.md)|Нет|Удаляет объект [macOSEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-macosenterprisewificonfiguration.md).|
|[Обновление macOSEnterpriseWiFiConfiguration](../api/intune-deviceconfig-macosenterprisewificonfiguration-update.md)|[macOSEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-macosenterprisewificonfiguration.md)|Обновление свойств объекта [macOSEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-macosenterprisewificonfiguration.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Ключ объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|roleScopeTagIds|Коллекция String|Список тегов областей для этого экземпляра сущности. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|Суппортсскопетагс|Boolean|Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области. Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия. Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure. Это свойство доступно только для чтения. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|createdDateTime|DateTimeOffset|Дата и время создания объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|description|String|Указанное администратором описание конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|displayName|String|Указанное администратором имя конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|version|Int32|Версия конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|Нетворкнаме|String|Сетевое имя, унаследованное от [макосвификонфигуратион](../resources/intune-deviceconfig-macoswificonfiguration.md)|
|SSID|String|Это имя сети Wi-Fi, которая отправляется на все устройства. НаСледуется от [макосвификонфигуратион](../resources/intune-deviceconfig-macoswificonfiguration.md)|
|Коннектаутоматикалли|Boolean|ПодКлючаться автоматически, если сеть находится в диапазоне. Если задать для этого параметра значение true, запрос пользователя будет пропущен и автоматически подключено устройство к сети Wi/Fi. НаСледуется от [макосвификонфигуратион](../resources/intune-deviceconfig-macoswificonfiguration.md)|
|Коннектвхеннетворкнамеишидден|Boolean|ПодКлючаться, если сеть не ведет вещание своего имени (SSID). Если задано значение true, этот профиль заставляет устройство подключаться к сети, на которой не выполняется трансляция идентификатора SSID на все устройства. НаСледуется от [макосвификонфигуратион](../resources/intune-deviceconfig-macoswificonfiguration.md)|
|Вифисекурититипе|[Вифисекурититипе](../resources/intune-deviceconfig-wifisecuritytype.md)|Указывает, использует ли конечная точка Wi/Fi тип безопасности на основе EAP. НаСледуется от [макосвификонфигуратион](../resources/intune-deviceconfig-macoswificonfiguration.md). Возможные значения: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.|
|proxySettings|[Вифипроксисеттинг](../resources/intune-deviceconfig-wifiproxysetting.md)|Тип прокси-сервера для этого подключения Wi-Fi наСледуется от [макосвификонфигуратион](../resources/intune-deviceconfig-macoswificonfiguration.md). Возможные значения: `none`, `manual`, `automatic`.|
|Проксимануаладдресс|String|IP-адрес или DNS-имя узла прокси-сервера при выборе конфигурации вручную. НаСледуется от [макосвификонфигуратион](../resources/intune-deviceconfig-macoswificonfiguration.md)|
|Проксимануалпорт|Int32|Порт прокси-сервера при выборе конфигурации вручную. НаСледуется от [макосвификонфигуратион](../resources/intune-deviceconfig-macoswificonfiguration.md)|
|Проксяутоматикконфигуратионурл|String|URL-адрес скрипта автоматической настройки прокси-сервера при выборе параметра Автоматическая настройка. Обычно это URL-адрес файла PAC (автоНастройка прокси-сервера). НаСледуется от [макосвификонфигуратион](../resources/intune-deviceconfig-macoswificonfiguration.md)|
|preSharedKey|String|Это предварительно общий ключ для частной сети Wi-Fi WPA. НаСледуется от [макосвификонфигуратион](../resources/intune-deviceconfig-macoswificonfiguration.md)|
|Еаптипе|[Еаптипе](../resources/intune-deviceconfig-eaptype.md)|Протокол расширенной проверки поДлинности (EAP). Указывает тип протокола EAP, установленный для конечной точки Wi-Fi (маршрутизатора). Возможные значения: `eapTls`, `leap`, `eapSim`, `eapTtls`, `peap`, `eapFast`.|
|Еапфастконфигуратион|[Еапфастконфигуратион](../resources/intune-deviceconfig-eapfastconfiguration.md)|Параметр конфигурации EAP-FAST, когда EAP-FAST выбран тип EAP. Возможные значения: `noProtectedAccessCredential`, `useProtectedAccessCredential`, `useProtectedAccessCredentialAndProvision`, `useProtectedAccessCredentialAndProvisionAnonymously`.|
|Трустедсерверцертификатенамес|Коллекция String|Имена сертификатов доверенных серверов, когда тип EAP настроен для EAP-TLS/TTLS/FAST или PEAP. Это общее имя, используемое в сертификатах, выдаваемых доверенным центром сертификации (CA). Если вы предоставляете эти сведения, вы можете обходить диалоговое окно динамического доверия, отображаемое на устройствах конечных пользователей, когда они подключаются к сети Wi-Fi.|
|Параметр authenticationmethod|[Вифиаусентикатионмесод](../resources/intune-deviceconfig-wifiauthenticationmethod.md)|Метод проверки поДлинности, когда тип EAP настроен для протокола PEAP или EAP-TTLS. Возможные значения: `certificate`, `usernameAndPassword`.|
|Свойства innerauthenticationprotocolforeapttls|[Нонеапаусентикатионмесодфореапттлстипе](../resources/intune-deviceconfig-noneapauthenticationmethodforeapttlstype.md)|Метод проверки поДлинности (внутреннее удостоверение), не относящийся к EAP, если тип EAP — EAP-TTLS, а параметр authenticationmethod — имя пользователя и пароль. Возможные значения: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.|
|outerIdentityPrivacyTemporaryValue|String|Включите конфиденциальность удостоверений (внешнее удостоверение), если тип EAP настроен для EAP-TTLS, EAP-FAST или PEAP. Это свойство маскирует имена пользователей с введенным текстом. Например, если вы используете анонимный доступ, все пользователи, которые проходят проверку подлинности с помощью этого подключения Wi-Fi, с помощью действительного имени пользователя отображаются как anonymous.|

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
|Рутцертификатефорсервервалидатион|[Макострустедрутцертификате](../resources/intune-deviceconfig-macostrustedrootcertificate.md)|Доверенный корневой сертификат для проверки сервера, если тип EAP настроен на АУТЕНТИФИКАЦИю EAP-TLS/TTLS/FAST или PEAP.|
|Идентитицертификатефорклиентаусентикатион|[Макосцертификатепрофилебасе](../resources/intune-deviceconfig-macoscertificateprofilebase.md)|Сертификат удостоверения для проверки подлинности клиента, если тип EAP настроен для EAP-TLS, EAP-TTLS (с проверкой поДлинности с помощью сертификата) или PEAP (с проверкой поДлинности сертификата).|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.macOSEnterpriseWiFiConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSEnterpriseWiFiConfiguration",
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
  "proxySettings": "String",
  "proxyManualAddress": "String",
  "proxyManualPort": 1024,
  "proxyAutomaticConfigurationUrl": "String",
  "preSharedKey": "String",
  "eapType": "String",
  "eapFastConfiguration": "String",
  "trustedServerCertificateNames": [
    "String"
  ],
  "authenticationMethod": "String",
  "innerAuthenticationProtocolForEapTtls": "String",
  "outerIdentityPrivacyTemporaryValue": "String"
}
```






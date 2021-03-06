---
title: Тип ресурса macOSEnterpriseWiFiConfiguration
description: MacOS Wi-Fi профиль конфигурации WPA-предприятие/WPA2-предприятие.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 1355b48aace3a10b274c641102e9665f61d66701
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49280013"
---
# <a name="macosenterprisewificonfiguration-resource-type"></a>Тип ресурса macOSEnterpriseWiFiConfiguration

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

MacOS Wi-Fi профиль конфигурации WPA-предприятие/WPA2-предприятие.


Наследуется от [макосвификонфигуратион](../resources/intune-deviceconfig-macoswificonfiguration.md)

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
|id|String|Ключ объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|roleScopeTagIds|Коллекция строк|Список тегов областей для этого экземпляра сущности. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|суппортсскопетагс|Boolean|Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области. Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия. Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure. Это свойство доступно только для чтения. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|deviceManagementApplicabilityRuleOsEdition|[deviceManagementApplicabilityRuleOsEdition](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|Применимость выпусков ОС для этой политики. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|deviceManagementApplicabilityRuleOsVersion|[deviceManagementApplicabilityRuleOsVersion](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|Правило применимости версии ОС для этой политики. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|deviceManagementApplicabilityRuleDeviceMode|[deviceManagementApplicabilityRuleDeviceMode](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|Правило применимости режима устройства для этой политики. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|createdDateTime|DateTimeOffset|Дата и время создания объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|description|String|Указанное администратором описание конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|displayName|String|Указанное администратором имя конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|version|Int32|Версия конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|нетворкнаме|String|Сетевое имя, унаследованное от [макосвификонфигуратион](../resources/intune-deviceconfig-macoswificonfiguration.md)|
|SSID|String|Это имя Wi-Fiной сети, которая отправляется на все устройства. Наследуется от [макосвификонфигуратион](../resources/intune-deviceconfig-macoswificonfiguration.md)|
|коннектаутоматикалли|Boolean|Подключаться автоматически, если сеть находится в диапазоне. Если задать для этого параметра значение true, запрос пользователя будет пропущен и устройство будет автоматически подключено к Wi-Fi сети. Наследуется от [макосвификонфигуратион](../resources/intune-deviceconfig-macoswificonfiguration.md)|
|коннектвхеннетворкнамеишидден|Boolean|Подключаться, если сеть не ведет вещание своего имени (SSID). Если задано значение true, этот профиль заставляет устройство подключаться к сети, на которой не выполняется трансляция идентификатора SSID на все устройства. Наследуется от [макосвификонфигуратион](../resources/intune-deviceconfig-macoswificonfiguration.md)|
|вифисекурититипе|[вифисекурититипе](../resources/intune-deviceconfig-wifisecuritytype.md)|Указывает, использует ли конечная точка Wi-Fi тип безопасности на основе EAP. Наследуется от [макосвификонфигуратион](../resources/intune-deviceconfig-macoswificonfiguration.md). Возможные значения: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.|
|proxySettings|[вифипроксисеттинг](../resources/intune-deviceconfig-wifiproxysetting.md)|Тип прокси-сервера для этого подключения Wi-Fi наследуется от [макосвификонфигуратион](../resources/intune-deviceconfig-macoswificonfiguration.md). Возможные значения: `none`, `manual`, `automatic`.|
|проксимануаладдресс|String|IP-адрес или DNS-имя узла прокси-сервера при выборе конфигурации вручную. Наследуется от [макосвификонфигуратион](../resources/intune-deviceconfig-macoswificonfiguration.md)|
|проксимануалпорт|Int32|Порт прокси-сервера при выборе конфигурации вручную. Наследуется от [макосвификонфигуратион](../resources/intune-deviceconfig-macoswificonfiguration.md)|
|проксяутоматикконфигуратионурл|String|URL-адрес скрипта автоматической настройки прокси-сервера при выборе параметра Автоматическая настройка. Обычно это URL-адрес файла PAC (Автонастройка прокси-сервера). Наследуется от [макосвификонфигуратион](../resources/intune-deviceconfig-macoswificonfiguration.md)|
|preSharedKey|String|Это предварительно общий ключ для сети WPA Personal Wi-Fi. Наследуется от [макосвификонфигуратион](../resources/intune-deviceconfig-macoswificonfiguration.md)|
|еаптипе|[еаптипе](../resources/intune-deviceconfig-eaptype.md)|Протокол расширенной проверки подлинности (EAP). Указывает тип протокола EAP, заданный для конечной точки Wi-Fi (маршрутизатора). Возможные значения: `eapTls`, `leap`, `eapSim`, `eapTtls`, `peap`, `eapFast`.|
|еапфастконфигуратион|[еапфастконфигуратион](../resources/intune-deviceconfig-eapfastconfiguration.md)|Параметр конфигурации EAP-FAST, когда EAP-FAST выбран тип EAP. Возможные значения: `noProtectedAccessCredential`, `useProtectedAccessCredential`, `useProtectedAccessCredentialAndProvision`, `useProtectedAccessCredentialAndProvisionAnonymously`.|
|трустедсерверцертификатенамес|Коллекция строк|Имена сертификатов доверенных серверов, когда тип EAP настроен для EAP-TLS/TTLS/FAST или PEAP. Это общее имя, используемое в сертификатах, выдаваемых доверенным центром сертификации (CA). Если вы предоставляете эти сведения, вы можете обходить диалоговое окно динамического доверия, отображаемое на устройствах конечных пользователей, когда они подключаются к этой сети Wi-Fi.|
|Параметр authenticationmethod|[вифиаусентикатионмесод](../resources/intune-deviceconfig-wifiauthenticationmethod.md)|Метод проверки подлинности, когда тип EAP настроен для протокола PEAP или EAP-TTLS. Возможные значения: `certificate`, `usernameAndPassword`, `derivedCredential`.|
|Свойства innerauthenticationprotocolforeapttls|[нонеапаусентикатионмесодфореапттлстипе](../resources/intune-deviceconfig-noneapauthenticationmethodforeapttlstype.md)|Метод проверки подлинности (внутреннее удостоверение), не относящийся к EAP, если тип EAP — EAP-TTLS, а параметр authenticationmethod — имя пользователя и пароль. Возможные значения: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.|
|outerIdentityPrivacyTemporaryValue|String|Включите конфиденциальность удостоверений (внешнее удостоверение), если тип EAP настроен для EAP-TTLS, EAP-FAST или PEAP. Это свойство маскирует имена пользователей с введенным текстом. Например, если вы используете анонимный доступ, каждый пользователь, который проверяет подлинность этого подключения Wi-Fi с помощью действительного имени пользователя, отображается как anonymous.|

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
|рутцертификатефорсервервалидатион|[макострустедрутцертификате](../resources/intune-deviceconfig-macostrustedrootcertificate.md)|Доверенный корневой сертификат для проверки сервера, если тип EAP настроен на аутентификацию EAP-TLS/TTLS/FAST или PEAP.|
|рутцертификатесфорсервервалидатион|Коллекция [макострустедрутцертификате](../resources/intune-deviceconfig-macostrustedrootcertificate.md)|Доверенные корневые сертификаты для проверки сервера, если тип EAP настроен для EAP-TLS/TTLS/FAST или PEAP. Если указать это значение, нет необходимости предоставлять Трустедсерверцертификатенамес и наоборот.|
|идентитицертификатефорклиентаусентикатион|[макосцертификатепрофилебасе](../resources/intune-deviceconfig-macoscertificateprofilebase.md)|Сертификат удостоверения для проверки подлинности клиента, если тип EAP настроен для EAP-TLS, EAP-TTLS (с проверкой подлинности с помощью сертификата) или PEAP (с проверкой подлинности сертификата).|

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





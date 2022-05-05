---
title: Тип ресурса aospDeviceOwnerEnterpriseWiFiConfiguration
description: Указав конфигурации в этом профиле, можно указать устройству владельца устройства AOSP подключиться к нужной Wi-Fi конечной точке. Указав метод проверки подлинности и типы безопасности, ожидаемые Wi-Fi конечной точкой, можно сделать подключение Wi-Fi простым для конечного пользователя.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: da1e031af52b8b19c8f6cbd6057998f9f716ca5c
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/05/2022
ms.locfileid: "65203199"
---
# <a name="aospdeviceownerenterprisewificonfiguration-resource-type"></a>Тип ресурса aospDeviceOwnerEnterpriseWiFiConfiguration

Пространство имен: microsoft.graph

> **Важно:** API Graph Майкрософт в версии /beta могут быть изменены; использование в рабочей области не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Указав конфигурации в этом профиле, можно указать устройству владельца устройства AOSP подключиться к нужной Wi-Fi конечной точке. Указав метод проверки подлинности и типы безопасности, ожидаемые Wi-Fi конечной точкой, можно сделать подключение Wi-Fi простым для конечного пользователя.


Наследует от [aospDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-aospdeviceownerwificonfiguration.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Перечисление aospDeviceOwnerEnterpriseWiFiConfigurations](../api/intune-deviceconfig-aospdeviceownerenterprisewificonfiguration-list.md)|[Коллекция aospDeviceOwnerEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-aospdeviceownerenterprisewificonfiguration.md)|Список свойств и связей объектов [aospDeviceOwnerEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-aospdeviceownerenterprisewificonfiguration.md) .|
|[Получение aospDeviceOwnerEnterpriseWiFiConfiguration](../api/intune-deviceconfig-aospdeviceownerenterprisewificonfiguration-get.md)|[aospDeviceOwnerEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-aospdeviceownerenterprisewificonfiguration.md)|Чтение свойств и связей объекта [aospDeviceOwnerEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-aospdeviceownerenterprisewificonfiguration.md) .|
|[Создание aospDeviceOwnerEnterpriseWiFiConfiguration](../api/intune-deviceconfig-aospdeviceownerenterprisewificonfiguration-create.md)|[aospDeviceOwnerEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-aospdeviceownerenterprisewificonfiguration.md)|Создайте объект [aospDeviceOwnerEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-aospdeviceownerenterprisewificonfiguration.md) .|
|[Удаление aospDeviceOwnerEnterpriseWiFiConfiguration](../api/intune-deviceconfig-aospdeviceownerenterprisewificonfiguration-delete.md)|Нет|Удаляет [aospDeviceOwnerEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-aospdeviceownerenterprisewificonfiguration.md).|
|[Обновление aospDeviceOwnerEnterpriseWiFiConfiguration](../api/intune-deviceconfig-aospdeviceownerenterprisewificonfiguration-update.md)|[aospDeviceOwnerEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-aospdeviceownerenterprisewificonfiguration.md)|Обновление свойств объекта [aospDeviceOwnerEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-aospdeviceownerenterprisewificonfiguration.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Ключ объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|Идентификаторы roleScopeTagId|Коллекция строк|Список тегов области для этого экземпляра сущности. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|supportsScopeTags|Логическое|Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области. Назначение свойству ScopeTags не допускается, если это значение имеет значение false и сущности не будут видны пользователям с заданной областью. Это происходит для устаревших политик, созданных в Silverlight, и их можно устранить, удалив и повторно создав политику на портале Azure. Это свойство доступно только для чтения. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|deviceManagementApplicabilityRuleOsEdition|[deviceManagementApplicabilityRuleOsEdition](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|Применимость выпуска ОС для этой политики. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|deviceManagementApplicabilityRuleOsVersion|[deviceManagementApplicabilityRuleOsVersion](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|Правило применимости версии ОС для этой политики. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|deviceManagementApplicabilityRuleDeviceMode|[deviceManagementApplicabilityRuleDeviceMode](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|Правило применимости режима устройства для этой политики. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|createdDateTime|DateTimeOffset|Дата и время создания объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|description|Строка|Указанное администратором описание конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|displayName|Строка|Указанное администратором имя конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|version|Int32|Версия конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|networkName|Строка|Сетевое имя, наследуемое [от aospDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-aospdeviceownerwificonfiguration.md)|
|Ssid|Строка|Это имя сети Wi-Fi, которая передается на все устройства. Наследуется от [aospDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-aospdeviceownerwificonfiguration.md)|
|connectAutomatically|Логическое|Подключение, если эта сеть находится в диапазоне. Если задано значение true, запрос пользователя будет пропущен и устройство будет автоматически подключено к Wi-Fi сети. Наследуется от [aospDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-aospdeviceownerwificonfiguration.md)|
|connectWhenNetworkNameIsHidden|Логическое|Если задано значение true, этот профиль принудительно подключает устройство к сети, которая не передает свой SSID на все устройства. Наследуется от [aospDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-aospdeviceownerwificonfiguration.md)|
|wiFiSecurityType|[aospDeviceOwnerWiFiSecurityType](../resources/intune-deviceconfig-aospdeviceownerwifisecuritytype.md)|Указывает, использует ли Wi-Fi конечная точка тип безопасности на основе EAP. Наследуется [от aospDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-aospdeviceownerwificonfiguration.md). Возможные значения: `open`, `wep`, `wpaPersonal`, `wpaEnterprise`.|
|preSharedKey|Строка|Это общий ключ для WPA Personal Wi-Fi сети. Наследуется от [aospDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-aospdeviceownerwificonfiguration.md)|
|preSharedKeyIsSet|Логическое|Это общий ключ для WPA Personal Wi-Fi сети. Наследуется от [aospDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-aospdeviceownerwificonfiguration.md)|
|eapType|[androidEapType](../resources/intune-deviceconfig-androideaptype.md)|Указывает тип протокола EAP, задаваемого в конечной Wi-Fi (маршрутизаторе). Возможные значения: `eapTls`, `eapTtls`, `peap`.|
|trustedServerCertificateNames|Коллекция строк|Имена сертификатов доверенных серверов, если тип EAP настроен на EAP-TLS/TTLS/FAST или PEAP. Это общее имя, используемого в сертификатах, выданных доверенным центром сертификации (ЦС). Если вы предоставите эти сведения, можно обойти диалоговое окно динамического доверия, отображаемое на устройствах конечных пользователей при подключении к этой Wi-Fi сети.|
|authenticationMethod|[wiFiAuthenticationMethod](../resources/intune-deviceconfig-wifiauthenticationmethod.md)|Указывает метод проверки подлинности, который клиент (устройство) должен использовать, если тип EAP настроен на PEAP или EAP-TTLS. Возможные значения: `certificate`, `usernameAndPassword`, `derivedCredential`.|
|innerAuthenticationProtocolForEapTtls|[nonEapAuthenticationMethodForEapTtlsType](../resources/intune-deviceconfig-noneapauthenticationmethodforeapttlstype.md)|Метод, отличный от EAP для проверки подлинности (внутреннее удостоверение), если тип EAP — EAP-TTLS, а authenticationmethod — имя пользователя и пароль. Возможные значения: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.|
|innerAuthenticationProtocolForPeap|[nonEapAuthenticationMethodForPeap](../resources/intune-deviceconfig-noneapauthenticationmethodforpeap.md)|Метод, отличный от EAP для проверки подлинности (внутреннее удостоверение), если тип EAP — PEAP, а authenticationmethod — имя пользователя и пароль. Эта коллекция может содержать не более 500 элементов. Возможные значения: `none`, `microsoftChapVersionTwo`.|
|outerIdentityPrivacyTemporaryValue|Строка|Включите конфиденциальность удостоверений (внешнее удостоверение), если тип EAP настроен на EAP-TTLS или PEAP. Указанная здесь строка используется для маскирования имени пользователя отдельных пользователей при попытке подключения к Wi-Fi сети.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|groupAssignments|[Коллекция deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)|Список назначений групп для профиля конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|assignments|Коллекция [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|Список назначений для профиля конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|deviceStatuses|Коллекция [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md)|Состояние установки конфигурации для каждого устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|userStatuses|Коллекция [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md)|Состояние установки конфигурации устройства по пользователю. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|Обзор состояния конфигурации устройств. Наследуется от [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|Обзор состояния конфигурации устройств для пользователей. Наследуется от [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|deviceSettingStateSummaries|Коллекция [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)|Сводка данных о состоянии настройки конфигурации устройств. Наследуется от [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|rootCertificateForServerValidation|[aospDeviceOwnerTrustedRootCertificate](../resources/intune-deviceconfig-aospdeviceownertrustedrootcertificate.md)|Доверенный корневой сертификат для проверки сервера, если тип EAP настроен на EAP-TLS, EAP-TTLS или PEAP. Это сертификат, представленный конечной точкой Wi-Fi, когда устройство пытается подключиться к Wi-Fi конечной точке. Устройство (или пользователь) должно принять этот сертификат, чтобы продолжить попытку подключения.|
|identityCertificateForClientAuthentication|[aospDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-aospdeviceownercertificateprofilebase.md)|Сертификат удостоверения для проверки подлинности клиента, если тип EAP настроен на EAP-TLS, EAP-TTLS (с проверкой подлинности на основе сертификата) или PEAP (с проверкой подлинности сертификата). Это сертификат, представленный клиентом конечной точке Wi-Fi. Сервер проверки подлинности, на котором находится Wi-Fi конечной точке, должен принять этот сертификат, чтобы успешно установить Wi-Fi подключения.|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.aospDeviceOwnerEnterpriseWiFiConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.aospDeviceOwnerEnterpriseWiFiConfiguration",
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
  "trustedServerCertificateNames": [
    "String"
  ],
  "authenticationMethod": "String",
  "innerAuthenticationProtocolForEapTtls": "String",
  "innerAuthenticationProtocolForPeap": "String",
  "outerIdentityPrivacyTemporaryValue": "String"
}
```





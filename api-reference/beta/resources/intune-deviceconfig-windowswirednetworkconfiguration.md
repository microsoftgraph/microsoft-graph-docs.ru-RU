---
title: тип ресурса windowsWiredNetworkConfiguration
description: Эта сущность содержит описания объявленных методов, свойств и связей, открытых CSP проводной сети.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f0f557826cac1a923324c817d5b30a4f06b9edad
ms.sourcegitcommit: 0076eb6abb89be3dca3575631924a74a5202be30
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/03/2022
ms.locfileid: "64631245"
---
# <a name="windowswirednetworkconfiguration-resource-type"></a>тип ресурса windowsWiredNetworkConfiguration

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Эта сущность содержит описания объявленных методов, свойств и связей, открытых CSP проводной сети.


Наследуется от [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список windowsWiredNetworkConfigurations](../api/intune-deviceconfig-windowswirednetworkconfiguration-list.md)|[коллекция windowsWiredNetworkConfiguration](../resources/intune-deviceconfig-windowswirednetworkconfiguration.md)|Список свойств и связей объектов [WindowsWiredNetworkConfiguration](../resources/intune-deviceconfig-windowswirednetworkconfiguration.md) .|
|[Get windowsWiredNetworkConfiguration](../api/intune-deviceconfig-windowswirednetworkconfiguration-get.md)|[windowsWiredNetworkConfiguration](../resources/intune-deviceconfig-windowswirednetworkconfiguration.md)|Чтение свойств и связей объекта [WindowsWiredNetworkConfiguration](../resources/intune-deviceconfig-windowswirednetworkconfiguration.md) .|
|[Создание windowsWiredNetworkConfiguration](../api/intune-deviceconfig-windowswirednetworkconfiguration-create.md)|[windowsWiredNetworkConfiguration](../resources/intune-deviceconfig-windowswirednetworkconfiguration.md)|Создайте [новый объект WindowsWiredNetworkConfiguration](../resources/intune-deviceconfig-windowswirednetworkconfiguration.md) .|
|[Удаление windowsWiredNetworkConfiguration](../api/intune-deviceconfig-windowswirednetworkconfiguration-delete.md)|Нет|Удаляет [windowsWiredNetworkConfiguration](../resources/intune-deviceconfig-windowswirednetworkconfiguration.md).|
|[Обновление windowsWiredNetworkConfiguration](../api/intune-deviceconfig-windowswirednetworkconfiguration-update.md)|[windowsWiredNetworkConfiguration](../resources/intune-deviceconfig-windowswirednetworkconfiguration.md)|Обновление свойств объекта [WindowsWiredNetworkConfiguration](../resources/intune-deviceconfig-windowswirednetworkconfiguration.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Ключ объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|roleScopeTagIds|Коллекция объектов string|Список тегов области для этого экземпляра Entity. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|supportsScopeTags|Логическое|Указывает, поддерживает ли вся конфигурация устройства назначение тегов области. Назначение свойства ScopeTags не допускается, если это значение является ложным и объекты не будут видны пользователям с охватом. Это происходит для политик Legacy, созданных в Silverlight, и их можно разрешить путем удаления и воссоздания политики на портале Azure. Это свойство доступно только для чтения. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|deviceManagementApplicabilityRuleOsEdition|[deviceManagementApplicabilityRuleOsEdition](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|Применимость к выпуску ОС для этой политики. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|deviceManagementApplicabilityRuleOsVersion|[deviceManagementApplicabilityRuleOsVersion](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|Правило применимости версии ОС для этой политики. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|deviceManagementApplicabilityRuleDeviceMode|[deviceManagementApplicabilityRuleDeviceMode](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|Правило применимости режима устройства для этой политики. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|createdDateTime|DateTimeOffset|Дата и время создания объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|description|Строка|Указанное администратором описание конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|displayName|Строка|Указанное администратором имя конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|version|Int32|Версия конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|authenticationType|[wiredNetworkAuthenticationType](../resources/intune-deviceconfig-wirednetworkauthenticationtype.md)|Укажите, следует ли проверить подлинность пользователя, устройства или использовать гостевую проверку подлинности (нет). Если вы используете проверку подлинности сертификатов, убедитесь, что тип сертификата соответствует типу проверки подлинности. Возможные значения: `none`, `user`, `machine`, `machineOrUser`, `guest`. Возможные значения: `none`, `user`, `machine`, `machineOrUser`, `guest`, `unknownFutureValue`.|
|cacheCredentials|Логический|Когда TRUE, кэш учетные данные пользователей на устройстве, чтобы пользователям не нужно продолжать вводить их каждый раз, когда они подключаются. Если false, не кэшить учетные данные. Значение по умолчанию false.|
|authenticationPeriodInSeconds|Int32|Укажите количество секунд, которые клиент должен ждать после попытки проверки подлинности перед сбоем. Допустимый диапазон 1-3600.|
|authenticationRetryDelayPeriodInSeconds|Int32|Укажите количество секунд между неудачной проверкой подлинности и следующей попыткой проверки подлинности. Допустимый диапазон 1-3600.|
|eapolStartPeriodInSeconds|Int32|Укажите количество секунд, которые необходимо подождать перед отправкой начните сообщение EAPOL (Extensible Authentication Protocol over LAN). Допустимый диапазон 1-3600.|
|maximumEAPOLStartMessages|Int32|Укажите максимальное число протоколов проверки подлинности EAPOL (extensible authentication protocol over LAN) Start messages to be sent before returning failure. Допустимый диапазон 1-100.|
|maximumAuthenticationFailures|Int32|Укажите максимально допустимые сбои проверки подлинности для набора учетных данных. Допустимый диапазон 1-100.|
|enforce8021X|Логическое|Когда true, автоматическая служба конфигурации для проводных сетей требует использования 802.1X для проверки подлинности порта. Если false, 802.1X не требуется. Значение по умолчанию false.|
|проверка подлинностиBlockPeriodInMinutes|Int32|Укажите продолжительность, в течение которой попытки автоматической проверки подлинности будут заблокированы после неудачной попытки проверки подлинности.|
|eapType|[eapType](../resources/intune-deviceconfig-eaptype.md)|Extensible Authentication Protocol (EAP). Указывает тип протокола EAP на конечной точке Wi-Fi (маршрутизатор). Возможные значения: `eapTls`, `leap`, `eapSim`, `eapTtls`, `peap`, `eapFast`, `teap`. Возможные значения: `eapTls`, `leap`, `eapSim`, `eapTtls`, `peap`, `eapFast`, `teap`.|
|trustedServerCertificateNames|Коллекция объектов string|Укажите имена доверенных сертификатов сервера.|
|authenticationMethod|[wiredNetworkAuthenticationMethod](../resources/intune-deviceconfig-wirednetworkauthenticationmethod.md)|Укажите метод проверки подлинности. Возможные значения: `certificate`, `usernameAndPassword`, `derivedCredential`. Возможные значения: `certificate`, `usernameAndPassword`, `derivedCredential`, `unknownFutureValue`.|
|secondaryAuthenticationMethod|[wiredNetworkAuthenticationMethod](../resources/intune-deviceconfig-wirednetworkauthenticationmethod.md)|Укажите метод вторичной проверки подлинности. Возможные значения: `certificate`, `usernameAndPassword`, `derivedCredential`. Возможные значения: `certificate`, `usernameAndPassword`, `derivedCredential`, `unknownFutureValue`.|
|innerAuthenticationProtocolForEAPTTLS|[nonEapAuthenticationMethodForEapTtlsType](../resources/intune-deviceconfig-noneapauthenticationmethodforeapttlstype.md)|Укажите внутренний протокол проверки подлинности для TTLS EAP. Возможные значения: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`. Возможные значения: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.|
|outerIdentityPrivacyTemporaryValue|Строка|Укажите строку для замены имен пользователей для конфиденциальности при использовании EAP TTLS или PEAP.|
|performServerValidation|Логическое|Когда TRUE, включает проверку удостоверения сервера путем проверки сертификата при выборе типа EAP в качестве PEAP. Если false, сертификат не проверяется. Значение по умолчанию — TRUE.|
|disableUserPromptForServerValidation|Логический|Если TRUE, не позволяет пользователю получить запрос на авторизации новых серверов для доверенных органов сертификации при выборе типа EAP в качестве PEAP. Если false, не препятствует запросу пользователя. Значение по умолчанию false.|
|requireCryptographicBinding|Boolean|Когда TRUE, включает криптографическую привязку, когда тип EAP выбран в качестве PEAP. При FALSE не включается криптогрпахическая привязка. Значение по умолчанию — TRUE.|
|forceFIPSCompliance|Boolean|Когда true, заставляет соответствие ТРЕБОВАНИЯМ FIPS. Если false, не включает соответствие ТРЕБОВАНИЯМ FIPS. Значение по умолчанию false.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|groupAssignments|[коллекция deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)|Список назначений групп для профиля конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|assignments|Коллекция [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|Список назначений для профиля конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|deviceStatuses|Коллекция [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md)|Состояние установки конфигурации для каждого устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|userStatuses|Коллекция [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md)|Состояние установки конфигурации устройства пользователем. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|Обзор состояния конфигурации устройств. Наследуется от [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|Обзор состояния конфигурации устройств для пользователей. Наследуется от [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|deviceSettingStateSummaries|Коллекция [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)|Сводка данных о состоянии настройки конфигурации устройств. Наследуется от [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|rootCertificatesForServerValidation|[коллекция windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md)|Укажите корневые сертификаты для проверки сервера. Эта коллекция может содержать не более 500 элементов.|
|identityCertificateForClientAuthentication|[windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)|Укажите сертификат удостоверения для проверки подлинности клиента.|
|secondaryIdentityCertificateForClientAuthentication|[windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)|Укажите дополнительный сертификат удостоверения для проверки подлинности клиента.|
|rootCertificateForClientValidation|[windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md)|Укажите корневой сертификат для проверки клиента.|
|secondaryRootCertificateForClientValidation|[windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md)|Укажите вторичный корневой сертификат для проверки клиента.|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsWiredNetworkConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsWiredNetworkConfiguration",
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
  "authenticationType": "String",
  "cacheCredentials": true,
  "authenticationPeriodInSeconds": 1024,
  "authenticationRetryDelayPeriodInSeconds": 1024,
  "eapolStartPeriodInSeconds": 1024,
  "maximumEAPOLStartMessages": 1024,
  "maximumAuthenticationFailures": 1024,
  "enforce8021X": true,
  "authenticationBlockPeriodInMinutes": 1024,
  "eapType": "String",
  "trustedServerCertificateNames": [
    "String"
  ],
  "authenticationMethod": "String",
  "secondaryAuthenticationMethod": "String",
  "innerAuthenticationProtocolForEAPTTLS": "String",
  "outerIdentityPrivacyTemporaryValue": "String",
  "performServerValidation": true,
  "disableUserPromptForServerValidation": true,
  "requireCryptographicBinding": true,
  "forceFIPSCompliance": true
}
```





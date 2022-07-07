---
title: Тип ресурса windowsWiredNetworkConfiguration
description: Эта сущность предоставляет описания объявленных методов, свойств и связей, предоставляемых CSP проводной сети.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: de125dfd9b73435ee3ebf7fd69fc2c41c4e6f81d
ms.sourcegitcommit: 7bc623e73fdfb970dbd0a62154d10bb2863afaf7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/07/2022
ms.locfileid: "66669506"
---
# <a name="windowswirednetworkconfiguration-resource-type"></a>Тип ресурса windowsWiredNetworkConfiguration

Пространство имен: microsoft.graph

> **Важно:** API Microsoft Graph в версии /beta могут быть изменены; использование в рабочей области не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Эта сущность предоставляет описания объявленных методов, свойств и связей, предоставляемых CSP проводной сети.


Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Перечисление объектов windowsWiredNetworkConfiguration](../api/intune-deviceconfig-windowswirednetworkconfiguration-list.md)|[Коллекция windowsWiredNetworkConfiguration](../resources/intune-deviceconfig-windowswirednetworkconfiguration.md)|Список свойств и связей объектов [windowsWiredNetworkConfiguration](../resources/intune-deviceconfig-windowswirednetworkconfiguration.md) .|
|[Получение объекта windowsWiredNetworkConfiguration](../api/intune-deviceconfig-windowswirednetworkconfiguration-get.md)|[windowsWiredNetworkConfiguration](../resources/intune-deviceconfig-windowswirednetworkconfiguration.md)|Чтение свойств и связей объекта [windowsWiredNetworkConfiguration](../resources/intune-deviceconfig-windowswirednetworkconfiguration.md) .|
|[Создание объекта windowsWiredNetworkConfiguration](../api/intune-deviceconfig-windowswirednetworkconfiguration-create.md)|[windowsWiredNetworkConfiguration](../resources/intune-deviceconfig-windowswirednetworkconfiguration.md)|Создайте объект [windowsWiredNetworkConfiguration](../resources/intune-deviceconfig-windowswirednetworkconfiguration.md) .|
|[Удаление объекта windowsWiredNetworkConfiguration](../api/intune-deviceconfig-windowswirednetworkconfiguration-delete.md)|Нет|Удаляет объект [windowsWiredNetworkConfiguration](../resources/intune-deviceconfig-windowswirednetworkconfiguration.md).|
|[Обновление объекта windowsWiredNetworkConfiguration](../api/intune-deviceconfig-windowswirednetworkconfiguration-update.md)|[windowsWiredNetworkConfiguration](../resources/intune-deviceconfig-windowswirednetworkconfiguration.md)|Обновление свойств объекта [windowsWiredNetworkConfiguration](../resources/intune-deviceconfig-windowswirednetworkconfiguration.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|Идентификаторы roleScopeTagId|Коллекция строк|Список тегов области для этого экземпляра сущности. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|supportsScopeTags|Логическое|Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области. Назначение свойству ScopeTags не допускается, если это значение имеет значение false и сущности не будут видны пользователям с заданной областью. Это происходит для устаревших политик, созданных в Silverlight, и их можно устранить, удалив и повторно создав политику на портале Azure. Это свойство доступно только для чтения. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|deviceManagementApplicabilityRuleOsEdition|[deviceManagementApplicabilityRuleOsEdition](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|Применимость выпуска ОС для этой политики. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|deviceManagementApplicabilityRuleOsVersion|[deviceManagementApplicabilityRuleOsVersion](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|Правило применимости версии ОС для этой политики. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|deviceManagementApplicabilityRuleDeviceMode|[deviceManagementApplicabilityRuleDeviceMode](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|Правило применимости режима устройства для этой политики. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|createdDateTime|DateTimeOffset|Дата и время создания объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|description|String|Указанное администратором описание конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|displayName|String|Указанное администратором имя конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|version|Int32|Версия конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|authenticationType|[WiredNetworkAuthenticationType](../resources/intune-deviceconfig-wirednetworkauthenticationtype.md)|Укажите, следует ли выполнить проверку подлинности пользователя, устройства или использовать гостевую проверку подлинности (нет). Если вы используете проверку подлинности сертификата, убедитесь, что тип сертификата соответствует типу проверки подлинности. Возможные значения: `none`, `user`, `machine`, `machineOrUser`, `guest`. Возможные значения: `none`, `user`, `machine`, `machineOrUser`, `guest`, `unknownFutureValue`.|
|cacheCredentials|Логический|При значении TRUE кэширует учетные данные пользователя на устройстве, чтобы пользователям не нужно было вводить их при каждом подключении. Если значение равно FALSE, не кэшировать учетные данные. Значение по умолчанию — FALSE.|
|authenticationPeriodInSeconds|Int32|Укажите время ожидания клиента в секундах после попытки проверки подлинности перед сбоем. Допустимый диапазон от 1 до 3600.|
|authenticationRetryDelayPeriodInSeconds|Int32|Укажите время в секундах между неудачной проверкой подлинности и следующей попыткой проверки подлинности. Допустимый диапазон от 1 до 3600.|
|eapolStartPeriodInSeconds|Int32|Укажите время ожидания в секундах перед отправкой начального сообщения EAPOL (расширяемого протокола проверки подлинности по локальной сети). Допустимый диапазон от 1 до 3600.|
|maximumEAPOLStartMessages|Int32|Укажите максимальное количество сообщений EAPOL (расширяемого протокола проверки подлинности по локальной сети), которые будут отправляться перед возвратом сбоя. Допустимый диапазон от 1 до 100.|
|maximumAuthenticationFailures|Int32|Укажите максимально допустимые сбои проверки подлинности для набора учетных данных. Допустимый диапазон от 1 до 100.|
|enforce8021X|Логическое|При значении TRUE служба автоматической настройки для проводных сетей требует использования 802.1X для проверки подлинности портов. При значении FALSE 802.1X не требуется. Значение по умолчанию — FALSE.|
|authenticationBlockPeriodInMinutes|Int32|Укажите длительность, в течение которой попытки автоматической проверки подлинности будут заблокированы после неудачной попытки проверки подлинности.|
|eapType|[eapType](../resources/intune-deviceconfig-eaptype.md)|Расширяемый протокол проверки подлинности (EAP). Указывает тип протокола EAP, задаваемого в конечной Wi-Fi (маршрутизаторе). Возможные значения: `eapTls`, `leap`, `eapSim`, `eapTtls`, `peap`, `eapFast`, `teap`. Возможные значения: `eapTls`, `leap`, `eapSim`, `eapTtls`, `peap`, `eapFast`, `teap`.|
|trustedServerCertificateNames|Коллекция строк|Укажите имена доверенных сертификатов сервера.|
|authenticationMethod|[wiredNetworkAuthenticationMethod](../resources/intune-deviceconfig-wirednetworkauthenticationmethod.md)|Укажите метод проверки подлинности. Возможные значения: `certificate`, `usernameAndPassword`, `derivedCredential`. Возможные значения: `certificate`, `usernameAndPassword`, `derivedCredential`, `unknownFutureValue`.|
|secondaryAuthenticationMethod|[wiredNetworkAuthenticationMethod](../resources/intune-deviceconfig-wirednetworkauthenticationmethod.md)|Укажите дополнительный метод проверки подлинности. Возможные значения: `certificate`, `usernameAndPassword`, `derivedCredential`. Возможные значения: `certificate`, `usernameAndPassword`, `derivedCredential`, `unknownFutureValue`.|
|innerAuthenticationProtocolForEAPTTLS|[nonEapAuthenticationMethodForEapTtlsType](../resources/intune-deviceconfig-noneapauthenticationmethodforeapttlstype.md)|Укажите внутренний протокол проверки подлинности для протокола TTLS EAP. Возможные значения: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`. Возможные значения: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.|
|outerIdentityPrivacyTemporaryValue|String|Укажите строку для замены имен пользователей для обеспечения конфиденциальности при использовании EAP TTLS или PEAP.|
|performServerValidation|Логическое|При значении TRUE включает проверку удостоверения сервера путем проверки сертификата при выборе типа EAP в качестве PEAP. Если значение равно FALSE, сертификат не проверяется. Значение по умолчанию — TRUE.|
|disableUserPromptForServerValidation|Логический|Значение TRUE запрещает пользователю запрашивать авторизацию новых серверов для доверенных центров сертификации при выборе типа EAP в качестве PEAP. Значение FALSE не запрещает пользователю запрашивать запросы. Значение по умолчанию — FALSE.|
|requireCryptographicBinding|Логический|Если значение равно TRUE, включает криптографическую привязку, если тип EAP выбран в качестве PEAP. При значении FALSE не включает криптографическое связывание. Значение по умолчанию — TRUE.|
|forceFIPSCompliance|Логический|Если значение равно TRUE, принудительное соответствие FIPS. Если значение равно FALSE, не включается соответствие FIPS. Значение по умолчанию — FALSE.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|groupAssignments|[Коллекция deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)|Список назначений групп для профиля конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|assignments|Коллекция [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|Список назначений для профиля конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|deviceStatuses|Коллекция [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md)|Состояние установки конфигурации для каждого устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|userStatuses|Коллекция [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md)|Состояние установки конфигурации устройства по пользователю. Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|Обзор состояния конфигурации устройств. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|Обзор состояния конфигурации устройств для пользователей. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|deviceSettingStateSummaries|Коллекция [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)|Сводка данных о состоянии настройки конфигурации устройств. Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).|
|rootCertificatesForServerValidation|[Коллекция windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md)|Укажите корневые сертификаты для проверки сервера. Эта коллекция может содержать не более 500 элементов.|
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





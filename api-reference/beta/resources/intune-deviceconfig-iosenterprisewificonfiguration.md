---
title: тип ресурса iosEnterpriseWiFiConfiguration
description: Предоставляя конфигурации в этом профиле, вы можете поручить устройству iOS подключиться к нужной Wi-Fi конечной точке. Указав метод проверки подлинности и типы безопасности, ожидаемые Wi-Fi конечной точкой, вы можете сделать подключение Wi-Fi бесшовным для конечного пользователя.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: eda4bd3ac28285771e4a303ed584f8b5afc87737
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59091757"
---
# <a name="iosenterprisewificonfiguration-resource-type"></a>тип ресурса iosEnterpriseWiFiConfiguration

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Предоставляя конфигурации в этом профиле, вы можете поручить устройству iOS подключиться к нужной Wi-Fi конечной точке. Указав метод проверки подлинности и типы безопасности, ожидаемые Wi-Fi конечной точкой, вы можете сделать подключение Wi-Fi бесшовным для конечного пользователя.


Наследуется [от iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список iosEnterpriseWiFiConfigurations](../api/intune-deviceconfig-iosenterprisewificonfiguration-list.md)|[коллекция iosEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-iosenterprisewificonfiguration.md)|Список свойств и связей объектов [iosEnterpriseWiFiConfiguration.](../resources/intune-deviceconfig-iosenterprisewificonfiguration.md)|
|[Get iosEnterpriseWiFiConfiguration](../api/intune-deviceconfig-iosenterprisewificonfiguration-get.md)|[iosEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-iosenterprisewificonfiguration.md)|Чтение свойств и связей объекта [iosEnterpriseWiFiConfiguration.](../resources/intune-deviceconfig-iosenterprisewificonfiguration.md)|
|[Создание iosEnterpriseWiFiConfiguration](../api/intune-deviceconfig-iosenterprisewificonfiguration-create.md)|[iosEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-iosenterprisewificonfiguration.md)|Создайте новый [объект iosEnterpriseWiFiConfiguration.](../resources/intune-deviceconfig-iosenterprisewificonfiguration.md)|
|[Удаление iosEnterpriseWiFiConfiguration](../api/intune-deviceconfig-iosenterprisewificonfiguration-delete.md)|Нет|Удаляет [iosEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-iosenterprisewificonfiguration.md).|
|[Обновление iosEnterpriseWiFiConfiguration](../api/intune-deviceconfig-iosenterprisewificonfiguration-update.md)|[iosEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-iosenterprisewificonfiguration.md)|Обновление свойств объекта [iosEnterpriseWiFiConfiguration.](../resources/intune-deviceconfig-iosenterprisewificonfiguration.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|roleScopeTagIds|Коллекция объектов string|Список тегов области для этого экземпляра Entity. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|supportsScopeTags|Логическое|Указывает, поддерживает ли вся конфигурация устройства назначение тегов области. Назначение свойства ScopeTags не допускается, если это значение является ложным и объекты не будут видны пользователям с охватом. Это происходит для политик Legacy, созданных в Silverlight, и их можно разрешить путем удаления и воссоздания политики на портале Azure. Это свойство доступно только для чтения. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|deviceManagementApplicabilityRuleOsEdition|[deviceManagementApplicabilityRuleOsEdition](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|Применимость к выпуску ОС для этой политики. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|deviceManagementApplicabilityRuleOsVersion|[deviceManagementApplicabilityRuleOsVersion](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|Правило применимости версии ОС для этой политики. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|deviceManagementApplicabilityRuleDeviceMode|[deviceManagementApplicabilityRuleDeviceMode](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|Правило применимости режима устройства для этой политики. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|createdDateTime|DateTimeOffset|Дата и время создания объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|description|String|Указанное администратором описание конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|displayName|String|Указанное администратором имя конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|version|Int32|Версия конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|networkName|String|Имя сети, унаследованные от [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)|
|ssid|String|Это имя сети Wi-Fi, которая транслируется на все устройства. Унаследованный от [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)|
|connectAutomatically|Логический|Подключение автоматически, когда эта сеть находится в диапазоне. Настройка этого параметра будет пропускать запрос пользователя и автоматически подключать устройство к Wi-Fi сети. Унаследованный от [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)|
|connectWhenNetworkNameIsHidden|Логическое|Подключение, когда сеть не передает свое имя (SSID). Если задана истина, этот профиль заставляет устройство подключаться к сети, которая не передает SSID на все устройства. Унаследованный от [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)|
|wiFiSecurityType|[wiFiSecurityType](../resources/intune-deviceconfig-wifisecuritytype.md)|Указывает, Wi-Fi конечная точка использует тип безопасности на основе EAP. Наследуется [от iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md). Возможные значения: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.|
|proxySettings|[wiFiProxySetting](../resources/intune-deviceconfig-wifiproxysetting.md)|Тип прокси для этого Wi-Fi, унаследованный от [iosWiFiConfiguration.](../resources/intune-deviceconfig-ioswificonfiguration.md) Возможные значения: `none`, `manual`, `automatic`.|
|proxyManualAddress|String|IP-адрес или DNS-имя прокси-сервера при выборе ручной конфигурации. Унаследованный от [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)|
|proxyManualPort|Int32|Порт прокси-сервера при выборе ручной конфигурации. Унаследованный от [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)|
|proxyAutomaticConfigurationUrl|String|URL-адрес сценария автоматической конфигурации прокси-сервера при выборе автоматической конфигурации. Этот URL-адрес обычно является расположением файла PAC (Proxy Auto Configuration). Унаследованный от [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)|
|отключениеMacAddressRandomization|Логическое|Если установлено истинное, устройства, подключающиеся с помощью этого Wi-Fi профиля, должны представить Wi-Fi mac-адрес, а не случайный MAC-адрес. Применяется к iOS 14 и более поздней. Унаследованный от [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)|
|preSharedKey|String|Это предварительный общий ключ для сети персональных Wi-Fi WPA. Унаследованный от [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)|
|eapType|[eapType](../resources/intune-deviceconfig-eaptype.md)|Extensible Authentication Protocol (EAP). Указывает тип протокола EAP на конечной точке Wi-Fi (маршрутизатор). Возможные значения: `eapTls`, `leap`, `eapSim`, `eapTtls`, `peap`, `eapFast`.|
|eapFastConfiguration|[eapFastConfiguration](../resources/intune-deviceconfig-eapfastconfiguration.md)|Вариант конфигурации FAST EAP-FAST является выбранным типом EAP. Возможные значения: `noProtectedAccessCredential`, `useProtectedAccessCredential`, `useProtectedAccessCredentialAndProvision`, `useProtectedAccessCredentialAndProvisionAnonymously`.|
|trustedServerCertificateNames|Коллекция объектов string|Доверенные имена сертификатов сервера при настройке типа EAP-TLS/TTLS/FAST или PEAP. Это общее имя, используемая в сертификатах, выдаванных доверенным органом сертификации (CA). Если вы предоставите эту информацию, можно обойти динамический диалог доверия, отображаемый на устройствах конечных пользователей при подключении к Wi-Fi сети.|
|authenticationMethod|[wiFiAuthenticationMethod](../resources/intune-deviceconfig-wifiauthenticationmethod.md)|Метод проверки подлинности при настройке типа EAP на PEAP или EAP-TTLS. Возможные значения: `certificate`, `usernameAndPassword`, `derivedCredential`.|
|innerAuthenticationProtocolForEapTtls|[nonEapAuthenticationMethodForEapTtlsType](../resources/intune-deviceconfig-noneapauthenticationmethodforeapttlstype.md)|Метод без EAP для проверки подлинности, если тип EAP — EAP-TTLS, а проверка подлинности — имя пользователя и пароль. Возможные значения: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.|
|outerIdentityPrivacyTemporaryValue|String|Включить конфиденциальность удостоверений (внешний идентификатор), когда тип EAP настроен на EAP - TTLS, EAP - FAST или PEAP. Это свойство маскирует имена пользователей с вводимым текстом. Например, если используется "анонимный", каждый пользователь, который Wi-Fi с этим подключением, используя свое реальное имя пользователя, отображается как "анонимный".|
|usernameFormatString|String|Строка формата username, используемая для создания имени пользователя для подключения к Wi-Fi|
|passwordFormatString|String|Строка формата пароля, используемая для создания пароля для подключения к Wi-Fi|

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
|rootCertificatesForServerValidation|[коллекция iosTrustedRootCertificate](../resources/intune-deviceconfig-iostrustedrootcertificate.md)|Надежные корневые сертификаты для проверки сервера при настройке типа EAP на EAP-TLS/TTLS/FAST или PEAP. Если вы предоставляете это значение, вам не нужно предоставлять trustedServerCertificateNames и наоборот.|
|identityCertificateForClientAuthentication|[iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)|Сертификат удостоверения для проверки подлинности клиента при настройке типа EAP на EAP-TLS, EAP-TTLS (с проверкой подлинности сертификата) или PEAP (с проверкой подлинности сертификата).|
|derivedCredentialSettings|[deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md)|Параметры уровня клиента для производных учетных данных, которые будут использоваться для проверки подлинности.|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iosEnterpriseWiFiConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosEnterpriseWiFiConfiguration",
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
  "preSharedKey": "String",
  "eapType": "String",
  "eapFastConfiguration": "String",
  "trustedServerCertificateNames": [
    "String"
  ],
  "authenticationMethod": "String",
  "innerAuthenticationProtocolForEapTtls": "String",
  "outerIdentityPrivacyTemporaryValue": "String",
  "usernameFormatString": "String",
  "passwordFormatString": "String"
}
```




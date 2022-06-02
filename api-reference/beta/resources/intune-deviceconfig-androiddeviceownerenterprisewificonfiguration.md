---
title: Тип ресурса androidDeviceOwnerEnterpriseWiFiConfiguration
description: Указав конфигурации в этом профиле, вы можете указать устройству Android устройства владельца устройства подключиться к нужной Wi-Fi конечной точке. Указав метод проверки подлинности и типы безопасности, ожидаемые Wi-Fi конечной точкой, можно сделать подключение Wi-Fi простым для конечного пользователя.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: eb6656a2d8e38629b3f80be6b5565724a5350b31
ms.sourcegitcommit: 435d70e7adb27e6cedaf485ebfdab7c3ef9ffacf
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/02/2022
ms.locfileid: "65858323"
---
# <a name="androiddeviceownerenterprisewificonfiguration-resource-type"></a>Тип ресурса androidDeviceOwnerEnterpriseWiFiConfiguration

Пространство имен: microsoft.graph

> **Важно:** API Graph Майкрософт в версии /beta могут быть изменены; использование в рабочей области не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Указав конфигурации в этом профиле, вы можете указать устройству Android устройства владельца устройства подключиться к нужной Wi-Fi конечной точке. Указав метод проверки подлинности и типы безопасности, ожидаемые Wi-Fi конечной точкой, можно сделать подключение Wi-Fi простым для конечного пользователя.


Наследует от [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Перечисление объектов androidDeviceOwnerEnterpriseWiFiConfigurations](../api/intune-deviceconfig-androiddeviceownerenterprisewificonfiguration-list.md)|[Коллекция androidDeviceOwnerEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerenterprisewificonfiguration.md)|Список свойств и связей объектов [androidDeviceOwnerEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerenterprisewificonfiguration.md) .|
|[Получение объекта androidDeviceOwnerEnterpriseWiFiConfiguration](../api/intune-deviceconfig-androiddeviceownerenterprisewificonfiguration-get.md)|[androidDeviceOwnerEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerenterprisewificonfiguration.md)|Чтение свойств и связей объекта [androidDeviceOwnerEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerenterprisewificonfiguration.md) .|
|[Создание объекта androidDeviceOwnerEnterpriseWiFiConfiguration](../api/intune-deviceconfig-androiddeviceownerenterprisewificonfiguration-create.md)|[androidDeviceOwnerEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerenterprisewificonfiguration.md)|Создайте объект [androidDeviceOwnerEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerenterprisewificonfiguration.md) .|
|[Удаление объекта androidDeviceOwnerEnterpriseWiFiConfiguration](../api/intune-deviceconfig-androiddeviceownerenterprisewificonfiguration-delete.md)|Нет|Удаляет [объект androidDeviceOwnerEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerenterprisewificonfiguration.md).|
|[Обновление объекта androidDeviceOwnerEnterpriseWiFiConfiguration](../api/intune-deviceconfig-androiddeviceownerenterprisewificonfiguration-update.md)|[androidDeviceOwnerEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerenterprisewificonfiguration.md)|Обновление свойств объекта [androidDeviceOwnerEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerenterprisewificonfiguration.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Ключ объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|Идентификаторы roleScopeTagId|Коллекция String|Список тегов области для этого экземпляра сущности. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|supportsScopeTags|Boolean|Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области. Назначение свойству ScopeTags не допускается, если это значение имеет значение false и сущности не будут видны пользователям с заданной областью. Это происходит для устаревших политик, созданных в Silverlight, и их можно устранить, удалив и повторно создав политику на портале Azure. Это свойство доступно только для чтения. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|deviceManagementApplicabilityRuleOsEdition|[deviceManagementApplicabilityRuleOsEdition](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|Применимость выпуска ОС для этой политики. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|deviceManagementApplicabilityRuleOsVersion|[deviceManagementApplicabilityRuleOsVersion](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|Правило применимости версии ОС для этой политики. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|deviceManagementApplicabilityRuleDeviceMode|[deviceManagementApplicabilityRuleDeviceMode](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|Правило применимости режима устройства для этой политики. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|createdDateTime|DateTimeOffset|Дата и время создания объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|description|Строка|Указанное администратором описание конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|displayName|Строка|Указанное администратором имя конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|version|Int32|Версия конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|networkName|Строка|Сетевое имя, наследуемое [от androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)|
|Ssid|Строка|Это имя сети Wi-Fi, которая передается на все устройства. Наследуется [от androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)|
|connectAutomatically|Boolean|Подключение, если эта сеть находится в диапазоне. Если задано значение true, запрос пользователя будет пропущен и устройство будет автоматически подключено к Wi-Fi сети. Наследуется [от androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)|
|connectWhenNetworkNameIsHidden|Boolean|Если задано значение true, этот профиль принудительно подключает устройство к сети, которая не передает свой SSID на все устройства. Наследуется [от androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)|
|wiFiSecurityType|[androidDeviceOwnerWiFiSecurityType](../resources/intune-deviceconfig-androiddeviceownerwifisecuritytype.md)|Указывает, использует ли Wi-Fi конечная точка тип безопасности на основе EAP. Наследуется [от androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md). Возможные значения: `open`, `wep`, `wpaPersonal`, `wpaEnterprise`.|
|preSharedKey|Строка|Это общий ключ для WPA Personal Wi-Fi сети. Наследуется [от androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)|
|preSharedKeyIsSet|Boolean|Это общий ключ для WPA Personal Wi-Fi сети. Наследуется [от androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)|
|proxySettings|[wiFiProxySetting](../resources/intune-deviceconfig-wifiproxysetting.md)|Укажите параметр прокси-сервера для Wi-Fi конфигурации. Возможные значения: none, manual и automatic. Наследуется [от androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md). Возможные значения: `none`, `manual`, `automatic`.|
|proxyManualAddress|Строка|Укажите IP-адрес прокси-сервера. Android документации не указывает IPv4 или IPv6. Например, 192.168.1.1. Наследуется [от androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)|
|proxyManualPort|Int32|Укажите порт прокси-сервера. Наследуется [от androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)|
|proxyAutomaticConfigurationUrl|String|Укажите URL-адрес скрипта конфигурации прокси-сервера. Наследуется [от androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)|
|proxyExclusionList|Строка|Список узлов, исключаемых с помощью прокси-сервера для подключений. Эти узлы могут использовать подстановочные знаки, такие как *.example.com. Наследуется [от androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)|
|eapType|[androidEapType](../resources/intune-deviceconfig-androideaptype.md)|Указывает тип протокола EAP, задаваемого в конечной Wi-Fi (маршрутизаторе). Возможные значения: `eapTls`, `eapTtls`, `peap`.|
|trustedServerCertificateNames|Коллекция объектов string|Имена сертификатов доверенных серверов, если тип EAP настроен на EAP-TLS/TTLS/FAST или PEAP. Это общее имя, используемого в сертификатах, выданных доверенным центром сертификации (ЦС). Если вы предоставите эти сведения, можно обойти диалоговое окно динамического доверия, отображаемое на устройствах конечных пользователей при подключении к этой Wi-Fi сети.|
|authenticationMethod|[wiFiAuthenticationMethod](../resources/intune-deviceconfig-wifiauthenticationmethod.md)|Указывает метод проверки подлинности, который клиент (устройство) должен использовать, если тип EAP настроен на PEAP или EAP-TTLS. Возможные значения: `certificate`, `usernameAndPassword`, `derivedCredential`.|
|innerAuthenticationProtocolForEapTtls|[nonEapAuthenticationMethodForEapTtlsType](../resources/intune-deviceconfig-noneapauthenticationmethodforeapttlstype.md)|Метод, отличный от EAP для проверки подлинности (внутреннее удостоверение), если тип EAP — EAP-TTLS, а authenticationmethod — имя пользователя и пароль. Возможные значения: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.|
|innerAuthenticationProtocolForPeap|[nonEapAuthenticationMethodForPeap](../resources/intune-deviceconfig-noneapauthenticationmethodforpeap.md)|Метод, отличный от EAP для проверки подлинности (внутреннее удостоверение), если тип EAP — PEAP, а authenticationmethod — имя пользователя и пароль. Возможные значения: `none`, `microsoftChapVersionTwo`.|
|outerIdentityPrivacyTemporaryValue|Строка|Включите конфиденциальность удостоверений (внешнее удостоверение), если тип EAP настроен на EAP-TTLS или PEAP. Указанная здесь строка используется для маскирования имени пользователя отдельных пользователей при попытке подключения к Wi-Fi сети.|

## <a name="relationships"></a>Отношения
|Связь|Тип|Описание|
|:---|:---|:---|
|groupAssignments|[Коллекция deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)|Список назначений групп для профиля конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|assignments|Коллекция [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|Список назначений для профиля конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|deviceStatuses|Коллекция [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md)|Состояние установки конфигурации для каждого устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|userStatuses|Коллекция [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md)|Состояние установки конфигурации устройства по пользователю. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|Обзор состояния конфигурации устройств. Наследуется от [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|Обзор состояния конфигурации устройств для пользователей. Наследуется от [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|deviceSettingStateSummaries|Коллекция [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)|Сводка данных о состоянии настройки конфигурации устройств. Наследуется от [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|rootCertificateForServerValidation|[androidDeviceOwnerTrustedRootCertificate](../resources/intune-deviceconfig-androiddeviceownertrustedrootcertificate.md)|Доверенный корневой сертификат для проверки сервера, если тип EAP настроен на EAP-TLS, EAP-TTLS или PEAP. Это сертификат, представленный конечной точкой Wi-Fi, когда устройство пытается подключиться к Wi-Fi конечной точке. Устройство (или пользователь) должно принять этот сертификат, чтобы продолжить попытку подключения.|
|identityCertificateForClientAuthentication|[androidDeviceOwnerCertificateProfileBase](../resources/intune-deviceconfig-androiddeviceownercertificateprofilebase.md)|Сертификат удостоверения для проверки подлинности клиента, если тип EAP настроен на EAP-TLS, EAP-TTLS (с проверкой подлинности на основе сертификата) или PEAP (с проверкой подлинности сертификата). Это сертификат, представленный клиентом конечной точке Wi-Fi. Сервер проверки подлинности, на котором находится Wi-Fi конечной точке, должен принять этот сертификат, чтобы успешно установить Wi-Fi подключения.|
|derivedCredentialSettings|[deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md)|Параметры уровня клиента для производных учетных данных, используемых для проверки подлинности.|

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
  "proxySettings": "String",
  "proxyManualAddress": "String",
  "proxyManualPort": 1024,
  "proxyAutomaticConfigurationUrl": "String",
  "proxyExclusionList": "String",
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





---
title: Обновление windowsWiredNetworkConfiguration
description: Обновление свойств объекта WindowsWiredNetworkConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1a9afc89ae5a9bfe224769e59c05870d1a33cb5e
ms.sourcegitcommit: 0076eb6abb89be3dca3575631924a74a5202be30
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/03/2022
ms.locfileid: "64631372"
---
# <a name="update-windowswirednetworkconfiguration"></a>Обновление windowsWiredNetworkConfiguration

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Обновление свойств объекта [WindowsWiredNetworkConfiguration](../resources/intune-deviceconfig-windowswirednetworkconfiguration.md) .

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementConfiguration.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|DeviceManagementConfiguration.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Authorization|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В теле запроса предоставляем представление JSON для [объекта WindowsWiredNetworkConfiguration](../resources/intune-deviceconfig-windowswirednetworkconfiguration.md) .

В следующей таблице показаны свойства, необходимые при создании [windowsWiredNetworkConfiguration](../resources/intune-deviceconfig-windowswirednetworkconfiguration.md).

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Ключ объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|roleScopeTagIds|Коллекция String|Список тегов области для этого экземпляра Entity. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
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
|enforce8021X|Boolean|Когда true, автоматическая служба конфигурации для проводных сетей требует использования 802.1X для проверки подлинности порта. Если false, 802.1X не требуется. Значение по умолчанию false.|
|проверка подлинностиBlockPeriodInMinutes|Int32|Укажите продолжительность, в течение которой попытки автоматической проверки подлинности будут заблокированы после неудачной попытки проверки подлинности.|
|eapType|[eapType](../resources/intune-deviceconfig-eaptype.md)|Extensible Authentication Protocol (EAP). Указывает тип протокола EAP на конечной точке Wi-Fi (маршрутизатор). Возможные значения: `eapTls`, `leap`, `eapSim`, `eapTtls`, `peap`, `eapFast`, `teap`. Возможные значения: `eapTls`, `leap`, `eapSim`, `eapTtls`, `peap`, `eapFast`, `teap`.|
|trustedServerCertificateNames|Коллекция объектов string|Укажите имена доверенных сертификатов сервера.|
|authenticationMethod|[wiredNetworkAuthenticationMethod](../resources/intune-deviceconfig-wirednetworkauthenticationmethod.md)|Укажите метод проверки подлинности. Возможные значения: `certificate`, `usernameAndPassword`, `derivedCredential`. Возможные значения: `certificate`, `usernameAndPassword`, `derivedCredential`, `unknownFutureValue`.|
|secondaryAuthenticationMethod|[wiredNetworkAuthenticationMethod](../resources/intune-deviceconfig-wirednetworkauthenticationmethod.md)|Укажите метод вторичной проверки подлинности. Возможные значения: `certificate`, `usernameAndPassword`, `derivedCredential`. Возможные значения: `certificate`, `usernameAndPassword`, `derivedCredential`, `unknownFutureValue`.|
|innerAuthenticationProtocolForEAPTTLS|[nonEapAuthenticationMethodForEapTtlsType](../resources/intune-deviceconfig-noneapauthenticationmethodforeapttlstype.md)|Укажите внутренний протокол проверки подлинности для TTLS EAP. Возможные значения: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`. Возможные значения: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.|
|outerIdentityPrivacyTemporaryValue|Строка|Укажите строку для замены имен пользователей для конфиденциальности при использовании EAP TTLS или PEAP.|
|performServerValidation|Boolean|Когда TRUE, включает проверку удостоверения сервера путем проверки сертификата при выборе типа EAP в качестве PEAP. Если false, сертификат не проверяется. Значение по умолчанию — TRUE.|
|disableUserPromptForServerValidation|Boolean|Если TRUE, не позволяет пользователю получить запрос на авторизации новых серверов для доверенных органов сертификации при выборе типа EAP в качестве PEAP. Если false, не препятствует запросу пользователя. Значение по умолчанию false.|
|requireCryptographicBinding|Логический|Когда TRUE, включает криптографическую привязку, когда тип EAP выбран в качестве PEAP. При FALSE не включается криптогрпахическая привязка. Значение по умолчанию — TRUE.|
|forceFIPSCompliance|Логическое|Когда true, заставляет соответствие ТРЕБОВАНИЯМ FIPS. Если false, не включает соответствие ТРЕБОВАНИЯМ FIPS. Значение по умолчанию false.|



## <a name="response"></a>Отклик
В случае успешной `200 OK` работы этот метод возвращает код отклика и обновленный [объект WindowsWiredNetworkConfiguration](../resources/intune-deviceconfig-windowswirednetworkconfiguration.md) в теле отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1920

{
  "@odata.type": "#microsoft.graph.windowsWiredNetworkConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "windows10EnterpriseN"
    ],
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "Min OSVersion value",
    "maxOSVersion": "Max OSVersion value",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "sModeConfiguration",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "authenticationType": "user",
  "cacheCredentials": true,
  "authenticationPeriodInSeconds": 13,
  "authenticationRetryDelayPeriodInSeconds": 7,
  "eapolStartPeriodInSeconds": 9,
  "maximumEAPOLStartMessages": 9,
  "maximumAuthenticationFailures": 13,
  "enforce8021X": true,
  "authenticationBlockPeriodInMinutes": 2,
  "eapType": "leap",
  "trustedServerCertificateNames": [
    "Trusted Server Certificate Names value"
  ],
  "authenticationMethod": "usernameAndPassword",
  "secondaryAuthenticationMethod": "usernameAndPassword",
  "innerAuthenticationProtocolForEAPTTLS": "challengeHandshakeAuthenticationProtocol",
  "outerIdentityPrivacyTemporaryValue": "Outer Identity Privacy Temporary Value value",
  "performServerValidation": true,
  "disableUserPromptForServerValidation": true,
  "requireCryptographicBinding": true,
  "forceFIPSCompliance": true
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2092

{
  "@odata.type": "#microsoft.graph.windowsWiredNetworkConfiguration",
  "id": "ec132acd-2acd-ec13-cd2a-13eccd2a13ec",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "windows10EnterpriseN"
    ],
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "Min OSVersion value",
    "maxOSVersion": "Max OSVersion value",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "sModeConfiguration",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "authenticationType": "user",
  "cacheCredentials": true,
  "authenticationPeriodInSeconds": 13,
  "authenticationRetryDelayPeriodInSeconds": 7,
  "eapolStartPeriodInSeconds": 9,
  "maximumEAPOLStartMessages": 9,
  "maximumAuthenticationFailures": 13,
  "enforce8021X": true,
  "authenticationBlockPeriodInMinutes": 2,
  "eapType": "leap",
  "trustedServerCertificateNames": [
    "Trusted Server Certificate Names value"
  ],
  "authenticationMethod": "usernameAndPassword",
  "secondaryAuthenticationMethod": "usernameAndPassword",
  "innerAuthenticationProtocolForEAPTTLS": "challengeHandshakeAuthenticationProtocol",
  "outerIdentityPrivacyTemporaryValue": "Outer Identity Privacy Temporary Value value",
  "performServerValidation": true,
  "disableUserPromptForServerValidation": true,
  "requireCryptographicBinding": true,
  "forceFIPSCompliance": true
}
```





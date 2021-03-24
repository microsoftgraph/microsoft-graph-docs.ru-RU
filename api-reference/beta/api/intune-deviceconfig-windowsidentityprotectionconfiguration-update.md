---
title: Обновление windowsIdentityProtectionConfiguration
description: Обновление свойств объекта WindowsIdentityProtectionConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2317747e73ab159004dd5e16c359b7963ccd3dc3
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51132382"
---
# <a name="update-windowsidentityprotectionconfiguration"></a>Обновление windowsIdentityProtectionConfiguration

Пространство имен: microsoft.graph

> **Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Обновление свойств объекта [WindowsIdentityProtectionConfiguration.](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md)

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированное (рабочая или учебная учетная запись)|DeviceManagementConfiguration.ReadWrite.All|
|Делегированное (личная учетная запись Майкрософт)|Не поддерживается.|
|Приложение|DeviceManagementConfiguration.ReadWrite.All|

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
В теле запроса поставляем представление JSON для [объекта WindowsIdentityProtectionConfiguration.](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md)

В следующей таблице показаны свойства, необходимые при создании [windowsIdentityProtectionConfiguration.](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md)

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Ключ объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|roleScopeTagIds|Коллекция String|Список тегов области для этого экземпляра Entity. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|supportsScopeTags|Boolean|Указывает, поддерживает ли вся конфигурация устройства назначение тегов области. Назначение свойства ScopeTags не допускается, если это значение является ложным и объекты не будут видны пользователям с охватом. Это происходит для политик Legacy, созданных в Silverlight, и их можно разрешить путем удаления и воссоздания политики на портале Azure. Это свойство доступно только для чтения. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|deviceManagementApplicabilityRuleOsEdition|[deviceManagementApplicabilityRuleOsEdition](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|Применимость к выпуску ОС для этой политики. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|deviceManagementApplicabilityRuleOsVersion|[deviceManagementApplicabilityRuleOsVersion](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|Правило применимости версии ОС для этой политики. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|deviceManagementApplicabilityRuleDeviceMode|[deviceManagementApplicabilityRuleDeviceMode](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|Правило применимости режима устройства для этой политики. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|createdDateTime|DateTimeOffset|Дата и время создания объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|description|Строка|Указанное администратором описание конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|displayName|Строка|Указанное администратором имя конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|version|Int32|Версия конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|useSecurityKeyForSignin|Boolean|Значение Boolean, используемая для того, чтобы включить ключ безопасности Windows Hello в качестве учетных данных с логотипом.|
|enhancedAntiSpoofingForFacialFeaturesEnabled|Boolean|Значение Boolean, используемого для расширения функции распознавания лиц для проверки подлинности лиц в Windows Hello.|
|pinMinimumLength|Int32|Значение Integer, которое задает минимальное количество символов, необходимых для ПИН-кода Windows Hello для бизнеса. Допустимые значения : от 4 до 127 включительно и меньше или меньше значения, установленного для максимального ПИН-кода. Допустимые значения от 4 до 127|
|pinMaximumLength|Int32|Значение Integer, которое задает максимальное количество символов, разрешенных для пин-кода работы. Допустимые значения от 4 до 127 включительно и больше или равны значению, за набором для минимального ПИН-кода. Допустимые значения от 4 до 127|
|pinUppercaseCharactersUsage|[configurationUsage](../resources/intune-deviceconfig-configurationusage.md)|Это значение настраивает использование символов верхнего шкафа в ПИН-коде Windows Hello для бизнеса. Возможные значения: `blocked`, `required`, `allowed`, `notConfigured`.|
|pinLowercaseCharactersUsage|[configurationUsage](../resources/intune-deviceconfig-configurationusage.md)|Это значение настраивает использование символов нижнего регистра в ПИН-коде Windows Hello для бизнеса. Возможные значения: `blocked`, `required`, `allowed`, `notConfigured`.|
|pinSpecialCharactersUsage|[configurationUsage](../resources/intune-deviceconfig-configurationusage.md)|Управление возможностью использования специальных символов в ПИН-коде Windows Hello для бизнеса. Возможные значения: `blocked`, `required`, `allowed`, `notConfigured`.|
|pinExpirationInDays|Int32|Значение integer указывает период (в днях), который ПИН-код можно использовать до того, как система потребует от пользователя его изменить. Допустимые значения : от 0 до 730 включительно. Допустимые значения: от 0 до 730.|
|pinPreviousBlockCount|Int32|Контролирует возможность предотвращения использования пользователями прошлых ПИН-данных. Это должно быть установлено между 0 и 50 включительно, и текущий ПИН-код пользователя включен в это число. Если установлено 0, предыдущие ПИН-данные не сохраняются. История ПИН-кода не сохраняется с помощью сброса ПИН-кода. Допустимые значения: от 0 до 50.|
|pinRecoveryEnabled|Boolean|Значение Boolean, которое позволяет пользователю изменять ПИН-код с помощью службы восстановления ПИН-кода Windows Hello для бизнеса.|
|securityDeviceRequired|Boolean|Управление, необходимо ли требовать доверенный модуль платформы (TPM) для обеспечения Windows Hello для бизнеса. TPM предоставляет дополнительные преимущества безопасности в том, что данные, хранимые на нем, не могут использоваться на других устройствах. Если установлено false, все устройства могут устанавливать Windows Hello для бизнеса, даже если не существует понятного TPM.|
|unlockWithBiometricsEnabled|Boolean|Управление использованием биометрических жестов, таких как лицо и отпечатки пальцев, в качестве альтернативы ПИН-коду Windows Hello для бизнеса.  Если установлено false, биометрические жесты не допускаются. Пользователи по-прежнему должны настраивать ПИН-код в качестве резервного копирования в случае сбоев.|
|useCertificatesForOnPremisesAuthEnabled|Boolean|Значение Boolean, которое позволяет Windows Hello для бизнеса использовать сертификаты для проверки подлинности локального ресурса.|
|windowsHelloForBusinessBlocked|Boolean|Значение Boolean, которое блокирует Windows Hello для бизнеса как метод для подписания в Windows.|



## <a name="response"></a>Отклик
В случае успешной работы этот метод возвращает код отклика и обновленный `200 OK` [объект WindowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md) в тексте ответа.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1583

{
  "@odata.type": "#microsoft.graph.windowsIdentityProtectionConfiguration",
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
  "useSecurityKeyForSignin": true,
  "enhancedAntiSpoofingForFacialFeaturesEnabled": true,
  "pinMinimumLength": 0,
  "pinMaximumLength": 0,
  "pinUppercaseCharactersUsage": "required",
  "pinLowercaseCharactersUsage": "required",
  "pinSpecialCharactersUsage": "required",
  "pinExpirationInDays": 3,
  "pinPreviousBlockCount": 5,
  "pinRecoveryEnabled": true,
  "securityDeviceRequired": true,
  "unlockWithBiometricsEnabled": true,
  "useCertificatesForOnPremisesAuthEnabled": true,
  "windowsHelloForBusinessBlocked": true
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1755

{
  "@odata.type": "#microsoft.graph.windowsIdentityProtectionConfiguration",
  "id": "b2e64303-4303-b2e6-0343-e6b20343e6b2",
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
  "useSecurityKeyForSignin": true,
  "enhancedAntiSpoofingForFacialFeaturesEnabled": true,
  "pinMinimumLength": 0,
  "pinMaximumLength": 0,
  "pinUppercaseCharactersUsage": "required",
  "pinLowercaseCharactersUsage": "required",
  "pinSpecialCharactersUsage": "required",
  "pinExpirationInDays": 3,
  "pinPreviousBlockCount": 5,
  "pinRecoveryEnabled": true,
  "securityDeviceRequired": true,
  "unlockWithBiometricsEnabled": true,
  "useCertificatesForOnPremisesAuthEnabled": true,
  "windowsHelloForBusinessBlocked": true
}
```





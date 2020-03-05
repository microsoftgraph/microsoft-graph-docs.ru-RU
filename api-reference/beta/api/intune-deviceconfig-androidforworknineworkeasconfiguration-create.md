---
title: Создание Андроидфорворкниневоркеасконфигуратион
description: Создание нового объекта Андроидфорворкниневоркеасконфигуратион.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 32a77e0985efbe4890b9c3c9158e5eaa2259962a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42449854"
---
# <a name="create-androidforworknineworkeasconfiguration"></a>Создание Андроидфорворкниневоркеасконфигуратион

Пространство имен: Microsoft. Graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Создание нового объекта [андроидфорворкниневоркеасконфигуратион](../resources/intune-deviceconfig-androidforworknineworkeasconfiguration.md) .

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке убывания привилегий)|
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
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Authorization|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В тексте запроса добавьте представление объекта Андроидфорворкниневоркеасконфигуратион в формате JSON.

В следующей таблице приведены свойства, необходимые при создании Андроидфорворкниневоркеасконфигуратион.

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Ключ объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|roleScopeTagIds|Коллекция String|Список тегов областей для этого экземпляра сущности. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|суппортсскопетагс|Логический|Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области. Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия. Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure. Это свойство доступно только для чтения. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|deviceManagementApplicabilityRuleOsEdition|[deviceManagementApplicabilityRuleOsEdition](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|Применимость выпусков ОС для этой политики. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|deviceManagementApplicabilityRuleOsVersion|[deviceManagementApplicabilityRuleOsVersion](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|Правило применимости версии ОС для этой политики. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|deviceManagementApplicabilityRuleDeviceMode|[deviceManagementApplicabilityRuleDeviceMode](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|Правило применимости режима устройства для этой политики. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|createdDateTime|DateTimeOffset|Дата и время создания объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|description|String|Указанное администратором описание конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|displayName|Строка|Указанное администратором имя конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|version|Int32|Версия конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|Параметр authenticationmethod|[еасаусентикатионмесод](../resources/intune-deviceconfig-easauthenticationmethod.md)|Способ проверки подлинности для Exchange ActiveSync. Наследуется от [андроидфорворкеасемаилпрофилебасе](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md). Возможные значения: `usernameAndPassword`, `certificate`, `derivedCredential`.|
|дуратионофемаилтосинк|[емаилсинкдуратион](../resources/intune-deviceconfig-emailsyncduration.md)|Продолжительность синхронизации электронной почты. Наследуется от [андроидфорворкеасемаилпрофилебасе](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md). Возможные значения: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.|
|емаиладдресссаурце|[усеремаилсаурце](../resources/intune-deviceconfig-useremailsource.md)|Атрибут электронной почты, выбранный из AAD и добавленный в этот профиль перед установкой на устройстве. Наследуется от [андроидфорворкеасемаилпрофилебасе](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md). Возможные значения: `userPrincipalName`, `primarySmtpAddress`.|
|hostName|String|Расположение Exchange (URL-адрес), к которому подключается почтовое приложение. Наследуется от [андроидфорворкеасемаилпрофилебасе](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)|
|рекуирессл|Логический|Указывает, следует ли использовать SSL. Наследуется от [андроидфорворкеасемаилпрофилебасе](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)|
|usernameSource|[андроидусернамесаурце](../resources/intune-deviceconfig-androidusernamesource.md)|Атрибут username, который выбирается из AAD и вставляется в этот профиль перед установкой на устройстве. Наследуется от [андроидфорворкеасемаилпрофилебасе](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md). Возможные значения: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.|
|синккалендар|Логический|Включает и выключает синхронизацию календаря. Если задано значение false, календарь отключен на устройстве.|
|синкконтактс|Логический|Включает и выключает синхронизацию контактов. Если задано значение false, контакты на устройстве отключены.|
|синктаскс|Логический|Включает и выключает синхронизацию задач. Если задано значение false, задачи на устройстве отключены.|



## <a name="response"></a>Отклик
В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [андроидфорворкниневоркеасконфигуратион](../resources/intune-deviceconfig-androidforworknineworkeasconfiguration.md) в тексте отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1339

{
  "@odata.type": "#microsoft.graph.androidForWorkNineWorkEasConfiguration",
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
  "authenticationMethod": "certificate",
  "durationOfEmailToSync": "oneDay",
  "emailAddressSource": "primarySmtpAddress",
  "hostName": "Host Name value",
  "requireSsl": true,
  "usernameSource": "userPrincipalName",
  "syncCalendar": true,
  "syncContacts": true,
  "syncTasks": true
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1511

{
  "@odata.type": "#microsoft.graph.androidForWorkNineWorkEasConfiguration",
  "id": "f8ef19e0-19e0-f8ef-e019-eff8e019eff8",
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
  "authenticationMethod": "certificate",
  "durationOfEmailToSync": "oneDay",
  "emailAddressSource": "primarySmtpAddress",
  "hostName": "Host Name value",
  "requireSsl": true,
  "usernameSource": "userPrincipalName",
  "syncCalendar": true,
  "syncContacts": true,
  "syncTasks": true
}
```






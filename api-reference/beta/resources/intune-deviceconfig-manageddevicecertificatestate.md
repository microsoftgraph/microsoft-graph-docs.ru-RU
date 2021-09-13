---
title: тип ресурса managedDeviceCertificateState
description: Пока не задокументировано.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 2d8ccb42118e611903484b30d43b6017c044c6ca
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59086815"
---
# <a name="manageddevicecertificatestate-resource-type"></a>тип ресурса managedDeviceCertificateState

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Н/Д

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список managedDeviceCertificateStates](../api/intune-deviceconfig-manageddevicecertificatestate-list.md)|[коллекция managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md)|Список свойств и связей [объектов managedDeviceCertificateState.](../resources/intune-deviceconfig-manageddevicecertificatestate.md)|
|[Get managedDeviceCertificateState](../api/intune-deviceconfig-manageddevicecertificatestate-get.md)|[managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md)|Чтение свойств и связей [объекта managedDeviceCertificateState.](../resources/intune-deviceconfig-manageddevicecertificatestate.md)|
|[Создание managedDeviceCertificateState](../api/intune-deviceconfig-manageddevicecertificatestate-create.md)|[managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md)|Создайте новый [объект managedDeviceCertificateState.](../resources/intune-deviceconfig-manageddevicecertificatestate.md)|
|[Удаление managedDeviceCertificateState](../api/intune-deviceconfig-manageddevicecertificatestate-delete.md)|Нет|Удаляет [управляемыйDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md).|
|[Обновление managedDeviceCertificateState](../api/intune-deviceconfig-manageddevicecertificatestate-update.md)|[managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md)|Обновление свойств объекта [managedDeviceCertificateState.](../resources/intune-deviceconfig-manageddevicecertificatestate.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта.|
|devicePlatform|[devicePlatformType](../resources/intune-deviceconfig-deviceplatformtype.md)|Платформа устройства. Возможные значения: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`, `androidAOSP`.|
|certificateKeyUsage|[keyUsages](../resources/intune-shared-keyusages.md)|Использование ключей. Возможные значения: `keyEncipherment`, `digitalSignature`.|
|certificateValidityPeriodUnits|[certificateValidityPeriodScale](../resources/intune-shared-certificatevalidityperiodscale.md)|Единицы периода действия. Возможные значения: `days`, `months`, `years`.|
|certificateIssuanceState|[certificateIssuanceStates](../resources/intune-deviceconfig-certificateissuancestates.md)|Состояние выдачи. Возможные значения: `unknown` `challengeIssued` , , `challengeIssueFailed` `requestCreationFailed` `requestSubmitFailed` `challengeValidationSucceeded` `challengeValidationFailed` `issueFailed` `issuePending` `issued` `responseProcessingFailed` `responsePending` , `enrollmentSucceeded` `enrollmentNotNeeded` `revoked` `removedFromCollection` `renewVerified` `installFailed` `installed` `deleteFailed` `deleted` `renewalRequested` `requested` .|
|certificateKeyStorageProvider|[keyStorageProviderOption](../resources/intune-shared-keystorageprovideroption.md)|Ключевой служба хранилища поставщик. Возможные значения: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.|
|certificateSubjectNameFormat|[subjectNameFormat](../resources/intune-deviceconfig-subjectnameformat.md)|Формат имен субъекта. Возможные значения: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.|
|certificateSubjectAlternativeNameFormat|[subjectAlternativeNameType](../resources/intune-shared-subjectalternativenametype.md)|Тема альтернативного формата имен. Возможные значения: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`, `universalResourceIdentifier`.|
|certificateRevokeStatus|[certificateRevocationStatus](../resources/intune-deviceconfig-certificaterevocationstatus.md)|Отзови статус. Возможные значения: `none`, `pending`, `issued`, `failed`, `revoked`.|
|certificateProfileDisplayName|String|Имя отображения профиля сертификата|
|deviceDisplayName|String|Имя отображения устройства|
|userDisplayName|String|Отображаемое имя пользователя|
|certificateExpirationDateTime|DateTimeOffset|Дата истечения срока действия сертификата|
|certificateLastIssuanceStateChangedDateTime|DateTimeOffset|Изменение состояния последнего сертификата|
|lastCertificateStateChangeDateTime|DateTimeOffset|Изменение состояния последнего сертификата|
|certificateIssuer|String|Издатель|
|certificateThumbprint|String|Thumbprint|
|certificateSerialNumber|String|Серийный номер|
|certificateKeyLength|Int32|Длина ключа|
|certificateEnhancedKeyUsage|String|Расширенное использование ключа|
|certificateValidityPeriod|Int32|Срок действия|
|certificateSubjectNameFormatString|String|Строка формата subject name для пользовательских форматов имен субъекта|
|certificateSubjectAlternativeNameFormatString|String|Строка альтернативного формата имен для настраиваемого формата|
|certificateIssuanceDateTime|DateTimeOffset|Дата выпуска|
|certificateErrorCode|Int32|Код ошибки|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedDeviceCertificateState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDeviceCertificateState",
  "id": "String (identifier)",
  "devicePlatform": "String",
  "certificateKeyUsage": "String",
  "certificateValidityPeriodUnits": "String",
  "certificateIssuanceState": "String",
  "certificateKeyStorageProvider": "String",
  "certificateSubjectNameFormat": "String",
  "certificateSubjectAlternativeNameFormat": "String",
  "certificateRevokeStatus": "String",
  "certificateProfileDisplayName": "String",
  "deviceDisplayName": "String",
  "userDisplayName": "String",
  "certificateExpirationDateTime": "String (timestamp)",
  "certificateLastIssuanceStateChangedDateTime": "String (timestamp)",
  "lastCertificateStateChangeDateTime": "String (timestamp)",
  "certificateIssuer": "String",
  "certificateThumbprint": "String",
  "certificateSerialNumber": "String",
  "certificateKeyLength": 1024,
  "certificateEnhancedKeyUsage": "String",
  "certificateValidityPeriod": 1024,
  "certificateSubjectNameFormatString": "String",
  "certificateSubjectAlternativeNameFormatString": "String",
  "certificateIssuanceDateTime": "String (timestamp)",
  "certificateErrorCode": 1024
}
```




---
title: Тип ресурса managedDeviceCertificateState
description: Н/Д
ms.openlocfilehash: 17128f812eca82f01d6d2fa632f11c6640d18fc6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27081488"
---
# <a name="manageddevicecertificatestate-resource-type"></a>Тип ресурса managedDeviceCertificateState

> **Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Н/Д
## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список managedDeviceCertificateStates](../api/intune-deviceconfig-manageddevicecertificatestate-list.md)|[managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md) коллекции|Свойства списка и связей объектов [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md) .|
|[Получение managedDeviceCertificateState](../api/intune-deviceconfig-manageddevicecertificatestate-get.md)|[managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md)|Чтение свойства и связи объекта [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md) .|
|[Создание managedDeviceCertificateState](../api/intune-deviceconfig-manageddevicecertificatestate-create.md)|[managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md)|Создание нового объекта [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md) .|
|[Удаление managedDeviceCertificateState](../api/intune-deviceconfig-manageddevicecertificatestate-delete.md)|Нет|Удаляет [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md).|
|[Обновление managedDeviceCertificateState](../api/intune-deviceconfig-manageddevicecertificatestate-update.md)|[managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md)|Обновление свойства объекта [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта.|
|devicePlatform|[devicePlatformType](../resources/intune-shared-deviceplatformtype.md)|Платформа устройства. Возможные значения: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`.|
|certificateKeyUsage|[keyUsages](../resources/intune-deviceconfig-keyusages.md)|Использование ключей. Возможные значения: `keyEncipherment`, `digitalSignature`.|
|certificateValidityPeriodUnits|[certificateValidityPeriodScale](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|Действия подразделений. Возможные значения: `days`, `months`, `years`.|
|certificateIssuanceState|[certificateIssuanceStates](../resources/intune-deviceconfig-certificateissuancestates.md)|Состояние выдачи. Возможные значения: `unknown`, `challengeIssued`, `challengeIssueFailed`, `requestCreationFailed`, `requestSubmitFailed`, `challengeValidationSucceeded`, `challengeValidationFailed`, `issueFailed`, `issuePending`, `issued`, `responseProcessingFailed`, `responsePending`, `enrollmentSucceeded`, `enrollmentNotNeeded`, `revoked`, `removedFromCollection`, `renewVerified`, `installFailed`, `installed` , `deleteFailed`, `deleted`, `renewalRequested`, `requested`.|
|certificateKeyStorageProvider|[keyStorageProviderOption](../resources/intune-deviceconfig-keystorageprovideroption.md)|Поставщика хранилища ключей. Возможные значения: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.|
|certificateSubjectNameFormat|[subjectNameFormat](../resources/intune-deviceconfig-subjectnameformat.md)|Формат имени субъекта. Возможные значения: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.|
|certificateSubjectAlternativeNameFormat|[subjectAlternativeNameType](../resources/intune-deviceconfig-subjectalternativenametype.md)|Формат альтернативное имя субъекта. Возможные значения: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.|
|certificateRevokeStatus|[certificateRevocationStatus](../resources/intune-deviceconfig-certificaterevocationstatus.md)|Отмените состояние. Возможные значения: `none`, `pending`, `issued`, `failed`, `revoked`.|
|certificateProfileDisplayName|String|Отображаемое имя сертификата профилей|
|deviceDisplayName|String|Отображаемое имя устройства|
|userDisplayName|String|Отображаемое имя пользователя|
|certificateExpirationDateTime|DateTimeOffset|Дата окончания срока действия сертификата|
|certificateLastIssuanceStateChangedDateTime|DateTimeOffset|Последнее изменение состояния выдачи сертификатов|
|lastCertificateStateChangeDateTime|DateTimeOffset|Последнее изменение состояния выдачи сертификатов|
|certificateIssuer|String|Издателя|
|certificateThumbprint|String|Отпечаток|
|серийный номер сертификата|String|Серийный номер|
|certificateKeyLength|Int32|Длина ключа|
|certificateEnhancedKeyUsage|String|Расширенного использования ключа|
|certificateValidityPeriod|Int32|Срок действия|
|certificateSubjectNameFormatString|String|Строку формата имени субъекта для форматов имя настраиваемой темы|
|certificateSubjectAlternativeNameFormatString|String|Строку формата альтернативное имя субъекта для настраиваемых форматов|
|certificateIssuanceDateTime|DateTimeOffset|Дата выдачи|
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






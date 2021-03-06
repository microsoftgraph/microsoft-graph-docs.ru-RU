---
title: Тип ресурса Манажеддевицецертификатестате
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b3a6b37d0fa01f5cb1105e9f8df8ef15221f814d
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49302868"
---
# <a name="manageddevicecertificatestate-resource-type"></a>Тип ресурса Манажеддевицецертификатестате

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Н/Д

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Manageddevicecertificatestates к объекту](../api/intune-deviceconfig-manageddevicecertificatestate-list.md)|Коллекция [манажеддевицецертификатестате](../resources/intune-deviceconfig-manageddevicecertificatestate.md)|Список свойств и связей объектов [манажеддевицецертификатестате](../resources/intune-deviceconfig-manageddevicecertificatestate.md) .|
|[Получение Манажеддевицецертификатестате](../api/intune-deviceconfig-manageddevicecertificatestate-get.md)|[managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md)|Чтение свойств и связей объекта [манажеддевицецертификатестате](../resources/intune-deviceconfig-manageddevicecertificatestate.md) .|
|[Создание Манажеддевицецертификатестате](../api/intune-deviceconfig-manageddevicecertificatestate-create.md)|[managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md)|Создание нового объекта [манажеддевицецертификатестате](../resources/intune-deviceconfig-manageddevicecertificatestate.md) .|
|[Удаление Манажеддевицецертификатестате](../api/intune-deviceconfig-manageddevicecertificatestate-delete.md)|Нет|Удаляет объект [манажеддевицецертификатестате](../resources/intune-deviceconfig-manageddevicecertificatestate.md).|
|[Обновление Манажеддевицецертификатестате](../api/intune-deviceconfig-manageddevicecertificatestate-update.md)|[managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md)|Обновление свойств объекта [манажеддевицецертификатестате](../resources/intune-deviceconfig-manageddevicecertificatestate.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта.|
|devicePlatform|[девицеплатформтипе](../resources/intune-shared-deviceplatformtype.md)|Платформа устройства. Возможные значения: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.|
|цертификатекэйусаже|[кэйусажес](../resources/intune-shared-keyusages.md)|Использование ключа. Возможные значения: `keyEncipherment`, `digitalSignature`.|
|цертификатевалидитипериодунитс|[certificateValidityPeriodScale](../resources/intune-shared-certificatevalidityperiodscale.md)|Единицы срока действия. Возможные значения: `days`, `months`, `years`.|
|цертификатеиссуанцестате|[цертификатеиссуанцестатес](../resources/intune-deviceconfig-certificateissuancestates.md)|Состояние выдачи. Возможные значения:,,,,,,,,,,, `unknown` `challengeIssued` `challengeIssueFailed` `requestCreationFailed` `requestSubmitFailed` `challengeValidationSucceeded` `challengeValidationFailed` `issueFailed` `issuePending` `issued` `responseProcessingFailed` `responsePending` `enrollmentSucceeded` , `enrollmentNotNeeded` , `revoked` , `removedFromCollection` `renewVerified` `installFailed` `installed` `deleteFailed` `deleted` `renewalRequested` `requested` ,,,,,,,,,,,,,,.|
|цертификатекэйсторажепровидер|[кэйсторажепровидероптион](../resources/intune-shared-keystorageprovideroption.md)|Поставщик хранилища ключей. Возможные значения: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.|
|цертификатесубжектнамеформат|[subjectNameFormat](../resources/intune-deviceconfig-subjectnameformat.md)|Формат имени субъекта. Возможные значения: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.|
|цертификатесубжекталтернативенамеформат|[subjectAlternativeNameType](../resources/intune-shared-subjectalternativenametype.md)|Формат альтернативного имени субъекта. Возможные значения: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`, `universalResourceIdentifier`.|
|цертификатеревокестатус|[цертификатеревокатионстатус](../resources/intune-deviceconfig-certificaterevocationstatus.md)|Отзыв состояния. Возможные значения: `none`, `pending`, `issued`, `failed`, `revoked`.|
|цертификатепрофиледисплайнаме|String|Отображаемое имя профиля сертификата|
|deviceDisplayName|String|Отображаемое имя устройства|
|userDisplayName|String|Отображаемое имя пользователя|
|цертификатикспиратиондатетиме|DateTimeOffset|Дата окончания срока действия сертификата|
|цертификателастиссуанцестатечанжеддатетиме|DateTimeOffset|Последнее изменение состояния выдачи сертификата|
|ластцертификатестатечанжедатетиме|DateTimeOffset|Последнее изменение состояния выдачи сертификата|
|цертификатеиссуер|String|Издатель|
|certificateThumbprint|String|Thumbprint|
|цертификатесериалнумбер|String|Серийный номер|
|цертификатекэйленгс|Int32|Длина ключа|
|цертификатинханцедкэйусаже|String|Расширенное использование ключа|
|цертификатевалидитипериод|Int32|Срок действия|
|цертификатесубжектнамеформатстринг|String|Строка формата имени субъекта для пользовательских форматов имен субъектов|
|цертификатесубжекталтернативенамеформатстринг|String|Строка формата альтернативного имени субъекта для пользовательских форматов|
|цертификатеиссуанцедатетиме|DateTimeOffset|Дата выпуска|
|цертификатирроркоде|Int32|Код ошибки|

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





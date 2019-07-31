---
title: Тип ресурса Манажеддевицецертификатестате
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: abfb70d50e7c023ac672613d8e3f9be4ffc1fe53
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35970117"
---
# <a name="manageddevicecertificatestate-resource-type"></a>Тип ресурса Манажеддевицецертификатестате

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

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
|id|Строка|Ключ объекта.|
|devicePlatform|[Девицеплатформтипе](../resources/intune-shared-deviceplatformtype.md)|Платформа устройства. Возможные значения: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.|
|Цертификатекэйусаже|[Кэйусажес](../resources/intune-deviceconfig-keyusages.md)|Использование ключа. Возможные значения: `keyEncipherment`, `digitalSignature`.|
|Цертификатевалидитипериодунитс|[certificateValidityPeriodScale](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|Единицы срока действия. Возможные значения: `days`, `months`, `years`.|
|Цертификатеиссуанцестате|[Цертификатеиссуанцестатес](../resources/intune-deviceconfig-certificateissuancestates.md)|Состояние выдачи. Возможные значения: `unknown`, `challengeIssued`, `challengeIssueFailed`, `requestCreationFailed` `requestSubmitFailed` `challengeValidationSucceeded` `challengeValidationFailed` `enrollmentNotNeeded` `revoked` `removedFromCollection` `renewVerified` `installFailed` `installed` `responsePending` `enrollmentSucceeded`,,,,,,,,,,,,,,,,,,,,, `issueFailed` `issuePending` `issued` `responseProcessingFailed` , `deleteFailed`, `deleted`, `renewalRequested`, `requested`.|
|Цертификатекэйсторажепровидер|[Кэйсторажепровидероптион](../resources/intune-deviceconfig-keystorageprovideroption.md)|Поставщик хранилища ключей. Возможные значения: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.|
|Цертификатесубжектнамеформат|[subjectNameFormat](../resources/intune-deviceconfig-subjectnameformat.md)|Формат имени субъекта. Возможные значения: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.|
|Цертификатесубжекталтернативенамеформат|[subjectAlternativeNameType](../resources/intune-deviceconfig-subjectalternativenametype.md)|Формат альтернативного имени субъекта. Возможные значения: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.|
|Цертификатеревокестатус|[Цертификатеревокатионстатус](../resources/intune-deviceconfig-certificaterevocationstatus.md)|Отзыв состояния. Возможные значения: `none`, `pending`, `issued`, `failed`, `revoked`.|
|Цертификатепрофиледисплайнаме|String|Отображаемое имя профиля сертификата|
|deviceDisplayName|String|Отображаемое имя устройства|
|userDisplayName|String|Отображаемое имя пользователя|
|Цертификатикспиратиондатетиме|DateTimeOffset|Дата окончания срока действия сертификата|
|Цертификателастиссуанцестатечанжеддатетиме|DateTimeOffset|Последнее изменение состояния выдачи сертификата|
|Ластцертификатестатечанжедатетиме|DateTimeOffset|Последнее изменение состояния выдачи сертификата|
|Цертификатеиссуер|String|Издатель|
|certificateThumbprint|String|Отпечаток|
|Цертификатесериалнумбер|String|Серийный номер|
|Цертификатекэйленгс|Int32|Длина ключа|
|Цертификатинханцедкэйусаже|String|Расширенное использование ключа|
|Цертификатевалидитипериод|Int32|Срок действия|
|Цертификатесубжектнамеформатстринг|String|Строка формата имени субъекта для пользовательских форматов имен субъектов|
|Цертификатесубжекталтернативенамеформатстринг|String|Строка формата альтернативного имени субъекта для пользовательских форматов|
|Цертификатеиссуанцедатетиме|DateTimeOffset|Дата выпуска|
|Цертификатирроркоде|Int32|Код ошибки|

## <a name="relationships"></a>Отношения
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






---
title: Тип ресурса enrollmentTroubleshootingEvent
description: Событие, представляющее сбой при регистрации.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4fa7a6d00ece79ad6a405a9b31c9db15f89531cb
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33939760"
---
# <a name="enrollmenttroubleshootingevent-resource-type"></a>Тип ресурса enrollmentTroubleshootingEvent

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Событие, представляющее сбой при регистрации.


Наследуется от [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список объектов enrollmentTroubleshootingEvents](../api/intune-troubleshooting-enrollmenttroubleshootingevent-list.md)|Коллекция [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md)|Список свойств и связей объектов [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md).|
|[Получение объекта enrollmentTroubleshootingEvent](../api/intune-troubleshooting-enrollmenttroubleshootingevent-get.md)|[enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md);|Чтение свойств и связей объекта [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md).|
|[Создание объекта enrollmentTroubleshootingEvent](../api/intune-troubleshooting-enrollmenttroubleshootingevent-create.md)|[enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md);|Создание объекта [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md).|
|[Удаление объекта enrollmentTroubleshootingEvent](../api/intune-troubleshooting-enrollmenttroubleshootingevent-delete.md)|Нет|Удаляет объект [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md).|
|[Обновление объекта enrollmentTroubleshootingEvent](../api/intune-troubleshooting-enrollmenttroubleshootingevent-update.md)|[enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md)|Обновление свойств объекта [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md).|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|UUID объекта. Наследуется от объекта [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).|
|eventDateTime|DateTimeOffset|Время возникновения события. Наследуется от объекта [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).|
|correlationId|Строка|Идентификатор, используемый для трассировки сбоя в службе. Наследуется от объекта [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).|
|Траублешутинжеррордетаилс|[deviceManagementTroubleshootingErrorDetails](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|Объект, содержащий подробные сведения об ошибке и ее исправлении. Наследуется от объекта [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).|
|eventName|Строка|Имя события, соответствующее событию устранения неполадок. Это необязательное поле, унаследованное от [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)|
|Аддитионалинформатион|Коллекция [keyValuePair](../resources/intune-shared-keyvaluepair.md)|Набор пар строкового ключа и строкового значения, предоставляющий дополнительные сведения о событии устранения неполадок, наследуемом от [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)|
|managedDeviceIdentifier|Строка|Идентификатор события, созданный или полученный службой Intune.|
|operatingSystem|Строка|Операционная система.|
|osVersion|Строка|Версия ОС.|
|userId|String|Идентификатор пользователя, который пытался зарегистрировать устройство.|
|deviceId|Строка|Идентификатор устройства Azure AD.|
|enrollmentType|[deviceEnrollmentType](../resources/intune-shared-deviceenrollmenttype.md)|Тип регистрации. Возможные значения: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.|
|failureCategory|[Девицеенроллментфаилуререасон](../resources/intune-troubleshooting-deviceenrollmentfailurereason.md)|Категория сбоя высокого уровня. Возможные значения: `unknown`, `authentication`, `authorization`, `accountValidation`, `userValidation`, `deviceNotSupported`, `inMaintenance`, `badRequest`, `featureNotSupported`, `enrollmentRestrictionsEnforced`, `clientDisconnected`, `userAbandonment`.|
|failureReason|String|Подробная причина ошибки.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.enrollmentTroubleshootingEvent"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.enrollmentTroubleshootingEvent",
  "id": "String (identifier)",
  "eventDateTime": "String (timestamp)",
  "correlationId": "String",
  "troubleshootingErrorDetails": {
    "@odata.type": "microsoft.graph.deviceManagementTroubleshootingErrorDetails",
    "context": "String",
    "failure": "String",
    "failureDetails": "String",
    "remediation": "String",
    "resources": [
      {
        "@odata.type": "microsoft.graph.deviceManagementTroubleshootingErrorResource",
        "text": "String",
        "link": "String"
      }
    ]
  },
  "eventName": "String",
  "additionalInformation": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "String",
      "value": "String"
    }
  ],
  "managedDeviceIdentifier": "String",
  "operatingSystem": "String",
  "osVersion": "String",
  "userId": "String",
  "deviceId": "String",
  "enrollmentType": "String",
  "failureCategory": "String",
  "failureReason": "String"
}
```





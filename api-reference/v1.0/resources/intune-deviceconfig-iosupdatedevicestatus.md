---
title: Тип ресурса iosUpdateDeviceStatus
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 2b7abb81a09fc4652574b088b18a5cfa973079b2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48062794"
---
# <a name="iosupdatedevicestatus-resource-type"></a>Тип ресурса iosUpdateDeviceStatus

Пространство имен: microsoft.graph

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Н/Д

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список объектов iosUpdateDeviceStatus](../api/intune-deviceconfig-iosupdatedevicestatus-list.md)|Коллекция [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md)|Список свойств и связей объектов [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md).|
|[Получение объекта iosUpdateDeviceStatus](../api/intune-deviceconfig-iosupdatedevicestatus-get.md)|[iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md)|Чтение свойств и связей объекта [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md).|
|[Создание объекта iosUpdateDeviceStatus](../api/intune-deviceconfig-iosupdatedevicestatus-create.md)|[iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md)|Создание объекта [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md).|
|[Удаление объекта iosUpdateDeviceStatus](../api/intune-deviceconfig-iosupdatedevicestatus-delete.md)|Нет|Удаляет объект [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md).|
|[Обновление объекта iosUpdateDeviceStatus](../api/intune-deviceconfig-iosupdatedevicestatus-update.md)|[iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md)|Обновление свойств объекта [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md).|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта.|
|installStatus|[иосупдатесинсталлстатус](../resources/intune-deviceconfig-iosupdatesinstallstatus.md)|Состояние установки отчета о политике. Возможные значения: `success` , `available` ,,,,, `idle` `unknown` `downloading` `downloadFailed` `downloadRequiresComputer` ,,, `downloadInsufficientSpace` `downloadInsufficientPower` `downloadInsufficientNetwork` ,,, `installing` `installInsufficientSpace` `installInsufficientPower` , `installPhoneCallInProgress` , `installFailed` , `notSupportedOperation` , `sharedDeviceUserLoggedInError` .|
|osVersion|String|Версия устройства в отчете.|
|deviceId|String|ИД устройства в отчете.|
|userId|String|ИД пользователя в отчете.|
|deviceDisplayName|String|Имя устройства в объекте DevicePolicyStatus.|
|userName|String|Имя пользователя в отчете|
|deviceModel|String|Модель устройства в отчете|
|complianceGracePeriodExpirationDateTime|DateTimeOffset|Дата и время, когда истекает период отсрочки применения политик на устройстве.|
|status|[комплианцестатус](../resources/intune-shared-compliancestatus.md)|Состояние соответствия требованиям для отчета о политике. Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.|
|lastReportedDateTime|DateTimeOffset|Дата и время последнего изменения отчета о политике.|
|userPrincipalName|String|Имя участника-пользователя.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iosUpdateDeviceStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosUpdateDeviceStatus",
  "id": "String (identifier)",
  "installStatus": "String",
  "osVersion": "String",
  "deviceId": "String",
  "userId": "String",
  "deviceDisplayName": "String",
  "userName": "String",
  "deviceModel": "String",
  "complianceGracePeriodExpirationDateTime": "String (timestamp)",
  "status": "String",
  "lastReportedDateTime": "String (timestamp)",
  "userPrincipalName": "String"
}
```










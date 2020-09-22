---
title: Тип ресурса Макосвппаппревокелиценсесактионресулт
description: Определяет результаты для действий в приложениях MacOS VPP, содержит унаследованные свойства для Актионресулт.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: acaa10168696dc81e012fb9f18f01efd6262bd7f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48019623"
---
# <a name="macosvppapprevokelicensesactionresult-resource-type"></a>Тип ресурса Макосвппаппревокелиценсесактионресулт

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Определяет результаты для действий в приложениях MacOS VPP, содержит унаследованные свойства для Актионресулт.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|userId|String|UserId, связанный с действием.|
|манажеддевицеид|String|DeviceId, связанный с действием.|
|тоталлиценсескаунт|Int32|Количество лицензий, для которых была предпринята попытка отзыва.|
|фаиледлиценсескаунт|Int32|Количество лицензий, для которых произошел сбой при отзыве.|
|актионфаилуререасон|[впптокенактионфаилуререасон](../resources/intune-shared-vpptokenactionfailurereason.md)|Причина сбоя действия "отзыв лицензий". Возможные значения: `none`, `appleFailure`, `internalError`, `expiredVppToken`, `expiredApplePushNotificationCertificate`.|
|actionName|String|Название действия|
|actionState|[actionState](../resources/intune-shared-actionstate.md)|Состояние действия. Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.|
|startDateTime|DateTimeOffset|Время начала действия|
|lastUpdatedDateTime|DateTimeOffset|Время последнего обновления состояния действия|

## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.macOsVppAppRevokeLicensesActionResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOsVppAppRevokeLicensesActionResult",
  "userId": "String",
  "managedDeviceId": "String",
  "totalLicensesCount": 1024,
  "failedLicensesCount": 1024,
  "actionFailureReason": "String",
  "actionName": "String",
  "actionState": "String",
  "startDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)"
}
```







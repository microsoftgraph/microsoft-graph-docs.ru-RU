---
title: Тип ресурса Макосвппаппревокелиценсесактионресулт
description: Определяет результаты для действий в приложениях MacOS VPP, содержит унаследованные свойства для Актионресулт.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ad7ad1a2cdf8eabd67c1578c387b424f3e6f6c85
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33950223"
---
# <a name="macosvppapprevokelicensesactionresult-resource-type"></a>Тип ресурса Макосвппаппревокелиценсесактионресулт

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Определяет результаты для действий в приложениях MacOS VPP, содержит унаследованные свойства для Актионресулт.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|userId|String|UserId, связанный с действием.|
|Манажеддевицеид|Строка|DeviceId, связанный с действием.|
|Тоталлиценсескаунт|Int32|Количество лицензий, для которых была предпринята попытка отзыва.|
|Фаиледлиценсескаунт|Int32|Количество лицензий, для которых произошел сбой при отзыве.|
|Актионфаилуререасон|[Впптокенактионфаилуререасон](../resources/intune-shared-vpptokenactionfailurereason.md)|Причина сбоя действия "отзыв лицензий". Возможные значения: `none`, `appleFailure`, `internalError`, `expiredVppToken`, `expiredApplePushNotificationCertificate`.|
|actionName|String|Название действия|
|actionState|[actionState](../resources/intune-shared-actionstate.md)|Состояние действия. Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.|
|startDateTime|DateTimeOffset|Время начала действия|
|lastUpdatedDateTime|DateTimeOffset|Время последнего обновления состояния действия|

## <a name="relationships"></a>Связи
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





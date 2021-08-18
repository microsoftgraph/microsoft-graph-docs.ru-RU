---
title: тип ресурса iosVppAppRevokeLicensesActionResult
description: Определяет результаты действий в приложениях Vpp для iOS, содержит унаследованные свойства для ActionResult.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 19deb0d6ce7f577c743dad7dbb724d83732a4b96cff54706b1aad1e1c7a4f855
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54253168"
---
# <a name="iosvppapprevokelicensesactionresult-resource-type"></a>тип ресурса iosVppAppRevokeLicensesActionResult

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Определяет результаты действий в приложениях Vpp для iOS, содержит унаследованные свойства для ActionResult.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|userId|String|UserId, связанный с действием.|
|managedDeviceId|Строка|DeviceId, связанный с действием.|
|totalLicensesCount|Int32|Количество лицензий, для которых была предпринята попытка отзыва.|
|failedLicensesCount|Int32|Количество лицензий, для которых отозвался сбой.|
|actionFailureReason|[vppTokenActionFailureReason](../resources/intune-shared-vpptokenactionfailurereason.md)|Причина отказа от отзыва лицензий. Возможные значения: `none`, `appleFailure`, `internalError`, `expiredVppToken`, `expiredApplePushNotificationCertificate`.|
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
  "@odata.type": "microsoft.graph.iosVppAppRevokeLicensesActionResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosVppAppRevokeLicensesActionResult",
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





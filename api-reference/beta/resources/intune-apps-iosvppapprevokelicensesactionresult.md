---
title: Тип ресурса iosVppAppRevokeLicensesActionResult
description: Определяет результаты для действий на iOS Vpp приложений, содержащий наследуемые свойства для ActionResult.
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: 13bc69a0c04eb7b9742f6c549fd1ae976cf25561
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27986994"
---
# <a name="iosvppapprevokelicensesactionresult-resource-type"></a>Тип ресурса iosVppAppRevokeLicensesActionResult

> **Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Определяет результаты для действий на iOS Vpp приложений, содержащий наследуемые свойства для ActionResult.
## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|userId|String|Идентификатор пользователя, связанные с действием.|
|managedDeviceId|String|DeviceId, связанные с действием.|
|totalLicensesCount|Int32|Подсчет числа лицензий, для которых осуществляется попытка revoke.|
|failedLicensesCount|Int32|Подсчет числа лицензий, для которых не удалось revoke.|
|actionFailureReason|[vppTokenActionFailureReason](../resources/intune-shared-vpptokenactionfailurereason.md)|Причина ошибки действие revoke лицензий. Возможные значения: `none`, `appleFailure`, `internalError`, `expiredVppToken`, `expiredApplePushNotificationCertificate`.|
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






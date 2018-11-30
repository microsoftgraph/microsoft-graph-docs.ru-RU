---
title: Тип ресурса officeClientCheckinStatus
description: Сущности, которая описывает клиента возврат stats.
ms.openlocfilehash: a87a085d42ce0754e046b319b270ddf90a3bdba7
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27077425"
---
# <a name="officeclientcheckinstatus-resource-type"></a>Тип ресурса officeClientCheckinStatus

> **Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Сущности, которая описывает клиента возврат stats.
## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|userPrincipalName|String|Имя участника-пользователя с помощью устройства.|
|deviceName|String|Имя устройства для возврата.|
|devicePlatform|String|Устройство платформы для возврата.|
|devicePlatformVersion|String|Для возврата версии платформы устройства.|
|wasSuccessful|Логический|Если последний checkin прошла успешно.|
|userId|String|Идентификатор пользователя, с помощью устройства.|
|checkinDateTime|DateTimeOffset|Последний устройства возврат времени в формате UTC.|
|сообщение об ошибке|String|Сообщение об ошибке, если какие-либо связанные для последнего checkin.|
|appliedPolicies|Коллекция String|Список политик доставки на устройство как последний checkin.|

## <a name="relationships"></a>Связи
Нет
## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.officeClientCheckinStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.officeClientCheckinStatus",
  "userPrincipalName": "String",
  "deviceName": "String",
  "devicePlatform": "String",
  "devicePlatformVersion": "String",
  "wasSuccessful": true,
  "userId": "String",
  "checkinDateTime": "String (timestamp)",
  "errorMessage": "String",
  "appliedPolicies": [
    "String"
  ]
}
```




---
title: Тип ресурса officeClientCheckinStatus
description: Сущности, которая описывает клиента возврат stats.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: a387e04b9ebc15d65eb8dd883ecd4a9bae78ad6d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27969291"
---
# <a name="officeclientcheckinstatus-resource-type"></a>Тип ресурса officeClientCheckinStatus

> **Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Сущности, которая описывает клиента возврат stats.
## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|userPrincipalName|Строка|Имя участника-пользователя с помощью устройства.|
|deviceName|String|Имя устройства для возврата.|
|devicePlatform|Строка|Устройство платформы для возврата.|
|devicePlatformVersion|Строка|Для возврата версии платформы устройства.|
|wasSuccessful|Логический|Если последний checkin прошла успешно.|
|userId|String|Идентификатор пользователя, с помощью устройства.|
|checkinDateTime|DateTimeOffset|Последний устройства возврат времени в формате UTC.|
|сообщение об ошибке|Строка|Сообщение об ошибке, если какие-либо связанные для последнего checkin.|
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




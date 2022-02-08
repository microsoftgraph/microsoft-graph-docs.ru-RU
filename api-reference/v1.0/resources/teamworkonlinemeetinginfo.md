---
title: тип ресурса teamworkOnlineMeetingInfo
description: Представляет сведения об онлайн-собрании в Microsoft Teams.
author: jecha
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: ac6dab85a12cdb339bb6527a6c1c436285c1ea75
ms.sourcegitcommit: 4c8444b732b8d6d0de8a95f6666c42095f146266
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/08/2022
ms.locfileid: "62443266"
---
# <a name="teamworkonlinemeetinginfo-resource-type"></a>тип ресурса teamworkOnlineMeetingInfo

Пространство имен: microsoft.graph

Представляет сведения об онлайн-собрании в Microsoft Teams.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|calendarEventId|Строка|Идентификатор события календаря, связанного с собранием.|
|joinWebUrl|String|URL-адрес, который пользователи щелкают, чтобы присоединиться к собранию или однозначно идентифицировать его.|
|organizer|[teamworkUserIdentity](teamworkuseridentity.md)|Организатор собрания.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamworkOnlineMeetingInfo"
}
-->
``` json
{
  "calendarEventId": "string",
  "joinWebUrl": "string",
  "organizer": {"@odata.type": "microsoft.graph.teamworkUserIdentity"}
}
```

## <a name="see-also"></a>См. также
- [Чат](chat.md)

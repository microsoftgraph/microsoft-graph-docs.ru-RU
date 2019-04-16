---
title: Тип ресурса Чатмессажементион
description: 'Представляет упоминание в объекте chatMessage. Упоминание может быть у пользователя, группы, ленты или канала. '
localization_priority: Normal
author: nkramer
ms.openlocfilehash: 5d7304325e48c87bfd75b57bf49585f66a77b262
ms.sourcegitcommit: a39db1154a07aa0dd7e96fb6f9d7e891a812207e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2019
ms.locfileid: "31889998"
---
# <a name="chatmessagemention-resource-type"></a>Тип ресурса Чатмессажементион

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет упоминание в объекте [chatMessage](chatmessage.md) . Упоминание может быть у пользователя, группы, ленты или канала. 

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|id|int|Индекс упоминаемого объекта. Соответствует <at id="index"> тегу основного текста сообщения.|
|Ментионтекст|string|Строка, используемая для представления упоминания. Например, отображаемое имя пользователя, имя группы.|
|котором|[identitySet](identityset.md)|Упоминаемая сущность (пользователь, приложение, группа или канал).|

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.chatMessageMention"
}-->

```json
{
  "id": "number",
  "mentionText": "string",
  "mentioned": "microsoft.graph.identitySet"
 }

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "chat mention resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/chatmessagemention.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

---
title: Тип ресурса chatMessageMention
description: 'Представляет упоминаются в сущности chatMessage. Упоминание может быть пользователь, группа, программа-робот или канала. '
localization_priority: Normal
ms.openlocfilehash: f37374a9793000ba641ed772e5dbfca5c0f1bd30
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515351"
---
# <a name="chatmessagemention-resource-type"></a>Тип ресурса chatMessageMention

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет упоминаются в сущности [chatMessage](chatmessage.md) . Упоминание может быть пользователь, группа, программа-робот или канала. 

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|id|string|Идентификатор сущности упоминаемые|
|mentionText|string|Строка, используемая для представления упоминание Ex: отображаемое имя пользователя, имя группы и т.д.|
|упомянутые|[identitySet](identityset.md)|Пользователь, который был упомянут|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.chatMessageMention"
}-->

```json
{
  "id": "string (identifier)",
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
    "Error: /api-reference/beta/resources/chatMention.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: CommentAction
localization_priority: Normal
ms.openlocfilehash: e674c996002b3a54c92886dd1c5dca7a76c56b51
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32543464"
---
# <a name="commentaction-resource-type"></a>Тип ресурса CommentAction

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

В ресурсе **CommentAction** содержатся сведения о [действии][] добавления комментария, выполненном над элементом.

[действии]: itemactivity.md

## <a name="json-representation"></a>Представление в формате JSON

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.commentAction"
}-->

```json
{
  "isReply": false,
  "parentAuthor": {"@odata.type": "microsoft.graph.identitySet"},
  "participants": [{"@odata.type": "microsoft.graph.identitySet"}]
}
```

## <a name="properties"></a>Свойства

| Имя свойства    | Тип                       | Описание
|:-----------------|:---------------------------|:-----------------------------
| isReply          | boolean                    | Если это свойство имеет значение true, то данное действие было ответом на существующий поток комментариев.
| parentAuthor     | [identitySet][]            | Удостоверение пользователя, начавшего ветвь комментариев.
| participants     | Коллекция [identitySet][] | Удостоверения пользователей, участвующих в ветви комментариев.

[identitySet]: identityset.md

## <a name="remarks"></a>Замечания

На данный момент записи о действиях над элементом доступны только в SharePoint и OneDrive для бизнеса.

<!--
{
  "type": "#page.annotation",
  "description": "The CommentAction object provides information about a comment that was made on an item.",
  "keywords": "activities,activity,action,comment",
  "section": "documentation",
  "tocPath": "Resources/CommentAction",
  "suppressions": [
    "Error: /api-reference/beta/resources/commentaction.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

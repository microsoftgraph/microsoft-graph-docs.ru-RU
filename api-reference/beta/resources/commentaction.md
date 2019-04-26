---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: CommentAction
localization_priority: Normal
ms.openlocfilehash: c472a0b1b992c91b60174859e4900ffcee04c007
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33341484"
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
  "suppressions": []
}
-->

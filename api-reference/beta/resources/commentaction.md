---
author: daspek
description: В ресурсе CommentAction содержатся сведения о действии добавления комментария, выполненном над элементом.
ms.date: 09/14/2017
title: CommentAction
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: files
ms.openlocfilehash: 984e9777c31fb1ce6b6b748b9ffb0cdfe9b6446a
ms.sourcegitcommit: a345f96fb22115f65840702a4acf0acc7c1b0679
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/08/2022
ms.locfileid: "65944174"
---
# <a name="commentaction-resource-type"></a>Тип ресурса CommentAction

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

В ресурсе **CommentAction** содержатся сведения о [действии][] добавления комментария, выполненном над элементом.

[действии]: itemactivity.md

## <a name="json-representation"></a>Представление в формате JSON

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type&quot;: &quot;microsoft.graph.commentAction"
}-->

```json
{
  "isReply": false,
  "parentAuthor": {"@odata.type": "microsoft.graph.identitySet"},
  "participants": [{"@odata.type": "microsoft.graph.identitySet"}]
}
```

## <a name="properties"></a>Свойства

| Свойство     | Тип                       | Описание                                                       |
| :----------- | :------------------------- | :---------------------------------------------------------------- |
| isReply      | boolean                    | Если это свойство имеет значение true, то данное действие было ответом на существующий поток комментариев. |
| parentAuthor | [identitySet][]            | Удостоверение пользователя, начавшего ветвь комментариев.          |
| participants | Коллекция [identitySet][] | Удостоверения пользователей, участвующих в ветви комментариев. |

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

---
author: daspek
title: Тип ресурса commentAction
description: Объект commentAction предоставляет сведения о комментарии к элементу.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: f2f3ab7f0798ee1020b107c38262a912fdae53ef
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/14/2021
ms.locfileid: "50238416"
---
# <a name="commentaction-resource-type"></a>Тип ресурса commentAction

Пространство имен: microsoft.graph

Ресурс **commentAction** предоставляет сведения о действии при [комментарии][] к элементу.

>**Примечание.** Записи о действиях с элементами в настоящее время доступны только в SharePoint и OneDrive для бизнеса.

[действии]: itemactivity.md

## <a name="properties"></a>Свойства

| Имя свойства    | Тип                       | Описание
|:-----------------|:---------------------------|:-----------------------------
| isReply          | boolean                    | Если это свойство имеет значение true, то данное действие было ответом на существующий поток комментариев.
| parentAuthor     | [identitySet][]            | Удостоверение пользователя, начавшего ветвь комментариев.
| participants     | Коллекция [identitySet][] | Удостоверения пользователей, участвующих в ветви комментариев.

[identitySet]: identityset.md

## <a name="json-representation"></a>Представление JSON

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
<!--
{
  "type": "#page.annotation",
  "description": "The commentAction object provides information about a comment that was made on an item.",
  "keywords": "activities,activity,action,comment",
  "section": "documentation",
  "tocPath": "Resources/commentAction",
  "suppressions": []
}
-->


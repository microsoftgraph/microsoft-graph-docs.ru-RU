---
author: daspek
title: тип ресурса commentAction
description: Объект commentAction предоставляет сведения о комментарии, который был сделан на элементе.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: bd146a400e83692754e1ca920dcba97339c1634f8fe81cc37374a6e37a30a872
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54135283"
---
# <a name="commentaction-resource-type"></a>тип ресурса commentAction

Пространство имен: microsoft.graph

Ресурс **commentAction** предоставляет сведения о действии [комментария, выполненного][] на элементе.

>**Примечание:** Записи действий элементов в настоящее время доступны только в SharePoint и OneDrive для бизнеса.

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
  "@type&quot;: &quot;microsoft.graph.commentAction"
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


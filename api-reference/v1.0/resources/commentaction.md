---
author: daspek
ms.author: dspektor
title: Тип ресурса commentAction
description: Объект commentAction предоставляет сведения о комментариях, сделанных для элемента.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 72502e466ff90ec0a299eb993346968c9038e2d1
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36029682"
---
# <a name="commentaction-resource-type"></a>Тип ресурса commentAction

Ресурс **commentAction** предоставляет сведения о действиях с [][] комментариями, выполняемых над элементом.

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

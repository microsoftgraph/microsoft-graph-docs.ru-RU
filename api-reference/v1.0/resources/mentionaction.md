---
author: daspek
ms.author: dspektor
title: Тип ресурса mentionAction
description: Объект MentionAction предоставляет сведения о пользователях, упомянутых во время действия.
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 8937a8f7acd55af93fdeac9eceb17d46e2cf495c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47991903"
---
# <a name="mentionaction-resource-type"></a>Тип ресурса mentionAction

Пространство имен: microsoft.graph

Ресурс **MentionAction** предоставляет сведения о ресурсе [activity][], в котором есть упоминания пользователей.

>**Примечание:** Записи действий элементов в настоящее время доступны только в SharePoint и OneDrive для бизнеса.

[действии]: itemactivity.md

## <a name="properties"></a>Свойства

| Имя свойства | Тип                       | Описание
|:--------------|:---------------------------|:-----------------------------
| mentionees    | Коллекция [identitySet][] | Удостоверения пользователей, упомянутых в этом действии.

[identitySet]: identityset.md

## <a name="json-representation"></a>Представление JSON

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.mentionAction"
}-->

```json
{
  "mentionees": [{"@odata.type": "microsoft.graph.identitySet"}]
}
```

<!--
{
  "type": "#page.annotation",
  "description": "The MentionAction object provides information about who was mentioned during an activity.",
  "keywords": "activities,activity,action,mention",
  "section": "documentation",
  "tocPath": "Resources/MentionAction",
  "suppressions": []
}
-->


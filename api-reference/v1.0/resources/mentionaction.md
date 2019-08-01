---
author: daspek
ms.author: dspektor
title: Тип ресурса mentionAction
description: Объект MentionAction предоставляет сведения о пользователях, упомянутых во время действия.
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 511519439f4079b2d7d618767855582f201c00f7
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36036185"
---
# <a name="mentionaction-resource-type"></a>Тип ресурса mentionAction

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

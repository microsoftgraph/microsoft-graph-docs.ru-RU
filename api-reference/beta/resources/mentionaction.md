---
author: daspek
description: Ресурс MentionAction предоставляет сведения о ресурсе activity, в котором есть упоминания пользователей.
ms.date: 09/14/2017
title: MentionAction
ms.localizationpriority: medium
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 4675a732738741dc5bb201f97753dca2be42a17d
ms.sourcegitcommit: e5d5095e26dca6f434354a0970e789e94ee6afb0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/22/2022
ms.locfileid: "63723488"
---
# <a name="mentionaction-resource-type"></a>Тип ресурса MentionAction

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Ресурс **MentionAction** предоставляет сведения о ресурсе [activity][], в котором есть упоминания пользователей.

[activity]: itemactivity.md

## <a name="json-representation"></a>Представление в формате JSON

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type&quot;: &quot;microsoft.graph.mentionAction"
}-->

```json
{
  "mentionees": [{"@odata.type": "microsoft.graph.identitySet"}]
}
```

## <a name="properties"></a>Свойства

| Свойство   | Тип                       | Описание                                           |
| :--------- | :------------------------- | :---------------------------------------------------- |
| mentionees | Коллекция [identitySet][] | Удостоверения пользователей, упомянутых в этом действии. |

[identitySet]: identityset.md

## <a name="remarks"></a>Замечания

На данный момент записи о действиях над элементом доступны только в SharePoint и OneDrive для бизнеса.

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

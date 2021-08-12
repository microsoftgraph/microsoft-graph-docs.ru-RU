---
author: daspek
title: тип ресурса mentionAction
description: Объект MentionAction предоставляет сведения о том, кто был упомянут во время действия.
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: bdcef79492604aa5ee2afae0897361eb41dd6889229b4b41259cc3d47f72bf92
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54152385"
---
# <a name="mentionaction-resource-type"></a>тип ресурса mentionAction

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
  "@type&quot;: &quot;microsoft.graph.mentionAction"
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


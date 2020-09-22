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
# <a name="mentionaction-resource-type"></a><span data-ttu-id="78db9-103">Тип ресурса mentionAction</span><span class="sxs-lookup"><span data-stu-id="78db9-103">mentionAction resource type</span></span>

<span data-ttu-id="78db9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="78db9-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="78db9-105">Ресурс **MentionAction** предоставляет сведения о ресурсе [activity][], в котором есть упоминания пользователей.</span><span class="sxs-lookup"><span data-stu-id="78db9-105">The **MentionAction** resource provides information about an [activity][] that mentioned people.</span></span>

><span data-ttu-id="78db9-106">**Примечание:** Записи действий элементов в настоящее время доступны только в SharePoint и OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="78db9-106">**Note:** Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

[действии]: itemactivity.md
[activity]: itemactivity.md

## <a name="properties"></a><span data-ttu-id="78db9-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="78db9-108">Properties</span></span>

| <span data-ttu-id="78db9-109">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="78db9-109">Property name</span></span> | <span data-ttu-id="78db9-110">Тип</span><span class="sxs-lookup"><span data-stu-id="78db9-110">Type</span></span>                       | <span data-ttu-id="78db9-111">Описание</span><span class="sxs-lookup"><span data-stu-id="78db9-111">Description</span></span>
|:--------------|:---------------------------|:-----------------------------
| <span data-ttu-id="78db9-112">mentionees</span><span class="sxs-lookup"><span data-stu-id="78db9-112">mentionees</span></span>    | <span data-ttu-id="78db9-113">Коллекция [identitySet][]</span><span class="sxs-lookup"><span data-stu-id="78db9-113">[identitySet][] collection</span></span> | <span data-ttu-id="78db9-114">Удостоверения пользователей, упомянутых в этом действии.</span><span class="sxs-lookup"><span data-stu-id="78db9-114">The identities of the users mentioned in this action.</span></span>

[identitySet]: identityset.md

## <a name="json-representation"></a><span data-ttu-id="78db9-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="78db9-116">JSON representation</span></span>

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


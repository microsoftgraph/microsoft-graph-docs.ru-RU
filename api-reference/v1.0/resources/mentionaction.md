---
author: daspek
ms.author: dspektor
title: Тип ресурса mentionAction
description: Объект MentionAction предоставляет сведения о пользователях, упомянутых во время действия.
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: d8c09de2a36be2cd83d5e33cf2ed948c25819fe4
ms.sourcegitcommit: 52baf24d1d08096214b12f60e7c755291fe03ab5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/13/2019
ms.locfileid: "33970818"
---
# <a name="mentionaction-resource-type"></a><span data-ttu-id="c365f-103">Тип ресурса mentionAction</span><span class="sxs-lookup"><span data-stu-id="c365f-103">mentionAction resource type</span></span>

<span data-ttu-id="c365f-104">Ресурс **MentionAction** предоставляет сведения о ресурсе [activity][], в котором есть упоминания пользователей.</span><span class="sxs-lookup"><span data-stu-id="c365f-104">The **MentionAction** resource provides information about an [activity][] that mentioned people.</span></span>

><span data-ttu-id="c365f-105">**Примечание:** Записи действий элементов в настоящее время доступны только в SharePoint и OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="c365f-105">**Note:** Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

[действии]: itemactivity.md
[activity]: itemactivity.md

## <a name="properties"></a><span data-ttu-id="c365f-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="c365f-107">Properties</span></span>

| <span data-ttu-id="c365f-108">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="c365f-108">Property name</span></span> | <span data-ttu-id="c365f-109">Тип</span><span class="sxs-lookup"><span data-stu-id="c365f-109">Type</span></span>                       | <span data-ttu-id="c365f-110">Описание</span><span class="sxs-lookup"><span data-stu-id="c365f-110">Description</span></span>
|:--------------|:---------------------------|:-----------------------------
| <span data-ttu-id="c365f-111">mentionees</span><span class="sxs-lookup"><span data-stu-id="c365f-111">mentionees</span></span>    | <span data-ttu-id="c365f-112">Коллекция [identitySet][]</span><span class="sxs-lookup"><span data-stu-id="c365f-112">[identitySet][] collection</span></span> | <span data-ttu-id="c365f-113">Удостоверения пользователей, упомянутых в этом действии.</span><span class="sxs-lookup"><span data-stu-id="c365f-113">The identities of the users mentioned in this action.</span></span>

[identitySet]: identityset.md

## <a name="json-representation"></a><span data-ttu-id="c365f-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c365f-115">JSON representation</span></span>

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

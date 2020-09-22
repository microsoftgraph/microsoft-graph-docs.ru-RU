---
author: daspek
description: Ресурс MentionAction предоставляет сведения о ресурсе activity, в котором есть упоминания пользователей.
ms.date: 09/14/2017
title: MentionAction
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: b0f8376c3fcc86cdd16c1eeb32507e5b26469285
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47971608"
---
# <a name="mentionaction-resource-type"></a><span data-ttu-id="c1b55-103">Тип ресурса MentionAction</span><span class="sxs-lookup"><span data-stu-id="c1b55-103">MentionAction resource type</span></span>

<span data-ttu-id="c1b55-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c1b55-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c1b55-105">Ресурс **MentionAction** предоставляет сведения о ресурсе [activity][], в котором есть упоминания пользователей.</span><span class="sxs-lookup"><span data-stu-id="c1b55-105">The **MentionAction** resource provides information about an [activity][] that mentioned people.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="c1b55-107">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="c1b55-107">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="c1b55-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="c1b55-108">Properties</span></span>

| <span data-ttu-id="c1b55-109">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="c1b55-109">Property name</span></span> | <span data-ttu-id="c1b55-110">Тип</span><span class="sxs-lookup"><span data-stu-id="c1b55-110">Type</span></span>                       | <span data-ttu-id="c1b55-111">Описание</span><span class="sxs-lookup"><span data-stu-id="c1b55-111">Description</span></span>
|:--------------|:---------------------------|:-----------------------------
| <span data-ttu-id="c1b55-112">mentionees</span><span class="sxs-lookup"><span data-stu-id="c1b55-112">mentionees</span></span>    | <span data-ttu-id="c1b55-113">Коллекция [identitySet][]</span><span class="sxs-lookup"><span data-stu-id="c1b55-113">[identitySet][] collection</span></span> | <span data-ttu-id="c1b55-114">Удостоверения пользователей, упомянутых в этом действии.</span><span class="sxs-lookup"><span data-stu-id="c1b55-114">The identities of the users mentioned in this action.</span></span>

[identitySet]: identityset.md

## <a name="remarks"></a><span data-ttu-id="c1b55-116">Замечания</span><span class="sxs-lookup"><span data-stu-id="c1b55-116">Remarks</span></span>

<span data-ttu-id="c1b55-117">На данный момент записи о действиях над элементом доступны только в SharePoint и OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="c1b55-117">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

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



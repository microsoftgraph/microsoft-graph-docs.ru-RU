---
author: daspek
description: Ресурс MentionAction предоставляет сведения о ресурсе activity, в котором есть упоминания пользователей.
ms.date: 09/14/2017
title: MentionAction
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 2e2a430ed25dd6a64049fc6dc49c282bf6a47e00
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522696"
---
# <a name="mentionaction-resource-type"></a><span data-ttu-id="e12ab-103">Тип ресурса MentionAction</span><span class="sxs-lookup"><span data-stu-id="e12ab-103">MentionAction resource type</span></span>

<span data-ttu-id="e12ab-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e12ab-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e12ab-105">Ресурс **MentionAction** предоставляет сведения о ресурсе [activity][], в котором есть упоминания пользователей.</span><span class="sxs-lookup"><span data-stu-id="e12ab-105">The **MentionAction** resource provides information about an [activity][] that mentioned people.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="e12ab-107">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="e12ab-107">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="e12ab-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="e12ab-108">Properties</span></span>

| <span data-ttu-id="e12ab-109">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="e12ab-109">Property name</span></span> | <span data-ttu-id="e12ab-110">Тип</span><span class="sxs-lookup"><span data-stu-id="e12ab-110">Type</span></span>                       | <span data-ttu-id="e12ab-111">Описание</span><span class="sxs-lookup"><span data-stu-id="e12ab-111">Description</span></span>
|:--------------|:---------------------------|:-----------------------------
| <span data-ttu-id="e12ab-112">mentionees</span><span class="sxs-lookup"><span data-stu-id="e12ab-112">mentionees</span></span>    | <span data-ttu-id="e12ab-113">Коллекция [identitySet][]</span><span class="sxs-lookup"><span data-stu-id="e12ab-113">[identitySet][] collection</span></span> | <span data-ttu-id="e12ab-114">Удостоверения пользователей, упомянутых в этом действии.</span><span class="sxs-lookup"><span data-stu-id="e12ab-114">The identities of the users mentioned in this action.</span></span>

[identitySet]: identityset.md

## <a name="remarks"></a><span data-ttu-id="e12ab-116">Замечания</span><span class="sxs-lookup"><span data-stu-id="e12ab-116">Remarks</span></span>

<span data-ttu-id="e12ab-117">На данный момент записи о действиях над элементом доступны только в SharePoint и OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="e12ab-117">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

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

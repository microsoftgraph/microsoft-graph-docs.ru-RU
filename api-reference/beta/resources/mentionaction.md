---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: MentionAction
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: ad75f3a796f29f7f9c4497a3a15fd31dec0f1c6f
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33342270"
---
# <a name="mentionaction-resource-type"></a><span data-ttu-id="9d1d2-102">Тип ресурса MentionAction</span><span class="sxs-lookup"><span data-stu-id="9d1d2-102">MentionAction resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9d1d2-103">Ресурс **MentionAction** предоставляет сведения о ресурсе [activity][], в котором есть упоминания пользователей.</span><span class="sxs-lookup"><span data-stu-id="9d1d2-103">The **MentionAction** resource provides information about an [activity][] that mentioned people.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="9d1d2-105">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="9d1d2-105">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="9d1d2-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="9d1d2-106">Properties</span></span>

| <span data-ttu-id="9d1d2-107">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="9d1d2-107">Property name</span></span> | <span data-ttu-id="9d1d2-108">Тип</span><span class="sxs-lookup"><span data-stu-id="9d1d2-108">Type</span></span>                       | <span data-ttu-id="9d1d2-109">Описание</span><span class="sxs-lookup"><span data-stu-id="9d1d2-109">Description</span></span>
|:--------------|:---------------------------|:-----------------------------
| <span data-ttu-id="9d1d2-110">mentionees</span><span class="sxs-lookup"><span data-stu-id="9d1d2-110">mentionees</span></span>    | <span data-ttu-id="9d1d2-111">Коллекция [identitySet][]</span><span class="sxs-lookup"><span data-stu-id="9d1d2-111">[identitySet][] collection</span></span> | <span data-ttu-id="9d1d2-112">Удостоверения пользователей, упомянутых в этом действии.</span><span class="sxs-lookup"><span data-stu-id="9d1d2-112">The identities of the users mentioned in this action.</span></span>

[identitySet]: identityset.md

## <a name="remarks"></a><span data-ttu-id="9d1d2-114">Замечания</span><span class="sxs-lookup"><span data-stu-id="9d1d2-114">Remarks</span></span>

<span data-ttu-id="9d1d2-115">На данный момент записи о действиях над элементом доступны только в SharePoint и OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="9d1d2-115">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

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

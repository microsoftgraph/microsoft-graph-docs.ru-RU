---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: MentionAction
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 9101ffed094fd78189b73eab511be88c8bf449de
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513013"
---
# <a name="mentionaction-resource-type"></a><span data-ttu-id="1e3d8-102">Тип ресурса MentionAction</span><span class="sxs-lookup"><span data-stu-id="1e3d8-102">MentionAction resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1e3d8-103">Ресурс **MentionAction** предоставляет сведения о ресурсе [activity][], в котором есть упоминания пользователей.</span><span class="sxs-lookup"><span data-stu-id="1e3d8-103">The **MentionAction** resource provides information about an [activity][] that mentioned people.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="1e3d8-105">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="1e3d8-105">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="1e3d8-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="1e3d8-106">Properties</span></span>

| <span data-ttu-id="1e3d8-107">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="1e3d8-107">Property name</span></span> | <span data-ttu-id="1e3d8-108">Тип</span><span class="sxs-lookup"><span data-stu-id="1e3d8-108">Type</span></span>                       | <span data-ttu-id="1e3d8-109">Описание</span><span class="sxs-lookup"><span data-stu-id="1e3d8-109">Description</span></span>
|:--------------|:---------------------------|:-----------------------------
| <span data-ttu-id="1e3d8-110">mentionees</span><span class="sxs-lookup"><span data-stu-id="1e3d8-110">mentionees</span></span>    | <span data-ttu-id="1e3d8-111">Коллекция [identitySet][]</span><span class="sxs-lookup"><span data-stu-id="1e3d8-111">[identitySet][] collection</span></span> | <span data-ttu-id="1e3d8-112">Удостоверения пользователей, упомянутых в этом действии.</span><span class="sxs-lookup"><span data-stu-id="1e3d8-112">The identities of the users mentioned in this action.</span></span>

[identitySet]: identityset.md

## <a name="remarks"></a><span data-ttu-id="1e3d8-114">Замечания</span><span class="sxs-lookup"><span data-stu-id="1e3d8-114">Remarks</span></span>

<span data-ttu-id="1e3d8-115">На данный момент записи о действиях над элементом доступны только в SharePoint и OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="1e3d8-115">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "The MentionAction object provides information about who was mentioned during an activity.",
  "keywords": "activities,activity,action,mention",
  "section": "documentation",
  "tocPath": "Resources/MentionAction",
  "suppressions": [
    "Error: /api-reference/beta/resources/mentionaction.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

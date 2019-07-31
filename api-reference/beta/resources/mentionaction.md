---
author: daspek
description: Ресурс MentionAction предоставляет сведения о ресурсе activity, в котором есть упоминания пользователей.
ms.date: 09/14/2017
title: MentionAction
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 1b08233569fe655b5a8f0e878c4e14d178be279f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966820"
---
# <a name="mentionaction-resource-type"></a><span data-ttu-id="f5faa-103">Тип ресурса MentionAction</span><span class="sxs-lookup"><span data-stu-id="f5faa-103">MentionAction resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f5faa-104">Ресурс **MentionAction** предоставляет сведения о ресурсе [activity][], в котором есть упоминания пользователей.</span><span class="sxs-lookup"><span data-stu-id="f5faa-104">The **MentionAction** resource provides information about an [activity][] that mentioned people.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="f5faa-106">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="f5faa-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="f5faa-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="f5faa-107">Properties</span></span>

| <span data-ttu-id="f5faa-108">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="f5faa-108">Property name</span></span> | <span data-ttu-id="f5faa-109">Тип</span><span class="sxs-lookup"><span data-stu-id="f5faa-109">Type</span></span>                       | <span data-ttu-id="f5faa-110">Описание</span><span class="sxs-lookup"><span data-stu-id="f5faa-110">Description</span></span>
|:--------------|:---------------------------|:-----------------------------
| <span data-ttu-id="f5faa-111">mentionees</span><span class="sxs-lookup"><span data-stu-id="f5faa-111">mentionees</span></span>    | <span data-ttu-id="f5faa-112">Коллекция [identitySet][]</span><span class="sxs-lookup"><span data-stu-id="f5faa-112">[identitySet][] collection</span></span> | <span data-ttu-id="f5faa-113">Удостоверения пользователей, упомянутых в этом действии.</span><span class="sxs-lookup"><span data-stu-id="f5faa-113">The identities of the users mentioned in this action.</span></span>

[identitySet]: identityset.md

## <a name="remarks"></a><span data-ttu-id="f5faa-115">Замечания</span><span class="sxs-lookup"><span data-stu-id="f5faa-115">Remarks</span></span>

<span data-ttu-id="f5faa-116">На данный момент записи о действиях над элементом доступны только в SharePoint и OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="f5faa-116">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

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

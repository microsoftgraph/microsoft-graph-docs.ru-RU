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
# <a name="mentionaction-resource-type"></a><span data-ttu-id="8f33b-103">Тип ресурса mentionAction</span><span class="sxs-lookup"><span data-stu-id="8f33b-103">mentionAction resource type</span></span>

<span data-ttu-id="8f33b-104">Ресурс **MentionAction** предоставляет сведения о ресурсе [activity][], в котором есть упоминания пользователей.</span><span class="sxs-lookup"><span data-stu-id="8f33b-104">The **MentionAction** resource provides information about an [activity][] that mentioned people.</span></span>

><span data-ttu-id="8f33b-105">**Примечание:** Записи действий элементов в настоящее время доступны только в SharePoint и OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="8f33b-105">**Note:** Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

[действии]: itemactivity.md
[activity]: itemactivity.md

## <a name="properties"></a><span data-ttu-id="8f33b-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="8f33b-107">Properties</span></span>

| <span data-ttu-id="8f33b-108">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="8f33b-108">Property name</span></span> | <span data-ttu-id="8f33b-109">Тип</span><span class="sxs-lookup"><span data-stu-id="8f33b-109">Type</span></span>                       | <span data-ttu-id="8f33b-110">Описание</span><span class="sxs-lookup"><span data-stu-id="8f33b-110">Description</span></span>
|:--------------|:---------------------------|:-----------------------------
| <span data-ttu-id="8f33b-111">mentionees</span><span class="sxs-lookup"><span data-stu-id="8f33b-111">mentionees</span></span>    | <span data-ttu-id="8f33b-112">Коллекция [identitySet][]</span><span class="sxs-lookup"><span data-stu-id="8f33b-112">[identitySet][] collection</span></span> | <span data-ttu-id="8f33b-113">Удостоверения пользователей, упомянутых в этом действии.</span><span class="sxs-lookup"><span data-stu-id="8f33b-113">The identities of the users mentioned in this action.</span></span>

[identitySet]: identityset.md

## <a name="json-representation"></a><span data-ttu-id="8f33b-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8f33b-115">JSON representation</span></span>

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

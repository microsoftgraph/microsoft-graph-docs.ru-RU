---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: MentionAction
localization_priority: Normal
ms.openlocfilehash: 7843feebd8ebca2022b276007d21a89b754217a0
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27804972"
---
# <a name="mentionaction-resource-type"></a><span data-ttu-id="5073c-102">Тип ресурса MentionAction</span><span class="sxs-lookup"><span data-stu-id="5073c-102">MentionAction resource type</span></span>

> <span data-ttu-id="5073c-103">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="5073c-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5073c-104">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5073c-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5073c-105">Ресурс **MentionAction** предоставляет сведения о ресурсе [activity][], в котором есть упоминания пользователей.</span><span class="sxs-lookup"><span data-stu-id="5073c-105">The **MentionAction** resource provides information about an [activity][] that mentioned people.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="5073c-107">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="5073c-107">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="5073c-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="5073c-108">Properties</span></span>

| <span data-ttu-id="5073c-109">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="5073c-109">Property name</span></span> | <span data-ttu-id="5073c-110">Тип</span><span class="sxs-lookup"><span data-stu-id="5073c-110">Type</span></span>                       | <span data-ttu-id="5073c-111">Описание</span><span class="sxs-lookup"><span data-stu-id="5073c-111">Description</span></span>
|:--------------|:---------------------------|:-----------------------------
| <span data-ttu-id="5073c-112">mentionees</span><span class="sxs-lookup"><span data-stu-id="5073c-112">mentionees</span></span>    | <span data-ttu-id="5073c-113">Коллекция [identitySet][]</span><span class="sxs-lookup"><span data-stu-id="5073c-113">[identitySet][] collection</span></span> | <span data-ttu-id="5073c-114">Удостоверения пользователей, упомянутых в этом действии.</span><span class="sxs-lookup"><span data-stu-id="5073c-114">The identities of the users mentioned in this action.</span></span>

[identitySet]: identityset.md

## <a name="remarks"></a><span data-ttu-id="5073c-116">Замечания</span><span class="sxs-lookup"><span data-stu-id="5073c-116">Remarks</span></span>

<span data-ttu-id="5073c-117">На данный момент записи о действиях над элементом доступны только в SharePoint и OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="5073c-117">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The MentionAction object provides information about who was mentioned during an activity.",
  "keywords": "activities,activity,action,mention",
  "section": "documentation",
  "tocPath": "Resources/MentionAction"
} -->

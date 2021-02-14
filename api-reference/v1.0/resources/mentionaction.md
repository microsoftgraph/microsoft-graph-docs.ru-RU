---
author: daspek
title: Тип ресурса mentionAction
description: Объект MentionAction предоставляет сведения о том, кто был упомянут во время действия.
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: bc876f05949beb09b3e495a8b9b0536070b352cb
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/14/2021
ms.locfileid: "50238388"
---
# <a name="mentionaction-resource-type"></a><span data-ttu-id="b44e0-103">Тип ресурса mentionAction</span><span class="sxs-lookup"><span data-stu-id="b44e0-103">mentionAction resource type</span></span>

<span data-ttu-id="b44e0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b44e0-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b44e0-105">Ресурс **MentionAction** предоставляет сведения о ресурсе [activity][], в котором есть упоминания пользователей.</span><span class="sxs-lookup"><span data-stu-id="b44e0-105">The **MentionAction** resource provides information about an [activity][] that mentioned people.</span></span>

><span data-ttu-id="b44e0-106">**Примечание.** Записи о действиях с элементами в настоящее время доступны только в SharePoint и OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="b44e0-106">**Note:** Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

[действии]: itemactivity.md
[activity]: itemactivity.md

## <a name="properties"></a><span data-ttu-id="b44e0-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="b44e0-108">Properties</span></span>

| <span data-ttu-id="b44e0-109">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="b44e0-109">Property name</span></span> | <span data-ttu-id="b44e0-110">Тип</span><span class="sxs-lookup"><span data-stu-id="b44e0-110">Type</span></span>                       | <span data-ttu-id="b44e0-111">Описание</span><span class="sxs-lookup"><span data-stu-id="b44e0-111">Description</span></span>
|:--------------|:---------------------------|:-----------------------------
| <span data-ttu-id="b44e0-112">mentionees</span><span class="sxs-lookup"><span data-stu-id="b44e0-112">mentionees</span></span>    | <span data-ttu-id="b44e0-113">Коллекция [identitySet][]</span><span class="sxs-lookup"><span data-stu-id="b44e0-113">[identitySet][] collection</span></span> | <span data-ttu-id="b44e0-114">Удостоверения пользователей, упомянутых в этом действии.</span><span class="sxs-lookup"><span data-stu-id="b44e0-114">The identities of the users mentioned in this action.</span></span>

[identitySet]: identityset.md

## <a name="json-representation"></a><span data-ttu-id="b44e0-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b44e0-116">JSON representation</span></span>

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


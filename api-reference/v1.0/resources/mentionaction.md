---
author: daspek
ms.author: dspektor
title: Тип ресурса mentionAction
description: Объект MentionAction предоставляет сведения о пользователях, упомянутых во время действия.
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: de6bf1657e9b9ba21d589a6ef27292553bf93f7e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42534249"
---
# <a name="mentionaction-resource-type"></a><span data-ttu-id="12792-103">Тип ресурса mentionAction</span><span class="sxs-lookup"><span data-stu-id="12792-103">mentionAction resource type</span></span>

<span data-ttu-id="12792-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="12792-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="12792-105">Ресурс **MentionAction** предоставляет сведения о ресурсе [activity][], в котором есть упоминания пользователей.</span><span class="sxs-lookup"><span data-stu-id="12792-105">The **MentionAction** resource provides information about an [activity][] that mentioned people.</span></span>

><span data-ttu-id="12792-106">**Примечание:** Записи действий элементов в настоящее время доступны только в SharePoint и OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="12792-106">**Note:** Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

[действии]: itemactivity.md
[activity]: itemactivity.md

## <a name="properties"></a><span data-ttu-id="12792-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="12792-108">Properties</span></span>

| <span data-ttu-id="12792-109">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="12792-109">Property name</span></span> | <span data-ttu-id="12792-110">Тип</span><span class="sxs-lookup"><span data-stu-id="12792-110">Type</span></span>                       | <span data-ttu-id="12792-111">Описание</span><span class="sxs-lookup"><span data-stu-id="12792-111">Description</span></span>
|:--------------|:---------------------------|:-----------------------------
| <span data-ttu-id="12792-112">mentionees</span><span class="sxs-lookup"><span data-stu-id="12792-112">mentionees</span></span>    | <span data-ttu-id="12792-113">Коллекция [identitySet][]</span><span class="sxs-lookup"><span data-stu-id="12792-113">[identitySet][] collection</span></span> | <span data-ttu-id="12792-114">Удостоверения пользователей, упомянутых в этом действии.</span><span class="sxs-lookup"><span data-stu-id="12792-114">The identities of the users mentioned in this action.</span></span>

[identitySet]: identityset.md

## <a name="json-representation"></a><span data-ttu-id="12792-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="12792-116">JSON representation</span></span>

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

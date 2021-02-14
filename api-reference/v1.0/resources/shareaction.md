---
author: daspek
title: Тип ресурса shareAction
description: Объект shareAction предоставляет сведения о том, кому был общим элемент в действии общего доступа.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 81292f302667123c0d22f78b655e4ef555329e52
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/14/2021
ms.locfileid: "50238892"
---
# <a name="shareaction-resource-type"></a><span data-ttu-id="5397d-103">Тип ресурса shareAction</span><span class="sxs-lookup"><span data-stu-id="5397d-103">shareAction resource type</span></span>

<span data-ttu-id="5397d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5397d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5397d-105">Ресурс **shareAction** предоставляет сведения о [действии, которое][activity] предоставляет общий доступ к элементу.</span><span class="sxs-lookup"><span data-stu-id="5397d-105">The **shareAction** resource provides information about an [activity][activity] that shared an item.</span></span>

><span data-ttu-id="5397d-106">**Примечание.** Записи о действиях с элементами в настоящее время доступны только в SharePoint и OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="5397d-106">**Note:** Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

[activity]: itemactivity.md

## <a name="properties"></a><span data-ttu-id="5397d-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="5397d-107">Properties</span></span>

| <span data-ttu-id="5397d-108">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="5397d-108">Property name</span></span> | <span data-ttu-id="5397d-109">Тип</span><span class="sxs-lookup"><span data-stu-id="5397d-109">Type</span></span>                       | <span data-ttu-id="5397d-110">Описание</span><span class="sxs-lookup"><span data-stu-id="5397d-110">Description</span></span>
|:--------------|:---------------------------|:-----------------------------
| <span data-ttu-id="5397d-111">recipients</span><span class="sxs-lookup"><span data-stu-id="5397d-111">recipients</span></span>    | <span data-ttu-id="5397d-112">Коллекция [identitySet][]</span><span class="sxs-lookup"><span data-stu-id="5397d-112">[identitySet][] collection</span></span> | <span data-ttu-id="5397d-113">Удостоверения, к которым был предоставлен доступ элементу в результате выполнения этого действия.</span><span class="sxs-lookup"><span data-stu-id="5397d-113">The identities the item was shared with in this action.</span></span>

[identitySet]: identityset.md

## <a name="json-representation"></a><span data-ttu-id="5397d-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5397d-115">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.shareAction"
}-->

```json
{
  "recipients": [{"@odata.type": "microsoft.graph.identitySet"}]
}
```

<!--
{
  "type": "#page.annotation",
  "description": "The shareAction object provides information about who an item was shared to in a share action.",
  "keywords": "activities,activity,action,mention",
  "section": "documentation",
  "tocPath": "Resources/shareAction",
  "suppressions": []
}
-->


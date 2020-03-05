---
author: daspek
description: Ресурс ShareAction содержит сведения о действии, в результате выполнения которого был предоставлен общий доступ к элементу.
ms.date: 09/14/2017
title: ShareAction
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 94bf1b519308043f3421dc211eac006cfc4fd601
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520747"
---
# <a name="shareaction-resource-type"></a><span data-ttu-id="69f00-103">Тип ресурса ShareAction</span><span class="sxs-lookup"><span data-stu-id="69f00-103">ShareAction resource type</span></span>

<span data-ttu-id="69f00-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="69f00-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="69f00-105">Ресурс **ShareAction** содержит сведения о [действии][activity], в результате выполнения которого был предоставлен общий доступ к элементу.</span><span class="sxs-lookup"><span data-stu-id="69f00-105">The **ShareAction** resource provides information about an [activity][activity] that shared an item.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="69f00-106">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="69f00-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="69f00-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="69f00-107">Properties</span></span>

| <span data-ttu-id="69f00-108">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="69f00-108">Property name</span></span> | <span data-ttu-id="69f00-109">Тип</span><span class="sxs-lookup"><span data-stu-id="69f00-109">Type</span></span>                       | <span data-ttu-id="69f00-110">Описание</span><span class="sxs-lookup"><span data-stu-id="69f00-110">Description</span></span>
|:--------------|:---------------------------|:-----------------------------
| <span data-ttu-id="69f00-111">recipients</span><span class="sxs-lookup"><span data-stu-id="69f00-111">recipients</span></span>    | <span data-ttu-id="69f00-112">Коллекция [identitySet][]</span><span class="sxs-lookup"><span data-stu-id="69f00-112">[identitySet][] collection</span></span> | <span data-ttu-id="69f00-113">Удостоверения, к которым был предоставлен доступ элементу в результате выполнения этого действия.</span><span class="sxs-lookup"><span data-stu-id="69f00-113">The identities the item was shared with in this action.</span></span>

[identitySet]: identityset.md

## <a name="remarks"></a><span data-ttu-id="69f00-115">Замечания</span><span class="sxs-lookup"><span data-stu-id="69f00-115">Remarks</span></span>

<span data-ttu-id="69f00-116">На данный момент записи о действиях над элементом доступны только в SharePoint и OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="69f00-116">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "The ShareAction object provides information about who an item was shared to in a share action.",
  "keywords": "activities,activity,action,mention",
  "section": "documentation",
  "tocPath": "Resources/ShareAction",
  "suppressions": []
}
-->

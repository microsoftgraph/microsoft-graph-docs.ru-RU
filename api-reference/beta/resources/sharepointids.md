---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: SharePointIds
localization_priority: Normal
ms.openlocfilehash: 6c67c45b333ead1d427c5b15ddd4ed5925b84eac
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27807814"
---
# <a name="sharepointids-resource-type"></a><span data-ttu-id="3c2e6-102">Тип ресурса SharePointIds</span><span class="sxs-lookup"><span data-stu-id="3c2e6-102">SharePointIds resource type</span></span>

> <span data-ttu-id="3c2e6-103">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="3c2e6-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3c2e6-104">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3c2e6-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3c2e6-105">Ресурс **SharePointIds** — это единая структура, объединяющая различные идентификаторы элемента, хранящегося на сайте SharePoint или в OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="3c2e6-105">The **SharePointIds** resource groups the various identifiers for an item stored in a SharePoint site or OneDrive for Business into a single structure.</span></span>

<span data-ttu-id="3c2e6-106">**Примечание.** Элементы, возвращаемые из личного хранилища OneDrive, не включают аспект **SharePointIds**.</span><span class="sxs-lookup"><span data-stu-id="3c2e6-106">**Note:** items returned from OneDrive personal will not include a **SharePointIds** facet.</span></span>

## <a name="json-representation"></a><span data-ttu-id="3c2e6-107">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3c2e6-107">JSON representation</span></span>

<span data-ttu-id="3c2e6-108">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="3c2e6-108">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ "listId", "listItemId", "listItemUniqueId", "siteId", "siteUrl", "webId" ],
  "@odata.type": "microsoft.graph.sharepointIds"
}-->

```json
{
    "listId": "string",
    "listItemId": "string",
    "listItemUniqueId": "string",
    "siteId": "string",
    "siteUrl": "url",
    "tenantId": "string",
    "webId": "string"
}
```

## <a name="properties"></a><span data-ttu-id="3c2e6-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="3c2e6-109">Properties</span></span>

| <span data-ttu-id="3c2e6-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="3c2e6-110">Property</span></span>         | <span data-ttu-id="3c2e6-111">Тип</span><span class="sxs-lookup"><span data-stu-id="3c2e6-111">Type</span></span>         | <span data-ttu-id="3c2e6-112">Описание</span><span class="sxs-lookup"><span data-stu-id="3c2e6-112">Description</span></span>
|:-----------------|:-------------|:-------------------------------------------
| <span data-ttu-id="3c2e6-113">listId</span><span class="sxs-lookup"><span data-stu-id="3c2e6-113">listId</span></span>           | <span data-ttu-id="3c2e6-114">string</span><span class="sxs-lookup"><span data-stu-id="3c2e6-114">string</span></span>       | <span data-ttu-id="3c2e6-115">Уникальный идентификатор (GUID) списка, содержащего элемент, в SharePoint.</span><span class="sxs-lookup"><span data-stu-id="3c2e6-115">The unique identifier (guid) for the item's list in SharePoint.</span></span>
| <span data-ttu-id="3c2e6-116">listItemId</span><span class="sxs-lookup"><span data-stu-id="3c2e6-116">listItemId</span></span>       | <span data-ttu-id="3c2e6-117">string</span><span class="sxs-lookup"><span data-stu-id="3c2e6-117">string</span></span>       | <span data-ttu-id="3c2e6-118">Целочисленный идентификатор элемента в списке.</span><span class="sxs-lookup"><span data-stu-id="3c2e6-118">An integer identifier for the item within the containing list.</span></span>
| <span data-ttu-id="3c2e6-119">listItemUniqueId</span><span class="sxs-lookup"><span data-stu-id="3c2e6-119">listItemUniqueId</span></span> | <span data-ttu-id="3c2e6-120">строка</span><span class="sxs-lookup"><span data-stu-id="3c2e6-120">string</span></span>       | <span data-ttu-id="3c2e6-121">Уникальный идентификатор (GUID) элемента в OneDrive для бизнеса или на сайте SharePoint.</span><span class="sxs-lookup"><span data-stu-id="3c2e6-121">The unique identifier (guid) for the item within OneDrive for Business or a SharePoint site.</span></span>
| <span data-ttu-id="3c2e6-122">siteId</span><span class="sxs-lookup"><span data-stu-id="3c2e6-122">siteId</span></span>           | <span data-ttu-id="3c2e6-123">string</span><span class="sxs-lookup"><span data-stu-id="3c2e6-123">string</span></span>       | <span data-ttu-id="3c2e6-124">Уникальный идентификатор (GUID) семейства веб-сайтов (SPSite), содержащего элемент.</span><span class="sxs-lookup"><span data-stu-id="3c2e6-124">The unique identifier (guid) for the item's site collection (SPSite).</span></span>
| <span data-ttu-id="3c2e6-125">siteUrl</span><span class="sxs-lookup"><span data-stu-id="3c2e6-125">siteUrl</span></span>          | <span data-ttu-id="3c2e6-126">string (url)</span><span class="sxs-lookup"><span data-stu-id="3c2e6-126">string (url)</span></span> | <span data-ttu-id="3c2e6-127">URL-адрес SharePoint для сайта, содержащего элемент.</span><span class="sxs-lookup"><span data-stu-id="3c2e6-127">The SharePoint URL for the site that contains the item.</span></span>
| <span data-ttu-id="3c2e6-128">tenantId</span><span class="sxs-lookup"><span data-stu-id="3c2e6-128">tenantId</span></span>         | <span data-ttu-id="3c2e6-129">string</span><span class="sxs-lookup"><span data-stu-id="3c2e6-129">string</span></span>       | <span data-ttu-id="3c2e6-130">Уникальный идентификатор (guid) аренды.</span><span class="sxs-lookup"><span data-stu-id="3c2e6-130">The unique identifier (guid) for the tenancy.</span></span>
| <span data-ttu-id="3c2e6-131">webId</span><span class="sxs-lookup"><span data-stu-id="3c2e6-131">webId</span></span>            | <span data-ttu-id="3c2e6-132">string</span><span class="sxs-lookup"><span data-stu-id="3c2e6-132">string</span></span>       | <span data-ttu-id="3c2e6-133">Уникальный идентификатор (GUID) семейства веб-сайтов (SPWeb), содержащего элемент.</span><span class="sxs-lookup"><span data-stu-id="3c2e6-133">The unique identifier (guid) for the item's site (SPWeb).</span></span>

## <a name="remarks"></a><span data-ttu-id="3c2e6-134">Заметки</span><span class="sxs-lookup"><span data-stu-id="3c2e6-134">Remarks</span></span>

<span data-ttu-id="3c2e6-135">Дополнительные сведения об аспектах ресурса **driveItem** см. в описании типа [**driveItem**](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="3c2e6-135">For more information about the facets on a **driveItem**, see [**driveItem**](driveitem.md).</span></span>



<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "The SharepointIds facet provides Sharepoint ids associated with an item.",
  "keywords": "item, unique, id, csom, facet",
  "section": "documentation",
  "tocPath": "Facets/SharepointIds"
} -->

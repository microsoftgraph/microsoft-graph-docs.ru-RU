---
author: JeremyKelley
description: Ресурс SharePointIds — это единая структура, объединяющая различные идентификаторы элемента, хранящегося на сайте SharePoint или в OneDrive для бизнеса.
ms.date: 09/10/2017
title: SharePointIds
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: c7e18e43bcbe9c73500701577c752e7a30d47194
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965126"
---
# <a name="sharepointids-resource-type"></a><span data-ttu-id="c07c4-103">Тип ресурса SharePointIds</span><span class="sxs-lookup"><span data-stu-id="c07c4-103">SharePointIds resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c07c4-104">Ресурс **SharePointIds** — это единая структура, объединяющая различные идентификаторы элемента, хранящегося на сайте SharePoint или в OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="c07c4-104">The **SharePointIds** resource groups the various identifiers for an item stored in a SharePoint site or OneDrive for Business into a single structure.</span></span>

<span data-ttu-id="c07c4-105">**Примечание.** Элементы, возвращаемые из личного хранилища OneDrive, не включают аспект **SharePointIds**.</span><span class="sxs-lookup"><span data-stu-id="c07c4-105">**Note:** items returned from OneDrive personal will not include a **SharePointIds** facet.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c07c4-106">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c07c4-106">JSON representation</span></span>

<span data-ttu-id="c07c4-107">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="c07c4-107">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="c07c4-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="c07c4-108">Properties</span></span>

| <span data-ttu-id="c07c4-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="c07c4-109">Property</span></span>         | <span data-ttu-id="c07c4-110">Тип</span><span class="sxs-lookup"><span data-stu-id="c07c4-110">Type</span></span>         | <span data-ttu-id="c07c4-111">Описание</span><span class="sxs-lookup"><span data-stu-id="c07c4-111">Description</span></span>
|:-----------------|:-------------|:-------------------------------------------
| <span data-ttu-id="c07c4-112">listId</span><span class="sxs-lookup"><span data-stu-id="c07c4-112">listId</span></span>           | <span data-ttu-id="c07c4-113">string</span><span class="sxs-lookup"><span data-stu-id="c07c4-113">string</span></span>       | <span data-ttu-id="c07c4-114">Уникальный идентификатор (GUID) списка, содержащего элемент, в SharePoint.</span><span class="sxs-lookup"><span data-stu-id="c07c4-114">The unique identifier (guid) for the item's list in SharePoint.</span></span>
| <span data-ttu-id="c07c4-115">listItemId</span><span class="sxs-lookup"><span data-stu-id="c07c4-115">listItemId</span></span>       | <span data-ttu-id="c07c4-116">string</span><span class="sxs-lookup"><span data-stu-id="c07c4-116">string</span></span>       | <span data-ttu-id="c07c4-117">Целочисленный идентификатор элемента в списке.</span><span class="sxs-lookup"><span data-stu-id="c07c4-117">An integer identifier for the item within the containing list.</span></span>
| <span data-ttu-id="c07c4-118">listItemUniqueId</span><span class="sxs-lookup"><span data-stu-id="c07c4-118">listItemUniqueId</span></span> | <span data-ttu-id="c07c4-119">string</span><span class="sxs-lookup"><span data-stu-id="c07c4-119">string</span></span>       | <span data-ttu-id="c07c4-120">Уникальный идентификатор (GUID) элемента в OneDrive для бизнеса или на сайте SharePoint.</span><span class="sxs-lookup"><span data-stu-id="c07c4-120">The unique identifier (guid) for the item within OneDrive for Business or a SharePoint site.</span></span>
| <span data-ttu-id="c07c4-121">siteId</span><span class="sxs-lookup"><span data-stu-id="c07c4-121">siteId</span></span>           | <span data-ttu-id="c07c4-122">string</span><span class="sxs-lookup"><span data-stu-id="c07c4-122">string</span></span>       | <span data-ttu-id="c07c4-123">Уникальный идентификатор (GUID) семейства веб-сайтов (SPSite), содержащего элемент.</span><span class="sxs-lookup"><span data-stu-id="c07c4-123">The unique identifier (guid) for the item's site collection (SPSite).</span></span>
| <span data-ttu-id="c07c4-124">siteUrl</span><span class="sxs-lookup"><span data-stu-id="c07c4-124">siteUrl</span></span>          | <span data-ttu-id="c07c4-125">string (url)</span><span class="sxs-lookup"><span data-stu-id="c07c4-125">string (url)</span></span> | <span data-ttu-id="c07c4-126">URL-адрес SharePoint для сайта, содержащего элемент.</span><span class="sxs-lookup"><span data-stu-id="c07c4-126">The SharePoint URL for the site that contains the item.</span></span>
| <span data-ttu-id="c07c4-127">tenantId</span><span class="sxs-lookup"><span data-stu-id="c07c4-127">tenantId</span></span>         | <span data-ttu-id="c07c4-128">string</span><span class="sxs-lookup"><span data-stu-id="c07c4-128">string</span></span>       | <span data-ttu-id="c07c4-129">Уникальный идентификатор (GUID) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c07c4-129">The unique identifier (guid) for the tenancy.</span></span>
| <span data-ttu-id="c07c4-130">webId</span><span class="sxs-lookup"><span data-stu-id="c07c4-130">webId</span></span>            | <span data-ttu-id="c07c4-131">string</span><span class="sxs-lookup"><span data-stu-id="c07c4-131">string</span></span>       | <span data-ttu-id="c07c4-132">Уникальный идентификатор (GUID) семейства веб-сайтов (SPWeb), содержащего элемент.</span><span class="sxs-lookup"><span data-stu-id="c07c4-132">The unique identifier (guid) for the item's site (SPWeb).</span></span>

## <a name="remarks"></a><span data-ttu-id="c07c4-133">Заметки</span><span class="sxs-lookup"><span data-stu-id="c07c4-133">Remarks</span></span>

<span data-ttu-id="c07c4-134">Дополнительные сведения об аспектах ресурса **driveItem** см. в описании типа [**driveItem**](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="c07c4-134">For more information about the facets on a **driveItem**, see [**driveItem**](driveitem.md).</span></span>



<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "The SharepointIds facet provides Sharepoint ids associated with an item.",
  "keywords": "item, unique, id, csom, facet",
  "section": "documentation",
  "tocPath": "Facets/SharepointIds",
  "suppressions": []
}
-->

---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: SharePointIds
localization_priority: Normal
ms.prod: sharepoint
description: Ресурс SharePointIds — это единая структура, объединяющая различные идентификаторы элемента, хранящегося на сайте SharePoint или в OneDrive для бизнеса.
doc_type: resourcePageType
ms.openlocfilehash: a7dfd936770ac85b458cb8b086ff05e328d2ea9c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36034281"
---
# <a name="sharepointids-resource-type"></a><span data-ttu-id="1bf5e-103">Тип ресурса SharePointIds</span><span class="sxs-lookup"><span data-stu-id="1bf5e-103">SharePointIds resource type</span></span>

<span data-ttu-id="1bf5e-104">Ресурс **SharePointIds** — это единая структура, объединяющая различные идентификаторы элемента, хранящегося на сайте SharePoint или в OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="1bf5e-104">The **SharePointIds** resource groups the various identifiers for an item stored in a SharePoint site or OneDrive for Business into a single structure.</span></span>

<span data-ttu-id="1bf5e-105">**Примечание.** Элементы, возвращаемые из личного хранилища OneDrive, не включают аспект **SharePointIds**.</span><span class="sxs-lookup"><span data-stu-id="1bf5e-105">**Note:** items returned from OneDrive personal will not include a **SharePointIds** facet.</span></span>

## <a name="json-representation"></a><span data-ttu-id="1bf5e-106">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1bf5e-106">JSON representation</span></span>

<span data-ttu-id="1bf5e-107">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="1bf5e-107">Here is a JSON representation of the resource</span></span>

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
    "webId": "string"
}
```

## <a name="properties"></a><span data-ttu-id="1bf5e-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="1bf5e-108">Properties</span></span>

| <span data-ttu-id="1bf5e-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="1bf5e-109">Property</span></span>         | <span data-ttu-id="1bf5e-110">Тип</span><span class="sxs-lookup"><span data-stu-id="1bf5e-110">Type</span></span>         | <span data-ttu-id="1bf5e-111">Описание</span><span class="sxs-lookup"><span data-stu-id="1bf5e-111">Description</span></span>
|:-----------------|:-------------|:-------------------------------------------
| <span data-ttu-id="1bf5e-112">listId</span><span class="sxs-lookup"><span data-stu-id="1bf5e-112">listId</span></span>           | <span data-ttu-id="1bf5e-113">string</span><span class="sxs-lookup"><span data-stu-id="1bf5e-113">string</span></span>       | <span data-ttu-id="1bf5e-114">Уникальный идентификатор (GUID) списка, содержащего элемент, в SharePoint.</span><span class="sxs-lookup"><span data-stu-id="1bf5e-114">The unique identifier (guid) for the item's list in SharePoint.</span></span>
| <span data-ttu-id="1bf5e-115">listItemId</span><span class="sxs-lookup"><span data-stu-id="1bf5e-115">listItemId</span></span>       | <span data-ttu-id="1bf5e-116">string</span><span class="sxs-lookup"><span data-stu-id="1bf5e-116">string</span></span>       | <span data-ttu-id="1bf5e-117">Целочисленный идентификатор элемента в списке.</span><span class="sxs-lookup"><span data-stu-id="1bf5e-117">An integer identifier for the item within the containing list.</span></span>
| <span data-ttu-id="1bf5e-118">listItemUniqueId</span><span class="sxs-lookup"><span data-stu-id="1bf5e-118">listItemUniqueId</span></span> | <span data-ttu-id="1bf5e-119">string</span><span class="sxs-lookup"><span data-stu-id="1bf5e-119">string</span></span>       | <span data-ttu-id="1bf5e-120">Уникальный идентификатор (GUID) элемента в OneDrive для бизнеса или на сайте SharePoint.</span><span class="sxs-lookup"><span data-stu-id="1bf5e-120">The unique identifier (guid) for the item within OneDrive for Business or a SharePoint site.</span></span>
| <span data-ttu-id="1bf5e-121">siteId</span><span class="sxs-lookup"><span data-stu-id="1bf5e-121">siteId</span></span>           | <span data-ttu-id="1bf5e-122">string</span><span class="sxs-lookup"><span data-stu-id="1bf5e-122">string</span></span>       | <span data-ttu-id="1bf5e-123">Уникальный идентификатор (GUID) семейства веб-сайтов (SPSite), содержащего элемент.</span><span class="sxs-lookup"><span data-stu-id="1bf5e-123">The unique identifier (guid) for the item's site collection (SPSite).</span></span>
| <span data-ttu-id="1bf5e-124">siteUrl</span><span class="sxs-lookup"><span data-stu-id="1bf5e-124">siteUrl</span></span>          | <span data-ttu-id="1bf5e-125">string (url)</span><span class="sxs-lookup"><span data-stu-id="1bf5e-125">string (url)</span></span> | <span data-ttu-id="1bf5e-126">URL-адрес SharePoint для сайта, содержащего элемент.</span><span class="sxs-lookup"><span data-stu-id="1bf5e-126">The SharePoint URL for the site that contains the item.</span></span>
| <span data-ttu-id="1bf5e-127">webId</span><span class="sxs-lookup"><span data-stu-id="1bf5e-127">webId</span></span>            | <span data-ttu-id="1bf5e-128">string</span><span class="sxs-lookup"><span data-stu-id="1bf5e-128">string</span></span>       | <span data-ttu-id="1bf5e-129">Уникальный идентификатор (GUID) семейства веб-сайтов (SPWeb), содержащего элемент.</span><span class="sxs-lookup"><span data-stu-id="1bf5e-129">The unique identifier (guid) for the item's site (SPWeb).</span></span>

## <a name="remarks"></a><span data-ttu-id="1bf5e-130">Заметки</span><span class="sxs-lookup"><span data-stu-id="1bf5e-130">Remarks</span></span>

<span data-ttu-id="1bf5e-131">Дополнительные сведения об аспектах ресурса **driveItem** см. в описании типа [**driveItem**](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="1bf5e-131">For more information about the facets on a **driveItem**, see [**driveItem**](driveitem.md).</span></span>



<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "The SharepointIds facet provides Sharepoint ids associated with an item.",
  "keywords": "item, unique, id, csom, facet",
  "section": "documentation",
  "tocPath": "Facets/SharepointIds"
} -->

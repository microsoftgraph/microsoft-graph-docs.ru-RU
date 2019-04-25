---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: SharePointIds
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 233c2aa4b8ce67b2382996181c9ba2ab57b9e69c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32549589"
---
# <a name="sharepointids-resource-type"></a><span data-ttu-id="64c3e-102">Тип ресурса SharePointIds</span><span class="sxs-lookup"><span data-stu-id="64c3e-102">SharePointIds resource type</span></span>

<span data-ttu-id="64c3e-103">Ресурс **SharePointIds** — это единая структура, объединяющая различные идентификаторы элемента, хранящегося на сайте SharePoint или в OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="64c3e-103">The **SharePointIds** resource groups the various identifiers for an item stored in a SharePoint site or OneDrive for Business into a single structure.</span></span>

<span data-ttu-id="64c3e-104">**Примечание.** Элементы, возвращаемые из личного хранилища OneDrive, не включают аспект **SharePointIds**.</span><span class="sxs-lookup"><span data-stu-id="64c3e-104">**Note:** items returned from OneDrive personal will not include a **SharePointIds** facet.</span></span>

## <a name="json-representation"></a><span data-ttu-id="64c3e-105">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="64c3e-105">JSON representation</span></span>

<span data-ttu-id="64c3e-106">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="64c3e-106">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="64c3e-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="64c3e-107">Properties</span></span>

| <span data-ttu-id="64c3e-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="64c3e-108">Property</span></span>         | <span data-ttu-id="64c3e-109">Тип</span><span class="sxs-lookup"><span data-stu-id="64c3e-109">Type</span></span>         | <span data-ttu-id="64c3e-110">Описание</span><span class="sxs-lookup"><span data-stu-id="64c3e-110">Description</span></span>
|:-----------------|:-------------|:-------------------------------------------
| <span data-ttu-id="64c3e-111">listId</span><span class="sxs-lookup"><span data-stu-id="64c3e-111">listId</span></span>           | <span data-ttu-id="64c3e-112">string</span><span class="sxs-lookup"><span data-stu-id="64c3e-112">string</span></span>       | <span data-ttu-id="64c3e-113">Уникальный идентификатор (GUID) списка, содержащего элемент, в SharePoint.</span><span class="sxs-lookup"><span data-stu-id="64c3e-113">The unique identifier (guid) for the item's list in SharePoint.</span></span>
| <span data-ttu-id="64c3e-114">listItemId</span><span class="sxs-lookup"><span data-stu-id="64c3e-114">listItemId</span></span>       | <span data-ttu-id="64c3e-115">string</span><span class="sxs-lookup"><span data-stu-id="64c3e-115">string</span></span>       | <span data-ttu-id="64c3e-116">Целочисленный идентификатор элемента в списке.</span><span class="sxs-lookup"><span data-stu-id="64c3e-116">An integer identifier for the item within the containing list.</span></span>
| <span data-ttu-id="64c3e-117">listItemUniqueId</span><span class="sxs-lookup"><span data-stu-id="64c3e-117">listItemUniqueId</span></span> | <span data-ttu-id="64c3e-118">string</span><span class="sxs-lookup"><span data-stu-id="64c3e-118">string</span></span>       | <span data-ttu-id="64c3e-119">Уникальный идентификатор (GUID) элемента в OneDrive для бизнеса или на сайте SharePoint.</span><span class="sxs-lookup"><span data-stu-id="64c3e-119">The unique identifier (guid) for the item within OneDrive for Business or a SharePoint site.</span></span>
| <span data-ttu-id="64c3e-120">siteId</span><span class="sxs-lookup"><span data-stu-id="64c3e-120">siteId</span></span>           | <span data-ttu-id="64c3e-121">string</span><span class="sxs-lookup"><span data-stu-id="64c3e-121">string</span></span>       | <span data-ttu-id="64c3e-122">Уникальный идентификатор (GUID) семейства веб-сайтов (SPSite), содержащего элемент.</span><span class="sxs-lookup"><span data-stu-id="64c3e-122">The unique identifier (guid) for the item's site collection (SPSite).</span></span>
| <span data-ttu-id="64c3e-123">siteUrl</span><span class="sxs-lookup"><span data-stu-id="64c3e-123">siteUrl</span></span>          | <span data-ttu-id="64c3e-124">string (url)</span><span class="sxs-lookup"><span data-stu-id="64c3e-124">string (url)</span></span> | <span data-ttu-id="64c3e-125">URL-адрес SharePoint для сайта, содержащего элемент.</span><span class="sxs-lookup"><span data-stu-id="64c3e-125">The SharePoint URL for the site that contains the item.</span></span>
| <span data-ttu-id="64c3e-126">webId</span><span class="sxs-lookup"><span data-stu-id="64c3e-126">webId</span></span>            | <span data-ttu-id="64c3e-127">string</span><span class="sxs-lookup"><span data-stu-id="64c3e-127">string</span></span>       | <span data-ttu-id="64c3e-128">Уникальный идентификатор (GUID) семейства веб-сайтов (SPWeb), содержащего элемент.</span><span class="sxs-lookup"><span data-stu-id="64c3e-128">The unique identifier (guid) for the item's site (SPWeb).</span></span>

## <a name="remarks"></a><span data-ttu-id="64c3e-129">Заметки</span><span class="sxs-lookup"><span data-stu-id="64c3e-129">Remarks</span></span>

<span data-ttu-id="64c3e-130">Дополнительные сведения об аспектах ресурса **driveItem** см. в описании типа [**driveItem**](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="64c3e-130">For more information about the facets on a **driveItem**, see [**driveItem**](driveitem.md).</span></span>



<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "The SharepointIds facet provides Sharepoint ids associated with an item.",
  "keywords": "item, unique, id, csom, facet",
  "section": "documentation",
  "tocPath": "Facets/SharepointIds"
} -->

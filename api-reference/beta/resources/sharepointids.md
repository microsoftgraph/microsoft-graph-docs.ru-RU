---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: SharePointIds
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: c9f4c3dc54b9eee6cc1ab24058e3fe238fed89a3
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2019
ms.locfileid: "30480602"
---
# <a name="sharepointids-resource-type"></a><span data-ttu-id="08e08-102">Тип ресурса SharePointIds</span><span class="sxs-lookup"><span data-stu-id="08e08-102">SharePointIds resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="08e08-103">Ресурс **SharePointIds** — это единая структура, объединяющая различные идентификаторы элемента, хранящегося на сайте SharePoint или в OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="08e08-103">The **SharePointIds** resource groups the various identifiers for an item stored in a SharePoint site or OneDrive for Business into a single structure.</span></span>

<span data-ttu-id="08e08-104">**Примечание.** Элементы, возвращаемые из личного хранилища OneDrive, не включают аспект **SharePointIds**.</span><span class="sxs-lookup"><span data-stu-id="08e08-104">**Note:** items returned from OneDrive personal will not include a **SharePointIds** facet.</span></span>

## <a name="json-representation"></a><span data-ttu-id="08e08-105">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="08e08-105">JSON representation</span></span>

<span data-ttu-id="08e08-106">Ниже этот ресурс представлен в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="08e08-106">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="08e08-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="08e08-107">Properties</span></span>

| <span data-ttu-id="08e08-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="08e08-108">Property</span></span>         | <span data-ttu-id="08e08-109">Тип</span><span class="sxs-lookup"><span data-stu-id="08e08-109">Type</span></span>         | <span data-ttu-id="08e08-110">Описание</span><span class="sxs-lookup"><span data-stu-id="08e08-110">Description</span></span>
|:-----------------|:-------------|:-------------------------------------------
| <span data-ttu-id="08e08-111">listId</span><span class="sxs-lookup"><span data-stu-id="08e08-111">listId</span></span>           | <span data-ttu-id="08e08-112">string</span><span class="sxs-lookup"><span data-stu-id="08e08-112">string</span></span>       | <span data-ttu-id="08e08-113">Уникальный идентификатор (GUID) списка, содержащего элемент, в SharePoint.</span><span class="sxs-lookup"><span data-stu-id="08e08-113">The unique identifier (guid) for the item's list in SharePoint.</span></span>
| <span data-ttu-id="08e08-114">listItemId</span><span class="sxs-lookup"><span data-stu-id="08e08-114">listItemId</span></span>       | <span data-ttu-id="08e08-115">string</span><span class="sxs-lookup"><span data-stu-id="08e08-115">string</span></span>       | <span data-ttu-id="08e08-116">Целочисленный идентификатор элемента в списке.</span><span class="sxs-lookup"><span data-stu-id="08e08-116">An integer identifier for the item within the containing list.</span></span>
| <span data-ttu-id="08e08-117">listItemUniqueId</span><span class="sxs-lookup"><span data-stu-id="08e08-117">listItemUniqueId</span></span> | <span data-ttu-id="08e08-118">string</span><span class="sxs-lookup"><span data-stu-id="08e08-118">string</span></span>       | <span data-ttu-id="08e08-119">Уникальный идентификатор (GUID) элемента в OneDrive для бизнеса или на сайте SharePoint.</span><span class="sxs-lookup"><span data-stu-id="08e08-119">The unique identifier (guid) for the item within OneDrive for Business or a SharePoint site.</span></span>
| <span data-ttu-id="08e08-120">siteId</span><span class="sxs-lookup"><span data-stu-id="08e08-120">siteId</span></span>           | <span data-ttu-id="08e08-121">string</span><span class="sxs-lookup"><span data-stu-id="08e08-121">string</span></span>       | <span data-ttu-id="08e08-122">Уникальный идентификатор (GUID) семейства веб-сайтов (SPSite), содержащего элемент.</span><span class="sxs-lookup"><span data-stu-id="08e08-122">The unique identifier (guid) for the item's site collection (SPSite).</span></span>
| <span data-ttu-id="08e08-123">siteUrl</span><span class="sxs-lookup"><span data-stu-id="08e08-123">siteUrl</span></span>          | <span data-ttu-id="08e08-124">string (url)</span><span class="sxs-lookup"><span data-stu-id="08e08-124">string (url)</span></span> | <span data-ttu-id="08e08-125">URL-адрес SharePoint для сайта, содержащего элемент.</span><span class="sxs-lookup"><span data-stu-id="08e08-125">The SharePoint URL for the site that contains the item.</span></span>
| <span data-ttu-id="08e08-126">tenantId</span><span class="sxs-lookup"><span data-stu-id="08e08-126">tenantId</span></span>         | <span data-ttu-id="08e08-127">string</span><span class="sxs-lookup"><span data-stu-id="08e08-127">string</span></span>       | <span data-ttu-id="08e08-128">Уникальный идентификатор (GUID) для клиента.</span><span class="sxs-lookup"><span data-stu-id="08e08-128">The unique identifier (guid) for the tenancy.</span></span>
| <span data-ttu-id="08e08-129">webId</span><span class="sxs-lookup"><span data-stu-id="08e08-129">webId</span></span>            | <span data-ttu-id="08e08-130">string</span><span class="sxs-lookup"><span data-stu-id="08e08-130">string</span></span>       | <span data-ttu-id="08e08-131">Уникальный идентификатор (GUID) семейства веб-сайтов (SPWeb), содержащего элемент.</span><span class="sxs-lookup"><span data-stu-id="08e08-131">The unique identifier (guid) for the item's site (SPWeb).</span></span>

## <a name="remarks"></a><span data-ttu-id="08e08-132">Заметки</span><span class="sxs-lookup"><span data-stu-id="08e08-132">Remarks</span></span>

<span data-ttu-id="08e08-133">Дополнительные сведения об аспектах ресурса **driveItem** см. в описании типа [**driveItem**](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="08e08-133">For more information about the facets on a **driveItem**, see [**driveItem**](driveitem.md).</span></span>



<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "The SharepointIds facet provides Sharepoint ids associated with an item.",
  "keywords": "item, unique, id, csom, facet",
  "section": "documentation",
  "tocPath": "Facets/SharepointIds",
  "suppressions": [
    "Error: /api-reference/beta/resources/sharepointids.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

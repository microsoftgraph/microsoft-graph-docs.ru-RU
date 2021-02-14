---
author: JeremyKelley
ms.date: 09/10/2017
title: SiteCollection
localization_priority: Normal
ms.prod: sharepoint
description: Ресурс siteCollection предоставляет больше сведений о семействе веб-сайтов.
doc_type: resourcePageType
ms.openlocfilehash: 1e80ad630fd1ac823ce76c44c3b789b0986d031f
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/14/2021
ms.locfileid: "50239438"
---
# <a name="sitecollection-resource"></a><span data-ttu-id="ff131-103">Ресурс SiteCollection</span><span class="sxs-lookup"><span data-stu-id="ff131-103">SiteCollection resource</span></span>

<span data-ttu-id="ff131-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ff131-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ff131-105">Ресурс **siteCollection** предоставляет больше сведений о семействе веб-сайтов.</span><span class="sxs-lookup"><span data-stu-id="ff131-105">The **siteCollection** resource provides more information about a site collection.</span></span>

<span data-ttu-id="ff131-106">Если для свойства **siteCollection** ресурса [**site**](site.md) задано значение, отличное от NULL, этот сайт является корневым для семейства веб-сайтов.</span><span class="sxs-lookup"><span data-stu-id="ff131-106">If a [**site**](site.md) resource has a non-null **siteCollection** property, then the site is a root site for a site collection.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ff131-107">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ff131-107">JSON representation</span></span>

<span data-ttu-id="ff131-108">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ff131-108">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  ],
  "@odata.type": "microsoft.graph.siteCollection"
}-->

```json
{
  "hostname": "contoso.sharepoint.com",
  "dataLocationCode": "EUR",
  "root": { "@odata.type": "microsoft.graph.root" }
}
```

## <a name="properties"></a><span data-ttu-id="ff131-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="ff131-109">Properties</span></span>

| <span data-ttu-id="ff131-110">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="ff131-110">Property name</span></span>        | <span data-ttu-id="ff131-111">Тип</span><span class="sxs-lookup"><span data-stu-id="ff131-111">Type</span></span>     | <span data-ttu-id="ff131-112">Описание</span><span class="sxs-lookup"><span data-stu-id="ff131-112">Description</span></span>
|:---------------------|:---------|:---------------------------------------------------
| <span data-ttu-id="ff131-113">**hostname**</span><span class="sxs-lookup"><span data-stu-id="ff131-113">**hostname**</span></span>         | <span data-ttu-id="ff131-114">строка</span><span class="sxs-lookup"><span data-stu-id="ff131-114">string</span></span>   | <span data-ttu-id="ff131-p101">Имя узла для семейства веб-сайтов. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ff131-p101">The hostname for the site collection. Read-only.</span></span>
| <span data-ttu-id="ff131-117">**dataLocationCode**</span><span class="sxs-lookup"><span data-stu-id="ff131-117">**dataLocationCode**</span></span> | <span data-ttu-id="ff131-118">string</span><span class="sxs-lookup"><span data-stu-id="ff131-118">string</span></span>   | <span data-ttu-id="ff131-119">Код географического региона для местоположения этого веб-сайта.</span><span class="sxs-lookup"><span data-stu-id="ff131-119">The geographic region code for where this site collection resides.</span></span> <span data-ttu-id="ff131-120">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ff131-120">Read-only.</span></span>
| <span data-ttu-id="ff131-121">**root**</span><span class="sxs-lookup"><span data-stu-id="ff131-121">**root**</span></span>             | <span data-ttu-id="ff131-122">[root][]</span><span class="sxs-lookup"><span data-stu-id="ff131-122">[root][]</span></span> | <span data-ttu-id="ff131-123">Если указан, означает, что это корневое коллекцию веб-сайтов в SharePoint.</span><span class="sxs-lookup"><span data-stu-id="ff131-123">If present, indicates that this is a root site collection in SharePoint.</span></span> <span data-ttu-id="ff131-124">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ff131-124">Read-only.</span></span>

[root]: root.md

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Facets/SiteCollection"
}-->


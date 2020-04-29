---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: SiteCollection
localization_priority: Normal
ms.prod: sharepoint
description: Ресурс siteCollection предоставляет больше сведений о семействе веб-сайтов.
doc_type: resourcePageType
ms.openlocfilehash: f73505ead4ad060f81bdfe7e77099783a8ff0242
ms.sourcegitcommit: 9b507499fb1ec61b4de47f36f915ae29c8594459
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/29/2020
ms.locfileid: "43934824"
---
# <a name="sitecollection-resource"></a><span data-ttu-id="94e90-103">Ресурс SiteCollection</span><span class="sxs-lookup"><span data-stu-id="94e90-103">SiteCollection resource</span></span>

<span data-ttu-id="94e90-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="94e90-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="94e90-105">Ресурс **siteCollection** предоставляет больше сведений о семействе веб-сайтов.</span><span class="sxs-lookup"><span data-stu-id="94e90-105">The **siteCollection** resource provides more information about a site collection.</span></span>

<span data-ttu-id="94e90-106">Если для свойства **siteCollection** ресурса [**site**](site.md) задано значение, отличное от NULL, этот сайт является корневым для семейства веб-сайтов.</span><span class="sxs-lookup"><span data-stu-id="94e90-106">If a [**site**](site.md) resource has a non-null **siteCollection** property, then the site is a root site for a site collection.</span></span>

## <a name="json-representation"></a><span data-ttu-id="94e90-107">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="94e90-107">JSON representation</span></span>

<span data-ttu-id="94e90-108">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="94e90-108">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="94e90-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="94e90-109">Properties</span></span>

| <span data-ttu-id="94e90-110">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="94e90-110">Property name</span></span>        | <span data-ttu-id="94e90-111">Тип</span><span class="sxs-lookup"><span data-stu-id="94e90-111">Type</span></span>     | <span data-ttu-id="94e90-112">Описание</span><span class="sxs-lookup"><span data-stu-id="94e90-112">Description</span></span>
|:---------------------|:---------|:---------------------------------------------------
| <span data-ttu-id="94e90-113">**hostname**</span><span class="sxs-lookup"><span data-stu-id="94e90-113">**hostname**</span></span>         | <span data-ttu-id="94e90-114">строка</span><span class="sxs-lookup"><span data-stu-id="94e90-114">string</span></span>   | <span data-ttu-id="94e90-p101">Имя узла для семейства веб-сайтов. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="94e90-p101">The hostname for the site collection. Read-only.</span></span>
| <span data-ttu-id="94e90-117">**даталокатионкоде**</span><span class="sxs-lookup"><span data-stu-id="94e90-117">**dataLocationCode**</span></span> | <span data-ttu-id="94e90-118">string</span><span class="sxs-lookup"><span data-stu-id="94e90-118">string</span></span>   | <span data-ttu-id="94e90-119">Код географического региона, в котором располагается это семейство веб-сайтов.</span><span class="sxs-lookup"><span data-stu-id="94e90-119">The geographic region code for where this site collection resides.</span></span> <span data-ttu-id="94e90-120">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="94e90-120">Read-only.</span></span>
| <span data-ttu-id="94e90-121">**root**</span><span class="sxs-lookup"><span data-stu-id="94e90-121">**root**</span></span>             | <span data-ttu-id="94e90-122">[root][]</span><span class="sxs-lookup"><span data-stu-id="94e90-122">[root][]</span></span> | <span data-ttu-id="94e90-123">Если задано, это указывает на то, что это корневое семейство веб-сайтов в SharePoint.</span><span class="sxs-lookup"><span data-stu-id="94e90-123">If present, indicates that this is a root site collection in SharePoint.</span></span> <span data-ttu-id="94e90-124">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="94e90-124">Read-only.</span></span>

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

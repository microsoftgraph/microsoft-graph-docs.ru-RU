---
author: JeremyKelley
description: Ресурс siteCollection предоставляет больше сведений о семействе веб-сайтов.
ms.date: 09/10/2017
title: SiteCollection
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 0989306be8fa8e456d2718079aec069097cab035
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36008294"
---
# <a name="sitecollection-resource"></a><span data-ttu-id="76d33-103">Ресурс SiteCollection</span><span class="sxs-lookup"><span data-stu-id="76d33-103">SiteCollection resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="76d33-104">Ресурс **siteCollection** предоставляет больше сведений о семействе веб-сайтов.</span><span class="sxs-lookup"><span data-stu-id="76d33-104">The **siteCollection** resource provides more information about a site collection.</span></span>

<span data-ttu-id="76d33-105">Если для свойства **siteCollection** ресурса [**site**](site.md) задано значение, отличное от NULL, этот сайт является корневым для семейства веб-сайтов.</span><span class="sxs-lookup"><span data-stu-id="76d33-105">If a [**site**](site.md) resource has a non-null **siteCollection** property, then the site is a root site for a site collection.</span></span>

## <a name="json-representation"></a><span data-ttu-id="76d33-106">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="76d33-106">JSON representation</span></span>

<span data-ttu-id="76d33-107">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="76d33-107">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "dataLocationCode", "root"
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

## <a name="properties"></a><span data-ttu-id="76d33-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="76d33-108">Properties</span></span>

| <span data-ttu-id="76d33-109">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="76d33-109">Property name</span></span>        | <span data-ttu-id="76d33-110">Тип</span><span class="sxs-lookup"><span data-stu-id="76d33-110">Type</span></span>     | <span data-ttu-id="76d33-111">Описание</span><span class="sxs-lookup"><span data-stu-id="76d33-111">Description</span></span>
|:---------------------|:---------|:---------------------------------------------------
| <span data-ttu-id="76d33-112">**hostname**</span><span class="sxs-lookup"><span data-stu-id="76d33-112">**hostname**</span></span>         | <span data-ttu-id="76d33-113">строка</span><span class="sxs-lookup"><span data-stu-id="76d33-113">string</span></span>   | <span data-ttu-id="76d33-p101">Имя узла для семейства веб-сайтов. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="76d33-p101">The hostname for the site collection. Read-only.</span></span>
| <span data-ttu-id="76d33-116">**Даталокатионкоде**</span><span class="sxs-lookup"><span data-stu-id="76d33-116">**dataLocationCode**</span></span> | <span data-ttu-id="76d33-117">string</span><span class="sxs-lookup"><span data-stu-id="76d33-117">string</span></span>   | <span data-ttu-id="76d33-118">Код географического региона, в котором располагается это семейство веб-сайтов.</span><span class="sxs-lookup"><span data-stu-id="76d33-118">The geographic region code for where this site collection resides.</span></span> <span data-ttu-id="76d33-119">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="76d33-119">Read-only.</span></span>
| <span data-ttu-id="76d33-120">**root**</span><span class="sxs-lookup"><span data-stu-id="76d33-120">**root**</span></span>             | <span data-ttu-id="76d33-121">[root][]</span><span class="sxs-lookup"><span data-stu-id="76d33-121">[root][]</span></span> | <span data-ttu-id="76d33-122">Если задано, это указывает на то, что это корневое семейство веб-сайтов в SharePoint.</span><span class="sxs-lookup"><span data-stu-id="76d33-122">If present, indicates that this is a root site collection in SharePoint.</span></span> <span data-ttu-id="76d33-123">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="76d33-123">Read-only.</span></span>

[root]: root.md

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

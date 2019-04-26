---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: SiteCollection
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 6dc6b5198e85f43609bb0c878439a1d0d5a22a11
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33343088"
---
# <a name="sitecollection-resource"></a><span data-ttu-id="a54bd-102">Ресурс SiteCollection</span><span class="sxs-lookup"><span data-stu-id="a54bd-102">SiteCollection resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a54bd-103">Ресурс **siteCollection** предоставляет больше сведений о семействе веб-сайтов.</span><span class="sxs-lookup"><span data-stu-id="a54bd-103">The **siteCollection** resource provides more information about a site collection.</span></span>

<span data-ttu-id="a54bd-104">Если для свойства **siteCollection** ресурса [**site**](site.md) задано значение, отличное от NULL, этот сайт является корневым для семейства веб-сайтов.</span><span class="sxs-lookup"><span data-stu-id="a54bd-104">If a [**site**](site.md) resource has a non-null **siteCollection** property, then the site is a root site for a site collection.</span></span>

## <a name="json-representation"></a><span data-ttu-id="a54bd-105">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a54bd-105">JSON representation</span></span>

<span data-ttu-id="a54bd-106">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a54bd-106">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="a54bd-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="a54bd-107">Properties</span></span>

| <span data-ttu-id="a54bd-108">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="a54bd-108">Property name</span></span>        | <span data-ttu-id="a54bd-109">Тип</span><span class="sxs-lookup"><span data-stu-id="a54bd-109">Type</span></span>     | <span data-ttu-id="a54bd-110">Описание</span><span class="sxs-lookup"><span data-stu-id="a54bd-110">Description</span></span>
|:---------------------|:---------|:---------------------------------------------------
| <span data-ttu-id="a54bd-111">**hostname**</span><span class="sxs-lookup"><span data-stu-id="a54bd-111">**hostname**</span></span>         | <span data-ttu-id="a54bd-112">строка</span><span class="sxs-lookup"><span data-stu-id="a54bd-112">string</span></span>   | <span data-ttu-id="a54bd-p101">Имя узла для семейства веб-сайтов. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a54bd-p101">The hostname for the site collection. Read-only.</span></span>
| <span data-ttu-id="a54bd-115">**Даталокатионкоде**</span><span class="sxs-lookup"><span data-stu-id="a54bd-115">**dataLocationCode**</span></span> | <span data-ttu-id="a54bd-116">string</span><span class="sxs-lookup"><span data-stu-id="a54bd-116">string</span></span>   | <span data-ttu-id="a54bd-117">Код географического региона, в котором располагается это семейство веб-сайтов.</span><span class="sxs-lookup"><span data-stu-id="a54bd-117">The geographic region code for where this site collection resides.</span></span> <span data-ttu-id="a54bd-118">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a54bd-118">Read-only.</span></span>
| <span data-ttu-id="a54bd-119">**root**</span><span class="sxs-lookup"><span data-stu-id="a54bd-119">**root**</span></span>             | <span data-ttu-id="a54bd-120">[root][]</span><span class="sxs-lookup"><span data-stu-id="a54bd-120">[root][]</span></span> | <span data-ttu-id="a54bd-121">Если задано, это указывает на то, что это корневое семейство веб-сайтов в SharePoint.</span><span class="sxs-lookup"><span data-stu-id="a54bd-121">If present, indicates that this is a root site collection in SharePoint.</span></span> <span data-ttu-id="a54bd-122">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a54bd-122">Read-only.</span></span>

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

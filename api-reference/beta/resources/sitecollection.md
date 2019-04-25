---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: SiteCollection
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: e9525882b08aaae5500ce23a4b54e95d0b0e0d65
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32583699"
---
# <a name="sitecollection-resource"></a><span data-ttu-id="4e5a3-102">Ресурс SiteCollection</span><span class="sxs-lookup"><span data-stu-id="4e5a3-102">SiteCollection resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4e5a3-103">Ресурс **siteCollection** предоставляет больше сведений о семействе веб-сайтов.</span><span class="sxs-lookup"><span data-stu-id="4e5a3-103">The **siteCollection** resource provides more information about a site collection.</span></span>

<span data-ttu-id="4e5a3-104">Если для свойства **siteCollection** ресурса [**site**](site.md) задано значение, отличное от NULL, этот сайт является корневым для семейства веб-сайтов.</span><span class="sxs-lookup"><span data-stu-id="4e5a3-104">If a [**site**](site.md) resource has a non-null **siteCollection** property, then the site is a root site for a site collection.</span></span>

## <a name="json-representation"></a><span data-ttu-id="4e5a3-105">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4e5a3-105">JSON representation</span></span>

<span data-ttu-id="4e5a3-106">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4e5a3-106">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="4e5a3-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="4e5a3-107">Properties</span></span>

| <span data-ttu-id="4e5a3-108">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="4e5a3-108">Property name</span></span>        | <span data-ttu-id="4e5a3-109">Тип</span><span class="sxs-lookup"><span data-stu-id="4e5a3-109">Type</span></span>     | <span data-ttu-id="4e5a3-110">Описание</span><span class="sxs-lookup"><span data-stu-id="4e5a3-110">Description</span></span>
|:---------------------|:---------|:---------------------------------------------------
| <span data-ttu-id="4e5a3-111">**hostname**</span><span class="sxs-lookup"><span data-stu-id="4e5a3-111">**hostname**</span></span>         | <span data-ttu-id="4e5a3-112">строка</span><span class="sxs-lookup"><span data-stu-id="4e5a3-112">string</span></span>   | <span data-ttu-id="4e5a3-p101">Имя узла для семейства веб-сайтов. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4e5a3-p101">The hostname for the site collection. Read-only.</span></span>
| <span data-ttu-id="4e5a3-115">**Даталокатионкоде**</span><span class="sxs-lookup"><span data-stu-id="4e5a3-115">**dataLocationCode**</span></span> | <span data-ttu-id="4e5a3-116">string</span><span class="sxs-lookup"><span data-stu-id="4e5a3-116">string</span></span>   | <span data-ttu-id="4e5a3-117">Код географического региона, в котором располагается это семейство веб-сайтов.</span><span class="sxs-lookup"><span data-stu-id="4e5a3-117">The geographic region code for where this site collection resides.</span></span> <span data-ttu-id="4e5a3-118">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4e5a3-118">Read-only.</span></span>
| <span data-ttu-id="4e5a3-119">**root**</span><span class="sxs-lookup"><span data-stu-id="4e5a3-119">**root**</span></span>             | <span data-ttu-id="4e5a3-120">[root][]</span><span class="sxs-lookup"><span data-stu-id="4e5a3-120">[root][]</span></span> | <span data-ttu-id="4e5a3-121">Если задано, это указывает на то, что это корневое семейство веб-сайтов в SharePoint.</span><span class="sxs-lookup"><span data-stu-id="4e5a3-121">If present, indicates that this is a root site collection in SharePoint.</span></span> <span data-ttu-id="4e5a3-122">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4e5a3-122">Read-only.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/sitecollection.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

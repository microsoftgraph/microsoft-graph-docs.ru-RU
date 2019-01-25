---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: SiteCollection
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 865fc21691eb37811300caaf675b123d1a544ac0
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29528132"
---
# <a name="sitecollection-resource"></a><span data-ttu-id="4ef51-102">Ресурс SiteCollection</span><span class="sxs-lookup"><span data-stu-id="4ef51-102">SiteCollection resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4ef51-103">Ресурс **siteCollection** предоставляет больше сведений о семействе веб-сайтов.</span><span class="sxs-lookup"><span data-stu-id="4ef51-103">The **siteCollection** resource provides more information about a site collection.</span></span>

<span data-ttu-id="4ef51-104">Если для свойства **siteCollection** ресурса [**site**](site.md) задано значение, отличное от NULL, этот сайт является корневым для семейства веб-сайтов.</span><span class="sxs-lookup"><span data-stu-id="4ef51-104">If a [**site**](site.md) resource has a non-null **siteCollection** property, then the site is a root site for a site collection.</span></span>

## <a name="json-representation"></a><span data-ttu-id="4ef51-105">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="4ef51-105">JSON representation</span></span>

<span data-ttu-id="4ef51-106">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4ef51-106">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="4ef51-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="4ef51-107">Properties</span></span>

| <span data-ttu-id="4ef51-108">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="4ef51-108">Property name</span></span>        | <span data-ttu-id="4ef51-109">Тип</span><span class="sxs-lookup"><span data-stu-id="4ef51-109">Type</span></span>     | <span data-ttu-id="4ef51-110">Описание</span><span class="sxs-lookup"><span data-stu-id="4ef51-110">Description</span></span>
|:---------------------|:---------|:---------------------------------------------------
| <span data-ttu-id="4ef51-111">**hostname**</span><span class="sxs-lookup"><span data-stu-id="4ef51-111">**hostname**</span></span>         | <span data-ttu-id="4ef51-112">строка</span><span class="sxs-lookup"><span data-stu-id="4ef51-112">string</span></span>   | <span data-ttu-id="4ef51-p101">Имя узла для семейства веб-сайтов. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4ef51-p101">The hostname for the site collection. Read-only.</span></span>
| <span data-ttu-id="4ef51-115">**dataLocationCode**</span><span class="sxs-lookup"><span data-stu-id="4ef51-115">**dataLocationCode**</span></span> | <span data-ttu-id="4ef51-116">string</span><span class="sxs-lookup"><span data-stu-id="4ef51-116">string</span></span>   | <span data-ttu-id="4ef51-117">Код географического региона для размещения семейства веб-сайтов.</span><span class="sxs-lookup"><span data-stu-id="4ef51-117">The geographic region code for where this site collection resides.</span></span> <span data-ttu-id="4ef51-118">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4ef51-118">Read-only.</span></span>
| <span data-ttu-id="4ef51-119">**root**</span><span class="sxs-lookup"><span data-stu-id="4ef51-119">**root**</span></span>             | <span data-ttu-id="4ef51-120">[root][]</span><span class="sxs-lookup"><span data-stu-id="4ef51-120">[root][]</span></span> | <span data-ttu-id="4ef51-121">Если этот параметр указан, указывает, что это корневого семейства сайтов в SharePoint.</span><span class="sxs-lookup"><span data-stu-id="4ef51-121">If present, indicates that this is a root site collection in SharePoint.</span></span> <span data-ttu-id="4ef51-122">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4ef51-122">Read-only.</span></span>

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

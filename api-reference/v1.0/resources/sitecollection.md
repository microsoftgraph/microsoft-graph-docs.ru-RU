---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: SiteCollection
localization_priority: Normal
ms.prod: sharepoint
description: Ресурс siteCollection предоставляет больше сведений о семействе веб-сайтов.
doc_type: resourcePageType
ms.openlocfilehash: 27a534f2f9afe99a1a5abb1aee91b1b53b29566d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36034162"
---
# <a name="sitecollection-resource"></a><span data-ttu-id="d1c9a-103">Ресурс SiteCollection</span><span class="sxs-lookup"><span data-stu-id="d1c9a-103">SiteCollection resource</span></span>

<span data-ttu-id="d1c9a-104">Ресурс **siteCollection** предоставляет больше сведений о семействе веб-сайтов.</span><span class="sxs-lookup"><span data-stu-id="d1c9a-104">The **siteCollection** resource provides more information about a site collection.</span></span>

<span data-ttu-id="d1c9a-105">Если для свойства **siteCollection** ресурса [**site**](site.md) задано значение, отличное от NULL, этот сайт является корневым для семейства веб-сайтов.</span><span class="sxs-lookup"><span data-stu-id="d1c9a-105">If a [**site**](site.md) resource has a non-null **siteCollection** property, then the site is a root site for a site collection.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d1c9a-106">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d1c9a-106">JSON representation</span></span>

<span data-ttu-id="d1c9a-107">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d1c9a-107">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  ],
  "@odata.type": "microsoft.graph.siteCollection"
}-->

```json
{
  "hostname": "contoso.sharepoint.com",
  "root": { "@odata.type": "microsoft.graph.root" }
}
```

## <a name="properties"></a><span data-ttu-id="d1c9a-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="d1c9a-108">Properties</span></span>

| <span data-ttu-id="d1c9a-109">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="d1c9a-109">Property name</span></span>        | <span data-ttu-id="d1c9a-110">Тип</span><span class="sxs-lookup"><span data-stu-id="d1c9a-110">Type</span></span>     | <span data-ttu-id="d1c9a-111">Описание</span><span class="sxs-lookup"><span data-stu-id="d1c9a-111">Description</span></span>
|:---------------------|:---------|:---------------------------------------------------
| <span data-ttu-id="d1c9a-112">**hostname**</span><span class="sxs-lookup"><span data-stu-id="d1c9a-112">**hostname**</span></span>         | <span data-ttu-id="d1c9a-113">строка</span><span class="sxs-lookup"><span data-stu-id="d1c9a-113">string</span></span>   | <span data-ttu-id="d1c9a-p101">Имя узла для семейства веб-сайтов. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d1c9a-p101">The hostname for the site collection. Read-only.</span></span>
| <span data-ttu-id="d1c9a-116">**root**</span><span class="sxs-lookup"><span data-stu-id="d1c9a-116">**root**</span></span>             | <span data-ttu-id="d1c9a-117">[root][]</span><span class="sxs-lookup"><span data-stu-id="d1c9a-117">[root][]</span></span> | <span data-ttu-id="d1c9a-118">Если задано, это указывает на то, что это корневое семейство веб-сайтов в SharePoint.</span><span class="sxs-lookup"><span data-stu-id="d1c9a-118">If present, indicates that this is a root site collection in SharePoint.</span></span> <span data-ttu-id="d1c9a-119">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d1c9a-119">Read-only.</span></span>

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

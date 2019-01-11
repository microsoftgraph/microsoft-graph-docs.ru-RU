---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: SiteCollection
localization_priority: Normal
ms.openlocfilehash: c366c39a71e952521425d9eb08fab7c77a9a3415
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27809984"
---
# <a name="sitecollection-resource"></a><span data-ttu-id="dbf89-102">Ресурс SiteCollection</span><span class="sxs-lookup"><span data-stu-id="dbf89-102">SiteCollection resource</span></span>

<span data-ttu-id="dbf89-103">Ресурс **siteCollection** предоставляет больше сведений о семействе веб-сайтов.</span><span class="sxs-lookup"><span data-stu-id="dbf89-103">The **siteCollection** resource provides more information about a site collection.</span></span>

<span data-ttu-id="dbf89-104">Если для свойства **siteCollection** ресурса [**site**](site.md) задано значение, отличное от NULL, этот сайт является корневым для семейства веб-сайтов.</span><span class="sxs-lookup"><span data-stu-id="dbf89-104">If a [**site**](site.md) resource has a non-null **siteCollection** property, then the site is a root site for a site collection.</span></span>

## <a name="json-representation"></a><span data-ttu-id="dbf89-105">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="dbf89-105">JSON representation</span></span>

<span data-ttu-id="dbf89-106">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="dbf89-106">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="dbf89-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="dbf89-107">Properties</span></span>

| <span data-ttu-id="dbf89-108">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="dbf89-108">Property name</span></span>        | <span data-ttu-id="dbf89-109">Тип</span><span class="sxs-lookup"><span data-stu-id="dbf89-109">Type</span></span>     | <span data-ttu-id="dbf89-110">Описание</span><span class="sxs-lookup"><span data-stu-id="dbf89-110">Description</span></span>
|:---------------------|:---------|:---------------------------------------------------
| <span data-ttu-id="dbf89-111">**hostname**</span><span class="sxs-lookup"><span data-stu-id="dbf89-111">**hostname**</span></span>         | <span data-ttu-id="dbf89-112">строка</span><span class="sxs-lookup"><span data-stu-id="dbf89-112">string</span></span>   | <span data-ttu-id="dbf89-p101">Имя узла для семейства веб-сайтов. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="dbf89-p101">The hostname for the site collection. Read-only.</span></span>
| <span data-ttu-id="dbf89-115">**root**</span><span class="sxs-lookup"><span data-stu-id="dbf89-115">**root**</span></span>             | <span data-ttu-id="dbf89-116">[root][]</span><span class="sxs-lookup"><span data-stu-id="dbf89-116">[root][]</span></span> | <span data-ttu-id="dbf89-117">Если этот параметр указан, указывает, что это корневого семейства сайтов в SharePoint.</span><span class="sxs-lookup"><span data-stu-id="dbf89-117">If present, indicates that this is a root site collection in SharePoint.</span></span> <span data-ttu-id="dbf89-118">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="dbf89-118">Read-only.</span></span>

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

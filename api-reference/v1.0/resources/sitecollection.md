---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: SiteCollection
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 006f239acdecb2fb93ecf1d70e25a42b056b9283
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32552785"
---
# <a name="sitecollection-resource"></a><span data-ttu-id="27c48-102">Ресурс SiteCollection</span><span class="sxs-lookup"><span data-stu-id="27c48-102">SiteCollection resource</span></span>

<span data-ttu-id="27c48-103">Ресурс **siteCollection** предоставляет больше сведений о семействе веб-сайтов.</span><span class="sxs-lookup"><span data-stu-id="27c48-103">The **siteCollection** resource provides more information about a site collection.</span></span>

<span data-ttu-id="27c48-104">Если для свойства **siteCollection** ресурса [**site**](site.md) задано значение, отличное от NULL, этот сайт является корневым для семейства веб-сайтов.</span><span class="sxs-lookup"><span data-stu-id="27c48-104">If a [**site**](site.md) resource has a non-null **siteCollection** property, then the site is a root site for a site collection.</span></span>

## <a name="json-representation"></a><span data-ttu-id="27c48-105">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="27c48-105">JSON representation</span></span>

<span data-ttu-id="27c48-106">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="27c48-106">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="27c48-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="27c48-107">Properties</span></span>

| <span data-ttu-id="27c48-108">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="27c48-108">Property name</span></span>        | <span data-ttu-id="27c48-109">Тип</span><span class="sxs-lookup"><span data-stu-id="27c48-109">Type</span></span>     | <span data-ttu-id="27c48-110">Описание</span><span class="sxs-lookup"><span data-stu-id="27c48-110">Description</span></span>
|:---------------------|:---------|:---------------------------------------------------
| <span data-ttu-id="27c48-111">**hostname**</span><span class="sxs-lookup"><span data-stu-id="27c48-111">**hostname**</span></span>         | <span data-ttu-id="27c48-112">строка</span><span class="sxs-lookup"><span data-stu-id="27c48-112">string</span></span>   | <span data-ttu-id="27c48-p101">Имя узла для семейства веб-сайтов. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="27c48-p101">The hostname for the site collection. Read-only.</span></span>
| <span data-ttu-id="27c48-115">**root**</span><span class="sxs-lookup"><span data-stu-id="27c48-115">**root**</span></span>             | <span data-ttu-id="27c48-116">[root][]</span><span class="sxs-lookup"><span data-stu-id="27c48-116">[root][]</span></span> | <span data-ttu-id="27c48-117">Если задано, это указывает на то, что это корневое семейство веб-сайтов в SharePoint.</span><span class="sxs-lookup"><span data-stu-id="27c48-117">If present, indicates that this is a root site collection in SharePoint.</span></span> <span data-ttu-id="27c48-118">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="27c48-118">Read-only.</span></span>

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

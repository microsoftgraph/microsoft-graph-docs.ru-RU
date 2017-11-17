---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: SiteCollection
ms.openlocfilehash: 6b36f3a0c2d958081f1b5663231a541f2e8a000f
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/28/2017
---
# <a name="sitecollection-resource"></a><span data-ttu-id="544c3-102">Ресурс SiteCollection</span><span class="sxs-lookup"><span data-stu-id="544c3-102">SiteCollection resource</span></span>

<span data-ttu-id="544c3-103">Ресурс **siteCollection** предоставляет больше сведений о семействе веб-сайтов.</span><span class="sxs-lookup"><span data-stu-id="544c3-103">The **siteCollection** resource provides more information about a site collection.</span></span>

<span data-ttu-id="544c3-104">Если для свойства **siteCollection** ресурса [**site**](site.md) задано значение, отличное от NULL, этот сайт является корневым для семейства веб-сайтов.</span><span class="sxs-lookup"><span data-stu-id="544c3-104">If a [**site**](site.md) resource has a non-null **siteCollection** property, then the site is a root site for a site collection.</span></span>

## <a name="json-representation"></a><span data-ttu-id="544c3-105">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="544c3-105">JSON representation</span></span>

<span data-ttu-id="544c3-106">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="544c3-106">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  ],
  "@odata.type": "microsoft.graph.siteCollection"
}-->

```json
{
  "hostname": "contoso.sharepoint.com"
}
```

## <a name="properties"></a><span data-ttu-id="544c3-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="544c3-107">Properties</span></span>

| <span data-ttu-id="544c3-108">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="544c3-108">Property name</span></span> | <span data-ttu-id="544c3-109">Тип</span><span class="sxs-lookup"><span data-stu-id="544c3-109">Type</span></span>    | <span data-ttu-id="544c3-110">Описание</span><span class="sxs-lookup"><span data-stu-id="544c3-110">Description</span></span>                                                                                                                  |
|:--------------|:--------|:---------------------------------------------------
| <span data-ttu-id="544c3-111">**hostname**</span><span class="sxs-lookup"><span data-stu-id="544c3-111">**hostname**</span></span>  | <span data-ttu-id="544c3-112">строка</span><span class="sxs-lookup"><span data-stu-id="544c3-112">string</span></span>  | <span data-ttu-id="544c3-p101">Имя узла для семейства веб-сайтов. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="544c3-p101">The hostname for the site collection. Read-only.</span></span>


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Facets/SiteCollection"
}-->

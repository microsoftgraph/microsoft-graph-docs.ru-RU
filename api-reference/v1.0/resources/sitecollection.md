---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: SiteCollection
ms.openlocfilehash: 84de2a8aa6796051b3b11ebec0d0f8f5934ea1fc
ms.sourcegitcommit: abf4b739257e3ffd9d045f783ec595d846172590
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/21/2018
ms.locfileid: "19069345"
---
# <a name="sitecollection-resource"></a><span data-ttu-id="d0352-102">Ресурс SiteCollection</span><span class="sxs-lookup"><span data-stu-id="d0352-102">SiteCollection resource</span></span>

<span data-ttu-id="d0352-103">Ресурс **siteCollection** предоставляет больше сведений о семействе веб-сайтов.</span><span class="sxs-lookup"><span data-stu-id="d0352-103">The **siteCollection** resource provides more information about a site collection.</span></span>

<span data-ttu-id="d0352-104">Если для свойства **siteCollection** ресурса [**site**](site.md) задано значение, отличное от NULL, этот сайт является корневым для семейства веб-сайтов.</span><span class="sxs-lookup"><span data-stu-id="d0352-104">If a [**site**](site.md) resource has a non-null **siteCollection** property, then the site is a root site for a site collection.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d0352-105">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="d0352-105">JSON representation</span></span>

<span data-ttu-id="d0352-106">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d0352-106">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="d0352-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="d0352-107">Properties</span></span>

| <span data-ttu-id="d0352-108">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="d0352-108">Property name</span></span>        | <span data-ttu-id="d0352-109">Тип</span><span class="sxs-lookup"><span data-stu-id="d0352-109">Type</span></span>     | <span data-ttu-id="d0352-110">Описание</span><span class="sxs-lookup"><span data-stu-id="d0352-110">Description</span></span>
|:---------------------|:---------|:---------------------------------------------------
| <span data-ttu-id="d0352-111">**hostname**</span><span class="sxs-lookup"><span data-stu-id="d0352-111">**hostname**</span></span>         | <span data-ttu-id="d0352-112">строка</span><span class="sxs-lookup"><span data-stu-id="d0352-112">string</span></span>   | <span data-ttu-id="d0352-p101">Имя узла для семейства веб-сайтов. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d0352-p101">The hostname for the site collection. Read-only.</span></span>
| <span data-ttu-id="d0352-115">**root**</span><span class="sxs-lookup"><span data-stu-id="d0352-115">**root**</span></span>             | <span data-ttu-id="d0352-116">[root][]</span><span class="sxs-lookup"><span data-stu-id="d0352-116">[root][]</span></span> | <span data-ttu-id="d0352-117">Если это свойство присутствует, оно указывает на то, что это корневое семейство сайтов в SharePoint.</span><span class="sxs-lookup"><span data-stu-id="d0352-117">If present, indicates that this is the root site in the site collection. Read-only.</span></span> <span data-ttu-id="d0352-118">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d0352-118">Read-only.</span></span>

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

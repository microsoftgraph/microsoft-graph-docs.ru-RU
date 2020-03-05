---
author: JeremyKelley
description: Ресурс siteCollection предоставляет больше сведений о семействе веб-сайтов.
ms.date: 09/10/2017
title: SiteCollection
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 240f0b804e8b87c0dc3aae1e03a46be3527bed22
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520543"
---
# <a name="sitecollection-resource"></a><span data-ttu-id="32180-103">Ресурс SiteCollection</span><span class="sxs-lookup"><span data-stu-id="32180-103">SiteCollection resource</span></span>

<span data-ttu-id="32180-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="32180-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="32180-105">Ресурс **siteCollection** предоставляет больше сведений о семействе веб-сайтов.</span><span class="sxs-lookup"><span data-stu-id="32180-105">The **siteCollection** resource provides more information about a site collection.</span></span>

<span data-ttu-id="32180-106">Если для свойства **siteCollection** ресурса [**site**](site.md) задано значение, отличное от NULL, этот сайт является корневым для семейства веб-сайтов.</span><span class="sxs-lookup"><span data-stu-id="32180-106">If a [**site**](site.md) resource has a non-null **siteCollection** property, then the site is a root site for a site collection.</span></span>

## <a name="json-representation"></a><span data-ttu-id="32180-107">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="32180-107">JSON representation</span></span>

<span data-ttu-id="32180-108">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="32180-108">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="32180-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="32180-109">Properties</span></span>

| <span data-ttu-id="32180-110">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="32180-110">Property name</span></span>        | <span data-ttu-id="32180-111">Тип</span><span class="sxs-lookup"><span data-stu-id="32180-111">Type</span></span>     | <span data-ttu-id="32180-112">Описание</span><span class="sxs-lookup"><span data-stu-id="32180-112">Description</span></span>
|:---------------------|:---------|:---------------------------------------------------
| <span data-ttu-id="32180-113">**hostname**</span><span class="sxs-lookup"><span data-stu-id="32180-113">**hostname**</span></span>         | <span data-ttu-id="32180-114">строка</span><span class="sxs-lookup"><span data-stu-id="32180-114">string</span></span>   | <span data-ttu-id="32180-p101">Имя узла для семейства веб-сайтов. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="32180-p101">The hostname for the site collection. Read-only.</span></span>
| <span data-ttu-id="32180-117">**даталокатионкоде**</span><span class="sxs-lookup"><span data-stu-id="32180-117">**dataLocationCode**</span></span> | <span data-ttu-id="32180-118">строка</span><span class="sxs-lookup"><span data-stu-id="32180-118">string</span></span>   | <span data-ttu-id="32180-119">Код географического региона, в котором располагается это семейство веб-сайтов.</span><span class="sxs-lookup"><span data-stu-id="32180-119">The geographic region code for where this site collection resides.</span></span> <span data-ttu-id="32180-120">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="32180-120">Read-only.</span></span>
| <span data-ttu-id="32180-121">**root**</span><span class="sxs-lookup"><span data-stu-id="32180-121">**root**</span></span>             | <span data-ttu-id="32180-122">[root][]</span><span class="sxs-lookup"><span data-stu-id="32180-122">[root][]</span></span> | <span data-ttu-id="32180-123">Если задано, это указывает на то, что это корневое семейство веб-сайтов в SharePoint.</span><span class="sxs-lookup"><span data-stu-id="32180-123">If present, indicates that this is a root site collection in SharePoint.</span></span> <span data-ttu-id="32180-124">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="32180-124">Read-only.</span></span>

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

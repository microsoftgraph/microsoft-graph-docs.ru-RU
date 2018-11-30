---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: SiteCollection
ms.openlocfilehash: d54246002c158270ae23cf81cdc93673f40bd78c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27078551"
---
# <a name="sitecollection-resource"></a><span data-ttu-id="7f582-102">Ресурс SiteCollection</span><span class="sxs-lookup"><span data-stu-id="7f582-102">SiteCollection resource</span></span>

> <span data-ttu-id="7f582-103">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="7f582-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7f582-104">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7f582-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7f582-105">Ресурс **siteCollection** предоставляет больше сведений о семействе веб-сайтов.</span><span class="sxs-lookup"><span data-stu-id="7f582-105">The **siteCollection** resource provides more information about a site collection.</span></span>

<span data-ttu-id="7f582-106">Если для свойства **siteCollection** ресурса [**site**](site.md) задано значение, отличное от NULL, этот сайт является корневым для семейства веб-сайтов.</span><span class="sxs-lookup"><span data-stu-id="7f582-106">If a [**site**](site.md) resource has a non-null **siteCollection** property, then the site is a root site for a site collection.</span></span>

## <a name="json-representation"></a><span data-ttu-id="7f582-107">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="7f582-107">JSON representation</span></span>

<span data-ttu-id="7f582-108">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7f582-108">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="7f582-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="7f582-109">Properties</span></span>

| <span data-ttu-id="7f582-110">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="7f582-110">Property name</span></span>        | <span data-ttu-id="7f582-111">Тип</span><span class="sxs-lookup"><span data-stu-id="7f582-111">Type</span></span>     | <span data-ttu-id="7f582-112">Описание</span><span class="sxs-lookup"><span data-stu-id="7f582-112">Description</span></span>
|:---------------------|:---------|:---------------------------------------------------
| <span data-ttu-id="7f582-113">**hostname**</span><span class="sxs-lookup"><span data-stu-id="7f582-113">**hostname**</span></span>         | <span data-ttu-id="7f582-114">строка</span><span class="sxs-lookup"><span data-stu-id="7f582-114">string</span></span>   | <span data-ttu-id="7f582-p102">Имя узла для семейства веб-сайтов. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7f582-p102">The hostname for the site collection. Read-only.</span></span>
| <span data-ttu-id="7f582-117">**dataLocationCode**</span><span class="sxs-lookup"><span data-stu-id="7f582-117">**dataLocationCode**</span></span> | <span data-ttu-id="7f582-118">string</span><span class="sxs-lookup"><span data-stu-id="7f582-118">string</span></span>   | <span data-ttu-id="7f582-119">Код географического региона для размещения семейства веб-сайтов.</span><span class="sxs-lookup"><span data-stu-id="7f582-119">The geographic region code for where this site collection resides.</span></span> <span data-ttu-id="7f582-120">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7f582-120">Read-only.</span></span>
| <span data-ttu-id="7f582-121">**root**</span><span class="sxs-lookup"><span data-stu-id="7f582-121">**root**</span></span>             | <span data-ttu-id="7f582-122">[root][]</span><span class="sxs-lookup"><span data-stu-id="7f582-122">[root][]</span></span> | <span data-ttu-id="7f582-123">Если этот параметр указан, указывает, что это корневого семейства сайтов в SharePoint.</span><span class="sxs-lookup"><span data-stu-id="7f582-123">If present, indicates that this is a root site collection in SharePoint.</span></span> <span data-ttu-id="7f582-124">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7f582-124">Read-only.</span></span>

[root]: root.md

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

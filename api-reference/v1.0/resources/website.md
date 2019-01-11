---
title: тип ресурса website
description: Представляет веб-сайт.
localization_priority: Normal
ms.openlocfilehash: 1ffbee8a67527aac97bb4f60b7f8b1637ba1ebe5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27851368"
---
# <a name="website-resource-type"></a><span data-ttu-id="2503e-103">тип ресурса website</span><span class="sxs-lookup"><span data-stu-id="2503e-103">website resource type</span></span>

<span data-ttu-id="2503e-104">Представляет веб-сайт.</span><span class="sxs-lookup"><span data-stu-id="2503e-104">Represents a website.</span></span>


## <a name="properties"></a><span data-ttu-id="2503e-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="2503e-105">Properties</span></span>
| <span data-ttu-id="2503e-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="2503e-106">Property</span></span>     | <span data-ttu-id="2503e-107">Тип</span><span class="sxs-lookup"><span data-stu-id="2503e-107">Type</span></span>   |<span data-ttu-id="2503e-108">Описание</span><span class="sxs-lookup"><span data-stu-id="2503e-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2503e-109">type</span><span class="sxs-lookup"><span data-stu-id="2503e-109">type</span></span>|<span data-ttu-id="2503e-110">websiteType</span><span class="sxs-lookup"><span data-stu-id="2503e-110">websiteType</span></span>| <span data-ttu-id="2503e-111">Возможные значения: `other`, `home`, `work`, `blog`, `profile`.</span><span class="sxs-lookup"><span data-stu-id="2503e-111">The possible values are: `other`, `home`, `work`, `blog`, `profile`.</span></span>|
|<span data-ttu-id="2503e-112">address</span><span class="sxs-lookup"><span data-stu-id="2503e-112">address</span></span>|<span data-ttu-id="2503e-113">string</span><span class="sxs-lookup"><span data-stu-id="2503e-113">string</span></span>|<span data-ttu-id="2503e-114">URL-адрес веб-сайта.</span><span class="sxs-lookup"><span data-stu-id="2503e-114">The URL of the website.</span></span>|
|<span data-ttu-id="2503e-115">displayName</span><span class="sxs-lookup"><span data-stu-id="2503e-115">displayName</span></span>|<span data-ttu-id="2503e-116">строка</span><span class="sxs-lookup"><span data-stu-id="2503e-116">string</span></span>|<span data-ttu-id="2503e-117">Отображаемое имя веб-сайта.</span><span class="sxs-lookup"><span data-stu-id="2503e-117">The display name of the web site.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2503e-118">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="2503e-118">JSON representation</span></span>

<span data-ttu-id="2503e-119">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2503e-119">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.website"
}-->

```json
{
  "type": "String",
  "address": "string",
  "displayName": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "webSite resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

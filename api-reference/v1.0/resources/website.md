---
title: Тип ресурса веб-сайта
description: Представляет веб-сайт.
localization_priority: Normal
author: AAmatino
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: ec3642ea513ae054e22537c86426df365cd41ba9
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46807670"
---
# <a name="website-resource-type"></a><span data-ttu-id="c2dc2-103">Тип ресурса веб-сайта</span><span class="sxs-lookup"><span data-stu-id="c2dc2-103">website resource type</span></span>

<span data-ttu-id="c2dc2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c2dc2-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c2dc2-105">Представляет веб-сайт.</span><span class="sxs-lookup"><span data-stu-id="c2dc2-105">Represents a website.</span></span>


## <a name="properties"></a><span data-ttu-id="c2dc2-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="c2dc2-106">Properties</span></span>
| <span data-ttu-id="c2dc2-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="c2dc2-107">Property</span></span>     | <span data-ttu-id="c2dc2-108">Тип</span><span class="sxs-lookup"><span data-stu-id="c2dc2-108">Type</span></span>   |<span data-ttu-id="c2dc2-109">Описание</span><span class="sxs-lookup"><span data-stu-id="c2dc2-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c2dc2-110">type</span><span class="sxs-lookup"><span data-stu-id="c2dc2-110">type</span></span>|<span data-ttu-id="c2dc2-111">websiteType</span><span class="sxs-lookup"><span data-stu-id="c2dc2-111">websiteType</span></span>| <span data-ttu-id="c2dc2-112">Допустимые значения: `other`, `home`, `work`, `blog`, `profile`.</span><span class="sxs-lookup"><span data-stu-id="c2dc2-112">The possible values are: `other`, `home`, `work`, `blog`, `profile`.</span></span>|
|<span data-ttu-id="c2dc2-113">address</span><span class="sxs-lookup"><span data-stu-id="c2dc2-113">address</span></span>|<span data-ttu-id="c2dc2-114">string</span><span class="sxs-lookup"><span data-stu-id="c2dc2-114">string</span></span>|<span data-ttu-id="c2dc2-115">URL-адрес веб-сайта.</span><span class="sxs-lookup"><span data-stu-id="c2dc2-115">The URL of the website.</span></span>|
|<span data-ttu-id="c2dc2-116">displayName</span><span class="sxs-lookup"><span data-stu-id="c2dc2-116">displayName</span></span>|<span data-ttu-id="c2dc2-117">string</span><span class="sxs-lookup"><span data-stu-id="c2dc2-117">string</span></span>|<span data-ttu-id="c2dc2-118">Отображаемое имя веб-сайта.</span><span class="sxs-lookup"><span data-stu-id="c2dc2-118">The display name of the web site.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c2dc2-119">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="c2dc2-119">JSON representation</span></span>

<span data-ttu-id="c2dc2-120">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c2dc2-120">The following is a JSON representation of the resource.</span></span>

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

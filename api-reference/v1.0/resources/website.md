---
title: Тип ресурса веб-сайта
description: Представляет веб-сайт.
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 6a59022426392bbf3a94c6fb82b941131db3c1d8
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36033385"
---
# <a name="website-resource-type"></a><span data-ttu-id="42683-103">Тип ресурса веб-сайта</span><span class="sxs-lookup"><span data-stu-id="42683-103">website resource type</span></span>

<span data-ttu-id="42683-104">Представляет веб-сайт.</span><span class="sxs-lookup"><span data-stu-id="42683-104">Represents a website.</span></span>


## <a name="properties"></a><span data-ttu-id="42683-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="42683-105">Properties</span></span>
| <span data-ttu-id="42683-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="42683-106">Property</span></span>     | <span data-ttu-id="42683-107">Тип</span><span class="sxs-lookup"><span data-stu-id="42683-107">Type</span></span>   |<span data-ttu-id="42683-108">Описание</span><span class="sxs-lookup"><span data-stu-id="42683-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="42683-109">type</span><span class="sxs-lookup"><span data-stu-id="42683-109">type</span></span>|<span data-ttu-id="42683-110">websiteType</span><span class="sxs-lookup"><span data-stu-id="42683-110">websiteType</span></span>| <span data-ttu-id="42683-111">Допустимые значения: `other`, `home`, `work`, `blog`, `profile`.</span><span class="sxs-lookup"><span data-stu-id="42683-111">The possible values are: `other`, `home`, `work`, `blog`, `profile`.</span></span>|
|<span data-ttu-id="42683-112">address</span><span class="sxs-lookup"><span data-stu-id="42683-112">address</span></span>|<span data-ttu-id="42683-113">string</span><span class="sxs-lookup"><span data-stu-id="42683-113">string</span></span>|<span data-ttu-id="42683-114">URL-адрес веб-сайта.</span><span class="sxs-lookup"><span data-stu-id="42683-114">The URL of the website.</span></span>|
|<span data-ttu-id="42683-115">displayName</span><span class="sxs-lookup"><span data-stu-id="42683-115">displayName</span></span>|<span data-ttu-id="42683-116">string</span><span class="sxs-lookup"><span data-stu-id="42683-116">string</span></span>|<span data-ttu-id="42683-117">Отображаемое имя веб-сайта.</span><span class="sxs-lookup"><span data-stu-id="42683-117">The display name of the web site.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="42683-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="42683-118">JSON representation</span></span>

<span data-ttu-id="42683-119">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="42683-119">The following is a JSON representation of the resource.</span></span>

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

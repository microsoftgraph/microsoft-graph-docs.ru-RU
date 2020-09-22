---
title: Тип ресурса веб-сайта
description: Представляет веб-сайт.
localization_priority: Normal
author: AAmatino
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: fbdb96a9a19a9edef98d73916dcbd01dd6ba9e66
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48015241"
---
# <a name="website-resource-type"></a><span data-ttu-id="48954-103">Тип ресурса веб-сайта</span><span class="sxs-lookup"><span data-stu-id="48954-103">website resource type</span></span>

<span data-ttu-id="48954-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="48954-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="48954-105">Представляет веб-сайт.</span><span class="sxs-lookup"><span data-stu-id="48954-105">Represents a website.</span></span>


## <a name="properties"></a><span data-ttu-id="48954-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="48954-106">Properties</span></span>
| <span data-ttu-id="48954-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="48954-107">Property</span></span>     | <span data-ttu-id="48954-108">Тип</span><span class="sxs-lookup"><span data-stu-id="48954-108">Type</span></span>   |<span data-ttu-id="48954-109">Описание</span><span class="sxs-lookup"><span data-stu-id="48954-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="48954-110">type</span><span class="sxs-lookup"><span data-stu-id="48954-110">type</span></span>|<span data-ttu-id="48954-111">websiteType</span><span class="sxs-lookup"><span data-stu-id="48954-111">websiteType</span></span>| <span data-ttu-id="48954-112">Допустимые значения: `other`, `home`, `work`, `blog`, `profile`.</span><span class="sxs-lookup"><span data-stu-id="48954-112">The possible values are: `other`, `home`, `work`, `blog`, `profile`.</span></span>|
|<span data-ttu-id="48954-113">address</span><span class="sxs-lookup"><span data-stu-id="48954-113">address</span></span>|<span data-ttu-id="48954-114">string</span><span class="sxs-lookup"><span data-stu-id="48954-114">string</span></span>|<span data-ttu-id="48954-115">URL-адрес веб-сайта.</span><span class="sxs-lookup"><span data-stu-id="48954-115">The URL of the website.</span></span>|
|<span data-ttu-id="48954-116">displayName</span><span class="sxs-lookup"><span data-stu-id="48954-116">displayName</span></span>|<span data-ttu-id="48954-117">string</span><span class="sxs-lookup"><span data-stu-id="48954-117">string</span></span>|<span data-ttu-id="48954-118">Отображаемое имя веб-сайта.</span><span class="sxs-lookup"><span data-stu-id="48954-118">The display name of the web site.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="48954-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="48954-119">JSON representation</span></span>

<span data-ttu-id="48954-120">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="48954-120">The following is a JSON representation of the resource.</span></span>

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


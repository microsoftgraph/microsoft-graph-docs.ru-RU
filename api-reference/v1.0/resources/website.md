---
title: Тип ресурса веб-сайта
description: Представляет веб-сайт.
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: f6d630a2cde87415cb8229f7d320cb32bc6260d9
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42446739"
---
# <a name="website-resource-type"></a><span data-ttu-id="9be16-103">Тип ресурса веб-сайта</span><span class="sxs-lookup"><span data-stu-id="9be16-103">website resource type</span></span>

<span data-ttu-id="9be16-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="9be16-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9be16-105">Представляет веб-сайт.</span><span class="sxs-lookup"><span data-stu-id="9be16-105">Represents a website.</span></span>


## <a name="properties"></a><span data-ttu-id="9be16-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="9be16-106">Properties</span></span>
| <span data-ttu-id="9be16-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="9be16-107">Property</span></span>     | <span data-ttu-id="9be16-108">Тип</span><span class="sxs-lookup"><span data-stu-id="9be16-108">Type</span></span>   |<span data-ttu-id="9be16-109">Описание</span><span class="sxs-lookup"><span data-stu-id="9be16-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9be16-110">type</span><span class="sxs-lookup"><span data-stu-id="9be16-110">type</span></span>|<span data-ttu-id="9be16-111">websiteType</span><span class="sxs-lookup"><span data-stu-id="9be16-111">websiteType</span></span>| <span data-ttu-id="9be16-112">Допустимые значения: `other`, `home`, `work`, `blog`, `profile`.</span><span class="sxs-lookup"><span data-stu-id="9be16-112">The possible values are: `other`, `home`, `work`, `blog`, `profile`.</span></span>|
|<span data-ttu-id="9be16-113">address</span><span class="sxs-lookup"><span data-stu-id="9be16-113">address</span></span>|<span data-ttu-id="9be16-114">string</span><span class="sxs-lookup"><span data-stu-id="9be16-114">string</span></span>|<span data-ttu-id="9be16-115">URL-адрес веб-сайта.</span><span class="sxs-lookup"><span data-stu-id="9be16-115">The URL of the website.</span></span>|
|<span data-ttu-id="9be16-116">displayName</span><span class="sxs-lookup"><span data-stu-id="9be16-116">displayName</span></span>|<span data-ttu-id="9be16-117">string</span><span class="sxs-lookup"><span data-stu-id="9be16-117">string</span></span>|<span data-ttu-id="9be16-118">Отображаемое имя веб-сайта.</span><span class="sxs-lookup"><span data-stu-id="9be16-118">The display name of the web site.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9be16-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9be16-119">JSON representation</span></span>

<span data-ttu-id="9be16-120">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9be16-120">The following is a JSON representation of the resource.</span></span>

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

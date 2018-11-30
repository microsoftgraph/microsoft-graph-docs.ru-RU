---
title: тип ресурса website
description: Представляет веб-сайт.
ms.openlocfilehash: 14934aae418581f4c75c880be67bf51fd0bc293c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27024938"
---
# <a name="website-resource-type"></a><span data-ttu-id="f2462-103">тип ресурса website</span><span class="sxs-lookup"><span data-stu-id="f2462-103">website resource type</span></span>

<span data-ttu-id="f2462-104">Представляет веб-сайт.</span><span class="sxs-lookup"><span data-stu-id="f2462-104">Represents a website.</span></span>


## <a name="properties"></a><span data-ttu-id="f2462-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="f2462-105">Properties</span></span>
| <span data-ttu-id="f2462-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="f2462-106">Property</span></span>     | <span data-ttu-id="f2462-107">Тип</span><span class="sxs-lookup"><span data-stu-id="f2462-107">Type</span></span>   |<span data-ttu-id="f2462-108">Описание</span><span class="sxs-lookup"><span data-stu-id="f2462-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f2462-109">type</span><span class="sxs-lookup"><span data-stu-id="f2462-109">type</span></span>|<span data-ttu-id="f2462-110">websiteType</span><span class="sxs-lookup"><span data-stu-id="f2462-110">websiteType</span></span>| <span data-ttu-id="f2462-111">Возможные значения: `other`, `home`, `work`, `blog`, `profile`.</span><span class="sxs-lookup"><span data-stu-id="f2462-111">The possible values are: `other`, `home`, `work`, `blog`, `profile`.</span></span>|
|<span data-ttu-id="f2462-112">address</span><span class="sxs-lookup"><span data-stu-id="f2462-112">address</span></span>|<span data-ttu-id="f2462-113">string</span><span class="sxs-lookup"><span data-stu-id="f2462-113">string</span></span>|<span data-ttu-id="f2462-114">URL-адрес веб-сайта.</span><span class="sxs-lookup"><span data-stu-id="f2462-114">The URL of the website.</span></span>|
|<span data-ttu-id="f2462-115">displayName</span><span class="sxs-lookup"><span data-stu-id="f2462-115">displayName</span></span>|<span data-ttu-id="f2462-116">строка</span><span class="sxs-lookup"><span data-stu-id="f2462-116">string</span></span>|<span data-ttu-id="f2462-117">Отображаемое имя веб-сайта.</span><span class="sxs-lookup"><span data-stu-id="f2462-117">The display name of the web site.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f2462-118">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="f2462-118">JSON representation</span></span>

<span data-ttu-id="f2462-119">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f2462-119">The following is a JSON representation of the resource.</span></span>

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

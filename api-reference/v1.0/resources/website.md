---
title: Тип ресурса веб-сайта
description: Представляет веб-сайт.
localization_priority: Normal
ms.openlocfilehash: 1ffbee8a67527aac97bb4f60b7f8b1637ba1ebe5
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32457027"
---
# <a name="website-resource-type"></a><span data-ttu-id="aebfb-103">Тип ресурса веб-сайта</span><span class="sxs-lookup"><span data-stu-id="aebfb-103">website resource type</span></span>

<span data-ttu-id="aebfb-104">Представляет веб-сайт.</span><span class="sxs-lookup"><span data-stu-id="aebfb-104">Represents a website.</span></span>


## <a name="properties"></a><span data-ttu-id="aebfb-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="aebfb-105">Properties</span></span>
| <span data-ttu-id="aebfb-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="aebfb-106">Property</span></span>     | <span data-ttu-id="aebfb-107">Тип</span><span class="sxs-lookup"><span data-stu-id="aebfb-107">Type</span></span>   |<span data-ttu-id="aebfb-108">Описание</span><span class="sxs-lookup"><span data-stu-id="aebfb-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="aebfb-109">type</span><span class="sxs-lookup"><span data-stu-id="aebfb-109">type</span></span>|<span data-ttu-id="aebfb-110">websiteType</span><span class="sxs-lookup"><span data-stu-id="aebfb-110">websiteType</span></span>| <span data-ttu-id="aebfb-111">Допустимые значения: `other`, `home`, `work`, `blog`, `profile`.</span><span class="sxs-lookup"><span data-stu-id="aebfb-111">The possible values are: `other`, `home`, `work`, `blog`, `profile`.</span></span>|
|<span data-ttu-id="aebfb-112">address</span><span class="sxs-lookup"><span data-stu-id="aebfb-112">address</span></span>|<span data-ttu-id="aebfb-113">string</span><span class="sxs-lookup"><span data-stu-id="aebfb-113">string</span></span>|<span data-ttu-id="aebfb-114">URL-адрес веб-сайта.</span><span class="sxs-lookup"><span data-stu-id="aebfb-114">The URL of the website.</span></span>|
|<span data-ttu-id="aebfb-115">displayName</span><span class="sxs-lookup"><span data-stu-id="aebfb-115">displayName</span></span>|<span data-ttu-id="aebfb-116">string</span><span class="sxs-lookup"><span data-stu-id="aebfb-116">string</span></span>|<span data-ttu-id="aebfb-117">Отображаемое имя веб-сайта.</span><span class="sxs-lookup"><span data-stu-id="aebfb-117">The display name of the web site.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="aebfb-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="aebfb-118">JSON representation</span></span>

<span data-ttu-id="aebfb-119">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="aebfb-119">The following is a JSON representation of the resource.</span></span>

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

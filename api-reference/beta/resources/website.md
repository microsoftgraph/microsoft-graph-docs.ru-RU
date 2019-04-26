---
title: Тип ресурса веб-сайта
description: Представляет веб-сайт.
localization_priority: Normal
ms.openlocfilehash: b44fcacf77f3b2afb5cdc9dfea2340d0a1fc1cd5
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33339658"
---
# <a name="website-resource-type"></a><span data-ttu-id="5ac54-103">Тип ресурса веб-сайта</span><span class="sxs-lookup"><span data-stu-id="5ac54-103">website resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5ac54-104">Представляет веб-сайт.</span><span class="sxs-lookup"><span data-stu-id="5ac54-104">Represents a web site.</span></span>


## <a name="properties"></a><span data-ttu-id="5ac54-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="5ac54-105">Properties</span></span>
| <span data-ttu-id="5ac54-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="5ac54-106">Property</span></span>     | <span data-ttu-id="5ac54-107">Тип</span><span class="sxs-lookup"><span data-stu-id="5ac54-107">Type</span></span>   |<span data-ttu-id="5ac54-108">Описание</span><span class="sxs-lookup"><span data-stu-id="5ac54-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5ac54-109">type</span><span class="sxs-lookup"><span data-stu-id="5ac54-109">type</span></span>|<span data-ttu-id="5ac54-110">String</span><span class="sxs-lookup"><span data-stu-id="5ac54-110">String</span></span>| <span data-ttu-id="5ac54-111">Возможные значения: `other`, `home`, `work`, `blog`, `profile`.</span><span class="sxs-lookup"><span data-stu-id="5ac54-111">Possible values are: `other`, `home`, `work`, `blog`, `profile`.</span></span>|
|<span data-ttu-id="5ac54-112">address</span><span class="sxs-lookup"><span data-stu-id="5ac54-112">address</span></span>|<span data-ttu-id="5ac54-113">string</span><span class="sxs-lookup"><span data-stu-id="5ac54-113">string</span></span>|<span data-ttu-id="5ac54-114">URL-адрес веб-сайта.</span><span class="sxs-lookup"><span data-stu-id="5ac54-114">The URL of the website.</span></span>|
|<span data-ttu-id="5ac54-115">displayName</span><span class="sxs-lookup"><span data-stu-id="5ac54-115">displayName</span></span>|<span data-ttu-id="5ac54-116">string</span><span class="sxs-lookup"><span data-stu-id="5ac54-116">string</span></span>|<span data-ttu-id="5ac54-117">Отображаемое имя веб-сайта.</span><span class="sxs-lookup"><span data-stu-id="5ac54-117">The display name of the web site.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5ac54-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5ac54-118">JSON representation</span></span>

<span data-ttu-id="5ac54-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5ac54-119">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "webSite resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

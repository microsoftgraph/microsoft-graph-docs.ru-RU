---
title: тип ресурса website
description: Представляет веб-сайта.
localization_priority: Normal
ms.openlocfilehash: 15cc926ad1c251fd169ccdb0b1374df7f434a645
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27826119"
---
# <a name="website-resource-type"></a><span data-ttu-id="8d0cc-103">тип ресурса website</span><span class="sxs-lookup"><span data-stu-id="8d0cc-103">website resource type</span></span>

> <span data-ttu-id="8d0cc-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="8d0cc-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8d0cc-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8d0cc-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8d0cc-106">Представляет веб-сайта.</span><span class="sxs-lookup"><span data-stu-id="8d0cc-106">Represents a web site.</span></span>


## <a name="properties"></a><span data-ttu-id="8d0cc-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="8d0cc-107">Properties</span></span>
| <span data-ttu-id="8d0cc-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="8d0cc-108">Property</span></span>     | <span data-ttu-id="8d0cc-109">Тип</span><span class="sxs-lookup"><span data-stu-id="8d0cc-109">Type</span></span>   |<span data-ttu-id="8d0cc-110">Описание</span><span class="sxs-lookup"><span data-stu-id="8d0cc-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8d0cc-111">type</span><span class="sxs-lookup"><span data-stu-id="8d0cc-111">type</span></span>|<span data-ttu-id="8d0cc-112">String</span><span class="sxs-lookup"><span data-stu-id="8d0cc-112">String</span></span>| <span data-ttu-id="8d0cc-113">Возможные значения: `other`, `home`, `work`, `blog`, `profile`.</span><span class="sxs-lookup"><span data-stu-id="8d0cc-113">Possible values are: `other`, `home`, `work`, `blog`, `profile`.</span></span>|
|<span data-ttu-id="8d0cc-114">address</span><span class="sxs-lookup"><span data-stu-id="8d0cc-114">address</span></span>|<span data-ttu-id="8d0cc-115">string</span><span class="sxs-lookup"><span data-stu-id="8d0cc-115">string</span></span>|<span data-ttu-id="8d0cc-116">URL-адрес веб-сайта.</span><span class="sxs-lookup"><span data-stu-id="8d0cc-116">The URL of the website.</span></span>|
|<span data-ttu-id="8d0cc-117">displayName</span><span class="sxs-lookup"><span data-stu-id="8d0cc-117">displayName</span></span>|<span data-ttu-id="8d0cc-118">строка</span><span class="sxs-lookup"><span data-stu-id="8d0cc-118">string</span></span>|<span data-ttu-id="8d0cc-119">Отображаемое имя веб-сайта.</span><span class="sxs-lookup"><span data-stu-id="8d0cc-119">The display name of the web site.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8d0cc-120">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="8d0cc-120">JSON representation</span></span>

<span data-ttu-id="8d0cc-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8d0cc-121">Here is a JSON representation of the resource.</span></span>

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

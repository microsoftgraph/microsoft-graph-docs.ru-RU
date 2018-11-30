---
title: тип ресурса website
description: Представляет веб-сайта.
ms.openlocfilehash: fa117dc6279e90b49c3c54d0a0ac534e30e633af
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27080310"
---
# <a name="website-resource-type"></a><span data-ttu-id="072ce-103">тип ресурса website</span><span class="sxs-lookup"><span data-stu-id="072ce-103">website resource type</span></span>

> <span data-ttu-id="072ce-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="072ce-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="072ce-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="072ce-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="072ce-106">Представляет веб-сайта.</span><span class="sxs-lookup"><span data-stu-id="072ce-106">Represents a web site.</span></span>


## <a name="properties"></a><span data-ttu-id="072ce-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="072ce-107">Properties</span></span>
| <span data-ttu-id="072ce-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="072ce-108">Property</span></span>     | <span data-ttu-id="072ce-109">Тип</span><span class="sxs-lookup"><span data-stu-id="072ce-109">Type</span></span>   |<span data-ttu-id="072ce-110">Описание</span><span class="sxs-lookup"><span data-stu-id="072ce-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="072ce-111">type</span><span class="sxs-lookup"><span data-stu-id="072ce-111">type</span></span>|<span data-ttu-id="072ce-112">String</span><span class="sxs-lookup"><span data-stu-id="072ce-112">String</span></span>| <span data-ttu-id="072ce-113">Возможные значения: `other`, `home`, `work`, `blog`, `profile`.</span><span class="sxs-lookup"><span data-stu-id="072ce-113">Possible values are: `other`, `home`, `work`, `blog`, `profile`.</span></span>|
|<span data-ttu-id="072ce-114">address</span><span class="sxs-lookup"><span data-stu-id="072ce-114">address</span></span>|<span data-ttu-id="072ce-115">string</span><span class="sxs-lookup"><span data-stu-id="072ce-115">string</span></span>|<span data-ttu-id="072ce-116">URL-адрес веб-сайта.</span><span class="sxs-lookup"><span data-stu-id="072ce-116">The URL of the website.</span></span>|
|<span data-ttu-id="072ce-117">displayName</span><span class="sxs-lookup"><span data-stu-id="072ce-117">displayName</span></span>|<span data-ttu-id="072ce-118">строка</span><span class="sxs-lookup"><span data-stu-id="072ce-118">string</span></span>|<span data-ttu-id="072ce-119">Отображаемое имя веб-сайта.</span><span class="sxs-lookup"><span data-stu-id="072ce-119">The display name of the web site.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="072ce-120">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="072ce-120">JSON representation</span></span>

<span data-ttu-id="072ce-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="072ce-121">Here is a JSON representation of the resource.</span></span>

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
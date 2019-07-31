---
title: Тип ресурса веб-сайта
description: Представляет веб-сайт.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 0f822c38c57d5e47d39a40b3285773e0e36fd2ee
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964146"
---
# <a name="website-resource-type"></a><span data-ttu-id="0df01-103">Тип ресурса веб-сайта</span><span class="sxs-lookup"><span data-stu-id="0df01-103">website resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0df01-104">Представляет веб-сайт.</span><span class="sxs-lookup"><span data-stu-id="0df01-104">Represents a web site.</span></span>


## <a name="properties"></a><span data-ttu-id="0df01-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="0df01-105">Properties</span></span>
| <span data-ttu-id="0df01-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="0df01-106">Property</span></span>     | <span data-ttu-id="0df01-107">Тип</span><span class="sxs-lookup"><span data-stu-id="0df01-107">Type</span></span>   |<span data-ttu-id="0df01-108">Описание</span><span class="sxs-lookup"><span data-stu-id="0df01-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0df01-109">type</span><span class="sxs-lookup"><span data-stu-id="0df01-109">type</span></span>|<span data-ttu-id="0df01-110">String</span><span class="sxs-lookup"><span data-stu-id="0df01-110">String</span></span>| <span data-ttu-id="0df01-111">Возможные значения: `other`, `home`, `work`, `blog`, `profile`.</span><span class="sxs-lookup"><span data-stu-id="0df01-111">Possible values are: `other`, `home`, `work`, `blog`, `profile`.</span></span>|
|<span data-ttu-id="0df01-112">address</span><span class="sxs-lookup"><span data-stu-id="0df01-112">address</span></span>|<span data-ttu-id="0df01-113">string</span><span class="sxs-lookup"><span data-stu-id="0df01-113">string</span></span>|<span data-ttu-id="0df01-114">URL-адрес веб-сайта.</span><span class="sxs-lookup"><span data-stu-id="0df01-114">The URL of the website.</span></span>|
|<span data-ttu-id="0df01-115">displayName</span><span class="sxs-lookup"><span data-stu-id="0df01-115">displayName</span></span>|<span data-ttu-id="0df01-116">string</span><span class="sxs-lookup"><span data-stu-id="0df01-116">string</span></span>|<span data-ttu-id="0df01-117">Отображаемое имя веб-сайта.</span><span class="sxs-lookup"><span data-stu-id="0df01-117">The display name of the web site.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0df01-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0df01-118">JSON representation</span></span>

<span data-ttu-id="0df01-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0df01-119">Here is a JSON representation of the resource.</span></span>

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

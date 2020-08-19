---
title: Тип ресурса веб-сайта
description: Представляет веб-сайт.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: AAmatino
ms.openlocfilehash: 758d802a67979c4e43aefcdb4e8a3998be15b993
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46809301"
---
# <a name="website-resource-type"></a><span data-ttu-id="75151-103">Тип ресурса веб-сайта</span><span class="sxs-lookup"><span data-stu-id="75151-103">website resource type</span></span>

<span data-ttu-id="75151-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="75151-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="75151-105">Представляет веб-сайт.</span><span class="sxs-lookup"><span data-stu-id="75151-105">Represents a web site.</span></span>


## <a name="properties"></a><span data-ttu-id="75151-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="75151-106">Properties</span></span>
| <span data-ttu-id="75151-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="75151-107">Property</span></span>     | <span data-ttu-id="75151-108">Тип</span><span class="sxs-lookup"><span data-stu-id="75151-108">Type</span></span>   |<span data-ttu-id="75151-109">Описание</span><span class="sxs-lookup"><span data-stu-id="75151-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="75151-110">type</span><span class="sxs-lookup"><span data-stu-id="75151-110">type</span></span>|<span data-ttu-id="75151-111">String</span><span class="sxs-lookup"><span data-stu-id="75151-111">String</span></span>| <span data-ttu-id="75151-112">Возможные значения: `other`, `home`, `work`, `blog`, `profile`.</span><span class="sxs-lookup"><span data-stu-id="75151-112">Possible values are: `other`, `home`, `work`, `blog`, `profile`.</span></span>|
|<span data-ttu-id="75151-113">address</span><span class="sxs-lookup"><span data-stu-id="75151-113">address</span></span>|<span data-ttu-id="75151-114">string</span><span class="sxs-lookup"><span data-stu-id="75151-114">string</span></span>|<span data-ttu-id="75151-115">URL-адрес веб-сайта.</span><span class="sxs-lookup"><span data-stu-id="75151-115">The URL of the website.</span></span>|
|<span data-ttu-id="75151-116">displayName</span><span class="sxs-lookup"><span data-stu-id="75151-116">displayName</span></span>|<span data-ttu-id="75151-117">string</span><span class="sxs-lookup"><span data-stu-id="75151-117">string</span></span>|<span data-ttu-id="75151-118">Отображаемое имя веб-сайта.</span><span class="sxs-lookup"><span data-stu-id="75151-118">The display name of the web site.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="75151-119">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="75151-119">JSON representation</span></span>

<span data-ttu-id="75151-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="75151-120">Here is a JSON representation of the resource.</span></span>

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

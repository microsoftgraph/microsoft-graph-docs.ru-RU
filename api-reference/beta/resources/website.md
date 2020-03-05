---
title: Тип ресурса веб-сайта
description: Представляет веб-сайт.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: ebdfef4a8ee4e11c2993dbd97a735c6e01960b6b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519430"
---
# <a name="website-resource-type"></a><span data-ttu-id="f273f-103">Тип ресурса веб-сайта</span><span class="sxs-lookup"><span data-stu-id="f273f-103">website resource type</span></span>

<span data-ttu-id="f273f-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="f273f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f273f-105">Представляет веб-сайт.</span><span class="sxs-lookup"><span data-stu-id="f273f-105">Represents a web site.</span></span>


## <a name="properties"></a><span data-ttu-id="f273f-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="f273f-106">Properties</span></span>
| <span data-ttu-id="f273f-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="f273f-107">Property</span></span>     | <span data-ttu-id="f273f-108">Тип</span><span class="sxs-lookup"><span data-stu-id="f273f-108">Type</span></span>   |<span data-ttu-id="f273f-109">Описание</span><span class="sxs-lookup"><span data-stu-id="f273f-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f273f-110">type</span><span class="sxs-lookup"><span data-stu-id="f273f-110">type</span></span>|<span data-ttu-id="f273f-111">String</span><span class="sxs-lookup"><span data-stu-id="f273f-111">String</span></span>| <span data-ttu-id="f273f-112">Возможные значения: `other`, `home`, `work`, `blog`, `profile`.</span><span class="sxs-lookup"><span data-stu-id="f273f-112">Possible values are: `other`, `home`, `work`, `blog`, `profile`.</span></span>|
|<span data-ttu-id="f273f-113">address</span><span class="sxs-lookup"><span data-stu-id="f273f-113">address</span></span>|<span data-ttu-id="f273f-114">string</span><span class="sxs-lookup"><span data-stu-id="f273f-114">string</span></span>|<span data-ttu-id="f273f-115">URL-адрес веб-сайта.</span><span class="sxs-lookup"><span data-stu-id="f273f-115">The URL of the website.</span></span>|
|<span data-ttu-id="f273f-116">displayName</span><span class="sxs-lookup"><span data-stu-id="f273f-116">displayName</span></span>|<span data-ttu-id="f273f-117">string</span><span class="sxs-lookup"><span data-stu-id="f273f-117">string</span></span>|<span data-ttu-id="f273f-118">Отображаемое имя веб-сайта.</span><span class="sxs-lookup"><span data-stu-id="f273f-118">The display name of the web site.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f273f-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f273f-119">JSON representation</span></span>

<span data-ttu-id="f273f-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f273f-120">Here is a JSON representation of the resource.</span></span>

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

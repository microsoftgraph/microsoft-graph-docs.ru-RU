---
title: Тип ресурса addIn
description: Ниже представлено описание ресурса в формате JSON.
localization_priority: Normal
ms.openlocfilehash: 777b9e2eac1ec4052fae30b13d09aaf91a808375
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33339131"
---
# <a name="addin-resource-type"></a><span data-ttu-id="e1c49-103">Тип ресурса addIn</span><span class="sxs-lookup"><span data-stu-id="e1c49-103">addIn resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]


## <a name="properties"></a><span data-ttu-id="e1c49-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="e1c49-104">Properties</span></span>
| <span data-ttu-id="e1c49-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="e1c49-105">Property</span></span>     | <span data-ttu-id="e1c49-106">Тип</span><span class="sxs-lookup"><span data-stu-id="e1c49-106">Type</span></span>   |<span data-ttu-id="e1c49-107">Описание</span><span class="sxs-lookup"><span data-stu-id="e1c49-107">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e1c49-108">id</span><span class="sxs-lookup"><span data-stu-id="e1c49-108">id</span></span>|<span data-ttu-id="e1c49-109">кодом</span><span class="sxs-lookup"><span data-stu-id="e1c49-109">guid</span></span>||
|<span data-ttu-id="e1c49-110">properties</span><span class="sxs-lookup"><span data-stu-id="e1c49-110">properties</span></span>|<span data-ttu-id="e1c49-111">Коллекция [keyValue](keyvalue.md)</span><span class="sxs-lookup"><span data-stu-id="e1c49-111">[keyValue](keyvalue.md) collection</span></span>||
|<span data-ttu-id="e1c49-112">type</span><span class="sxs-lookup"><span data-stu-id="e1c49-112">type</span></span>|<span data-ttu-id="e1c49-113">string</span><span class="sxs-lookup"><span data-stu-id="e1c49-113">string</span></span>||

## <a name="json-representation"></a><span data-ttu-id="e1c49-114">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e1c49-114">JSON representation</span></span>

<span data-ttu-id="e1c49-115">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e1c49-115">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.addIn"
}-->

```json
{
  "id": "guid",
  "properties": [{"@odata.type": "microsoft.graph.keyValue"}],
  "type": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "addIn resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

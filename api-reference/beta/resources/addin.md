---
title: Тип ресурса addIn
description: Ниже представлено описание ресурса в формате JSON.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 46daa8c4f1218b3de485643a47f7acbe881c661c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35974551"
---
# <a name="addin-resource-type"></a><span data-ttu-id="f8488-103">Тип ресурса addIn</span><span class="sxs-lookup"><span data-stu-id="f8488-103">addIn resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]


## <a name="properties"></a><span data-ttu-id="f8488-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="f8488-104">Properties</span></span>
| <span data-ttu-id="f8488-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="f8488-105">Property</span></span>     | <span data-ttu-id="f8488-106">Тип</span><span class="sxs-lookup"><span data-stu-id="f8488-106">Type</span></span>   |<span data-ttu-id="f8488-107">Описание</span><span class="sxs-lookup"><span data-stu-id="f8488-107">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f8488-108">id</span><span class="sxs-lookup"><span data-stu-id="f8488-108">id</span></span>|<span data-ttu-id="f8488-109">кодом</span><span class="sxs-lookup"><span data-stu-id="f8488-109">guid</span></span>||
|<span data-ttu-id="f8488-110">properties</span><span class="sxs-lookup"><span data-stu-id="f8488-110">properties</span></span>|<span data-ttu-id="f8488-111">Коллекция [keyValue](keyvalue.md)</span><span class="sxs-lookup"><span data-stu-id="f8488-111">[keyValue](keyvalue.md) collection</span></span>||
|<span data-ttu-id="f8488-112">type</span><span class="sxs-lookup"><span data-stu-id="f8488-112">type</span></span>|<span data-ttu-id="f8488-113">string</span><span class="sxs-lookup"><span data-stu-id="f8488-113">string</span></span>||

## <a name="json-representation"></a><span data-ttu-id="f8488-114">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f8488-114">JSON representation</span></span>

<span data-ttu-id="f8488-115">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f8488-115">Here is a JSON representation of the resource.</span></span>

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

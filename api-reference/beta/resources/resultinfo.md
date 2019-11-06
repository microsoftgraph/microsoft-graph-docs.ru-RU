---
title: Тип ресурса Ресултинфо
description: Тип Ресултинфо.
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: acc01a17420390343c3eb1f866761d54d5c81c79
ms.sourcegitcommit: 9bddc0b7746383e8d05ce50d163af3f4196f12a6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/06/2019
ms.locfileid: "38006552"
---
# <a name="resultinfo-resource-type"></a><span data-ttu-id="0a6b9-103">Тип ресурса Ресултинфо</span><span class="sxs-lookup"><span data-stu-id="0a6b9-103">resultInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0a6b9-104">Тип Ресултинфо.</span><span class="sxs-lookup"><span data-stu-id="0a6b9-104">The resultInfo type.</span></span>

## <a name="properties"></a><span data-ttu-id="0a6b9-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="0a6b9-105">Properties</span></span>

| <span data-ttu-id="0a6b9-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="0a6b9-106">Property</span></span> | <span data-ttu-id="0a6b9-107">Тип</span><span class="sxs-lookup"><span data-stu-id="0a6b9-107">Type</span></span>   | <span data-ttu-id="0a6b9-108">Описание</span><span class="sxs-lookup"><span data-stu-id="0a6b9-108">Description</span></span>          |
| :------- | :----- | :------------------  |
| <span data-ttu-id="0a6b9-109">code</span><span class="sxs-lookup"><span data-stu-id="0a6b9-109">code</span></span>     | <span data-ttu-id="0a6b9-110">Int32</span><span class="sxs-lookup"><span data-stu-id="0a6b9-110">Int32</span></span> | <span data-ttu-id="0a6b9-111">Код результата.</span><span class="sxs-lookup"><span data-stu-id="0a6b9-111">The result code.</span></span>     |
| <span data-ttu-id="0a6b9-112">message</span><span class="sxs-lookup"><span data-stu-id="0a6b9-112">message</span></span>  | <span data-ttu-id="0a6b9-113">String</span><span class="sxs-lookup"><span data-stu-id="0a6b9-113">String</span></span> | <span data-ttu-id="0a6b9-114">Сообщение.</span><span class="sxs-lookup"><span data-stu-id="0a6b9-114">The message.</span></span>         |
| <span data-ttu-id="0a6b9-115">Subcode</span><span class="sxs-lookup"><span data-stu-id="0a6b9-115">subcode</span></span>  | <span data-ttu-id="0a6b9-116">Int32</span><span class="sxs-lookup"><span data-stu-id="0a6b9-116">Int32</span></span> | <span data-ttu-id="0a6b9-117">Дочерний код результата.</span><span class="sxs-lookup"><span data-stu-id="0a6b9-117">The result sub-code.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="0a6b9-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0a6b9-118">JSON representation</span></span>

<span data-ttu-id="0a6b9-119">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0a6b9-119">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.resultInfo"
}-->
```json
{
  "code": 0,
  "message": "String",
  "subcode": 0
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "resultInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

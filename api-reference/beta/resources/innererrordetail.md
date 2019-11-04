---
title: Тип ресурса Иннереррордетаил
description: Внутренняя ошибка, которая находится в объекте Еррордетаил
localization_priority: Normal
author: snlraju-msft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 5a5b85f17b87343766a4edb00c6d620c185ecaf5
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939658"
---
# <a name="innererrordetail-resource-type"></a><span data-ttu-id="51aa2-103">Тип ресурса Иннереррордетаил</span><span class="sxs-lookup"><span data-stu-id="51aa2-103">innerErrorDetail resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="51aa2-104">Внутренняя ошибка, которая находится в объекте [еррордетаил](errordetail.md)</span><span class="sxs-lookup"><span data-stu-id="51aa2-104">An inner error contained in an [errorDetail](errordetail.md) object.</span></span>

## <a name="properties"></a><span data-ttu-id="51aa2-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="51aa2-105">Properties</span></span>

| <span data-ttu-id="51aa2-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="51aa2-106">Property</span></span> | <span data-ttu-id="51aa2-107">Тип</span><span class="sxs-lookup"><span data-stu-id="51aa2-107">Type</span></span>   | <span data-ttu-id="51aa2-108">Описание</span><span class="sxs-lookup"><span data-stu-id="51aa2-108">Description</span></span>                                  |
|:---------|:-------|:---------------------------------------------|
| <span data-ttu-id="51aa2-109">message</span><span class="sxs-lookup"><span data-stu-id="51aa2-109">message</span></span>  | <span data-ttu-id="51aa2-110">String</span><span class="sxs-lookup"><span data-stu-id="51aa2-110">String</span></span> | <span data-ttu-id="51aa2-111">Сообщение об ошибке, читаемое человеком.</span><span class="sxs-lookup"><span data-stu-id="51aa2-111">The human-readable error message.</span></span> <span data-ttu-id="51aa2-112">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="51aa2-112">Read-only.</span></span> |
| <span data-ttu-id="51aa2-113">source</span><span class="sxs-lookup"><span data-stu-id="51aa2-113">source</span></span>   | <span data-ttu-id="51aa2-114">Строка</span><span class="sxs-lookup"><span data-stu-id="51aa2-114">String</span></span> | <span data-ttu-id="51aa2-115">Источник ошибки.</span><span class="sxs-lookup"><span data-stu-id="51aa2-115">The source of the error.</span></span> <span data-ttu-id="51aa2-116">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="51aa2-116">Read-only.</span></span>          |

## <a name="json-representation"></a><span data-ttu-id="51aa2-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="51aa2-117">JSON representation</span></span>

<span data-ttu-id="51aa2-118">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="51aa2-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.innerErrorDetail",
  "baseType": null
}-->

```json
{
  "message": "String",
  "source": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "innerErrorDetail resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

---
title: Тип ресурса Иннереррордетаил
description: Внутренняя ошибка, которая находится в объекте Еррордетаил
localization_priority: Normal
author: snlraju-msft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: c1dd87e6af015423441b75ada256456e748e3805
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42495930"
---
# <a name="innererrordetail-resource-type"></a><span data-ttu-id="a14d3-103">Тип ресурса Иннереррордетаил</span><span class="sxs-lookup"><span data-stu-id="a14d3-103">innerErrorDetail resource type</span></span>

<span data-ttu-id="a14d3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a14d3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a14d3-105">Внутренняя ошибка, которая находится в объекте [еррордетаил](errordetail.md)</span><span class="sxs-lookup"><span data-stu-id="a14d3-105">An inner error contained in an [errorDetail](errordetail.md) object.</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="properties"></a><span data-ttu-id="a14d3-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="a14d3-106">Properties</span></span>

| <span data-ttu-id="a14d3-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="a14d3-107">Property</span></span> | <span data-ttu-id="a14d3-108">Тип</span><span class="sxs-lookup"><span data-stu-id="a14d3-108">Type</span></span>   | <span data-ttu-id="a14d3-109">Описание</span><span class="sxs-lookup"><span data-stu-id="a14d3-109">Description</span></span>                                  |
|:---------|:-------|:---------------------------------------------|
| <span data-ttu-id="a14d3-110">message</span><span class="sxs-lookup"><span data-stu-id="a14d3-110">message</span></span>  | <span data-ttu-id="a14d3-111">String</span><span class="sxs-lookup"><span data-stu-id="a14d3-111">String</span></span> | <span data-ttu-id="a14d3-112">Сообщение об ошибке, читаемое человеком.</span><span class="sxs-lookup"><span data-stu-id="a14d3-112">The human-readable error message.</span></span> <span data-ttu-id="a14d3-113">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a14d3-113">Read-only.</span></span> |
| <span data-ttu-id="a14d3-114">source</span><span class="sxs-lookup"><span data-stu-id="a14d3-114">source</span></span>   | <span data-ttu-id="a14d3-115">String</span><span class="sxs-lookup"><span data-stu-id="a14d3-115">String</span></span> | <span data-ttu-id="a14d3-116">Источник ошибки.</span><span class="sxs-lookup"><span data-stu-id="a14d3-116">The source of the error.</span></span> <span data-ttu-id="a14d3-117">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a14d3-117">Read-only.</span></span>          |

## <a name="json-representation"></a><span data-ttu-id="a14d3-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a14d3-118">JSON representation</span></span>

<span data-ttu-id="a14d3-119">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a14d3-119">The following is a JSON representation of the resource.</span></span>

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

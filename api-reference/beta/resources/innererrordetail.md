---
title: Тип ресурса Иннереррордетаил
description: Внутренняя ошибка, которая находится в объекте Еррордетаил
localization_priority: Normal
author: snlraju-msft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 07220eaead4035dafcb7cd7032916ae4a5db0d75
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48021905"
---
# <a name="innererrordetail-resource-type"></a><span data-ttu-id="f3aca-103">Тип ресурса Иннереррордетаил</span><span class="sxs-lookup"><span data-stu-id="f3aca-103">innerErrorDetail resource type</span></span>

<span data-ttu-id="f3aca-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f3aca-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f3aca-105">Внутренняя ошибка, которая находится в объекте [еррордетаил](errordetail.md)</span><span class="sxs-lookup"><span data-stu-id="f3aca-105">An inner error contained in an [errorDetail](errordetail.md) object.</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="properties"></a><span data-ttu-id="f3aca-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="f3aca-106">Properties</span></span>

| <span data-ttu-id="f3aca-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="f3aca-107">Property</span></span> | <span data-ttu-id="f3aca-108">Тип</span><span class="sxs-lookup"><span data-stu-id="f3aca-108">Type</span></span>   | <span data-ttu-id="f3aca-109">Описание</span><span class="sxs-lookup"><span data-stu-id="f3aca-109">Description</span></span>                                  |
|:---------|:-------|:---------------------------------------------|
| <span data-ttu-id="f3aca-110">message</span><span class="sxs-lookup"><span data-stu-id="f3aca-110">message</span></span>  | <span data-ttu-id="f3aca-111">String</span><span class="sxs-lookup"><span data-stu-id="f3aca-111">String</span></span> | <span data-ttu-id="f3aca-112">Сообщение об ошибке, читаемое человеком.</span><span class="sxs-lookup"><span data-stu-id="f3aca-112">The human-readable error message.</span></span> <span data-ttu-id="f3aca-113">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f3aca-113">Read-only.</span></span> |
| <span data-ttu-id="f3aca-114">source</span><span class="sxs-lookup"><span data-stu-id="f3aca-114">source</span></span>   | <span data-ttu-id="f3aca-115">String</span><span class="sxs-lookup"><span data-stu-id="f3aca-115">String</span></span> | <span data-ttu-id="f3aca-116">Источник ошибки.</span><span class="sxs-lookup"><span data-stu-id="f3aca-116">The source of the error.</span></span> <span data-ttu-id="f3aca-117">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f3aca-117">Read-only.</span></span>          |

## <a name="json-representation"></a><span data-ttu-id="f3aca-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f3aca-118">JSON representation</span></span>

<span data-ttu-id="f3aca-119">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f3aca-119">The following is a JSON representation of the resource.</span></span>

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



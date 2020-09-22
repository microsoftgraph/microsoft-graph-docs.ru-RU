---
title: Тип ресурса Еррордетаил
description: Описание ошибки неудачного запроса на асинхронное создание схемы подключения Microsoft Search.
localization_priority: Normal
author: snlraju-msft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 6f37f3ca432dcd9c755556b37f4f0ea330907426
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48013729"
---
# <a name="errordetail-resource-type"></a><span data-ttu-id="ce06e-103">Тип ресурса Еррордетаил</span><span class="sxs-lookup"><span data-stu-id="ce06e-103">errorDetail resource type</span></span>

<span data-ttu-id="ce06e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ce06e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ce06e-105">Описание ошибки неудачного запроса на асинхронное создание [схемы](schema.md) подключения Microsoft Search.</span><span class="sxs-lookup"><span data-stu-id="ce06e-105">Describes an error for a failed request to create a Microsoft Search connection [schema](schema.md) asynchronously.</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="properties"></a><span data-ttu-id="ce06e-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="ce06e-106">Properties</span></span>

| <span data-ttu-id="ce06e-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="ce06e-107">Property</span></span>  | <span data-ttu-id="ce06e-108">Тип</span><span class="sxs-lookup"><span data-stu-id="ce06e-108">Type</span></span>                                               | <span data-ttu-id="ce06e-109">Описание</span><span class="sxs-lookup"><span data-stu-id="ce06e-109">Description</span></span> |
|:----------|:---------------------------------------------------|:------------|
| <span data-ttu-id="ce06e-110">details</span><span class="sxs-lookup"><span data-stu-id="ce06e-110">details</span></span>   | <span data-ttu-id="ce06e-111">Коллекция [иннереррордетаил](innererrordetail.md)</span><span class="sxs-lookup"><span data-stu-id="ce06e-111">[innerErrorDetail](innererrordetail.md) collection</span></span> | <span data-ttu-id="ce06e-112">Коллекция внутренних ошибок (при наличии).</span><span class="sxs-lookup"><span data-stu-id="ce06e-112">A collection of inner errors, if any.</span></span> <span data-ttu-id="ce06e-113">Только для чтения, допускает значение null.</span><span class="sxs-lookup"><span data-stu-id="ce06e-113">Read-only, nullable.</span></span> |
| <span data-ttu-id="ce06e-114">errorCode</span><span class="sxs-lookup"><span data-stu-id="ce06e-114">errorCode</span></span> | <span data-ttu-id="ce06e-115">String</span><span class="sxs-lookup"><span data-stu-id="ce06e-115">String</span></span>                                             | <span data-ttu-id="ce06e-116">Код ошибки, связанный с ошибкой (при наличии).</span><span class="sxs-lookup"><span data-stu-id="ce06e-116">The error code associated with the error, if any.</span></span> <span data-ttu-id="ce06e-117">Только для чтения, допускает значение null.</span><span class="sxs-lookup"><span data-stu-id="ce06e-117">Read-only, nullable.</span></span> |
| <span data-ttu-id="ce06e-118">message</span><span class="sxs-lookup"><span data-stu-id="ce06e-118">message</span></span>   | <span data-ttu-id="ce06e-119">String</span><span class="sxs-lookup"><span data-stu-id="ce06e-119">String</span></span>                                             | <span data-ttu-id="ce06e-120">Сообщение об ошибке, читаемое человеком.</span><span class="sxs-lookup"><span data-stu-id="ce06e-120">The human-readable error message.</span></span> <span data-ttu-id="ce06e-121">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ce06e-121">Read-only.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="ce06e-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ce06e-122">JSON representation</span></span>

<span data-ttu-id="ce06e-123">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ce06e-123">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "details",
    "errorCode"
  ],
  "@odata.type": "microsoft.graph.errorDetail",
  "baseType": null
}-->

```json
{
  "details": [{"@odata.type": "microsoft.graph.innerErrorDetail"}],
  "errorCode": "String",
  "message": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "errorDetail resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->



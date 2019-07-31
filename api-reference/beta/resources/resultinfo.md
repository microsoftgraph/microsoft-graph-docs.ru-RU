---
title: Тип ресурса Ресултинфо
description: Тип Ресултинфо.
author: VinodRavichandran
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 1e5f6a523a8aca4454cd3355e2a0287fef9fc90d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965371"
---
# <a name="resultinfo-resource-type"></a><span data-ttu-id="5841d-103">Тип ресурса Ресултинфо</span><span class="sxs-lookup"><span data-stu-id="5841d-103">resultInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5841d-104">Тип Ресултинфо.</span><span class="sxs-lookup"><span data-stu-id="5841d-104">The resultInfo type.</span></span>

## <a name="properties"></a><span data-ttu-id="5841d-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="5841d-105">Properties</span></span>

| <span data-ttu-id="5841d-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="5841d-106">Property</span></span> | <span data-ttu-id="5841d-107">Тип</span><span class="sxs-lookup"><span data-stu-id="5841d-107">Type</span></span>   | <span data-ttu-id="5841d-108">Описание</span><span class="sxs-lookup"><span data-stu-id="5841d-108">Description</span></span>          |
| :------- | :----- | :------------------  |
| <span data-ttu-id="5841d-109">code</span><span class="sxs-lookup"><span data-stu-id="5841d-109">code</span></span>     | <span data-ttu-id="5841d-110">String</span><span class="sxs-lookup"><span data-stu-id="5841d-110">String</span></span> | <span data-ttu-id="5841d-111">Код результата.</span><span class="sxs-lookup"><span data-stu-id="5841d-111">The result code.</span></span>     |
| <span data-ttu-id="5841d-112">message</span><span class="sxs-lookup"><span data-stu-id="5841d-112">message</span></span>  | <span data-ttu-id="5841d-113">String</span><span class="sxs-lookup"><span data-stu-id="5841d-113">String</span></span> | <span data-ttu-id="5841d-114">Сообщение.</span><span class="sxs-lookup"><span data-stu-id="5841d-114">The message.</span></span>         |
| <span data-ttu-id="5841d-115">subCode</span><span class="sxs-lookup"><span data-stu-id="5841d-115">subCode</span></span>  | <span data-ttu-id="5841d-116">String</span><span class="sxs-lookup"><span data-stu-id="5841d-116">String</span></span> | <span data-ttu-id="5841d-117">Дочерний код результата.</span><span class="sxs-lookup"><span data-stu-id="5841d-117">The result sub-code.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="5841d-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5841d-118">JSON representation</span></span>

<span data-ttu-id="5841d-119">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5841d-119">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.resultInfo"
}-->
```json
{
  "code": "String",
  "message": "String",
  "subCode": "String"
}
```

## <a name="example-error-result"></a><span data-ttu-id="5841d-120">Пример результата ошибки</span><span class="sxs-lookup"><span data-stu-id="5841d-120">Example Error result</span></span>

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.resultInfo"
}-->
```json
{
  "code": "100",
  "message": "Internal Server Error.",
  "subCode": "20"
}
```

## <a name="example-generic-success-result"></a><span data-ttu-id="5841d-121">Пример общего результата успеха</span><span class="sxs-lookup"><span data-stu-id="5841d-121">Example Generic success result</span></span>

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.resultInfo"
}-->
```json
{
  "code": "200",
  "message": "",
  "subCode": "0"
}
```

## <a name="example-record-success-result"></a><span data-ttu-id="5841d-122">Пример результатов записи</span><span class="sxs-lookup"><span data-stu-id="5841d-122">Example Record Success result</span></span>

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.resultInfo"
}-->
```json
{
  "code": "200",
  "message": "",
  "subCode": "completedSilenceDetected"
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

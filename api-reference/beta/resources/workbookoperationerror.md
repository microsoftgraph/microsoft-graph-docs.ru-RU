---
title: Тип ресурса Воркбукоператионеррор
description: Представляет ошибку при выполнении неудачной операции с книгой.
localization_priority: Normal
author: grangeryy
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 42e8eea86222c360d9b08e70b7d6fded2a12afb4
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48070396"
---
# <a name="workbookoperationerror-resource-type"></a><span data-ttu-id="64b47-103">Тип ресурса Воркбукоператионеррор</span><span class="sxs-lookup"><span data-stu-id="64b47-103">workbookOperationError resource type</span></span>

<span data-ttu-id="64b47-104">Представляет ошибку при выполнении неудачной операции с книгой.</span><span class="sxs-lookup"><span data-stu-id="64b47-104">Represents an error from a failed workbook operation.</span></span>

## <a name="properties"></a><span data-ttu-id="64b47-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="64b47-105">Properties</span></span>

| <span data-ttu-id="64b47-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="64b47-106">Property</span></span>     | <span data-ttu-id="64b47-107">Тип</span><span class="sxs-lookup"><span data-stu-id="64b47-107">Type</span></span>        | <span data-ttu-id="64b47-108">Описание</span><span class="sxs-lookup"><span data-stu-id="64b47-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="64b47-109">code</span><span class="sxs-lookup"><span data-stu-id="64b47-109">code</span></span>|<span data-ttu-id="64b47-110">String</span><span class="sxs-lookup"><span data-stu-id="64b47-110">String</span></span>| <span data-ttu-id="64b47-111">Код ошибки.</span><span class="sxs-lookup"><span data-stu-id="64b47-111">The error code.</span></span>|
|<span data-ttu-id="64b47-112">message</span><span class="sxs-lookup"><span data-stu-id="64b47-112">message</span></span>|<span data-ttu-id="64b47-113">String</span><span class="sxs-lookup"><span data-stu-id="64b47-113">String</span></span>| <span data-ttu-id="64b47-114">Сообщение об ошибке.</span><span class="sxs-lookup"><span data-stu-id="64b47-114">The error message.</span></span>|
|<span data-ttu-id="64b47-115">innererror</span><span class="sxs-lookup"><span data-stu-id="64b47-115">innererror</span></span>|<span data-ttu-id="64b47-116">error object</span><span class="sxs-lookup"><span data-stu-id="64b47-116">error object</span></span>| <span data-ttu-id="64b47-p101">Необязательное. Дополнительные объекты ошибки, которые могут быть более информативны, чем сообщение об ошибке верхнего уровня.</span><span class="sxs-lookup"><span data-stu-id="64b47-p101">Optional. Additional error objects that may be more specific than the top level error.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="64b47-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="64b47-119">JSON representation</span></span>

<span data-ttu-id="64b47-120">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="64b47-120">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookOperationError",
  "baseType": null
}-->

```json
{
  "code": "String",
  "message": "String",
  "innererror": { "@odata.type": "odata.error" }
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "workbookOperationError resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->



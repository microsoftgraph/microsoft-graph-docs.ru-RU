---
title: Тип ресурса Воркбукоператионеррор
description: Представляет ошибку при выполнении неудачной операции с книгой.
localization_priority: Normal
author: grangeryy
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: ce65847d6ddbb0a8db0c1277e38753ecab7080e9
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48015143"
---
# <a name="workbookoperationerror-resource-type"></a><span data-ttu-id="d39d5-103">Тип ресурса Воркбукоператионеррор</span><span class="sxs-lookup"><span data-stu-id="d39d5-103">workbookOperationError resource type</span></span>

<span data-ttu-id="d39d5-104">Представляет ошибку при выполнении неудачной операции с книгой.</span><span class="sxs-lookup"><span data-stu-id="d39d5-104">Represents an error from a failed workbook operation.</span></span>

## <a name="properties"></a><span data-ttu-id="d39d5-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="d39d5-105">Properties</span></span>

| <span data-ttu-id="d39d5-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="d39d5-106">Property</span></span>     | <span data-ttu-id="d39d5-107">Тип</span><span class="sxs-lookup"><span data-stu-id="d39d5-107">Type</span></span>        | <span data-ttu-id="d39d5-108">Описание</span><span class="sxs-lookup"><span data-stu-id="d39d5-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="d39d5-109">code</span><span class="sxs-lookup"><span data-stu-id="d39d5-109">code</span></span>|<span data-ttu-id="d39d5-110">String</span><span class="sxs-lookup"><span data-stu-id="d39d5-110">String</span></span>| <span data-ttu-id="d39d5-111">Код ошибки.</span><span class="sxs-lookup"><span data-stu-id="d39d5-111">The error code.</span></span>|
|<span data-ttu-id="d39d5-112">message</span><span class="sxs-lookup"><span data-stu-id="d39d5-112">message</span></span>|<span data-ttu-id="d39d5-113">String</span><span class="sxs-lookup"><span data-stu-id="d39d5-113">String</span></span>| <span data-ttu-id="d39d5-114">Сообщение об ошибке.</span><span class="sxs-lookup"><span data-stu-id="d39d5-114">The error message.</span></span>|
|<span data-ttu-id="d39d5-115">innererror</span><span class="sxs-lookup"><span data-stu-id="d39d5-115">innererror</span></span>|<span data-ttu-id="d39d5-116">error object</span><span class="sxs-lookup"><span data-stu-id="d39d5-116">error object</span></span>| <span data-ttu-id="d39d5-p101">Необязательное. Дополнительные объекты ошибки, которые могут быть более информативны, чем сообщение об ошибке верхнего уровня.</span><span class="sxs-lookup"><span data-stu-id="d39d5-p101">Optional. Additional error objects that may be more specific than the top level error.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d39d5-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d39d5-119">JSON representation</span></span>

<span data-ttu-id="d39d5-120">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d39d5-120">The following is a JSON representation of the resource.</span></span>

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


---
title: Тип ресурса Воркбукоператион
description: Представляет состояние длительных операций с книгой.
localization_priority: Normal
author: grangeryy
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 957f94087fa8c11cf3a5cc794bf194e21bbba346
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48075380"
---
# <a name="workbookoperation-resource-type"></a><span data-ttu-id="65ca9-103">Тип ресурса Воркбукоператион</span><span class="sxs-lookup"><span data-stu-id="65ca9-103">workbookOperation resource type</span></span>

<span data-ttu-id="65ca9-104">Представляет состояние длительной операции с книгой.</span><span class="sxs-lookup"><span data-stu-id="65ca9-104">Represents the status of a long-running workbook operation.</span></span>

## <a name="methods"></a><span data-ttu-id="65ca9-105">Методы</span><span class="sxs-lookup"><span data-stu-id="65ca9-105">Methods</span></span>

| <span data-ttu-id="65ca9-106">Метод</span><span class="sxs-lookup"><span data-stu-id="65ca9-106">Method</span></span>       | <span data-ttu-id="65ca9-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="65ca9-107">Return Type</span></span> | <span data-ttu-id="65ca9-108">Описание</span><span class="sxs-lookup"><span data-stu-id="65ca9-108">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="65ca9-109">Получение Воркбукоператион</span><span class="sxs-lookup"><span data-stu-id="65ca9-109">Get workbookOperation</span></span>](../api/workbookoperation-get.md) | [<span data-ttu-id="65ca9-110">воркбукоператион</span><span class="sxs-lookup"><span data-stu-id="65ca9-110">workbookOperation</span></span>](workbookoperation.md) | <span data-ttu-id="65ca9-111">Получение состояния объекта **воркбукоператион** .</span><span class="sxs-lookup"><span data-stu-id="65ca9-111">Retrieve the status of a **workbookOperation** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="65ca9-112">Свойства</span><span class="sxs-lookup"><span data-stu-id="65ca9-112">Properties</span></span>

| <span data-ttu-id="65ca9-113">Свойство</span><span class="sxs-lookup"><span data-stu-id="65ca9-113">Property</span></span>     | <span data-ttu-id="65ca9-114">Тип</span><span class="sxs-lookup"><span data-stu-id="65ca9-114">Type</span></span>        | <span data-ttu-id="65ca9-115">Описание</span><span class="sxs-lookup"><span data-stu-id="65ca9-115">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="65ca9-116">id</span><span class="sxs-lookup"><span data-stu-id="65ca9-116">id</span></span>|<span data-ttu-id="65ca9-117">String</span><span class="sxs-lookup"><span data-stu-id="65ca9-117">String</span></span>| <span data-ttu-id="65ca9-118">Идентификатор операции. только для чтения.</span><span class="sxs-lookup"><span data-stu-id="65ca9-118">The operation id. Read-only.</span></span>|
|<span data-ttu-id="65ca9-119">status</span><span class="sxs-lookup"><span data-stu-id="65ca9-119">status</span></span>|<span data-ttu-id="65ca9-120">String</span><span class="sxs-lookup"><span data-stu-id="65ca9-120">String</span></span>| <span data-ttu-id="65ca9-121">Текущее состояние операции.</span><span class="sxs-lookup"><span data-stu-id="65ca9-121">The current status of the operation.</span></span> <span data-ttu-id="65ca9-122">Возможные значения: `notStarted`, `running`, `succeeded`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="65ca9-122">Possible values are: `notStarted`, `running`, `succeeded`, `failed`.</span></span>|
|<span data-ttu-id="65ca9-123">error</span><span class="sxs-lookup"><span data-stu-id="65ca9-123">error</span></span>|[<span data-ttu-id="65ca9-124">воркбукоператионеррор</span><span class="sxs-lookup"><span data-stu-id="65ca9-124">workbookOperationError</span></span>](workbookoperationerror.md)| <span data-ttu-id="65ca9-125">Ошибка, возвращенная операцией.</span><span class="sxs-lookup"><span data-stu-id="65ca9-125">The error returned by the operation.</span></span>|
|<span data-ttu-id="65ca9-126">ресаурцелокатион</span><span class="sxs-lookup"><span data-stu-id="65ca9-126">resourceLocation</span></span>|<span data-ttu-id="65ca9-127">String</span><span class="sxs-lookup"><span data-stu-id="65ca9-127">String</span></span>| <span data-ttu-id="65ca9-128">URI ресурса для результата.</span><span class="sxs-lookup"><span data-stu-id="65ca9-128">The resource URI for the result.</span></span>|

## <a name="relationships"></a><span data-ttu-id="65ca9-129">Отношения</span><span class="sxs-lookup"><span data-stu-id="65ca9-129">Relationships</span></span>

<span data-ttu-id="65ca9-130">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="65ca9-130">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="65ca9-131">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="65ca9-131">JSON representation</span></span>

<span data-ttu-id="65ca9-132">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="65ca9-132">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookOperation",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "id": "String (identifier)",
  "status": {"@odata.type": "microsoft.graph.workbookOperationStatus"},
  "error": {"@odata.type": "microsoft.graph.workbookOperationError"},
  "resourceLocation": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "workbookOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->



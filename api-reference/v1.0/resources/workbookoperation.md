---
title: Тип ресурса workbookOperation
description: Представляет состояние длительных операций с книгой.
localization_priority: Normal
author: grangeryy
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: c674186befbb6a24c41cd8741f554876a17a4394
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50158949"
---
# <a name="workbookoperation-resource-type"></a><span data-ttu-id="a59b2-103">Тип ресурса workbookOperation</span><span class="sxs-lookup"><span data-stu-id="a59b2-103">workbookOperation resource type</span></span>

<span data-ttu-id="a59b2-104">Представляет состояние длительной операции с книгой.</span><span class="sxs-lookup"><span data-stu-id="a59b2-104">Represents the status of a long-running workbook operation.</span></span>


## <a name="methods"></a><span data-ttu-id="a59b2-105">Методы</span><span class="sxs-lookup"><span data-stu-id="a59b2-105">Methods</span></span>

| <span data-ttu-id="a59b2-106">Метод</span><span class="sxs-lookup"><span data-stu-id="a59b2-106">Method</span></span>       | <span data-ttu-id="a59b2-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="a59b2-107">Return Type</span></span> | <span data-ttu-id="a59b2-108">Описание</span><span class="sxs-lookup"><span data-stu-id="a59b2-108">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="a59b2-109">Get workbookOperation</span><span class="sxs-lookup"><span data-stu-id="a59b2-109">Get workbookOperation</span></span>](../api/workbookoperation-get.md) | [<span data-ttu-id="a59b2-110">workbookOperation</span><span class="sxs-lookup"><span data-stu-id="a59b2-110">workbookOperation</span></span>](workbookoperation.md) | <span data-ttu-id="a59b2-111">Получите операцию с `{operation-id}` помощью .</span><span class="sxs-lookup"><span data-stu-id="a59b2-111">Get the operation with `{operation-id}`.</span></span> |


## <a name="properties"></a><span data-ttu-id="a59b2-112">Свойства</span><span class="sxs-lookup"><span data-stu-id="a59b2-112">Properties</span></span>

| <span data-ttu-id="a59b2-113">Свойство</span><span class="sxs-lookup"><span data-stu-id="a59b2-113">Property</span></span>     | <span data-ttu-id="a59b2-114">Тип</span><span class="sxs-lookup"><span data-stu-id="a59b2-114">Type</span></span>        | <span data-ttu-id="a59b2-115">Описание</span><span class="sxs-lookup"><span data-stu-id="a59b2-115">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="a59b2-116">status</span><span class="sxs-lookup"><span data-stu-id="a59b2-116">status</span></span>|<span data-ttu-id="a59b2-117">String</span><span class="sxs-lookup"><span data-stu-id="a59b2-117">String</span></span>| <span data-ttu-id="a59b2-118">Текущее состояние операции.</span><span class="sxs-lookup"><span data-stu-id="a59b2-118">The current status of the operation.</span></span> <span data-ttu-id="a59b2-119">Возможные значения: `NotStarted`, `Running`, `Completed`, `Failed`.</span><span class="sxs-lookup"><span data-stu-id="a59b2-119">Possible values are: `NotStarted`, `Running`, `Completed`, `Failed`.</span></span>|
|<span data-ttu-id="a59b2-120">id</span><span class="sxs-lookup"><span data-stu-id="a59b2-120">id</span></span>|<span data-ttu-id="a59b2-121">String</span><span class="sxs-lookup"><span data-stu-id="a59b2-121">String</span></span>| <span data-ttu-id="a59b2-122">ИД операции. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a59b2-122">The operation id. Read-only.</span></span>|
|<span data-ttu-id="a59b2-123">error</span><span class="sxs-lookup"><span data-stu-id="a59b2-123">error</span></span>|[<span data-ttu-id="a59b2-124">workbookOperationError</span><span class="sxs-lookup"><span data-stu-id="a59b2-124">workbookOperationError</span></span>](workbookoperationerror.md)| <span data-ttu-id="a59b2-125">Ошибка, возвращенная операцией.</span><span class="sxs-lookup"><span data-stu-id="a59b2-125">The error returned by the operation.</span></span>|
|<span data-ttu-id="a59b2-126">resourceLocation</span><span class="sxs-lookup"><span data-stu-id="a59b2-126">resourceLocation</span></span>|<span data-ttu-id="a59b2-127">String</span><span class="sxs-lookup"><span data-stu-id="a59b2-127">String</span></span>| <span data-ttu-id="a59b2-128">URI ресурса для результата.</span><span class="sxs-lookup"><span data-stu-id="a59b2-128">The resource URI for the result.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a59b2-129">Связи</span><span class="sxs-lookup"><span data-stu-id="a59b2-129">Relationships</span></span>

<span data-ttu-id="a59b2-130">Нет</span><span class="sxs-lookup"><span data-stu-id="a59b2-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a59b2-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a59b2-131">JSON representation</span></span>

<span data-ttu-id="a59b2-132">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a59b2-132">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookOperation",
  "keyProperty": "id"
}-->

```json
{
  "id": "String (identifier)",
  "status": {"@odata.type": "microsoft.graph.workbookOperationStatus"},
  "error": {"@odata.type": "microsoft.graph.workbookOperationError"},
  "resourceLocation": "String",
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

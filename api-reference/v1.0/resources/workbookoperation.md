---
title: Тип ресурса Воркбукоператион
description: Представляет состояние длительных операций с книгой.
localization_priority: Normal
author: grangeryy
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 4fa98cdfdfc013386f7d615c54c832d27c5f826e
ms.sourcegitcommit: 233ac43db0eb5edd46fe944a5515d7dd9abb1298
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/24/2020
ms.locfileid: "45408164"
---
# <a name="workbookoperation-resource-type"></a><span data-ttu-id="91420-103">Тип ресурса Воркбукоператион</span><span class="sxs-lookup"><span data-stu-id="91420-103">workbookOperation resource type</span></span>

<span data-ttu-id="91420-104">Представляет состояние длительной операции с книгой.</span><span class="sxs-lookup"><span data-stu-id="91420-104">Represents the status of a long-running workbook operation.</span></span>


## <a name="methods"></a><span data-ttu-id="91420-105">Методы</span><span class="sxs-lookup"><span data-stu-id="91420-105">Methods</span></span>

| <span data-ttu-id="91420-106">Метод</span><span class="sxs-lookup"><span data-stu-id="91420-106">Method</span></span>       | <span data-ttu-id="91420-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="91420-107">Return Type</span></span> | <span data-ttu-id="91420-108">Описание</span><span class="sxs-lookup"><span data-stu-id="91420-108">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="91420-109">Получение Воркбукоператион</span><span class="sxs-lookup"><span data-stu-id="91420-109">Get workbookOperation</span></span>](../api/workbookoperation-get.md) | [<span data-ttu-id="91420-110">воркбукоператион</span><span class="sxs-lookup"><span data-stu-id="91420-110">workbookOperation</span></span>](workbookoperation.md) | <span data-ttu-id="91420-111">Получение операции с помощью `{operation-id}` .</span><span class="sxs-lookup"><span data-stu-id="91420-111">Get the operation with `{operation-id}`.</span></span> |


## <a name="properties"></a><span data-ttu-id="91420-112">Свойства</span><span class="sxs-lookup"><span data-stu-id="91420-112">Properties</span></span>

| <span data-ttu-id="91420-113">Свойство</span><span class="sxs-lookup"><span data-stu-id="91420-113">Property</span></span>     | <span data-ttu-id="91420-114">Тип</span><span class="sxs-lookup"><span data-stu-id="91420-114">Type</span></span>        | <span data-ttu-id="91420-115">Описание</span><span class="sxs-lookup"><span data-stu-id="91420-115">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="91420-116">status</span><span class="sxs-lookup"><span data-stu-id="91420-116">status</span></span>|<span data-ttu-id="91420-117">String</span><span class="sxs-lookup"><span data-stu-id="91420-117">String</span></span>| <span data-ttu-id="91420-118">Текущее состояние операции.</span><span class="sxs-lookup"><span data-stu-id="91420-118">The current status of the operation.</span></span> <span data-ttu-id="91420-119">Возможные значения: `NotStarted`, `Running`, `Completed`, `Failed`.</span><span class="sxs-lookup"><span data-stu-id="91420-119">Possible values are: `NotStarted`, `Running`, `Completed`, `Failed`.</span></span>|
|<span data-ttu-id="91420-120">id</span><span class="sxs-lookup"><span data-stu-id="91420-120">id</span></span>|<span data-ttu-id="91420-121">Строка</span><span class="sxs-lookup"><span data-stu-id="91420-121">String</span></span>| <span data-ttu-id="91420-122">Идентификатор операции. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="91420-122">The operation id. Read-only.</span></span>|
|<span data-ttu-id="91420-123">error</span><span class="sxs-lookup"><span data-stu-id="91420-123">error</span></span>|[<span data-ttu-id="91420-124">воркбукоператионеррор</span><span class="sxs-lookup"><span data-stu-id="91420-124">workbookOperationError</span></span>](workbookoperationerror.md)| <span data-ttu-id="91420-125">Ошибка, возвращенная операцией.</span><span class="sxs-lookup"><span data-stu-id="91420-125">The error returned by the operation.</span></span>|
|<span data-ttu-id="91420-126">ресаурцелокатион</span><span class="sxs-lookup"><span data-stu-id="91420-126">resourceLocation</span></span>|<span data-ttu-id="91420-127">Строка</span><span class="sxs-lookup"><span data-stu-id="91420-127">String</span></span>| <span data-ttu-id="91420-128">URI ресурса для результата.</span><span class="sxs-lookup"><span data-stu-id="91420-128">The resource URI for the result.</span></span>|

## <a name="relationships"></a><span data-ttu-id="91420-129">Связи</span><span class="sxs-lookup"><span data-stu-id="91420-129">Relationships</span></span>

<span data-ttu-id="91420-130">Нет</span><span class="sxs-lookup"><span data-stu-id="91420-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="91420-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="91420-131">JSON representation</span></span>

<span data-ttu-id="91420-132">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="91420-132">The following is a JSON representation of the resource.</span></span>

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
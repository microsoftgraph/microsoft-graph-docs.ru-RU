---
title: Тип ресурса Воркбукоператион
description: Представляет состояние длительных операций с книгой.
localization_priority: Normal
author: grangeryy
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 9f186fe1c6c5e7ac917508ed75f6fb8488cbdc94
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48015150"
---
# <a name="workbookoperation-resource-type"></a><span data-ttu-id="23618-103">Тип ресурса Воркбукоператион</span><span class="sxs-lookup"><span data-stu-id="23618-103">workbookOperation resource type</span></span>

<span data-ttu-id="23618-104">Представляет состояние длительной операции с книгой.</span><span class="sxs-lookup"><span data-stu-id="23618-104">Represents the status of a long-running workbook operation.</span></span>


## <a name="methods"></a><span data-ttu-id="23618-105">Методы</span><span class="sxs-lookup"><span data-stu-id="23618-105">Methods</span></span>

| <span data-ttu-id="23618-106">Метод</span><span class="sxs-lookup"><span data-stu-id="23618-106">Method</span></span>       | <span data-ttu-id="23618-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="23618-107">Return Type</span></span> | <span data-ttu-id="23618-108">Описание</span><span class="sxs-lookup"><span data-stu-id="23618-108">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="23618-109">Получение Воркбукоператион</span><span class="sxs-lookup"><span data-stu-id="23618-109">Get workbookOperation</span></span>](../api/workbookoperation-get.md) | [<span data-ttu-id="23618-110">воркбукоператион</span><span class="sxs-lookup"><span data-stu-id="23618-110">workbookOperation</span></span>](workbookoperation.md) | <span data-ttu-id="23618-111">Получение операции с помощью `{operation-id}` .</span><span class="sxs-lookup"><span data-stu-id="23618-111">Get the operation with `{operation-id}`.</span></span> |


## <a name="properties"></a><span data-ttu-id="23618-112">Свойства</span><span class="sxs-lookup"><span data-stu-id="23618-112">Properties</span></span>

| <span data-ttu-id="23618-113">Свойство</span><span class="sxs-lookup"><span data-stu-id="23618-113">Property</span></span>     | <span data-ttu-id="23618-114">Тип</span><span class="sxs-lookup"><span data-stu-id="23618-114">Type</span></span>        | <span data-ttu-id="23618-115">Описание</span><span class="sxs-lookup"><span data-stu-id="23618-115">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="23618-116">status</span><span class="sxs-lookup"><span data-stu-id="23618-116">status</span></span>|<span data-ttu-id="23618-117">String</span><span class="sxs-lookup"><span data-stu-id="23618-117">String</span></span>| <span data-ttu-id="23618-118">Текущее состояние операции.</span><span class="sxs-lookup"><span data-stu-id="23618-118">The current status of the operation.</span></span> <span data-ttu-id="23618-119">Возможные значения: `NotStarted`, `Running`, `Completed`, `Failed`.</span><span class="sxs-lookup"><span data-stu-id="23618-119">Possible values are: `NotStarted`, `Running`, `Completed`, `Failed`.</span></span>|
|<span data-ttu-id="23618-120">id</span><span class="sxs-lookup"><span data-stu-id="23618-120">id</span></span>|<span data-ttu-id="23618-121">String</span><span class="sxs-lookup"><span data-stu-id="23618-121">String</span></span>| <span data-ttu-id="23618-122">Идентификатор операции. только для чтения.</span><span class="sxs-lookup"><span data-stu-id="23618-122">The operation id. Read-only.</span></span>|
|<span data-ttu-id="23618-123">error</span><span class="sxs-lookup"><span data-stu-id="23618-123">error</span></span>|[<span data-ttu-id="23618-124">воркбукоператионеррор</span><span class="sxs-lookup"><span data-stu-id="23618-124">workbookOperationError</span></span>](workbookoperationerror.md)| <span data-ttu-id="23618-125">Ошибка, возвращенная операцией.</span><span class="sxs-lookup"><span data-stu-id="23618-125">The error returned by the operation.</span></span>|
|<span data-ttu-id="23618-126">ресаурцелокатион</span><span class="sxs-lookup"><span data-stu-id="23618-126">resourceLocation</span></span>|<span data-ttu-id="23618-127">String</span><span class="sxs-lookup"><span data-stu-id="23618-127">String</span></span>| <span data-ttu-id="23618-128">URI ресурса для результата.</span><span class="sxs-lookup"><span data-stu-id="23618-128">The resource URI for the result.</span></span>|

## <a name="relationships"></a><span data-ttu-id="23618-129">Связи</span><span class="sxs-lookup"><span data-stu-id="23618-129">Relationships</span></span>

<span data-ttu-id="23618-130">Нет</span><span class="sxs-lookup"><span data-stu-id="23618-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="23618-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="23618-131">JSON representation</span></span>

<span data-ttu-id="23618-132">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="23618-132">The following is a JSON representation of the resource.</span></span>

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

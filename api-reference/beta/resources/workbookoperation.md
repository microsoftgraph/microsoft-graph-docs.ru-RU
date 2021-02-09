---
title: Тип ресурса workbookOperation
description: Представляет состояние длительных операций с книгой.
localization_priority: Normal
author: grangeryy
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 04dc2afc707c4a991f9bb638102bb7180f9b1fab
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50154231"
---
# <a name="workbookoperation-resource-type"></a><span data-ttu-id="236ef-103">Тип ресурса workbookOperation</span><span class="sxs-lookup"><span data-stu-id="236ef-103">workbookOperation resource type</span></span>

<span data-ttu-id="236ef-104">Представляет состояние длительной операции с книгой.</span><span class="sxs-lookup"><span data-stu-id="236ef-104">Represents the status of a long-running workbook operation.</span></span>

## <a name="methods"></a><span data-ttu-id="236ef-105">Методы</span><span class="sxs-lookup"><span data-stu-id="236ef-105">Methods</span></span>

| <span data-ttu-id="236ef-106">Метод</span><span class="sxs-lookup"><span data-stu-id="236ef-106">Method</span></span>       | <span data-ttu-id="236ef-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="236ef-107">Return Type</span></span> | <span data-ttu-id="236ef-108">Описание</span><span class="sxs-lookup"><span data-stu-id="236ef-108">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="236ef-109">Get workbookOperation</span><span class="sxs-lookup"><span data-stu-id="236ef-109">Get workbookOperation</span></span>](../api/workbookoperation-get.md) | [<span data-ttu-id="236ef-110">workbookOperation</span><span class="sxs-lookup"><span data-stu-id="236ef-110">workbookOperation</span></span>](workbookoperation.md) | <span data-ttu-id="236ef-111">Извлечение состояния объекта **workbookOperation.**</span><span class="sxs-lookup"><span data-stu-id="236ef-111">Retrieve the status of a **workbookOperation** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="236ef-112">Свойства</span><span class="sxs-lookup"><span data-stu-id="236ef-112">Properties</span></span>

| <span data-ttu-id="236ef-113">Свойство</span><span class="sxs-lookup"><span data-stu-id="236ef-113">Property</span></span>     | <span data-ttu-id="236ef-114">Тип</span><span class="sxs-lookup"><span data-stu-id="236ef-114">Type</span></span>        | <span data-ttu-id="236ef-115">Описание</span><span class="sxs-lookup"><span data-stu-id="236ef-115">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="236ef-116">id</span><span class="sxs-lookup"><span data-stu-id="236ef-116">id</span></span>|<span data-ttu-id="236ef-117">String</span><span class="sxs-lookup"><span data-stu-id="236ef-117">String</span></span>| <span data-ttu-id="236ef-118">ИД операции. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="236ef-118">The operation id. Read-only.</span></span>|
|<span data-ttu-id="236ef-119">status</span><span class="sxs-lookup"><span data-stu-id="236ef-119">status</span></span>|<span data-ttu-id="236ef-120">String</span><span class="sxs-lookup"><span data-stu-id="236ef-120">String</span></span>| <span data-ttu-id="236ef-121">Текущее состояние операции.</span><span class="sxs-lookup"><span data-stu-id="236ef-121">The current status of the operation.</span></span> <span data-ttu-id="236ef-122">Возможные значения: `notStarted`, `running`, `succeeded`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="236ef-122">Possible values are: `notStarted`, `running`, `succeeded`, `failed`.</span></span>|
|<span data-ttu-id="236ef-123">error</span><span class="sxs-lookup"><span data-stu-id="236ef-123">error</span></span>|[<span data-ttu-id="236ef-124">workbookOperationError</span><span class="sxs-lookup"><span data-stu-id="236ef-124">workbookOperationError</span></span>](workbookoperationerror.md)| <span data-ttu-id="236ef-125">Ошибка, возвращенная операцией.</span><span class="sxs-lookup"><span data-stu-id="236ef-125">The error returned by the operation.</span></span>|
|<span data-ttu-id="236ef-126">resourceLocation</span><span class="sxs-lookup"><span data-stu-id="236ef-126">resourceLocation</span></span>|<span data-ttu-id="236ef-127">String</span><span class="sxs-lookup"><span data-stu-id="236ef-127">String</span></span>| <span data-ttu-id="236ef-128">URI ресурса для результата.</span><span class="sxs-lookup"><span data-stu-id="236ef-128">The resource URI for the result.</span></span>|

## <a name="relationships"></a><span data-ttu-id="236ef-129">Связи</span><span class="sxs-lookup"><span data-stu-id="236ef-129">Relationships</span></span>

<span data-ttu-id="236ef-130">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="236ef-130">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="236ef-131">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="236ef-131">JSON representation</span></span>

<span data-ttu-id="236ef-132">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="236ef-132">The following is a JSON representation of the resource.</span></span>

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



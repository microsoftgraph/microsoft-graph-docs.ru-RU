---
title: Тип ресурса Воркбукоператион
description: Представляет состояние длительных операций с книгой.
localization_priority: Normal
author: grangeryy
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: bd015045b01d0a7f886ecf0f5165a347d76dc061
ms.sourcegitcommit: b469176f49aacbd02cd06838cc7c8d36cf5bc768
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/17/2020
ms.locfileid: "45165149"
---
# <a name="workbookoperation-resource-type"></a><span data-ttu-id="7bd4b-103">Тип ресурса Воркбукоператион</span><span class="sxs-lookup"><span data-stu-id="7bd4b-103">workbookOperation resource type</span></span>

<span data-ttu-id="7bd4b-104">Представляет состояние длительной операции с книгой.</span><span class="sxs-lookup"><span data-stu-id="7bd4b-104">Represents the status of a long-running workbook operation.</span></span>

## <a name="methods"></a><span data-ttu-id="7bd4b-105">Методы</span><span class="sxs-lookup"><span data-stu-id="7bd4b-105">Methods</span></span>

| <span data-ttu-id="7bd4b-106">Метод</span><span class="sxs-lookup"><span data-stu-id="7bd4b-106">Method</span></span>       | <span data-ttu-id="7bd4b-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="7bd4b-107">Return Type</span></span> | <span data-ttu-id="7bd4b-108">Описание</span><span class="sxs-lookup"><span data-stu-id="7bd4b-108">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="7bd4b-109">Получение Воркбукоператион</span><span class="sxs-lookup"><span data-stu-id="7bd4b-109">Get workbookOperation</span></span>](../api/workbookoperation-get.md) | [<span data-ttu-id="7bd4b-110">воркбукоператион</span><span class="sxs-lookup"><span data-stu-id="7bd4b-110">workbookOperation</span></span>](workbookoperation.md) | <span data-ttu-id="7bd4b-111">Получение состояния объекта **воркбукоператион** .</span><span class="sxs-lookup"><span data-stu-id="7bd4b-111">Retrieve the status of a **workbookOperation** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="7bd4b-112">Свойства</span><span class="sxs-lookup"><span data-stu-id="7bd4b-112">Properties</span></span>

| <span data-ttu-id="7bd4b-113">Свойство</span><span class="sxs-lookup"><span data-stu-id="7bd4b-113">Property</span></span>     | <span data-ttu-id="7bd4b-114">Тип</span><span class="sxs-lookup"><span data-stu-id="7bd4b-114">Type</span></span>        | <span data-ttu-id="7bd4b-115">Описание</span><span class="sxs-lookup"><span data-stu-id="7bd4b-115">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="7bd4b-116">id</span><span class="sxs-lookup"><span data-stu-id="7bd4b-116">id</span></span>|<span data-ttu-id="7bd4b-117">Строка</span><span class="sxs-lookup"><span data-stu-id="7bd4b-117">String</span></span>| <span data-ttu-id="7bd4b-118">Идентификатор операции. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7bd4b-118">The operation id. Read-only.</span></span>|
|<span data-ttu-id="7bd4b-119">status</span><span class="sxs-lookup"><span data-stu-id="7bd4b-119">status</span></span>|<span data-ttu-id="7bd4b-120">String</span><span class="sxs-lookup"><span data-stu-id="7bd4b-120">String</span></span>| <span data-ttu-id="7bd4b-121">Текущее состояние операции.</span><span class="sxs-lookup"><span data-stu-id="7bd4b-121">The current status of the operation.</span></span> <span data-ttu-id="7bd4b-122">Возможные значения: `notStarted`, `running`, `succeeded`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="7bd4b-122">Possible values are: `notStarted`, `running`, `succeeded`, `failed`.</span></span>|
|<span data-ttu-id="7bd4b-123">error</span><span class="sxs-lookup"><span data-stu-id="7bd4b-123">error</span></span>|[<span data-ttu-id="7bd4b-124">воркбукоператионеррор</span><span class="sxs-lookup"><span data-stu-id="7bd4b-124">workbookOperationError</span></span>](workbookoperationerror.md)| <span data-ttu-id="7bd4b-125">Ошибка, возвращенная операцией.</span><span class="sxs-lookup"><span data-stu-id="7bd4b-125">The error returned by the operation.</span></span>|
|<span data-ttu-id="7bd4b-126">ресаурцелокатион</span><span class="sxs-lookup"><span data-stu-id="7bd4b-126">resourceLocation</span></span>|<span data-ttu-id="7bd4b-127">String</span><span class="sxs-lookup"><span data-stu-id="7bd4b-127">String</span></span>| <span data-ttu-id="7bd4b-128">URI ресурса для результата.</span><span class="sxs-lookup"><span data-stu-id="7bd4b-128">The resource URI for the result.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7bd4b-129">Связи</span><span class="sxs-lookup"><span data-stu-id="7bd4b-129">Relationships</span></span>

<span data-ttu-id="7bd4b-130">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="7bd4b-130">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="7bd4b-131">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="7bd4b-131">JSON representation</span></span>

<span data-ttu-id="7bd4b-132">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7bd4b-132">The following is a JSON representation of the resource.</span></span>

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

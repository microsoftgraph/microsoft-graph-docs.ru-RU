---
title: Тип ресурса onenoteOperation
description: Состояние определенных операций OneNote, выполняющихся в течение длительного времени.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: 9fb490d38b975291b8f3b710f5e2f702f0fee7df
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27962263"
---
# <a name="onenoteoperation-resource-type"></a><span data-ttu-id="3d77b-103">Тип ресурса onenoteOperation</span><span class="sxs-lookup"><span data-stu-id="3d77b-103">onenoteOperation resource type</span></span>

> <span data-ttu-id="3d77b-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="3d77b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3d77b-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3d77b-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3d77b-106">Состояние определенных операций OneNote, выполняющихся в течение длительного времени.</span><span class="sxs-lookup"><span data-stu-id="3d77b-106">The status of certain long-running OneNote operations.</span></span>

## <a name="json-representation"></a><span data-ttu-id="3d77b-107">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="3d77b-107">JSON representation</span></span>

<span data-ttu-id="3d77b-108">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3d77b-108">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onenoteOperation"
}-->

```json
{
  "createdDateTime": "String (timestamp)",
  "error": {"@odata.type": "microsoft.graph.onenoteOperationError"},
  "id": "string (identifier)",
  "lastActionDateTime": "String (timestamp)",
  "resourceId": "string",
  "resourceLocation": "string",
  "status": "string",
  "percentComplete": "string"
}

```
## <a name="properties"></a><span data-ttu-id="3d77b-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="3d77b-109">Properties</span></span>
| <span data-ttu-id="3d77b-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="3d77b-110">Property</span></span>     | <span data-ttu-id="3d77b-111">Тип</span><span class="sxs-lookup"><span data-stu-id="3d77b-111">Type</span></span>   |<span data-ttu-id="3d77b-112">Описание</span><span class="sxs-lookup"><span data-stu-id="3d77b-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3d77b-113">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3d77b-113">createdDateTime</span></span>| <span data-ttu-id="3d77b-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3d77b-114">DateTimeOffset</span></span> |<span data-ttu-id="3d77b-115">Время начала операции.</span><span class="sxs-lookup"><span data-stu-id="3d77b-115">The start time of the operation.</span></span>|
|<span data-ttu-id="3d77b-116">error</span><span class="sxs-lookup"><span data-stu-id="3d77b-116">error</span></span>|[<span data-ttu-id="3d77b-117">onenoteOperationError</span><span class="sxs-lookup"><span data-stu-id="3d77b-117">onenoteOperationError</span></span>](onenoteoperationerror.md)|<span data-ttu-id="3d77b-118">Ошибка при выполнении операции.</span><span class="sxs-lookup"><span data-stu-id="3d77b-118">The error returned by the operation.</span></span>|
|<span data-ttu-id="3d77b-119">id</span><span class="sxs-lookup"><span data-stu-id="3d77b-119">id</span></span>|<span data-ttu-id="3d77b-120">строка</span><span class="sxs-lookup"><span data-stu-id="3d77b-120">string</span></span>|<span data-ttu-id="3d77b-121">Идентификатор операции. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3d77b-121">The operation id. Read-only.</span></span>|
|<span data-ttu-id="3d77b-122">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="3d77b-122">lastActionDateTime</span></span>| <span data-ttu-id="3d77b-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3d77b-123">DateTimeOffset</span></span> |<span data-ttu-id="3d77b-124">Время последнего действия операции.</span><span class="sxs-lookup"><span data-stu-id="3d77b-124">The time of the last action of the operation.</span></span>|
|<span data-ttu-id="3d77b-125">resourceId</span><span class="sxs-lookup"><span data-stu-id="3d77b-125">resourceId</span></span>|<span data-ttu-id="3d77b-126">строка</span><span class="sxs-lookup"><span data-stu-id="3d77b-126">string</span></span>|<span data-ttu-id="3d77b-127">Идентификатор ресурса.</span><span class="sxs-lookup"><span data-stu-id="3d77b-127">The resource id.</span></span>|
|<span data-ttu-id="3d77b-128">resourceLocation</span><span class="sxs-lookup"><span data-stu-id="3d77b-128">resourceLocation</span></span>|<span data-ttu-id="3d77b-129">строка</span><span class="sxs-lookup"><span data-stu-id="3d77b-129">string</span></span>|<span data-ttu-id="3d77b-p102">URI ресурса для объекта. Например, URI ресурса для скопированной страницы или раздела.</span><span class="sxs-lookup"><span data-stu-id="3d77b-p102">The resource URI for the object. For example, the resource URI for a copied page or section.</span></span> |
|<span data-ttu-id="3d77b-132">status</span><span class="sxs-lookup"><span data-stu-id="3d77b-132">status</span></span>|<span data-ttu-id="3d77b-133">строка</span><span class="sxs-lookup"><span data-stu-id="3d77b-133">string</span></span>|<span data-ttu-id="3d77b-134">Текущее состояние операции: `notstarted`, `running`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="3d77b-134">The current status of the operation: `notstarted`, `running`, `completed`, `failed`</span></span> |
|<span data-ttu-id="3d77b-135">percentComplete</span><span class="sxs-lookup"><span data-stu-id="3d77b-135">percentComplete</span></span>|<span data-ttu-id="3d77b-136">строка</span><span class="sxs-lookup"><span data-stu-id="3d77b-136">string</span></span>|<span data-ttu-id="3d77b-137">Процент завершения операции, если операция в состоянии `running`.</span><span class="sxs-lookup"><span data-stu-id="3d77b-137">The operation percent complete if the operation is still in `running` status</span></span>

## <a name="relationships"></a><span data-ttu-id="3d77b-138">Связи</span><span class="sxs-lookup"><span data-stu-id="3d77b-138">Relationships</span></span>
<span data-ttu-id="3d77b-139">Нет</span><span class="sxs-lookup"><span data-stu-id="3d77b-139">None</span></span>


## <a name="methods"></a><span data-ttu-id="3d77b-140">Методы</span><span class="sxs-lookup"><span data-stu-id="3d77b-140">Methods</span></span>

| <span data-ttu-id="3d77b-141">Метод</span><span class="sxs-lookup"><span data-stu-id="3d77b-141">Method</span></span>           | <span data-ttu-id="3d77b-142">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="3d77b-142">Return Type</span></span>    |<span data-ttu-id="3d77b-143">Описание</span><span class="sxs-lookup"><span data-stu-id="3d77b-143">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="3d77b-144">Получение операции</span><span class="sxs-lookup"><span data-stu-id="3d77b-144">Get operation</span></span>](../api/onenoteoperation-get.md) | [<span data-ttu-id="3d77b-145">onenoteOperation</span><span class="sxs-lookup"><span data-stu-id="3d77b-145">onenoteOperation</span></span>](onenoteoperation.md) |<span data-ttu-id="3d77b-146">Получение состояния операции.</span><span class="sxs-lookup"><span data-stu-id="3d77b-146">Get the status of the operation.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onenoteOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

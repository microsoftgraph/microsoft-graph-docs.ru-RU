---
title: Тип ресурса dataPolicyOperation
description: Представляет операцию политики отправленных данных. Он содержит сведения, необходимые для отслеживания состояния операции. Например администратор компании запрос данных политики операции экспорта данных сотрудника компании и затем отслеживать этот запрос.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 4547221c8c1b859d4738a5468603ac6890246263
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2019
ms.locfileid: "29570927"
---
# <a name="datapolicyoperation-resource-type"></a><span data-ttu-id="5f991-105">Тип ресурса dataPolicyOperation</span><span class="sxs-lookup"><span data-stu-id="5f991-105">dataPolicyOperation resource type</span></span>

<span data-ttu-id="5f991-106">Представляет операцию политики отправленных данных.</span><span class="sxs-lookup"><span data-stu-id="5f991-106">Represents a submitted data policy operation.</span></span> <span data-ttu-id="5f991-107">Он содержит сведения, необходимые для отслеживания состояния операции.</span><span class="sxs-lookup"><span data-stu-id="5f991-107">It contains necessary information for tracking the status of an operation.</span></span> <span data-ttu-id="5f991-108">Например администратор компании запрос данных политики операции экспорта данных сотрудника компании и затем отслеживать этот запрос.</span><span class="sxs-lookup"><span data-stu-id="5f991-108">For example, a company administrator can submit a data policy operation request to export an employee's company data, and then later track that request.</span></span>

## <a name="methods"></a><span data-ttu-id="5f991-109">Методы</span><span class="sxs-lookup"><span data-stu-id="5f991-109">Methods</span></span>

| <span data-ttu-id="5f991-110">Метод</span><span class="sxs-lookup"><span data-stu-id="5f991-110">Method</span></span>           | <span data-ttu-id="5f991-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="5f991-111">Return Type</span></span>    |<span data-ttu-id="5f991-112">Описание</span><span class="sxs-lookup"><span data-stu-id="5f991-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="5f991-113">Получение dataPolicyOperation</span><span class="sxs-lookup"><span data-stu-id="5f991-113">Get dataPolicyOperation</span></span>](../api/datapolicyoperation-get.md) | [<span data-ttu-id="5f991-114">dataPolicyOperation</span><span class="sxs-lookup"><span data-stu-id="5f991-114">dataPolicyOperation</span></span>](datapolicyoperation.md) |<span data-ttu-id="5f991-115">Чтение свойств объекта dataPolicyOperation.</span><span class="sxs-lookup"><span data-stu-id="5f991-115">Read properties of the dataPolicyOperation object.</span></span>|

## <a name="properties"></a><span data-ttu-id="5f991-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="5f991-116">Properties</span></span>

> <span data-ttu-id="5f991-117">**Примечание:** Все свойства в этом ресурсов доступны только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5f991-117">**Note:** All properties of this resource are read-only.</span></span>

| <span data-ttu-id="5f991-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="5f991-118">Property</span></span>     | <span data-ttu-id="5f991-119">Тип</span><span class="sxs-lookup"><span data-stu-id="5f991-119">Type</span></span>   |<span data-ttu-id="5f991-120">Описание</span><span class="sxs-lookup"><span data-stu-id="5f991-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5f991-121">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="5f991-121">completedDateTime</span></span>|<span data-ttu-id="5f991-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5f991-122">DateTimeOffset</span></span>|<span data-ttu-id="5f991-123">Представляет, когда запрос для этой операции политики данных был выполнен, в формате UTC, в формате ISO 8601.</span><span class="sxs-lookup"><span data-stu-id="5f991-123">Represents when the request for this data policy operation was completed, in UTC time, using the ISO 8601 format.</span></span> <span data-ttu-id="5f991-124">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="5f991-124">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="5f991-125">NULL до завершения операции.</span><span class="sxs-lookup"><span data-stu-id="5f991-125">Null until the operation completes.</span></span>|
|<span data-ttu-id="5f991-126">id</span><span class="sxs-lookup"><span data-stu-id="5f991-126">id</span></span>|<span data-ttu-id="5f991-127">Строка</span><span class="sxs-lookup"><span data-stu-id="5f991-127">String</span></span>| <span data-ttu-id="5f991-128">Уникальный ключ для этой операции.</span><span class="sxs-lookup"><span data-stu-id="5f991-128">Unique key for this operation.</span></span> |
|<span data-ttu-id="5f991-129">status</span><span class="sxs-lookup"><span data-stu-id="5f991-129">status</span></span>|<span data-ttu-id="5f991-130">string</span><span class="sxs-lookup"><span data-stu-id="5f991-130">string</span></span>| <span data-ttu-id="5f991-131">Возможные значения: `notStarted`, `running`, `complete`, `failed`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="5f991-131">Possible values are: `notStarted`, `running`, `complete`, `failed`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="5f991-132">storageLocation</span><span class="sxs-lookup"><span data-stu-id="5f991-132">storageLocation</span></span>|<span data-ttu-id="5f991-133">Строка</span><span class="sxs-lookup"><span data-stu-id="5f991-133">String</span></span>|<span data-ttu-id="5f991-134">URL-адрес расположения, в котором выполняется экспорт данных для запросы на экспорт.</span><span class="sxs-lookup"><span data-stu-id="5f991-134">The URL location to where data is being exported for export requests.</span></span>|
|<span data-ttu-id="5f991-135">userId</span><span class="sxs-lookup"><span data-stu-id="5f991-135">userId</span></span>|<span data-ttu-id="5f991-136">String</span><span class="sxs-lookup"><span data-stu-id="5f991-136">String</span></span>|<span data-ttu-id="5f991-137">Идентификатор пользователя, для которого выполняется операция.</span><span class="sxs-lookup"><span data-stu-id="5f991-137">The id for the user on whom the operation is performed.</span></span>|
|<span data-ttu-id="5f991-138">submittedDateTime</span><span class="sxs-lookup"><span data-stu-id="5f991-138">submittedDateTime</span></span>|<span data-ttu-id="5f991-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5f991-139">DateTimeOffset</span></span>|<span data-ttu-id="5f991-140">Представляет, когда для этой операции с данными был отправлен запрос, в формате UTC, в формате ISO 8601.</span><span class="sxs-lookup"><span data-stu-id="5f991-140">Represents when the request for this data operation was submitted, in UTC time, using the ISO 8601 format.</span></span> <span data-ttu-id="5f991-141">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="5f991-141">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|

## <a name="relationships"></a><span data-ttu-id="5f991-142">Связи</span><span class="sxs-lookup"><span data-stu-id="5f991-142">Relationships</span></span>
<span data-ttu-id="5f991-143">Нет</span><span class="sxs-lookup"><span data-stu-id="5f991-143">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="5f991-144">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5f991-144">JSON representation</span></span>

<span data-ttu-id="5f991-145">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5f991-145">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.dataPolicyOperation"
}-->

```json
{
  "completedDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "status": "string",
  "storageLocation": "String",
  "userId": "String",
  "submittedDateTime": "String (timestamp)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "dataPolicyOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

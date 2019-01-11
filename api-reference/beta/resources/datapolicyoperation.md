---
title: Тип ресурса dataPolicyOperation
description: Представляет операцию политики отправленных данных. Он содержит сведения, необходимые для отслеживания состояния операции. Например администратор компании запрос данных политики операции экспорта данных сотрудника компании и затем отслеживать этот запрос.
localization_priority: Normal
ms.openlocfilehash: b56cfe766bbfcae9339805dd61ce816e372d02f4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27876008"
---
# <a name="datapolicyoperation-resource-type"></a><span data-ttu-id="aadfa-105">Тип ресурса dataPolicyOperation</span><span class="sxs-lookup"><span data-stu-id="aadfa-105">dataPolicyOperation resource type</span></span>

<span data-ttu-id="aadfa-106">Представляет операцию политики отправленных данных.</span><span class="sxs-lookup"><span data-stu-id="aadfa-106">Represents a submitted data policy operation.</span></span> <span data-ttu-id="aadfa-107">Он содержит сведения, необходимые для отслеживания состояния операции.</span><span class="sxs-lookup"><span data-stu-id="aadfa-107">It contains necessary information for tracking the status of an operation.</span></span> <span data-ttu-id="aadfa-108">Например администратор компании запрос данных политики операции экспорта данных сотрудника компании и затем отслеживать этот запрос.</span><span class="sxs-lookup"><span data-stu-id="aadfa-108">For example, a company administrator can submit a data policy operation request to export an employee's company data, and then later track that request.</span></span>

## <a name="methods"></a><span data-ttu-id="aadfa-109">Методы</span><span class="sxs-lookup"><span data-stu-id="aadfa-109">Methods</span></span>

| <span data-ttu-id="aadfa-110">Метод</span><span class="sxs-lookup"><span data-stu-id="aadfa-110">Method</span></span>           | <span data-ttu-id="aadfa-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="aadfa-111">Return Type</span></span>    |<span data-ttu-id="aadfa-112">Описание</span><span class="sxs-lookup"><span data-stu-id="aadfa-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="aadfa-113">Получение dataPolicyOperation</span><span class="sxs-lookup"><span data-stu-id="aadfa-113">Get dataPolicyOperation</span></span>](../api/datapolicyoperation-get.md) | [<span data-ttu-id="aadfa-114">dataPolicyOperation</span><span class="sxs-lookup"><span data-stu-id="aadfa-114">dataPolicyOperation</span></span>](datapolicyoperation.md) |<span data-ttu-id="aadfa-115">Чтение свойств объекта dataPolicyOperation.</span><span class="sxs-lookup"><span data-stu-id="aadfa-115">Read properties of the dataPolicyOperation object.</span></span>|

## <a name="properties"></a><span data-ttu-id="aadfa-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="aadfa-116">Properties</span></span>

> <span data-ttu-id="aadfa-117">**Примечание:** Все свойства в этом ресурсов доступны только для чтения.</span><span class="sxs-lookup"><span data-stu-id="aadfa-117">**Note:** All properties of this resource are read-only.</span></span>

| <span data-ttu-id="aadfa-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="aadfa-118">Property</span></span>     | <span data-ttu-id="aadfa-119">Тип</span><span class="sxs-lookup"><span data-stu-id="aadfa-119">Type</span></span>   |<span data-ttu-id="aadfa-120">Описание</span><span class="sxs-lookup"><span data-stu-id="aadfa-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="aadfa-121">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="aadfa-121">completedDateTime</span></span>|<span data-ttu-id="aadfa-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aadfa-122">DateTimeOffset</span></span>|<span data-ttu-id="aadfa-123">Представляет, когда запрос для этой операции политики данных был выполнен, в формате UTC, в формате ISO 8601.</span><span class="sxs-lookup"><span data-stu-id="aadfa-123">Represents when the request for this data policy operation was completed, in UTC time, using the ISO 8601 format.</span></span> <span data-ttu-id="aadfa-124">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="aadfa-124">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="aadfa-125">NULL до завершения операции.</span><span class="sxs-lookup"><span data-stu-id="aadfa-125">Null until the operation completes.</span></span>|
|<span data-ttu-id="aadfa-126">id</span><span class="sxs-lookup"><span data-stu-id="aadfa-126">id</span></span>|<span data-ttu-id="aadfa-127">Строка</span><span class="sxs-lookup"><span data-stu-id="aadfa-127">String</span></span>| <span data-ttu-id="aadfa-128">Уникальный ключ для этой операции.</span><span class="sxs-lookup"><span data-stu-id="aadfa-128">Unique key for this operation.</span></span> |
|<span data-ttu-id="aadfa-129">status</span><span class="sxs-lookup"><span data-stu-id="aadfa-129">status</span></span>|<span data-ttu-id="aadfa-130">string</span><span class="sxs-lookup"><span data-stu-id="aadfa-130">string</span></span>| <span data-ttu-id="aadfa-131">Возможные значения: `notStarted`, `running`, `complete`, `failed`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="aadfa-131">Possible values are: `notStarted`, `running`, `complete`, `failed`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="aadfa-132">storageLocation</span><span class="sxs-lookup"><span data-stu-id="aadfa-132">storageLocation</span></span>|<span data-ttu-id="aadfa-133">Строка</span><span class="sxs-lookup"><span data-stu-id="aadfa-133">String</span></span>|<span data-ttu-id="aadfa-134">URL-адрес расположения, в котором выполняется экспорт данных для запросы на экспорт.</span><span class="sxs-lookup"><span data-stu-id="aadfa-134">The URL location to where data is being exported for export requests.</span></span>|
|<span data-ttu-id="aadfa-135">userId</span><span class="sxs-lookup"><span data-stu-id="aadfa-135">userId</span></span>|<span data-ttu-id="aadfa-136">String</span><span class="sxs-lookup"><span data-stu-id="aadfa-136">String</span></span>|<span data-ttu-id="aadfa-137">Идентификатор пользователя, для которого выполняется операция.</span><span class="sxs-lookup"><span data-stu-id="aadfa-137">The id for the user on whom the operation is performed.</span></span>|
|<span data-ttu-id="aadfa-138">submittedDateTime</span><span class="sxs-lookup"><span data-stu-id="aadfa-138">submittedDateTime</span></span>|<span data-ttu-id="aadfa-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aadfa-139">DateTimeOffset</span></span>|<span data-ttu-id="aadfa-140">Представляет, когда для этой операции с данными был отправлен запрос, в формате UTC, в формате ISO 8601.</span><span class="sxs-lookup"><span data-stu-id="aadfa-140">Represents when the request for this data operation was submitted, in UTC time, using the ISO 8601 format.</span></span> <span data-ttu-id="aadfa-141">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="aadfa-141">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="aadfa-142">progress</span><span class="sxs-lookup"><span data-stu-id="aadfa-142">progress</span></span>|<span data-ttu-id="aadfa-143">Double</span><span class="sxs-lookup"><span data-stu-id="aadfa-143">Double</span></span>|<span data-ttu-id="aadfa-144">Указывает ход выполнения операции.</span><span class="sxs-lookup"><span data-stu-id="aadfa-144">Specifies the progress of an operation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="aadfa-145">Связи</span><span class="sxs-lookup"><span data-stu-id="aadfa-145">Relationships</span></span>
<span data-ttu-id="aadfa-146">Нет</span><span class="sxs-lookup"><span data-stu-id="aadfa-146">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="aadfa-147">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="aadfa-147">JSON representation</span></span>

<span data-ttu-id="aadfa-148">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="aadfa-148">Here is a JSON representation of the resource.</span></span>

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
  "submittedDateTime": "String (timestamp)",
  "progress": "Double"
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

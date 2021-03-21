---
title: тип ресурса dataPolicyOperation
description: Представляет собой операцию по отправке политики данных. Он содержит необходимые сведения для отслеживания состояния операции. Например, администратор компании может отправить запрос на операцию политики данных для экспорта данных компании сотрудника, а затем отслеживать этот запрос.
localization_priority: Normal
author: dkershaw10
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: f12d83ace221a64754e4227ff292e780abf7ea82
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50962632"
---
# <a name="datapolicyoperation-resource-type"></a><span data-ttu-id="ff4f6-105">тип ресурса dataPolicyOperation</span><span class="sxs-lookup"><span data-stu-id="ff4f6-105">dataPolicyOperation resource type</span></span>

<span data-ttu-id="ff4f6-106">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ff4f6-106">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ff4f6-107">Представляет собой операцию по отправке политики данных.</span><span class="sxs-lookup"><span data-stu-id="ff4f6-107">Represents a submitted data policy operation.</span></span> <span data-ttu-id="ff4f6-108">Он содержит необходимые сведения для отслеживания состояния операции.</span><span class="sxs-lookup"><span data-stu-id="ff4f6-108">It contains necessary information for tracking the status of an operation.</span></span> <span data-ttu-id="ff4f6-109">Например, администратор компании может отправить запрос на операцию политики данных для экспорта данных компании сотрудника, а затем отслеживать этот запрос.</span><span class="sxs-lookup"><span data-stu-id="ff4f6-109">For example, a company administrator can submit a data policy operation request to export an employee's company data, and then later track that request.</span></span>

## <a name="methods"></a><span data-ttu-id="ff4f6-110">Методы</span><span class="sxs-lookup"><span data-stu-id="ff4f6-110">Methods</span></span>

| <span data-ttu-id="ff4f6-111">Метод</span><span class="sxs-lookup"><span data-stu-id="ff4f6-111">Method</span></span>           | <span data-ttu-id="ff4f6-112">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="ff4f6-112">Return Type</span></span>    |<span data-ttu-id="ff4f6-113">Описание</span><span class="sxs-lookup"><span data-stu-id="ff4f6-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ff4f6-114">Get dataPolicyOperation</span><span class="sxs-lookup"><span data-stu-id="ff4f6-114">Get dataPolicyOperation</span></span>](../api/datapolicyoperation-get.md) | [<span data-ttu-id="ff4f6-115">dataPolicyOperation</span><span class="sxs-lookup"><span data-stu-id="ff4f6-115">dataPolicyOperation</span></span>](datapolicyoperation.md) |<span data-ttu-id="ff4f6-116">Чтение свойств объекта dataPolicyOperation.</span><span class="sxs-lookup"><span data-stu-id="ff4f6-116">Read properties of the dataPolicyOperation object.</span></span>|

## <a name="properties"></a><span data-ttu-id="ff4f6-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="ff4f6-117">Properties</span></span>

> <span data-ttu-id="ff4f6-118">**Примечание:** Все свойства этого ресурса являются только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ff4f6-118">**Note:** All properties of this resource are read-only.</span></span>

| <span data-ttu-id="ff4f6-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="ff4f6-119">Property</span></span>     | <span data-ttu-id="ff4f6-120">Тип</span><span class="sxs-lookup"><span data-stu-id="ff4f6-120">Type</span></span>   |<span data-ttu-id="ff4f6-121">Описание</span><span class="sxs-lookup"><span data-stu-id="ff4f6-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ff4f6-122">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="ff4f6-122">completedDateTime</span></span>|<span data-ttu-id="ff4f6-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ff4f6-123">DateTimeOffset</span></span>|<span data-ttu-id="ff4f6-124">Представляет, когда запрос на эту операцию политики данных был выполнен во время UTC с помощью формата ISO 8601.</span><span class="sxs-lookup"><span data-stu-id="ff4f6-124">Represents when the request for this data policy operation was completed, in UTC time, using the ISO 8601 format.</span></span> <span data-ttu-id="ff4f6-125">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="ff4f6-125">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="ff4f6-126">Null до завершения операции.</span><span class="sxs-lookup"><span data-stu-id="ff4f6-126">Null until the operation completes.</span></span>|
|<span data-ttu-id="ff4f6-127">id</span><span class="sxs-lookup"><span data-stu-id="ff4f6-127">id</span></span>|<span data-ttu-id="ff4f6-128">Строка</span><span class="sxs-lookup"><span data-stu-id="ff4f6-128">String</span></span>| <span data-ttu-id="ff4f6-129">Уникальный ключ для этой операции.</span><span class="sxs-lookup"><span data-stu-id="ff4f6-129">Unique key for this operation.</span></span> |
|<span data-ttu-id="ff4f6-130">status</span><span class="sxs-lookup"><span data-stu-id="ff4f6-130">status</span></span>|<span data-ttu-id="ff4f6-131">dataPolicyOperationStatus</span><span class="sxs-lookup"><span data-stu-id="ff4f6-131">dataPolicyOperationStatus</span></span>| <span data-ttu-id="ff4f6-132">Возможные значения: `notStarted`, `running`, `complete`, `failed`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="ff4f6-132">Possible values are: `notStarted`, `running`, `complete`, `failed`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="ff4f6-133">storageLocation</span><span class="sxs-lookup"><span data-stu-id="ff4f6-133">storageLocation</span></span>|<span data-ttu-id="ff4f6-134">Строка</span><span class="sxs-lookup"><span data-stu-id="ff4f6-134">String</span></span>|<span data-ttu-id="ff4f6-135">Расположение URL-адреса, куда экспортируются данные для запросов на экспорт.</span><span class="sxs-lookup"><span data-stu-id="ff4f6-135">The URL location to where data is being exported for export requests.</span></span>|
|<span data-ttu-id="ff4f6-136">userId</span><span class="sxs-lookup"><span data-stu-id="ff4f6-136">userId</span></span>|<span data-ttu-id="ff4f6-137">String</span><span class="sxs-lookup"><span data-stu-id="ff4f6-137">String</span></span>|<span data-ttu-id="ff4f6-138">ID для пользователя, на котором выполняется операция.</span><span class="sxs-lookup"><span data-stu-id="ff4f6-138">The id for the user on whom the operation is performed.</span></span>|
|<span data-ttu-id="ff4f6-139">submittedDateTime</span><span class="sxs-lookup"><span data-stu-id="ff4f6-139">submittedDateTime</span></span>|<span data-ttu-id="ff4f6-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ff4f6-140">DateTimeOffset</span></span>|<span data-ttu-id="ff4f6-141">Представляет при отправке запроса на эту операцию данных во время UTC с помощью формата ISO 8601.</span><span class="sxs-lookup"><span data-stu-id="ff4f6-141">Represents when the request for this data operation was submitted, in UTC time, using the ISO 8601 format.</span></span> <span data-ttu-id="ff4f6-142">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="ff4f6-142">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="ff4f6-143">progress</span><span class="sxs-lookup"><span data-stu-id="ff4f6-143">progress</span></span>|<span data-ttu-id="ff4f6-144">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="ff4f6-144">Double</span></span>|<span data-ttu-id="ff4f6-145">Указывает ход операции.</span><span class="sxs-lookup"><span data-stu-id="ff4f6-145">Specifies the progress of an operation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ff4f6-146">Связи</span><span class="sxs-lookup"><span data-stu-id="ff4f6-146">Relationships</span></span>
<span data-ttu-id="ff4f6-147">Нет</span><span class="sxs-lookup"><span data-stu-id="ff4f6-147">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="ff4f6-148">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ff4f6-148">JSON representation</span></span>

<span data-ttu-id="ff4f6-149">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ff4f6-149">Here is a JSON representation of the resource.</span></span>

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



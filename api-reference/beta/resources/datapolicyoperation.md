---
title: тип ресурса dataPolicyOperation
description: Представляет собой операцию по отправке политики данных. Он содержит необходимые сведения для отслеживания состояния операции. Например, администратор компании может отправить запрос на операцию политики данных для экспорта данных компании сотрудника, а затем отслеживать этот запрос.
localization_priority: Normal
author: dkershaw10
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 498d03180eca9a0508f513f0051a6f9b0079b45d
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50720706"
---
# <a name="datapolicyoperation-resource-type"></a><span data-ttu-id="dd27d-105">тип ресурса dataPolicyOperation</span><span class="sxs-lookup"><span data-stu-id="dd27d-105">dataPolicyOperation resource type</span></span>

<span data-ttu-id="dd27d-106">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dd27d-106">Namespace: microsoft.graph</span></span>

<span data-ttu-id="dd27d-107">Представляет собой операцию по отправке политики данных.</span><span class="sxs-lookup"><span data-stu-id="dd27d-107">Represents a submitted data policy operation.</span></span> <span data-ttu-id="dd27d-108">Он содержит необходимые сведения для отслеживания состояния операции.</span><span class="sxs-lookup"><span data-stu-id="dd27d-108">It contains necessary information for tracking the status of an operation.</span></span> <span data-ttu-id="dd27d-109">Например, администратор компании может отправить запрос на операцию политики данных для экспорта данных компании сотрудника, а затем отслеживать этот запрос.</span><span class="sxs-lookup"><span data-stu-id="dd27d-109">For example, a company administrator can submit a data policy operation request to export an employee's company data, and then later track that request.</span></span>

## <a name="methods"></a><span data-ttu-id="dd27d-110">Методы</span><span class="sxs-lookup"><span data-stu-id="dd27d-110">Methods</span></span>

| <span data-ttu-id="dd27d-111">Метод</span><span class="sxs-lookup"><span data-stu-id="dd27d-111">Method</span></span>           | <span data-ttu-id="dd27d-112">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="dd27d-112">Return Type</span></span>    |<span data-ttu-id="dd27d-113">Описание</span><span class="sxs-lookup"><span data-stu-id="dd27d-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="dd27d-114">Get dataPolicyOperation</span><span class="sxs-lookup"><span data-stu-id="dd27d-114">Get dataPolicyOperation</span></span>](../api/datapolicyoperation-get.md) | [<span data-ttu-id="dd27d-115">dataPolicyOperation</span><span class="sxs-lookup"><span data-stu-id="dd27d-115">dataPolicyOperation</span></span>](datapolicyoperation.md) |<span data-ttu-id="dd27d-116">Чтение свойств объекта dataPolicyOperation.</span><span class="sxs-lookup"><span data-stu-id="dd27d-116">Read properties of the dataPolicyOperation object.</span></span>|

## <a name="properties"></a><span data-ttu-id="dd27d-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="dd27d-117">Properties</span></span>

> <span data-ttu-id="dd27d-118">**Примечание:** Все свойства этого ресурса являются только для чтения.</span><span class="sxs-lookup"><span data-stu-id="dd27d-118">**Note:** All properties of this resource are read-only.</span></span>

| <span data-ttu-id="dd27d-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="dd27d-119">Property</span></span>     | <span data-ttu-id="dd27d-120">Тип</span><span class="sxs-lookup"><span data-stu-id="dd27d-120">Type</span></span>   |<span data-ttu-id="dd27d-121">Описание</span><span class="sxs-lookup"><span data-stu-id="dd27d-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="dd27d-122">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="dd27d-122">completedDateTime</span></span>|<span data-ttu-id="dd27d-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dd27d-123">DateTimeOffset</span></span>|<span data-ttu-id="dd27d-124">Представляет, когда запрос на эту операцию политики данных был выполнен во время UTC с помощью формата ISO 8601.</span><span class="sxs-lookup"><span data-stu-id="dd27d-124">Represents when the request for this data policy operation was completed, in UTC time, using the ISO 8601 format.</span></span> <span data-ttu-id="dd27d-125">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="dd27d-125">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="dd27d-126">Null до завершения операции.</span><span class="sxs-lookup"><span data-stu-id="dd27d-126">Null until the operation completes.</span></span>|
|<span data-ttu-id="dd27d-127">id</span><span class="sxs-lookup"><span data-stu-id="dd27d-127">id</span></span>|<span data-ttu-id="dd27d-128">String</span><span class="sxs-lookup"><span data-stu-id="dd27d-128">String</span></span>| <span data-ttu-id="dd27d-129">Уникальный ключ для этой операции.</span><span class="sxs-lookup"><span data-stu-id="dd27d-129">Unique key for this operation.</span></span> |
|<span data-ttu-id="dd27d-130">status</span><span class="sxs-lookup"><span data-stu-id="dd27d-130">status</span></span>|<span data-ttu-id="dd27d-131">string</span><span class="sxs-lookup"><span data-stu-id="dd27d-131">string</span></span>| <span data-ttu-id="dd27d-132">Возможные значения: `notStarted`, `running`, `complete`, `failed`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="dd27d-132">Possible values are: `notStarted`, `running`, `complete`, `failed`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="dd27d-133">storageLocation</span><span class="sxs-lookup"><span data-stu-id="dd27d-133">storageLocation</span></span>|<span data-ttu-id="dd27d-134">String</span><span class="sxs-lookup"><span data-stu-id="dd27d-134">String</span></span>|<span data-ttu-id="dd27d-135">Расположение URL-адреса, куда экспортируются данные для запросов на экспорт.</span><span class="sxs-lookup"><span data-stu-id="dd27d-135">The URL location to where data is being exported for export requests.</span></span>|
|<span data-ttu-id="dd27d-136">userId</span><span class="sxs-lookup"><span data-stu-id="dd27d-136">userId</span></span>|<span data-ttu-id="dd27d-137">String</span><span class="sxs-lookup"><span data-stu-id="dd27d-137">String</span></span>|<span data-ttu-id="dd27d-138">ID для пользователя, на котором выполняется операция.</span><span class="sxs-lookup"><span data-stu-id="dd27d-138">The id for the user on whom the operation is performed.</span></span>|
|<span data-ttu-id="dd27d-139">submittedDateTime</span><span class="sxs-lookup"><span data-stu-id="dd27d-139">submittedDateTime</span></span>|<span data-ttu-id="dd27d-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dd27d-140">DateTimeOffset</span></span>|<span data-ttu-id="dd27d-141">Представляет при отправке запроса на эту операцию данных во время UTC с помощью формата ISO 8601.</span><span class="sxs-lookup"><span data-stu-id="dd27d-141">Represents when the request for this data operation was submitted, in UTC time, using the ISO 8601 format.</span></span> <span data-ttu-id="dd27d-142">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="dd27d-142">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="dd27d-143">progress</span><span class="sxs-lookup"><span data-stu-id="dd27d-143">progress</span></span>|<span data-ttu-id="dd27d-144">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="dd27d-144">Double</span></span>|<span data-ttu-id="dd27d-145">Указывает ход операции.</span><span class="sxs-lookup"><span data-stu-id="dd27d-145">Specifies the progress of an operation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="dd27d-146">Связи</span><span class="sxs-lookup"><span data-stu-id="dd27d-146">Relationships</span></span>
<span data-ttu-id="dd27d-147">Нет</span><span class="sxs-lookup"><span data-stu-id="dd27d-147">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="dd27d-148">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="dd27d-148">JSON representation</span></span>

<span data-ttu-id="dd27d-149">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="dd27d-149">Here is a JSON representation of the resource.</span></span>

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



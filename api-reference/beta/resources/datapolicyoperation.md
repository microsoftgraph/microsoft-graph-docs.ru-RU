---
title: Тип ресурса dataPolicyOperation
description: Представляет отправленную операцию политики данных. Содержит необходимые сведения для отслеживания состояния операции. Например, администратор компании может отправить запрос операции политики данных для экспорта данных компании сотрудника, а затем отследить этот запрос.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 4e0d8916cb13c91a52d7df66fe907d611e78d908
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35973169"
---
# <a name="datapolicyoperation-resource-type"></a><span data-ttu-id="d8a98-105">Тип ресурса dataPolicyOperation</span><span class="sxs-lookup"><span data-stu-id="d8a98-105">dataPolicyOperation resource type</span></span>

<span data-ttu-id="d8a98-106">Представляет отправленную операцию политики данных.</span><span class="sxs-lookup"><span data-stu-id="d8a98-106">Represents a submitted data policy operation.</span></span> <span data-ttu-id="d8a98-107">Содержит необходимые сведения для отслеживания состояния операции.</span><span class="sxs-lookup"><span data-stu-id="d8a98-107">It contains necessary information for tracking the status of an operation.</span></span> <span data-ttu-id="d8a98-108">Например, администратор компании может отправить запрос операции политики данных для экспорта данных компании сотрудника, а затем отследить этот запрос.</span><span class="sxs-lookup"><span data-stu-id="d8a98-108">For example, a company administrator can submit a data policy operation request to export an employee's company data, and then later track that request.</span></span>

## <a name="methods"></a><span data-ttu-id="d8a98-109">Методы</span><span class="sxs-lookup"><span data-stu-id="d8a98-109">Methods</span></span>

| <span data-ttu-id="d8a98-110">Метод</span><span class="sxs-lookup"><span data-stu-id="d8a98-110">Method</span></span>           | <span data-ttu-id="d8a98-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="d8a98-111">Return Type</span></span>    |<span data-ttu-id="d8a98-112">Описание</span><span class="sxs-lookup"><span data-stu-id="d8a98-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d8a98-113">Получение dataPolicyOperation</span><span class="sxs-lookup"><span data-stu-id="d8a98-113">Get dataPolicyOperation</span></span>](../api/datapolicyoperation-get.md) | [<span data-ttu-id="d8a98-114">dataPolicyOperation</span><span class="sxs-lookup"><span data-stu-id="d8a98-114">dataPolicyOperation</span></span>](datapolicyoperation.md) |<span data-ttu-id="d8a98-115">Чтение свойств объекта dataPolicyOperation.</span><span class="sxs-lookup"><span data-stu-id="d8a98-115">Read properties of the dataPolicyOperation object.</span></span>|

## <a name="properties"></a><span data-ttu-id="d8a98-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="d8a98-116">Properties</span></span>

> <span data-ttu-id="d8a98-117">**Примечание:** Все свойства этого ресурса доступны только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d8a98-117">**Note:** All properties of this resource are read-only.</span></span>

| <span data-ttu-id="d8a98-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="d8a98-118">Property</span></span>     | <span data-ttu-id="d8a98-119">Тип</span><span class="sxs-lookup"><span data-stu-id="d8a98-119">Type</span></span>   |<span data-ttu-id="d8a98-120">Описание</span><span class="sxs-lookup"><span data-stu-id="d8a98-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d8a98-121">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="d8a98-121">completedDateTime</span></span>|<span data-ttu-id="d8a98-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d8a98-122">DateTimeOffset</span></span>|<span data-ttu-id="d8a98-123">Представляет время завершения запроса для этой операции политики данных в формате UTC с использованием формата ISO 8601.</span><span class="sxs-lookup"><span data-stu-id="d8a98-123">Represents when the request for this data policy operation was completed, in UTC time, using the ISO 8601 format.</span></span> <span data-ttu-id="d8a98-124">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="d8a98-124">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="d8a98-125">Значение null до завершения операции.</span><span class="sxs-lookup"><span data-stu-id="d8a98-125">Null until the operation completes.</span></span>|
|<span data-ttu-id="d8a98-126">id</span><span class="sxs-lookup"><span data-stu-id="d8a98-126">id</span></span>|<span data-ttu-id="d8a98-127">Строка</span><span class="sxs-lookup"><span data-stu-id="d8a98-127">String</span></span>| <span data-ttu-id="d8a98-128">Уникальный ключ для этой операции.</span><span class="sxs-lookup"><span data-stu-id="d8a98-128">Unique key for this operation.</span></span> |
|<span data-ttu-id="d8a98-129">status</span><span class="sxs-lookup"><span data-stu-id="d8a98-129">status</span></span>|<span data-ttu-id="d8a98-130">string</span><span class="sxs-lookup"><span data-stu-id="d8a98-130">string</span></span>| <span data-ttu-id="d8a98-131">Возможные значения: `notStarted`, `running`, `complete`, `failed`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="d8a98-131">Possible values are: `notStarted`, `running`, `complete`, `failed`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="d8a98-132">Сторажелокатион</span><span class="sxs-lookup"><span data-stu-id="d8a98-132">storageLocation</span></span>|<span data-ttu-id="d8a98-133">String</span><span class="sxs-lookup"><span data-stu-id="d8a98-133">String</span></span>|<span data-ttu-id="d8a98-134">URL-адрес, по которому выполняется экспорт данных для запросов на экспорт.</span><span class="sxs-lookup"><span data-stu-id="d8a98-134">The URL location to where data is being exported for export requests.</span></span>|
|<span data-ttu-id="d8a98-135">userId</span><span class="sxs-lookup"><span data-stu-id="d8a98-135">userId</span></span>|<span data-ttu-id="d8a98-136">String</span><span class="sxs-lookup"><span data-stu-id="d8a98-136">String</span></span>|<span data-ttu-id="d8a98-137">Идентификатор пользователя, для которого выполняется операция.</span><span class="sxs-lookup"><span data-stu-id="d8a98-137">The id for the user on whom the operation is performed.</span></span>|
|<span data-ttu-id="d8a98-138">Субмиттеддатетиме</span><span class="sxs-lookup"><span data-stu-id="d8a98-138">submittedDateTime</span></span>|<span data-ttu-id="d8a98-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d8a98-139">DateTimeOffset</span></span>|<span data-ttu-id="d8a98-140">Представляет время отправки запроса для этой операции с данными в формате UTC с использованием формата ISO 8601.</span><span class="sxs-lookup"><span data-stu-id="d8a98-140">Represents when the request for this data operation was submitted, in UTC time, using the ISO 8601 format.</span></span> <span data-ttu-id="d8a98-141">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="d8a98-141">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="d8a98-142">progress</span><span class="sxs-lookup"><span data-stu-id="d8a98-142">progress</span></span>|<span data-ttu-id="d8a98-143">Двойное</span><span class="sxs-lookup"><span data-stu-id="d8a98-143">Double</span></span>|<span data-ttu-id="d8a98-144">Задает ход выполнения операции.</span><span class="sxs-lookup"><span data-stu-id="d8a98-144">Specifies the progress of an operation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d8a98-145">Отношения</span><span class="sxs-lookup"><span data-stu-id="d8a98-145">Relationships</span></span>
<span data-ttu-id="d8a98-146">Нет</span><span class="sxs-lookup"><span data-stu-id="d8a98-146">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="d8a98-147">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d8a98-147">JSON representation</span></span>

<span data-ttu-id="d8a98-148">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d8a98-148">Here is a JSON representation of the resource.</span></span>

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

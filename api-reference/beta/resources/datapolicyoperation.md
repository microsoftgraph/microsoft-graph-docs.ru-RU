---
title: Тип ресурса dataPolicyOperation
description: Представляет отправленную операцию политики данных. Содержит необходимые сведения для отслеживания состояния операции. Например, администратор компании может отправить запрос операции политики данных для экспорта данных компании сотрудника, а затем отследить этот запрос.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 0d3ec392bb30614346d2726262851eebc29ee779
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32543179"
---
# <a name="datapolicyoperation-resource-type"></a><span data-ttu-id="c5979-105">Тип ресурса dataPolicyOperation</span><span class="sxs-lookup"><span data-stu-id="c5979-105">dataPolicyOperation resource type</span></span>

<span data-ttu-id="c5979-106">Представляет отправленную операцию политики данных.</span><span class="sxs-lookup"><span data-stu-id="c5979-106">Represents a submitted data policy operation.</span></span> <span data-ttu-id="c5979-107">Содержит необходимые сведения для отслеживания состояния операции.</span><span class="sxs-lookup"><span data-stu-id="c5979-107">It contains necessary information for tracking the status of an operation.</span></span> <span data-ttu-id="c5979-108">Например, администратор компании может отправить запрос операции политики данных для экспорта данных компании сотрудника, а затем отследить этот запрос.</span><span class="sxs-lookup"><span data-stu-id="c5979-108">For example, a company administrator can submit a data policy operation request to export an employee's company data, and then later track that request.</span></span>

## <a name="methods"></a><span data-ttu-id="c5979-109">Методы</span><span class="sxs-lookup"><span data-stu-id="c5979-109">Methods</span></span>

| <span data-ttu-id="c5979-110">Метод</span><span class="sxs-lookup"><span data-stu-id="c5979-110">Method</span></span>           | <span data-ttu-id="c5979-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="c5979-111">Return Type</span></span>    |<span data-ttu-id="c5979-112">Описание</span><span class="sxs-lookup"><span data-stu-id="c5979-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c5979-113">Получение dataPolicyOperation</span><span class="sxs-lookup"><span data-stu-id="c5979-113">Get dataPolicyOperation</span></span>](../api/datapolicyoperation-get.md) | [<span data-ttu-id="c5979-114">dataPolicyOperation</span><span class="sxs-lookup"><span data-stu-id="c5979-114">dataPolicyOperation</span></span>](datapolicyoperation.md) |<span data-ttu-id="c5979-115">Чтение свойств объекта dataPolicyOperation.</span><span class="sxs-lookup"><span data-stu-id="c5979-115">Read properties of the dataPolicyOperation object.</span></span>|

## <a name="properties"></a><span data-ttu-id="c5979-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="c5979-116">Properties</span></span>

> <span data-ttu-id="c5979-117">**Примечание:** Все свойства этого ресурса доступны только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c5979-117">**Note:** All properties of this resource are read-only.</span></span>

| <span data-ttu-id="c5979-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="c5979-118">Property</span></span>     | <span data-ttu-id="c5979-119">Тип</span><span class="sxs-lookup"><span data-stu-id="c5979-119">Type</span></span>   |<span data-ttu-id="c5979-120">Описание</span><span class="sxs-lookup"><span data-stu-id="c5979-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c5979-121">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="c5979-121">completedDateTime</span></span>|<span data-ttu-id="c5979-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c5979-122">DateTimeOffset</span></span>|<span data-ttu-id="c5979-123">Представляет время завершения запроса для этой операции политики данных в формате UTC с использованием формата ISO 8601.</span><span class="sxs-lookup"><span data-stu-id="c5979-123">Represents when the request for this data policy operation was completed, in UTC time, using the ISO 8601 format.</span></span> <span data-ttu-id="c5979-124">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="c5979-124">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="c5979-125">Значение null до завершения операции.</span><span class="sxs-lookup"><span data-stu-id="c5979-125">Null until the operation completes.</span></span>|
|<span data-ttu-id="c5979-126">id</span><span class="sxs-lookup"><span data-stu-id="c5979-126">id</span></span>|<span data-ttu-id="c5979-127">Строка</span><span class="sxs-lookup"><span data-stu-id="c5979-127">String</span></span>| <span data-ttu-id="c5979-128">Уникальный ключ для этой операции.</span><span class="sxs-lookup"><span data-stu-id="c5979-128">Unique key for this operation.</span></span> |
|<span data-ttu-id="c5979-129">status</span><span class="sxs-lookup"><span data-stu-id="c5979-129">status</span></span>|<span data-ttu-id="c5979-130">string</span><span class="sxs-lookup"><span data-stu-id="c5979-130">string</span></span>| <span data-ttu-id="c5979-131">Возможные значения: `notStarted`, `running`, `complete`, `failed`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="c5979-131">Possible values are: `notStarted`, `running`, `complete`, `failed`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="c5979-132">Сторажелокатион</span><span class="sxs-lookup"><span data-stu-id="c5979-132">storageLocation</span></span>|<span data-ttu-id="c5979-133">String</span><span class="sxs-lookup"><span data-stu-id="c5979-133">String</span></span>|<span data-ttu-id="c5979-134">URL-адрес, по которому выполняется экспорт данных для запросов на экспорт.</span><span class="sxs-lookup"><span data-stu-id="c5979-134">The URL location to where data is being exported for export requests.</span></span>|
|<span data-ttu-id="c5979-135">userId</span><span class="sxs-lookup"><span data-stu-id="c5979-135">userId</span></span>|<span data-ttu-id="c5979-136">String</span><span class="sxs-lookup"><span data-stu-id="c5979-136">String</span></span>|<span data-ttu-id="c5979-137">Идентификатор пользователя, для которого выполняется операция.</span><span class="sxs-lookup"><span data-stu-id="c5979-137">The id for the user on whom the operation is performed.</span></span>|
|<span data-ttu-id="c5979-138">Субмиттеддатетиме</span><span class="sxs-lookup"><span data-stu-id="c5979-138">submittedDateTime</span></span>|<span data-ttu-id="c5979-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c5979-139">DateTimeOffset</span></span>|<span data-ttu-id="c5979-140">Представляет время отправки запроса для этой операции с данными в формате UTC с использованием формата ISO 8601.</span><span class="sxs-lookup"><span data-stu-id="c5979-140">Represents when the request for this data operation was submitted, in UTC time, using the ISO 8601 format.</span></span> <span data-ttu-id="c5979-141">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="c5979-141">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="c5979-142">progress</span><span class="sxs-lookup"><span data-stu-id="c5979-142">progress</span></span>|<span data-ttu-id="c5979-143">Двойное</span><span class="sxs-lookup"><span data-stu-id="c5979-143">Double</span></span>|<span data-ttu-id="c5979-144">Задает ход выполнения операции.</span><span class="sxs-lookup"><span data-stu-id="c5979-144">Specifies the progress of an operation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c5979-145">Отношения</span><span class="sxs-lookup"><span data-stu-id="c5979-145">Relationships</span></span>
<span data-ttu-id="c5979-146">Нет</span><span class="sxs-lookup"><span data-stu-id="c5979-146">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="c5979-147">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="c5979-147">JSON representation</span></span>

<span data-ttu-id="c5979-148">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c5979-148">Here is a JSON representation of the resource.</span></span>

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

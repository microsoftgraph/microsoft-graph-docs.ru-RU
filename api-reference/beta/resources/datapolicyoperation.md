---
title: Тип ресурса dataPolicyOperation
description: Представляет отправленную операцию политики данных. Содержит необходимые сведения для отслеживания состояния операции. Например, администратор компании может отправить запрос операции политики данных для экспорта данных компании сотрудника, а затем отследить этот запрос.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: bec2403ca4e1bad13af801b67d95f3ec9b30d4f4
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48049991"
---
# <a name="datapolicyoperation-resource-type"></a><span data-ttu-id="8a57d-105">Тип ресурса dataPolicyOperation</span><span class="sxs-lookup"><span data-stu-id="8a57d-105">dataPolicyOperation resource type</span></span>

<span data-ttu-id="8a57d-106">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8a57d-106">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8a57d-107">Представляет отправленную операцию политики данных.</span><span class="sxs-lookup"><span data-stu-id="8a57d-107">Represents a submitted data policy operation.</span></span> <span data-ttu-id="8a57d-108">Содержит необходимые сведения для отслеживания состояния операции.</span><span class="sxs-lookup"><span data-stu-id="8a57d-108">It contains necessary information for tracking the status of an operation.</span></span> <span data-ttu-id="8a57d-109">Например, администратор компании может отправить запрос операции политики данных для экспорта данных компании сотрудника, а затем отследить этот запрос.</span><span class="sxs-lookup"><span data-stu-id="8a57d-109">For example, a company administrator can submit a data policy operation request to export an employee's company data, and then later track that request.</span></span>

## <a name="methods"></a><span data-ttu-id="8a57d-110">Методы</span><span class="sxs-lookup"><span data-stu-id="8a57d-110">Methods</span></span>

| <span data-ttu-id="8a57d-111">Метод</span><span class="sxs-lookup"><span data-stu-id="8a57d-111">Method</span></span>           | <span data-ttu-id="8a57d-112">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="8a57d-112">Return Type</span></span>    |<span data-ttu-id="8a57d-113">Описание</span><span class="sxs-lookup"><span data-stu-id="8a57d-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="8a57d-114">Получение dataPolicyOperation</span><span class="sxs-lookup"><span data-stu-id="8a57d-114">Get dataPolicyOperation</span></span>](../api/datapolicyoperation-get.md) | [<span data-ttu-id="8a57d-115">dataPolicyOperation</span><span class="sxs-lookup"><span data-stu-id="8a57d-115">dataPolicyOperation</span></span>](datapolicyoperation.md) |<span data-ttu-id="8a57d-116">Чтение свойств объекта dataPolicyOperation.</span><span class="sxs-lookup"><span data-stu-id="8a57d-116">Read properties of the dataPolicyOperation object.</span></span>|

## <a name="properties"></a><span data-ttu-id="8a57d-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="8a57d-117">Properties</span></span>

> <span data-ttu-id="8a57d-118">**Примечание:** Все свойства этого ресурса доступны только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8a57d-118">**Note:** All properties of this resource are read-only.</span></span>

| <span data-ttu-id="8a57d-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="8a57d-119">Property</span></span>     | <span data-ttu-id="8a57d-120">Тип</span><span class="sxs-lookup"><span data-stu-id="8a57d-120">Type</span></span>   |<span data-ttu-id="8a57d-121">Описание</span><span class="sxs-lookup"><span data-stu-id="8a57d-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8a57d-122">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="8a57d-122">completedDateTime</span></span>|<span data-ttu-id="8a57d-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8a57d-123">DateTimeOffset</span></span>|<span data-ttu-id="8a57d-124">Представляет время завершения запроса для этой операции политики данных в формате UTC с использованием формата ISO 8601.</span><span class="sxs-lookup"><span data-stu-id="8a57d-124">Represents when the request for this data policy operation was completed, in UTC time, using the ISO 8601 format.</span></span> <span data-ttu-id="8a57d-125">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="8a57d-125">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="8a57d-126">Значение null до завершения операции.</span><span class="sxs-lookup"><span data-stu-id="8a57d-126">Null until the operation completes.</span></span>|
|<span data-ttu-id="8a57d-127">id</span><span class="sxs-lookup"><span data-stu-id="8a57d-127">id</span></span>|<span data-ttu-id="8a57d-128">Строка</span><span class="sxs-lookup"><span data-stu-id="8a57d-128">String</span></span>| <span data-ttu-id="8a57d-129">Уникальный ключ для этой операции.</span><span class="sxs-lookup"><span data-stu-id="8a57d-129">Unique key for this operation.</span></span> |
|<span data-ttu-id="8a57d-130">status</span><span class="sxs-lookup"><span data-stu-id="8a57d-130">status</span></span>|<span data-ttu-id="8a57d-131">string</span><span class="sxs-lookup"><span data-stu-id="8a57d-131">string</span></span>| <span data-ttu-id="8a57d-132">Возможные значения: `notStarted`, `running`, `complete`, `failed`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="8a57d-132">Possible values are: `notStarted`, `running`, `complete`, `failed`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="8a57d-133">сторажелокатион</span><span class="sxs-lookup"><span data-stu-id="8a57d-133">storageLocation</span></span>|<span data-ttu-id="8a57d-134">Строка</span><span class="sxs-lookup"><span data-stu-id="8a57d-134">String</span></span>|<span data-ttu-id="8a57d-135">URL-адрес, по которому выполняется экспорт данных для запросов на экспорт.</span><span class="sxs-lookup"><span data-stu-id="8a57d-135">The URL location to where data is being exported for export requests.</span></span>|
|<span data-ttu-id="8a57d-136">userId</span><span class="sxs-lookup"><span data-stu-id="8a57d-136">userId</span></span>|<span data-ttu-id="8a57d-137">String</span><span class="sxs-lookup"><span data-stu-id="8a57d-137">String</span></span>|<span data-ttu-id="8a57d-138">Идентификатор пользователя, для которого выполняется операция.</span><span class="sxs-lookup"><span data-stu-id="8a57d-138">The id for the user on whom the operation is performed.</span></span>|
|<span data-ttu-id="8a57d-139">субмиттеддатетиме</span><span class="sxs-lookup"><span data-stu-id="8a57d-139">submittedDateTime</span></span>|<span data-ttu-id="8a57d-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8a57d-140">DateTimeOffset</span></span>|<span data-ttu-id="8a57d-141">Представляет время отправки запроса для этой операции с данными в формате UTC с использованием формата ISO 8601.</span><span class="sxs-lookup"><span data-stu-id="8a57d-141">Represents when the request for this data operation was submitted, in UTC time, using the ISO 8601 format.</span></span> <span data-ttu-id="8a57d-142">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="8a57d-142">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="8a57d-143">progress</span><span class="sxs-lookup"><span data-stu-id="8a57d-143">progress</span></span>|<span data-ttu-id="8a57d-144">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="8a57d-144">Double</span></span>|<span data-ttu-id="8a57d-145">Задает ход выполнения операции.</span><span class="sxs-lookup"><span data-stu-id="8a57d-145">Specifies the progress of an operation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8a57d-146">Связи</span><span class="sxs-lookup"><span data-stu-id="8a57d-146">Relationships</span></span>
<span data-ttu-id="8a57d-147">Нет</span><span class="sxs-lookup"><span data-stu-id="8a57d-147">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="8a57d-148">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8a57d-148">JSON representation</span></span>

<span data-ttu-id="8a57d-149">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8a57d-149">Here is a JSON representation of the resource.</span></span>

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



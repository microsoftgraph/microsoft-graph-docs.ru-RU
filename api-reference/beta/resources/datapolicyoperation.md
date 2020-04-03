---
title: Тип ресурса dataPolicyOperation
description: Представляет отправленную операцию политики данных. Содержит необходимые сведения для отслеживания состояния операции. Например, администратор компании может отправить запрос операции политики данных для экспорта данных компании сотрудника, а затем отследить этот запрос.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 9057d46a3d01b525f2c430817e875e7ef7bf62d5
ms.sourcegitcommit: bd40e302ce04b686e86989246ab7c4cc9ad3f320
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/03/2020
ms.locfileid: "43124800"
---
# <a name="datapolicyoperation-resource-type"></a><span data-ttu-id="fc680-105">Тип ресурса dataPolicyOperation</span><span class="sxs-lookup"><span data-stu-id="fc680-105">dataPolicyOperation resource type</span></span>

<span data-ttu-id="fc680-106">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fc680-106">Namespace: microsoft.graph</span></span>

<span data-ttu-id="fc680-107">Представляет отправленную операцию политики данных.</span><span class="sxs-lookup"><span data-stu-id="fc680-107">Represents a submitted data policy operation.</span></span> <span data-ttu-id="fc680-108">Содержит необходимые сведения для отслеживания состояния операции.</span><span class="sxs-lookup"><span data-stu-id="fc680-108">It contains necessary information for tracking the status of an operation.</span></span> <span data-ttu-id="fc680-109">Например, администратор компании может отправить запрос операции политики данных для экспорта данных компании сотрудника, а затем отследить этот запрос.</span><span class="sxs-lookup"><span data-stu-id="fc680-109">For example, a company administrator can submit a data policy operation request to export an employee's company data, and then later track that request.</span></span>

## <a name="methods"></a><span data-ttu-id="fc680-110">Методы</span><span class="sxs-lookup"><span data-stu-id="fc680-110">Methods</span></span>

| <span data-ttu-id="fc680-111">Метод</span><span class="sxs-lookup"><span data-stu-id="fc680-111">Method</span></span>           | <span data-ttu-id="fc680-112">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="fc680-112">Return Type</span></span>    |<span data-ttu-id="fc680-113">Описание</span><span class="sxs-lookup"><span data-stu-id="fc680-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="fc680-114">Получение dataPolicyOperation</span><span class="sxs-lookup"><span data-stu-id="fc680-114">Get dataPolicyOperation</span></span>](../api/datapolicyoperation-get.md) | [<span data-ttu-id="fc680-115">dataPolicyOperation</span><span class="sxs-lookup"><span data-stu-id="fc680-115">dataPolicyOperation</span></span>](datapolicyoperation.md) |<span data-ttu-id="fc680-116">Чтение свойств объекта dataPolicyOperation.</span><span class="sxs-lookup"><span data-stu-id="fc680-116">Read properties of the dataPolicyOperation object.</span></span>|

## <a name="properties"></a><span data-ttu-id="fc680-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="fc680-117">Properties</span></span>

> <span data-ttu-id="fc680-118">**Примечание:** Все свойства этого ресурса доступны только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fc680-118">**Note:** All properties of this resource are read-only.</span></span>

| <span data-ttu-id="fc680-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="fc680-119">Property</span></span>     | <span data-ttu-id="fc680-120">Тип</span><span class="sxs-lookup"><span data-stu-id="fc680-120">Type</span></span>   |<span data-ttu-id="fc680-121">Описание</span><span class="sxs-lookup"><span data-stu-id="fc680-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fc680-122">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="fc680-122">completedDateTime</span></span>|<span data-ttu-id="fc680-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fc680-123">DateTimeOffset</span></span>|<span data-ttu-id="fc680-124">Представляет время завершения запроса для этой операции политики данных в формате UTC с использованием формата ISO 8601.</span><span class="sxs-lookup"><span data-stu-id="fc680-124">Represents when the request for this data policy operation was completed, in UTC time, using the ISO 8601 format.</span></span> <span data-ttu-id="fc680-125">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="fc680-125">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="fc680-126">Значение null до завершения операции.</span><span class="sxs-lookup"><span data-stu-id="fc680-126">Null until the operation completes.</span></span>|
|<span data-ttu-id="fc680-127">id</span><span class="sxs-lookup"><span data-stu-id="fc680-127">id</span></span>|<span data-ttu-id="fc680-128">Строка</span><span class="sxs-lookup"><span data-stu-id="fc680-128">String</span></span>| <span data-ttu-id="fc680-129">Уникальный ключ для этой операции.</span><span class="sxs-lookup"><span data-stu-id="fc680-129">Unique key for this operation.</span></span> |
|<span data-ttu-id="fc680-130">status</span><span class="sxs-lookup"><span data-stu-id="fc680-130">status</span></span>|<span data-ttu-id="fc680-131">string</span><span class="sxs-lookup"><span data-stu-id="fc680-131">string</span></span>| <span data-ttu-id="fc680-132">Возможные значения: `notStarted`, `running`, `complete`, `failed`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="fc680-132">Possible values are: `notStarted`, `running`, `complete`, `failed`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="fc680-133">сторажелокатион</span><span class="sxs-lookup"><span data-stu-id="fc680-133">storageLocation</span></span>|<span data-ttu-id="fc680-134">Строка</span><span class="sxs-lookup"><span data-stu-id="fc680-134">String</span></span>|<span data-ttu-id="fc680-135">URL-адрес, по которому выполняется экспорт данных для запросов на экспорт.</span><span class="sxs-lookup"><span data-stu-id="fc680-135">The URL location to where data is being exported for export requests.</span></span>|
|<span data-ttu-id="fc680-136">userId</span><span class="sxs-lookup"><span data-stu-id="fc680-136">userId</span></span>|<span data-ttu-id="fc680-137">String</span><span class="sxs-lookup"><span data-stu-id="fc680-137">String</span></span>|<span data-ttu-id="fc680-138">Идентификатор пользователя, для которого выполняется операция.</span><span class="sxs-lookup"><span data-stu-id="fc680-138">The id for the user on whom the operation is performed.</span></span>|
|<span data-ttu-id="fc680-139">субмиттеддатетиме</span><span class="sxs-lookup"><span data-stu-id="fc680-139">submittedDateTime</span></span>|<span data-ttu-id="fc680-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fc680-140">DateTimeOffset</span></span>|<span data-ttu-id="fc680-141">Представляет время отправки запроса для этой операции с данными в формате UTC с использованием формата ISO 8601.</span><span class="sxs-lookup"><span data-stu-id="fc680-141">Represents when the request for this data operation was submitted, in UTC time, using the ISO 8601 format.</span></span> <span data-ttu-id="fc680-142">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="fc680-142">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="fc680-143">progress</span><span class="sxs-lookup"><span data-stu-id="fc680-143">progress</span></span>|<span data-ttu-id="fc680-144">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="fc680-144">Double</span></span>|<span data-ttu-id="fc680-145">Задает ход выполнения операции.</span><span class="sxs-lookup"><span data-stu-id="fc680-145">Specifies the progress of an operation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fc680-146">Связи</span><span class="sxs-lookup"><span data-stu-id="fc680-146">Relationships</span></span>
<span data-ttu-id="fc680-147">Нет</span><span class="sxs-lookup"><span data-stu-id="fc680-147">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="fc680-148">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="fc680-148">JSON representation</span></span>

<span data-ttu-id="fc680-149">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fc680-149">Here is a JSON representation of the resource.</span></span>

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

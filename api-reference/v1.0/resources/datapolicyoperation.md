---
title: тип ресурса dataPolicyOperation
description: Представляет собой операцию по отправке политики данных. Он содержит необходимые сведения для отслеживания состояния операции. Например, администратор компании может отправить запрос на операцию политики данных для экспорта данных компании сотрудника, а затем отслеживать этот запрос.
author: dkershaw10
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: f7b07cb2906eb1a3d01d6c24ca5b91fec35ec7c8
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50962002"
---
# <a name="datapolicyoperation-resource-type"></a><span data-ttu-id="89f30-105">тип ресурса dataPolicyOperation</span><span class="sxs-lookup"><span data-stu-id="89f30-105">dataPolicyOperation resource type</span></span>

<span data-ttu-id="89f30-106">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="89f30-106">Namespace: microsoft.graph</span></span>

<span data-ttu-id="89f30-107">Представляет собой операцию по отправке политики данных.</span><span class="sxs-lookup"><span data-stu-id="89f30-107">Represents a submitted data policy operation.</span></span> <span data-ttu-id="89f30-108">Он содержит необходимые сведения для отслеживания состояния операции.</span><span class="sxs-lookup"><span data-stu-id="89f30-108">It contains necessary information for tracking the status of an operation.</span></span> <span data-ttu-id="89f30-109">Например, администратор компании может отправить запрос на операцию политики данных для экспорта данных компании сотрудника, а затем отслеживать этот запрос.</span><span class="sxs-lookup"><span data-stu-id="89f30-109">For example, a company administrator can submit a data policy operation request to export an employee's company data, and then later track that request.</span></span>

## <a name="methods"></a><span data-ttu-id="89f30-110">Методы</span><span class="sxs-lookup"><span data-stu-id="89f30-110">Methods</span></span>

| <span data-ttu-id="89f30-111">Метод</span><span class="sxs-lookup"><span data-stu-id="89f30-111">Method</span></span>           | <span data-ttu-id="89f30-112">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="89f30-112">Return Type</span></span>    |<span data-ttu-id="89f30-113">Описание</span><span class="sxs-lookup"><span data-stu-id="89f30-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="89f30-114">Get dataPolicyOperation</span><span class="sxs-lookup"><span data-stu-id="89f30-114">Get dataPolicyOperation</span></span>](../api/datapolicyoperation-get.md) | [<span data-ttu-id="89f30-115">dataPolicyOperation</span><span class="sxs-lookup"><span data-stu-id="89f30-115">dataPolicyOperation</span></span>](datapolicyoperation.md) |<span data-ttu-id="89f30-116">Извлечение свойств **объекта dataPolicyOperation.**</span><span class="sxs-lookup"><span data-stu-id="89f30-116">Retrieve properties of the **dataPolicyOperation** object.</span></span>|
|[<span data-ttu-id="89f30-117">Экспорт личных данных</span><span class="sxs-lookup"><span data-stu-id="89f30-117">Export personal data</span></span>](../api/user-exportpersonaldata.md) | <span data-ttu-id="89f30-118">Нет</span><span class="sxs-lookup"><span data-stu-id="89f30-118">None</span></span> |<span data-ttu-id="89f30-119">Отправка запроса на операцию политики данных для экспорта данных пользователя организации, которые можно прочитать с помощью [Get dataPolicyOperation](../api/datapolicyoperation-get.md)</span><span class="sxs-lookup"><span data-stu-id="89f30-119">Submit a data policy operation request to export organizational user's data which can later be read using [Get dataPolicyOperation](../api/datapolicyoperation-get.md)</span></span>|

## <a name="properties"></a><span data-ttu-id="89f30-120">Свойства</span><span class="sxs-lookup"><span data-stu-id="89f30-120">Properties</span></span>

> <span data-ttu-id="89f30-121">**Примечание:** Все свойства этого ресурса являются только для чтения.</span><span class="sxs-lookup"><span data-stu-id="89f30-121">**Note:** All properties of this resource are read-only.</span></span>

| <span data-ttu-id="89f30-122">Свойство</span><span class="sxs-lookup"><span data-stu-id="89f30-122">Property</span></span>     | <span data-ttu-id="89f30-123">Тип</span><span class="sxs-lookup"><span data-stu-id="89f30-123">Type</span></span>   |<span data-ttu-id="89f30-124">Описание</span><span class="sxs-lookup"><span data-stu-id="89f30-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="89f30-125">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="89f30-125">completedDateTime</span></span>|<span data-ttu-id="89f30-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="89f30-126">DateTimeOffset</span></span>|<span data-ttu-id="89f30-127">Представляет, когда запрос на эту операцию политики данных был выполнен во время UTC с помощью формата ISO 8601.</span><span class="sxs-lookup"><span data-stu-id="89f30-127">Represents when the request for this data policy operation was completed, in UTC time, using the ISO 8601 format.</span></span> <span data-ttu-id="89f30-128">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="89f30-128">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="89f30-129">Null до завершения операции.</span><span class="sxs-lookup"><span data-stu-id="89f30-129">Null until the operation completes.</span></span>|
|<span data-ttu-id="89f30-130">id</span><span class="sxs-lookup"><span data-stu-id="89f30-130">id</span></span>|<span data-ttu-id="89f30-131">String</span><span class="sxs-lookup"><span data-stu-id="89f30-131">String</span></span>| <span data-ttu-id="89f30-132">Уникальный ключ для этой операции.</span><span class="sxs-lookup"><span data-stu-id="89f30-132">Unique key for this operation.</span></span> |
|<span data-ttu-id="89f30-133">status</span><span class="sxs-lookup"><span data-stu-id="89f30-133">status</span></span>|<span data-ttu-id="89f30-134">dataPolicyOperationStatus</span><span class="sxs-lookup"><span data-stu-id="89f30-134">dataPolicyOperationStatus</span></span>| <span data-ttu-id="89f30-135">Возможные значения: `notStarted`, `running`, `complete`, `failed`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="89f30-135">Possible values are: `notStarted`, `running`, `complete`, `failed`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="89f30-136">storageLocation</span><span class="sxs-lookup"><span data-stu-id="89f30-136">storageLocation</span></span>|<span data-ttu-id="89f30-137">String</span><span class="sxs-lookup"><span data-stu-id="89f30-137">String</span></span>|<span data-ttu-id="89f30-138">Расположение URL-адреса, куда экспортируются данные для запросов на экспорт.</span><span class="sxs-lookup"><span data-stu-id="89f30-138">The URL location to where data is being exported for export requests.</span></span>|
|<span data-ttu-id="89f30-139">userId</span><span class="sxs-lookup"><span data-stu-id="89f30-139">userId</span></span>|<span data-ttu-id="89f30-140">String</span><span class="sxs-lookup"><span data-stu-id="89f30-140">String</span></span>|<span data-ttu-id="89f30-141">ID для пользователя, на котором выполняется операция.</span><span class="sxs-lookup"><span data-stu-id="89f30-141">The id for the user on whom the operation is performed.</span></span>|
|<span data-ttu-id="89f30-142">submittedDateTime</span><span class="sxs-lookup"><span data-stu-id="89f30-142">submittedDateTime</span></span>|<span data-ttu-id="89f30-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="89f30-143">DateTimeOffset</span></span>|<span data-ttu-id="89f30-144">Представляет при отправке запроса на эту операцию данных во время UTC с помощью формата ISO 8601.</span><span class="sxs-lookup"><span data-stu-id="89f30-144">Represents when the request for this data operation was submitted, in UTC time, using the ISO 8601 format.</span></span> <span data-ttu-id="89f30-145">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="89f30-145">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="89f30-146">progress</span><span class="sxs-lookup"><span data-stu-id="89f30-146">progress</span></span>|<span data-ttu-id="89f30-147">String</span><span class="sxs-lookup"><span data-stu-id="89f30-147">String</span></span>|<span data-ttu-id="89f30-148">Указывает ход операции.</span><span class="sxs-lookup"><span data-stu-id="89f30-148">Specifies the progress of an operation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="89f30-149">Связи</span><span class="sxs-lookup"><span data-stu-id="89f30-149">Relationships</span></span>
<span data-ttu-id="89f30-150">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="89f30-150">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="89f30-151">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="89f30-151">JSON representation</span></span>

<span data-ttu-id="89f30-152">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="89f30-152">The following is a JSON representation of the resource.</span></span>

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
  "progress": "String (double)"
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


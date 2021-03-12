---
title: тип ресурса dataPolicyOperation
description: Представляет собой операцию по отправке политики данных. Он содержит необходимые сведения для отслеживания состояния операции. Например, администратор компании может отправить запрос на операцию политики данных для экспорта данных компании сотрудника, а затем отслеживать этот запрос.
author: dkershaw10
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 18294905754cd962ec1c18136b61ca20799eee3d
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50718445"
---
# <a name="datapolicyoperation-resource-type"></a><span data-ttu-id="69770-105">тип ресурса dataPolicyOperation</span><span class="sxs-lookup"><span data-stu-id="69770-105">dataPolicyOperation resource type</span></span>

<span data-ttu-id="69770-106">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="69770-106">Namespace: microsoft.graph</span></span>

<span data-ttu-id="69770-107">Представляет собой операцию по отправке политики данных.</span><span class="sxs-lookup"><span data-stu-id="69770-107">Represents a submitted data policy operation.</span></span> <span data-ttu-id="69770-108">Он содержит необходимые сведения для отслеживания состояния операции.</span><span class="sxs-lookup"><span data-stu-id="69770-108">It contains necessary information for tracking the status of an operation.</span></span> <span data-ttu-id="69770-109">Например, администратор компании может отправить запрос на операцию политики данных для экспорта данных компании сотрудника, а затем отслеживать этот запрос.</span><span class="sxs-lookup"><span data-stu-id="69770-109">For example, a company administrator can submit a data policy operation request to export an employee's company data, and then later track that request.</span></span>

## <a name="methods"></a><span data-ttu-id="69770-110">Методы</span><span class="sxs-lookup"><span data-stu-id="69770-110">Methods</span></span>

| <span data-ttu-id="69770-111">Метод</span><span class="sxs-lookup"><span data-stu-id="69770-111">Method</span></span>           | <span data-ttu-id="69770-112">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="69770-112">Return Type</span></span>    |<span data-ttu-id="69770-113">Описание</span><span class="sxs-lookup"><span data-stu-id="69770-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="69770-114">Get dataPolicyOperation</span><span class="sxs-lookup"><span data-stu-id="69770-114">Get dataPolicyOperation</span></span>](../api/datapolicyoperation-get.md) | [<span data-ttu-id="69770-115">dataPolicyOperation</span><span class="sxs-lookup"><span data-stu-id="69770-115">dataPolicyOperation</span></span>](datapolicyoperation.md) |<span data-ttu-id="69770-116">Извлечение свойств **объекта dataPolicyOperation.**</span><span class="sxs-lookup"><span data-stu-id="69770-116">Retrieve properties of the **dataPolicyOperation** object.</span></span>|
|[<span data-ttu-id="69770-117">Экспорт личных данных</span><span class="sxs-lookup"><span data-stu-id="69770-117">Export personal data</span></span>](../api/user-exportpersonaldata.md) | <span data-ttu-id="69770-118">Нет</span><span class="sxs-lookup"><span data-stu-id="69770-118">None</span></span> |<span data-ttu-id="69770-119">Отправка запроса на операцию политики данных для экспорта данных пользователя организации, которые можно прочитать с помощью [Get dataPolicyOperation](../api/datapolicyoperation-get.md)</span><span class="sxs-lookup"><span data-stu-id="69770-119">Submit a data policy operation request to export organizational user's data which can later be read using [Get dataPolicyOperation](../api/datapolicyoperation-get.md)</span></span>|

## <a name="properties"></a><span data-ttu-id="69770-120">Свойства</span><span class="sxs-lookup"><span data-stu-id="69770-120">Properties</span></span>

> <span data-ttu-id="69770-121">**Примечание:** Все свойства этого ресурса являются только для чтения.</span><span class="sxs-lookup"><span data-stu-id="69770-121">**Note:** All properties of this resource are read-only.</span></span>

| <span data-ttu-id="69770-122">Свойство</span><span class="sxs-lookup"><span data-stu-id="69770-122">Property</span></span>     | <span data-ttu-id="69770-123">Тип</span><span class="sxs-lookup"><span data-stu-id="69770-123">Type</span></span>   |<span data-ttu-id="69770-124">Описание</span><span class="sxs-lookup"><span data-stu-id="69770-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="69770-125">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="69770-125">completedDateTime</span></span>|<span data-ttu-id="69770-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="69770-126">DateTimeOffset</span></span>|<span data-ttu-id="69770-127">Представляет, когда запрос на эту операцию политики данных был выполнен во время UTC с помощью формата ISO 8601.</span><span class="sxs-lookup"><span data-stu-id="69770-127">Represents when the request for this data policy operation was completed, in UTC time, using the ISO 8601 format.</span></span> <span data-ttu-id="69770-128">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="69770-128">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="69770-129">Null до завершения операции.</span><span class="sxs-lookup"><span data-stu-id="69770-129">Null until the operation completes.</span></span>|
|<span data-ttu-id="69770-130">id</span><span class="sxs-lookup"><span data-stu-id="69770-130">id</span></span>|<span data-ttu-id="69770-131">String</span><span class="sxs-lookup"><span data-stu-id="69770-131">String</span></span>| <span data-ttu-id="69770-132">Уникальный ключ для этой операции.</span><span class="sxs-lookup"><span data-stu-id="69770-132">Unique key for this operation.</span></span> |
|<span data-ttu-id="69770-133">status</span><span class="sxs-lookup"><span data-stu-id="69770-133">status</span></span>|<span data-ttu-id="69770-134">string</span><span class="sxs-lookup"><span data-stu-id="69770-134">string</span></span>| <span data-ttu-id="69770-135">Возможные значения: `notStarted`, `running`, `complete`, `failed`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="69770-135">Possible values are: `notStarted`, `running`, `complete`, `failed`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="69770-136">storageLocation</span><span class="sxs-lookup"><span data-stu-id="69770-136">storageLocation</span></span>|<span data-ttu-id="69770-137">String</span><span class="sxs-lookup"><span data-stu-id="69770-137">String</span></span>|<span data-ttu-id="69770-138">Расположение URL-адреса, куда экспортируются данные для запросов на экспорт.</span><span class="sxs-lookup"><span data-stu-id="69770-138">The URL location to where data is being exported for export requests.</span></span>|
|<span data-ttu-id="69770-139">userId</span><span class="sxs-lookup"><span data-stu-id="69770-139">userId</span></span>|<span data-ttu-id="69770-140">String</span><span class="sxs-lookup"><span data-stu-id="69770-140">String</span></span>|<span data-ttu-id="69770-141">ID для пользователя, на котором выполняется операция.</span><span class="sxs-lookup"><span data-stu-id="69770-141">The id for the user on whom the operation is performed.</span></span>|
|<span data-ttu-id="69770-142">submittedDateTime</span><span class="sxs-lookup"><span data-stu-id="69770-142">submittedDateTime</span></span>|<span data-ttu-id="69770-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="69770-143">DateTimeOffset</span></span>|<span data-ttu-id="69770-144">Представляет при отправке запроса на эту операцию данных во время UTC с помощью формата ISO 8601.</span><span class="sxs-lookup"><span data-stu-id="69770-144">Represents when the request for this data operation was submitted, in UTC time, using the ISO 8601 format.</span></span> <span data-ttu-id="69770-145">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="69770-145">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="69770-146">progress</span><span class="sxs-lookup"><span data-stu-id="69770-146">progress</span></span>|<span data-ttu-id="69770-147">String</span><span class="sxs-lookup"><span data-stu-id="69770-147">String</span></span>|<span data-ttu-id="69770-148">Указывает ход операции.</span><span class="sxs-lookup"><span data-stu-id="69770-148">Specifies the progress of an operation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="69770-149">Связи</span><span class="sxs-lookup"><span data-stu-id="69770-149">Relationships</span></span>
<span data-ttu-id="69770-150">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="69770-150">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="69770-151">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="69770-151">JSON representation</span></span>

<span data-ttu-id="69770-152">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="69770-152">The following is a JSON representation of the resource.</span></span>

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


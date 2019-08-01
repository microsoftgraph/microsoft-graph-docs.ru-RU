---
title: Тип ресурса dataPolicyOperation
description: Представляет отправленную операцию политики данных. Содержит необходимые сведения для отслеживания состояния операции. Например, администратор компании может отправить запрос операции политики данных для экспорта данных компании сотрудника, а затем отследить этот запрос.
author: ''
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 3c73bef8a640c950b6d85eb74ad93089aaad4f74
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36029556"
---
# <a name="datapolicyoperation-resource-type"></a><span data-ttu-id="0f4a4-105">Тип ресурса dataPolicyOperation</span><span class="sxs-lookup"><span data-stu-id="0f4a4-105">dataPolicyOperation resource type</span></span>

<span data-ttu-id="0f4a4-106">Представляет отправленную операцию политики данных.</span><span class="sxs-lookup"><span data-stu-id="0f4a4-106">Represents a submitted data policy operation.</span></span> <span data-ttu-id="0f4a4-107">Содержит необходимые сведения для отслеживания состояния операции.</span><span class="sxs-lookup"><span data-stu-id="0f4a4-107">It contains necessary information for tracking the status of an operation.</span></span> <span data-ttu-id="0f4a4-108">Например, администратор компании может отправить запрос операции политики данных для экспорта данных компании сотрудника, а затем отследить этот запрос.</span><span class="sxs-lookup"><span data-stu-id="0f4a4-108">For example, a company administrator can submit a data policy operation request to export an employee's company data, and then later track that request.</span></span>

## <a name="methods"></a><span data-ttu-id="0f4a4-109">Методы</span><span class="sxs-lookup"><span data-stu-id="0f4a4-109">Methods</span></span>

| <span data-ttu-id="0f4a4-110">Метод</span><span class="sxs-lookup"><span data-stu-id="0f4a4-110">Method</span></span>           | <span data-ttu-id="0f4a4-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="0f4a4-111">Return Type</span></span>    |<span data-ttu-id="0f4a4-112">Описание</span><span class="sxs-lookup"><span data-stu-id="0f4a4-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="0f4a4-113">Получение dataPolicyOperation</span><span class="sxs-lookup"><span data-stu-id="0f4a4-113">Get dataPolicyOperation</span></span>](../api/datapolicyoperation-get.md) | [<span data-ttu-id="0f4a4-114">dataPolicyOperation</span><span class="sxs-lookup"><span data-stu-id="0f4a4-114">dataPolicyOperation</span></span>](datapolicyoperation.md) |<span data-ttu-id="0f4a4-115">Получение свойств объекта **dataPolicyOperation** .</span><span class="sxs-lookup"><span data-stu-id="0f4a4-115">Retrieve properties of the **dataPolicyOperation** object.</span></span>|
|[<span data-ttu-id="0f4a4-116">Экспорт личных данных</span><span class="sxs-lookup"><span data-stu-id="0f4a4-116">Export personal data</span></span>](../api/user-exportpersonaldata.md) | <span data-ttu-id="0f4a4-117">Нет</span><span class="sxs-lookup"><span data-stu-id="0f4a4-117">None</span></span> |<span data-ttu-id="0f4a4-118">Отправить запрос операции политики данных для экспорта данных пользователя организации, которые впоследствии можно прочитать с помощью [Get dataPolicyOperation](../api/datapolicyoperation-get.md)</span><span class="sxs-lookup"><span data-stu-id="0f4a4-118">Submit a data policy operation request to export organizational user's data which can later be read using [Get dataPolicyOperation](../api/datapolicyoperation-get.md)</span></span>|

## <a name="properties"></a><span data-ttu-id="0f4a4-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="0f4a4-119">Properties</span></span>

> <span data-ttu-id="0f4a4-120">**Примечание:** Все свойства этого ресурса доступны только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0f4a4-120">**Note:** All properties of this resource are read-only.</span></span>

| <span data-ttu-id="0f4a4-121">Свойство</span><span class="sxs-lookup"><span data-stu-id="0f4a4-121">Property</span></span>     | <span data-ttu-id="0f4a4-122">Тип</span><span class="sxs-lookup"><span data-stu-id="0f4a4-122">Type</span></span>   |<span data-ttu-id="0f4a4-123">Описание</span><span class="sxs-lookup"><span data-stu-id="0f4a4-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0f4a4-124">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="0f4a4-124">completedDateTime</span></span>|<span data-ttu-id="0f4a4-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0f4a4-125">DateTimeOffset</span></span>|<span data-ttu-id="0f4a4-126">Представляет время завершения запроса для этой операции политики данных в формате UTC с использованием формата ISO 8601.</span><span class="sxs-lookup"><span data-stu-id="0f4a4-126">Represents when the request for this data policy operation was completed, in UTC time, using the ISO 8601 format.</span></span> <span data-ttu-id="0f4a4-127">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="0f4a4-127">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="0f4a4-128">Значение null до завершения операции.</span><span class="sxs-lookup"><span data-stu-id="0f4a4-128">Null until the operation completes.</span></span>|
|<span data-ttu-id="0f4a4-129">id</span><span class="sxs-lookup"><span data-stu-id="0f4a4-129">id</span></span>|<span data-ttu-id="0f4a4-130">Строка</span><span class="sxs-lookup"><span data-stu-id="0f4a4-130">String</span></span>| <span data-ttu-id="0f4a4-131">Уникальный ключ для этой операции.</span><span class="sxs-lookup"><span data-stu-id="0f4a4-131">Unique key for this operation.</span></span> |
|<span data-ttu-id="0f4a4-132">status</span><span class="sxs-lookup"><span data-stu-id="0f4a4-132">status</span></span>|<span data-ttu-id="0f4a4-133">string</span><span class="sxs-lookup"><span data-stu-id="0f4a4-133">string</span></span>| <span data-ttu-id="0f4a4-134">Возможные значения: `notStarted`, `running`, `complete`, `failed`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="0f4a4-134">Possible values are: `notStarted`, `running`, `complete`, `failed`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="0f4a4-135">Сторажелокатион</span><span class="sxs-lookup"><span data-stu-id="0f4a4-135">storageLocation</span></span>|<span data-ttu-id="0f4a4-136">String</span><span class="sxs-lookup"><span data-stu-id="0f4a4-136">String</span></span>|<span data-ttu-id="0f4a4-137">URL-адрес, по которому выполняется экспорт данных для запросов на экспорт.</span><span class="sxs-lookup"><span data-stu-id="0f4a4-137">The URL location to where data is being exported for export requests.</span></span>|
|<span data-ttu-id="0f4a4-138">userId</span><span class="sxs-lookup"><span data-stu-id="0f4a4-138">userId</span></span>|<span data-ttu-id="0f4a4-139">String</span><span class="sxs-lookup"><span data-stu-id="0f4a4-139">String</span></span>|<span data-ttu-id="0f4a4-140">Идентификатор пользователя, для которого выполняется операция.</span><span class="sxs-lookup"><span data-stu-id="0f4a4-140">The id for the user on whom the operation is performed.</span></span>|
|<span data-ttu-id="0f4a4-141">Субмиттеддатетиме</span><span class="sxs-lookup"><span data-stu-id="0f4a4-141">submittedDateTime</span></span>|<span data-ttu-id="0f4a4-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0f4a4-142">DateTimeOffset</span></span>|<span data-ttu-id="0f4a4-143">Представляет время отправки запроса для этой операции с данными в формате UTC с использованием формата ISO 8601.</span><span class="sxs-lookup"><span data-stu-id="0f4a4-143">Represents when the request for this data operation was submitted, in UTC time, using the ISO 8601 format.</span></span> <span data-ttu-id="0f4a4-144">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="0f4a4-144">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="0f4a4-145">progress</span><span class="sxs-lookup"><span data-stu-id="0f4a4-145">progress</span></span>|<span data-ttu-id="0f4a4-146">String</span><span class="sxs-lookup"><span data-stu-id="0f4a4-146">String</span></span>|<span data-ttu-id="0f4a4-147">Задает ход выполнения операции.</span><span class="sxs-lookup"><span data-stu-id="0f4a4-147">Specifies the progress of an operation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0f4a4-148">Отношения</span><span class="sxs-lookup"><span data-stu-id="0f4a4-148">Relationships</span></span>
<span data-ttu-id="0f4a4-149">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="0f4a4-149">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="0f4a4-150">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="0f4a4-150">JSON representation</span></span>

<span data-ttu-id="0f4a4-151">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0f4a4-151">The following is a JSON representation of the resource.</span></span>

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

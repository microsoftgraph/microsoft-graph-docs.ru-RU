---
title: Тип ресурса dataPolicyOperation
description: Представляет отправленную операцию политики данных. Содержит необходимые сведения для отслеживания состояния операции. Например, администратор компании может отправить запрос операции политики данных для экспорта данных компании сотрудника, а затем отследить этот запрос.
author: ''
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 80222ac0ab75d5ca3b67c62401b87882cc5b0209
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531727"
---
# <a name="datapolicyoperation-resource-type"></a><span data-ttu-id="fa571-105">Тип ресурса dataPolicyOperation</span><span class="sxs-lookup"><span data-stu-id="fa571-105">dataPolicyOperation resource type</span></span>

<span data-ttu-id="fa571-106">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fa571-106">Namespace: microsoft.graph</span></span>

<span data-ttu-id="fa571-107">Представляет отправленную операцию политики данных.</span><span class="sxs-lookup"><span data-stu-id="fa571-107">Represents a submitted data policy operation.</span></span> <span data-ttu-id="fa571-108">Содержит необходимые сведения для отслеживания состояния операции.</span><span class="sxs-lookup"><span data-stu-id="fa571-108">It contains necessary information for tracking the status of an operation.</span></span> <span data-ttu-id="fa571-109">Например, администратор компании может отправить запрос операции политики данных для экспорта данных компании сотрудника, а затем отследить этот запрос.</span><span class="sxs-lookup"><span data-stu-id="fa571-109">For example, a company administrator can submit a data policy operation request to export an employee's company data, and then later track that request.</span></span>

## <a name="methods"></a><span data-ttu-id="fa571-110">Методы</span><span class="sxs-lookup"><span data-stu-id="fa571-110">Methods</span></span>

| <span data-ttu-id="fa571-111">Метод</span><span class="sxs-lookup"><span data-stu-id="fa571-111">Method</span></span>           | <span data-ttu-id="fa571-112">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="fa571-112">Return Type</span></span>    |<span data-ttu-id="fa571-113">Описание</span><span class="sxs-lookup"><span data-stu-id="fa571-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="fa571-114">Получение dataPolicyOperation</span><span class="sxs-lookup"><span data-stu-id="fa571-114">Get dataPolicyOperation</span></span>](../api/datapolicyoperation-get.md) | [<span data-ttu-id="fa571-115">dataPolicyOperation</span><span class="sxs-lookup"><span data-stu-id="fa571-115">dataPolicyOperation</span></span>](datapolicyoperation.md) |<span data-ttu-id="fa571-116">Получение свойств объекта **dataPolicyOperation** .</span><span class="sxs-lookup"><span data-stu-id="fa571-116">Retrieve properties of the **dataPolicyOperation** object.</span></span>|
|[<span data-ttu-id="fa571-117">Экспорт личных данных</span><span class="sxs-lookup"><span data-stu-id="fa571-117">Export personal data</span></span>](../api/user-exportpersonaldata.md) | <span data-ttu-id="fa571-118">Нет</span><span class="sxs-lookup"><span data-stu-id="fa571-118">None</span></span> |<span data-ttu-id="fa571-119">Отправить запрос операции политики данных для экспорта данных пользователя организации, которые впоследствии можно прочитать с помощью [Get dataPolicyOperation](../api/datapolicyoperation-get.md)</span><span class="sxs-lookup"><span data-stu-id="fa571-119">Submit a data policy operation request to export organizational user's data which can later be read using [Get dataPolicyOperation](../api/datapolicyoperation-get.md)</span></span>|

## <a name="properties"></a><span data-ttu-id="fa571-120">Свойства</span><span class="sxs-lookup"><span data-stu-id="fa571-120">Properties</span></span>

> <span data-ttu-id="fa571-121">**Примечание:** Все свойства этого ресурса доступны только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fa571-121">**Note:** All properties of this resource are read-only.</span></span>

| <span data-ttu-id="fa571-122">Свойство</span><span class="sxs-lookup"><span data-stu-id="fa571-122">Property</span></span>     | <span data-ttu-id="fa571-123">Тип</span><span class="sxs-lookup"><span data-stu-id="fa571-123">Type</span></span>   |<span data-ttu-id="fa571-124">Описание</span><span class="sxs-lookup"><span data-stu-id="fa571-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fa571-125">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="fa571-125">completedDateTime</span></span>|<span data-ttu-id="fa571-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fa571-126">DateTimeOffset</span></span>|<span data-ttu-id="fa571-127">Представляет время завершения запроса для этой операции политики данных в формате UTC с использованием формата ISO 8601.</span><span class="sxs-lookup"><span data-stu-id="fa571-127">Represents when the request for this data policy operation was completed, in UTC time, using the ISO 8601 format.</span></span> <span data-ttu-id="fa571-128">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="fa571-128">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="fa571-129">Значение null до завершения операции.</span><span class="sxs-lookup"><span data-stu-id="fa571-129">Null until the operation completes.</span></span>|
|<span data-ttu-id="fa571-130">id</span><span class="sxs-lookup"><span data-stu-id="fa571-130">id</span></span>|<span data-ttu-id="fa571-131">Строка</span><span class="sxs-lookup"><span data-stu-id="fa571-131">String</span></span>| <span data-ttu-id="fa571-132">Уникальный ключ для этой операции.</span><span class="sxs-lookup"><span data-stu-id="fa571-132">Unique key for this operation.</span></span> |
|<span data-ttu-id="fa571-133">status</span><span class="sxs-lookup"><span data-stu-id="fa571-133">status</span></span>|<span data-ttu-id="fa571-134">string</span><span class="sxs-lookup"><span data-stu-id="fa571-134">string</span></span>| <span data-ttu-id="fa571-135">Возможные значения: `notStarted`, `running`, `complete`, `failed`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="fa571-135">Possible values are: `notStarted`, `running`, `complete`, `failed`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="fa571-136">сторажелокатион</span><span class="sxs-lookup"><span data-stu-id="fa571-136">storageLocation</span></span>|<span data-ttu-id="fa571-137">Строка</span><span class="sxs-lookup"><span data-stu-id="fa571-137">String</span></span>|<span data-ttu-id="fa571-138">URL-адрес, по которому выполняется экспорт данных для запросов на экспорт.</span><span class="sxs-lookup"><span data-stu-id="fa571-138">The URL location to where data is being exported for export requests.</span></span>|
|<span data-ttu-id="fa571-139">userId</span><span class="sxs-lookup"><span data-stu-id="fa571-139">userId</span></span>|<span data-ttu-id="fa571-140">String</span><span class="sxs-lookup"><span data-stu-id="fa571-140">String</span></span>|<span data-ttu-id="fa571-141">Идентификатор пользователя, для которого выполняется операция.</span><span class="sxs-lookup"><span data-stu-id="fa571-141">The id for the user on whom the operation is performed.</span></span>|
|<span data-ttu-id="fa571-142">субмиттеддатетиме</span><span class="sxs-lookup"><span data-stu-id="fa571-142">submittedDateTime</span></span>|<span data-ttu-id="fa571-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fa571-143">DateTimeOffset</span></span>|<span data-ttu-id="fa571-144">Представляет время отправки запроса для этой операции с данными в формате UTC с использованием формата ISO 8601.</span><span class="sxs-lookup"><span data-stu-id="fa571-144">Represents when the request for this data operation was submitted, in UTC time, using the ISO 8601 format.</span></span> <span data-ttu-id="fa571-145">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="fa571-145">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="fa571-146">progress</span><span class="sxs-lookup"><span data-stu-id="fa571-146">progress</span></span>|<span data-ttu-id="fa571-147">Строка</span><span class="sxs-lookup"><span data-stu-id="fa571-147">String</span></span>|<span data-ttu-id="fa571-148">Задает ход выполнения операции.</span><span class="sxs-lookup"><span data-stu-id="fa571-148">Specifies the progress of an operation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fa571-149">Связи</span><span class="sxs-lookup"><span data-stu-id="fa571-149">Relationships</span></span>
<span data-ttu-id="fa571-150">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="fa571-150">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="fa571-151">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="fa571-151">JSON representation</span></span>

<span data-ttu-id="fa571-152">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fa571-152">The following is a JSON representation of the resource.</span></span>

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

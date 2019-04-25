# <a name="datapolicyoperation-resource-type"></a><span data-ttu-id="2d81c-101">Тип ресурса dataPolicyOperation</span><span class="sxs-lookup"><span data-stu-id="2d81c-101">dataPolicyOperation resource type</span></span>

<span data-ttu-id="2d81c-102">Представляет отправленную операцию политики данных.</span><span class="sxs-lookup"><span data-stu-id="2d81c-102">Represents a submitted data policy operation.</span></span> <span data-ttu-id="2d81c-103">Содержит необходимые сведения для отслеживания состояния операции.</span><span class="sxs-lookup"><span data-stu-id="2d81c-103">It contains necessary information for tracking the status of an operation.</span></span> <span data-ttu-id="2d81c-104">Например, администратор компании может отправить запрос операции политики данных для экспорта данных компании сотрудника, а затем отследить этот запрос.</span><span class="sxs-lookup"><span data-stu-id="2d81c-104">For example, a company administrator can submit a data policy operation request to export an employee's company data, and then later track that request.</span></span>

## <a name="methods"></a><span data-ttu-id="2d81c-105">Методы</span><span class="sxs-lookup"><span data-stu-id="2d81c-105">Methods</span></span>

| <span data-ttu-id="2d81c-106">Метод</span><span class="sxs-lookup"><span data-stu-id="2d81c-106">Method</span></span>           | <span data-ttu-id="2d81c-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="2d81c-107">Return Type</span></span>    |<span data-ttu-id="2d81c-108">Описание</span><span class="sxs-lookup"><span data-stu-id="2d81c-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="2d81c-109">Получение dataPolicyOperation</span><span class="sxs-lookup"><span data-stu-id="2d81c-109">Get dataPolicyOperation</span></span>](../api/datapolicyoperation-get.md) | [<span data-ttu-id="2d81c-110">dataPolicyOperation</span><span class="sxs-lookup"><span data-stu-id="2d81c-110">dataPolicyOperation</span></span>](datapolicyoperation.md) |<span data-ttu-id="2d81c-111">Получение свойств объекта **dataPolicyOperation** .</span><span class="sxs-lookup"><span data-stu-id="2d81c-111">Retrieve properties of the **dataPolicyOperation** object.</span></span>|
|[<span data-ttu-id="2d81c-112">Экспорт личных данных</span><span class="sxs-lookup"><span data-stu-id="2d81c-112">Export personal data</span></span>](../api/user-exportpersonaldata.md) | <span data-ttu-id="2d81c-113">Нет</span><span class="sxs-lookup"><span data-stu-id="2d81c-113">None</span></span> |<span data-ttu-id="2d81c-114">Отправить запрос операции политики данных для экспорта данных пользователя организации, которые впоследствии можно прочитать с помощью [Get dataPolicyOperation](../api/datapolicyoperation-get.md)</span><span class="sxs-lookup"><span data-stu-id="2d81c-114">Submit a data policy operation request to export organizational user's data which can later be read using [Get dataPolicyOperation](../api/datapolicyoperation-get.md)</span></span>|

## <a name="properties"></a><span data-ttu-id="2d81c-115">Свойства</span><span class="sxs-lookup"><span data-stu-id="2d81c-115">Properties</span></span>

> <span data-ttu-id="2d81c-116">**Примечание:** Все свойства этого ресурса доступны только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2d81c-116">**Note:** All properties of this resource are read-only.</span></span>

| <span data-ttu-id="2d81c-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="2d81c-117">Property</span></span>     | <span data-ttu-id="2d81c-118">Тип</span><span class="sxs-lookup"><span data-stu-id="2d81c-118">Type</span></span>   |<span data-ttu-id="2d81c-119">Описание</span><span class="sxs-lookup"><span data-stu-id="2d81c-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2d81c-120">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="2d81c-120">completedDateTime</span></span>|<span data-ttu-id="2d81c-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2d81c-121">DateTimeOffset</span></span>|<span data-ttu-id="2d81c-122">Представляет время завершения запроса для этой операции политики данных в формате UTC с использованием формата ISO 8601.</span><span class="sxs-lookup"><span data-stu-id="2d81c-122">Represents when the request for this data policy operation was completed, in UTC time, using the ISO 8601 format.</span></span> <span data-ttu-id="2d81c-123">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="2d81c-123">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="2d81c-124">Значение null до завершения операции.</span><span class="sxs-lookup"><span data-stu-id="2d81c-124">Null until the operation completes.</span></span>|
|<span data-ttu-id="2d81c-125">id</span><span class="sxs-lookup"><span data-stu-id="2d81c-125">id</span></span>|<span data-ttu-id="2d81c-126">Строка</span><span class="sxs-lookup"><span data-stu-id="2d81c-126">String</span></span>| <span data-ttu-id="2d81c-127">Уникальный ключ для этой операции.</span><span class="sxs-lookup"><span data-stu-id="2d81c-127">Unique key for this operation.</span></span> |
|<span data-ttu-id="2d81c-128">status</span><span class="sxs-lookup"><span data-stu-id="2d81c-128">status</span></span>|<span data-ttu-id="2d81c-129">string</span><span class="sxs-lookup"><span data-stu-id="2d81c-129">string</span></span>| <span data-ttu-id="2d81c-130">Возможные значения: `notStarted`, `running`, `complete`, `failed`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="2d81c-130">Possible values are: `notStarted`, `running`, `complete`, `failed`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="2d81c-131">Сторажелокатион</span><span class="sxs-lookup"><span data-stu-id="2d81c-131">storageLocation</span></span>|<span data-ttu-id="2d81c-132">String</span><span class="sxs-lookup"><span data-stu-id="2d81c-132">String</span></span>|<span data-ttu-id="2d81c-133">URL-адрес, по которому выполняется экспорт данных для запросов на экспорт.</span><span class="sxs-lookup"><span data-stu-id="2d81c-133">The URL location to where data is being exported for export requests.</span></span>|
|<span data-ttu-id="2d81c-134">userId</span><span class="sxs-lookup"><span data-stu-id="2d81c-134">userId</span></span>|<span data-ttu-id="2d81c-135">String</span><span class="sxs-lookup"><span data-stu-id="2d81c-135">String</span></span>|<span data-ttu-id="2d81c-136">Идентификатор пользователя, для которого выполняется операция.</span><span class="sxs-lookup"><span data-stu-id="2d81c-136">The id for the user on whom the operation is performed.</span></span>|
|<span data-ttu-id="2d81c-137">Субмиттеддатетиме</span><span class="sxs-lookup"><span data-stu-id="2d81c-137">submittedDateTime</span></span>|<span data-ttu-id="2d81c-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2d81c-138">DateTimeOffset</span></span>|<span data-ttu-id="2d81c-139">Представляет время отправки запроса для этой операции с данными в формате UTC с использованием формата ISO 8601.</span><span class="sxs-lookup"><span data-stu-id="2d81c-139">Represents when the request for this data operation was submitted, in UTC time, using the ISO 8601 format.</span></span> <span data-ttu-id="2d81c-140">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="2d81c-140">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="2d81c-141">progress</span><span class="sxs-lookup"><span data-stu-id="2d81c-141">progress</span></span>|<span data-ttu-id="2d81c-142">String</span><span class="sxs-lookup"><span data-stu-id="2d81c-142">String</span></span>|<span data-ttu-id="2d81c-143">Задает ход выполнения операции.</span><span class="sxs-lookup"><span data-stu-id="2d81c-143">Specifies the progress of an operation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2d81c-144">Связи</span><span class="sxs-lookup"><span data-stu-id="2d81c-144">Relationships</span></span>
<span data-ttu-id="2d81c-145">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="2d81c-145">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="2d81c-146">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2d81c-146">JSON representation</span></span>

<span data-ttu-id="2d81c-147">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2d81c-147">The following is a JSON representation of the resource.</span></span>

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

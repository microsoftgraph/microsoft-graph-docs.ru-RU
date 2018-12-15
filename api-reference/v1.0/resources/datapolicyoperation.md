# <a name="datapolicyoperation-resource-type"></a><span data-ttu-id="e60c1-101">Тип ресурса dataPolicyOperation</span><span class="sxs-lookup"><span data-stu-id="e60c1-101">dataPolicyOperation resource type</span></span>

<span data-ttu-id="e60c1-102">Представляет операцию политики отправленных данных.</span><span class="sxs-lookup"><span data-stu-id="e60c1-102">Represents a submitted data policy operation.</span></span> <span data-ttu-id="e60c1-103">Он содержит сведения, необходимые для отслеживания состояния операции.</span><span class="sxs-lookup"><span data-stu-id="e60c1-103">It contains necessary information for tracking the status of an operation.</span></span> <span data-ttu-id="e60c1-104">Например администратор компании запрос данных политики операции экспорта данных сотрудника компании и затем отслеживать этот запрос.</span><span class="sxs-lookup"><span data-stu-id="e60c1-104">For example, a company administrator can submit a data policy operation request to export an employee's company data, and then later track that request.</span></span>

## <a name="methods"></a><span data-ttu-id="e60c1-105">Методы</span><span class="sxs-lookup"><span data-stu-id="e60c1-105">Methods</span></span>

| <span data-ttu-id="e60c1-106">Метод</span><span class="sxs-lookup"><span data-stu-id="e60c1-106">Method</span></span>           | <span data-ttu-id="e60c1-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="e60c1-107">Return Type</span></span>    |<span data-ttu-id="e60c1-108">Описание</span><span class="sxs-lookup"><span data-stu-id="e60c1-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e60c1-109">Получение dataPolicyOperation</span><span class="sxs-lookup"><span data-stu-id="e60c1-109">Get dataPolicyOperation</span></span>](../api/datapolicyoperation-get.md) | [<span data-ttu-id="e60c1-110">dataPolicyOperation</span><span class="sxs-lookup"><span data-stu-id="e60c1-110">dataPolicyOperation</span></span>](datapolicyoperation.md) |<span data-ttu-id="e60c1-111">Извлечение свойств объекта **dataPolicyOperation** .</span><span class="sxs-lookup"><span data-stu-id="e60c1-111">Retrieve properties of the **dataPolicyOperation** object.</span></span>|
|[<span data-ttu-id="e60c1-112">Экспорт личных данных</span><span class="sxs-lookup"><span data-stu-id="e60c1-112">Export personal data</span></span>](../api/user-exportpersonaldata.md) | <span data-ttu-id="e60c1-113">Нет</span><span class="sxs-lookup"><span data-stu-id="e60c1-113">None</span></span> |<span data-ttu-id="e60c1-114">Запрос данных политики операция экспортировать данные организации пользователя, можно просмотреть более поздней версии с помощью [получения dataPolicyOperation](../api/datapolicyoperation-get.md)</span><span class="sxs-lookup"><span data-stu-id="e60c1-114">Submit a data policy operation request to export organizational user's data which can later be read using [Get dataPolicyOperation](../api/datapolicyoperation-get.md)</span></span>|

## <a name="properties"></a><span data-ttu-id="e60c1-115">Свойства</span><span class="sxs-lookup"><span data-stu-id="e60c1-115">Properties</span></span>

> <span data-ttu-id="e60c1-116">**Примечание:** Все свойства в этом ресурсов доступны только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e60c1-116">**Note:** All properties of this resource are read-only.</span></span>

| <span data-ttu-id="e60c1-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="e60c1-117">Property</span></span>     | <span data-ttu-id="e60c1-118">Тип</span><span class="sxs-lookup"><span data-stu-id="e60c1-118">Type</span></span>   |<span data-ttu-id="e60c1-119">Описание</span><span class="sxs-lookup"><span data-stu-id="e60c1-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e60c1-120">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="e60c1-120">completedDateTime</span></span>|<span data-ttu-id="e60c1-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e60c1-121">DateTimeOffset</span></span>|<span data-ttu-id="e60c1-122">Представляет, когда запрос для этой операции политики данных был выполнен, в формате UTC, в формате ISO 8601.</span><span class="sxs-lookup"><span data-stu-id="e60c1-122">Represents when the request for this data policy operation was completed, in UTC time, using the ISO 8601 format.</span></span> <span data-ttu-id="e60c1-123">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="e60c1-123">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="e60c1-124">NULL до завершения операции.</span><span class="sxs-lookup"><span data-stu-id="e60c1-124">Null until the operation completes.</span></span>|
|<span data-ttu-id="e60c1-125">id</span><span class="sxs-lookup"><span data-stu-id="e60c1-125">id</span></span>|<span data-ttu-id="e60c1-126">Строка</span><span class="sxs-lookup"><span data-stu-id="e60c1-126">String</span></span>| <span data-ttu-id="e60c1-127">Уникальный ключ для этой операции.</span><span class="sxs-lookup"><span data-stu-id="e60c1-127">Unique key for this operation.</span></span> |
|<span data-ttu-id="e60c1-128">status</span><span class="sxs-lookup"><span data-stu-id="e60c1-128">status</span></span>|<span data-ttu-id="e60c1-129">строка</span><span class="sxs-lookup"><span data-stu-id="e60c1-129">string</span></span>| <span data-ttu-id="e60c1-130">Возможные значения: `notStarted`, `running`, `complete`, `failed`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="e60c1-130">Possible values are: `notStarted`, `running`, `complete`, `failed`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="e60c1-131">storageLocation</span><span class="sxs-lookup"><span data-stu-id="e60c1-131">storageLocation</span></span>|<span data-ttu-id="e60c1-132">String.</span><span class="sxs-lookup"><span data-stu-id="e60c1-132">String</span></span>|<span data-ttu-id="e60c1-133">URL-адрес расположения, в котором выполняется экспорт данных для запросы на экспорт.</span><span class="sxs-lookup"><span data-stu-id="e60c1-133">The URL location to where data is being exported for export requests.</span></span>|
|<span data-ttu-id="e60c1-134">userId</span><span class="sxs-lookup"><span data-stu-id="e60c1-134">userId</span></span>|<span data-ttu-id="e60c1-135">String</span><span class="sxs-lookup"><span data-stu-id="e60c1-135">String</span></span>|<span data-ttu-id="e60c1-136">Идентификатор пользователя, для которого выполняется операция.</span><span class="sxs-lookup"><span data-stu-id="e60c1-136">The id for the user on whom the operation is performed.</span></span>|
|<span data-ttu-id="e60c1-137">submittedDateTime</span><span class="sxs-lookup"><span data-stu-id="e60c1-137">submittedDateTime</span></span>|<span data-ttu-id="e60c1-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e60c1-138">DateTimeOffset</span></span>|<span data-ttu-id="e60c1-139">Представляет, когда для этой операции с данными был отправлен запрос, в формате UTC, в формате ISO 8601.</span><span class="sxs-lookup"><span data-stu-id="e60c1-139">Represents when the request for this data operation was submitted, in UTC time, using the ISO 8601 format.</span></span> <span data-ttu-id="e60c1-140">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="e60c1-140">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="e60c1-141">Ход выполнения</span><span class="sxs-lookup"><span data-stu-id="e60c1-141">progress</span></span>|<span data-ttu-id="e60c1-142">String.</span><span class="sxs-lookup"><span data-stu-id="e60c1-142">String</span></span>|<span data-ttu-id="e60c1-143">Указывает ход выполнения операции.</span><span class="sxs-lookup"><span data-stu-id="e60c1-143">Specifies the progress of an operation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e60c1-144">Связи</span><span class="sxs-lookup"><span data-stu-id="e60c1-144">Relationships</span></span>
<span data-ttu-id="e60c1-145">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="e60c1-145">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="e60c1-146">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="e60c1-146">JSON representation</span></span>

<span data-ttu-id="e60c1-147">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e60c1-147">The following is a JSON representation of the resource.</span></span>

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

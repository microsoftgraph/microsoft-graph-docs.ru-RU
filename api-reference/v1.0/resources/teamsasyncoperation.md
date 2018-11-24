# <a name="teamsasyncoperation-resource-type"></a><span data-ttu-id="d4b37-101">Тип ресурса teamsAsyncOperation</span><span class="sxs-lookup"><span data-stu-id="d4b37-101">teamsAsyncOperation resource type</span></span>



<span data-ttu-id="d4b37-102">Операцию асинхронного группами Майкрософт — это операция, выходит за рамки жизненным циклом одним запросом API.</span><span class="sxs-lookup"><span data-stu-id="d4b37-102">A Microsoft Teams async operation is an operation that transcends the lifetime of a single API request.</span></span> <span data-ttu-id="d4b37-103">Эти операции выполняются длительным или слишком дорого для выполнения в рамках интервала времени их исходного запроса.</span><span class="sxs-lookup"><span data-stu-id="d4b37-103">These operations are long-running or too expensive to complete within the timeframe of their originating request.</span></span>

<span data-ttu-id="d4b37-104">При запуске асинхронной операции, метод возвращает 202 код ответа принято.</span><span class="sxs-lookup"><span data-stu-id="d4b37-104">When an async operation is initiated, the method returns a 202 Accepted response code.</span></span> <span data-ttu-id="d4b37-105">Ответ также будет содержать заголовок расположения, который содержит расположение teamsAsyncOperation.</span><span class="sxs-lookup"><span data-stu-id="d4b37-105">The response will also contain a Location header, which contains the location of the teamsAsyncOperation.</span></span> <span data-ttu-id="d4b37-106">Периодически проверяйте состояние операции, сделав запрос GET по этому адресу; Подождите > 30 секунд между проверок.</span><span class="sxs-lookup"><span data-stu-id="d4b37-106">Periodically check the status of the operation by making a GET request to this location; wait >30 seconds between checks.</span></span>
<span data-ttu-id="d4b37-107">После успешного завершения запроса состояния будет иметь «выполнена успешно» и targetResourceLocation будет указывать на ресурс созданные или измененные.</span><span class="sxs-lookup"><span data-stu-id="d4b37-107">When the request completes successfully, the status will be "succeeded" and the targetResourceLocation will point to the created/modified resource.</span></span>

## <a name="properties"></a><span data-ttu-id="d4b37-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="d4b37-108">Properties</span></span>

| <span data-ttu-id="d4b37-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="d4b37-109">Property</span></span> | <span data-ttu-id="d4b37-110">Тип</span><span class="sxs-lookup"><span data-stu-id="d4b37-110">Type</span></span>   | <span data-ttu-id="d4b37-111">Описание</span><span class="sxs-lookup"><span data-stu-id="d4b37-111">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="d4b37-112">id</span><span class="sxs-lookup"><span data-stu-id="d4b37-112">id</span></span>|<span data-ttu-id="d4b37-113">строка</span><span class="sxs-lookup"><span data-stu-id="d4b37-113">string</span></span> |<span data-ttu-id="d4b37-114">Операция уникальный идентификатор.</span><span class="sxs-lookup"><span data-stu-id="d4b37-114">Unique operation id.</span></span>|
|<span data-ttu-id="d4b37-115">operationType</span><span class="sxs-lookup"><span data-stu-id="d4b37-115">operationType</span></span>|[<span data-ttu-id="d4b37-116">teamsAsyncOperationType</span><span class="sxs-lookup"><span data-stu-id="d4b37-116">teamsAsyncOperationType</span></span>](teamsasyncoperationtype.md) |<span data-ttu-id="d4b37-117">Указывает, какой тип операции, описанного.</span><span class="sxs-lookup"><span data-stu-id="d4b37-117">Denotes which type of operation is being described.</span></span>|
|<span data-ttu-id="d4b37-118">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d4b37-118">createdDateTime</span></span>|<span data-ttu-id="d4b37-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d4b37-119">DateTimeOffset</span></span> |<span data-ttu-id="d4b37-120">Время создания операции.</span><span class="sxs-lookup"><span data-stu-id="d4b37-120">Time when the operation was created.</span></span>|
|<span data-ttu-id="d4b37-121">status</span><span class="sxs-lookup"><span data-stu-id="d4b37-121">status</span></span>|[<span data-ttu-id="d4b37-122">teamsAsyncOperationStatus</span><span class="sxs-lookup"><span data-stu-id="d4b37-122">teamsAsyncOperationStatus</span></span>](teamsasyncoperationstatus.md)| <span data-ttu-id="d4b37-123">Состояние операции.</span><span class="sxs-lookup"><span data-stu-id="d4b37-123">Operation status.</span></span>|
|<span data-ttu-id="d4b37-124">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="d4b37-124">lastActionDateTime</span></span>|<span data-ttu-id="d4b37-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d4b37-125">DateTimeOffset</span></span> |<span data-ttu-id="d4b37-126">Время последнего обновления асинхронной операции.</span><span class="sxs-lookup"><span data-stu-id="d4b37-126">Time when the async operation was last updated.</span></span>|
|<span data-ttu-id="d4b37-127">attemptsCount</span><span class="sxs-lookup"><span data-stu-id="d4b37-127">attemptsCount</span></span>|<span data-ttu-id="d4b37-128">Int32</span><span class="sxs-lookup"><span data-stu-id="d4b37-128">Int32</span></span>|<span data-ttu-id="d4b37-129">Количество раз, когда операция перед помечаются как успешные и неудачные.</span><span class="sxs-lookup"><span data-stu-id="d4b37-129">Number of times the operation was attempted before being marked successful or failed.</span></span>|
|<span data-ttu-id="d4b37-130">targetResourceId</span><span class="sxs-lookup"><span data-stu-id="d4b37-130">targetResourceId</span></span>|<span data-ttu-id="d4b37-131">Идентификатор GUID</span><span class="sxs-lookup"><span data-stu-id="d4b37-131">guid</span></span> |<span data-ttu-id="d4b37-132">Идентификатор объекта, который создал или изменены в результате этой асинхронной операции, обычно [группы](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="d4b37-132">The ID of the object that's created or modified as result of this async operation, typically a [team](../resources/team.md).</span></span>|
|<span data-ttu-id="d4b37-133">targetResourceLocation</span><span class="sxs-lookup"><span data-stu-id="d4b37-133">targetResourceLocation</span></span>|<span data-ttu-id="d4b37-134">string</span><span class="sxs-lookup"><span data-stu-id="d4b37-134">string</span></span>|<span data-ttu-id="d4b37-135">Расположение объекта, который создал или изменил как результат этой асинхронной операции.</span><span class="sxs-lookup"><span data-stu-id="d4b37-135">The location of the object that's created or modified as result of this async operation.</span></span> <span data-ttu-id="d4b37-136">Этот URL-адрес следует рассматривать как Непрозрачное значение и не синтаксический анализ в его компонента пути.</span><span class="sxs-lookup"><span data-stu-id="d4b37-136">This URL should be treated as an opaque value and not parsed into its component paths.</span></span>|
|<span data-ttu-id="d4b37-137">error</span><span class="sxs-lookup"><span data-stu-id="d4b37-137">error</span></span>|[<span data-ttu-id="d4b37-138">operationError</span><span class="sxs-lookup"><span data-stu-id="d4b37-138">operationError</span></span>](operationerror.md)|<span data-ttu-id="d4b37-139">Любая ошибка, которая приводит к сбою асинхронной операции.</span><span class="sxs-lookup"><span data-stu-id="d4b37-139">Any error that causes the async operation to fail.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d4b37-140">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d4b37-140">JSON representation</span></span>

<span data-ttu-id="d4b37-141">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d4b37-141">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.teamsasyncoperation"
}-->

```json
{
    "id": "string",
    "operationType": "archiveTeam",
    "createdDateTime": "2018-01-01T00:00:00.0000000Z",
    "status": "succeeded",
    "lastActionDateTime": "2018-01-01T00:00:00.0000000Z",
    "attemptsCount": 1,
    "targetResourceId": "fa4aa5a2-a75b-4769-86f4-9e2742a18fda",
    "targetResourceLocation": "/groups('fa4aa5a2-a75b-4769-86f4-9e2742a18fda')/team",
    "error": null
}
```

<!-- uuid: 20fd7863-9545-40d4-ae8f-fee2d115a690
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teams async operation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

# <a name="onenoteoperation-resource-type"></a><span data-ttu-id="1378a-101">Тип ресурса onenoteOperation</span><span class="sxs-lookup"><span data-stu-id="1378a-101">onenoteOperation resource type</span></span>

<span data-ttu-id="1378a-102">Состояние определенных операций OneNote, выполняющихся в течение длительного времени.</span><span class="sxs-lookup"><span data-stu-id="1378a-102">The status of certain long-running OneNote operations.</span></span>

## <a name="json-representation"></a><span data-ttu-id="1378a-103">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="1378a-103">JSON representation</span></span>

<span data-ttu-id="1378a-104">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1378a-104">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onenoteOperation"
}-->

```json
{
  "createdDateTime": "String (timestamp)",
  "error": {"@odata.type": "microsoft.graph.onenoteOperationError"},
  "id": "string (identifier)",
  "lastActionDateTime": "String (timestamp)",
  "resourceId": "string",
  "resourceLocation": "string",
  "status": "string",
  "percentComplete": "string"
}

```
## <a name="properties"></a><span data-ttu-id="1378a-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="1378a-105">Properties</span></span>
| <span data-ttu-id="1378a-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="1378a-106">Property</span></span>     | <span data-ttu-id="1378a-107">Тип</span><span class="sxs-lookup"><span data-stu-id="1378a-107">Type</span></span>   |<span data-ttu-id="1378a-108">Описание</span><span class="sxs-lookup"><span data-stu-id="1378a-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1378a-109">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1378a-109">createdDateTime</span></span>| <span data-ttu-id="1378a-110">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1378a-110">DateTimeOffset</span></span> |<span data-ttu-id="1378a-111">Время начала операции.</span><span class="sxs-lookup"><span data-stu-id="1378a-111">The start time of the operation.</span></span>|
|<span data-ttu-id="1378a-112">error</span><span class="sxs-lookup"><span data-stu-id="1378a-112">error</span></span>|[<span data-ttu-id="1378a-113">onenoteOperationError</span><span class="sxs-lookup"><span data-stu-id="1378a-113">onenoteOperationError</span></span>](onenoteoperationerror.md)|<span data-ttu-id="1378a-114">Ошибка при выполнении операции.</span><span class="sxs-lookup"><span data-stu-id="1378a-114">The error returned by the operation.</span></span>|
|<span data-ttu-id="1378a-115">id</span><span class="sxs-lookup"><span data-stu-id="1378a-115">id</span></span>|<span data-ttu-id="1378a-116">string</span><span class="sxs-lookup"><span data-stu-id="1378a-116">string</span></span>|<span data-ttu-id="1378a-117">Идентификатор операции. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1378a-117">The operation id. Read-only.</span></span>|
|<span data-ttu-id="1378a-118">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="1378a-118">lastActionDateTime</span></span>| <span data-ttu-id="1378a-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1378a-119">DateTimeOffset</span></span> |<span data-ttu-id="1378a-120">Время последнего действия операции.</span><span class="sxs-lookup"><span data-stu-id="1378a-120">The time of the last action of the operation.</span></span>|
|<span data-ttu-id="1378a-121">resourceId</span><span class="sxs-lookup"><span data-stu-id="1378a-121">resourceId</span></span>|<span data-ttu-id="1378a-122">string</span><span class="sxs-lookup"><span data-stu-id="1378a-122">string</span></span>|<span data-ttu-id="1378a-123">Идентификатор ресурса.</span><span class="sxs-lookup"><span data-stu-id="1378a-123">The resource id.</span></span>|
|<span data-ttu-id="1378a-124">resourceLocation</span><span class="sxs-lookup"><span data-stu-id="1378a-124">resourceLocation</span></span>|<span data-ttu-id="1378a-125">string</span><span class="sxs-lookup"><span data-stu-id="1378a-125">string</span></span>|<span data-ttu-id="1378a-p101">URI ресурса для объекта. Например, URI ресурса для скопированной страницы или раздела.</span><span class="sxs-lookup"><span data-stu-id="1378a-p101">The resource URI for the object. For example, the resource URI for a copied page or section.</span></span> |
|<span data-ttu-id="1378a-128">status</span><span class="sxs-lookup"><span data-stu-id="1378a-128">status</span></span>|<span data-ttu-id="1378a-129">string</span><span class="sxs-lookup"><span data-stu-id="1378a-129">string</span></span>|<span data-ttu-id="1378a-130">Текущее состояние операции: `notstarted`, `running`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="1378a-130">The current status of the operation: `notstarted`, `running`, `completed`, `failed`</span></span> |
|<span data-ttu-id="1378a-131">percentComplete</span><span class="sxs-lookup"><span data-stu-id="1378a-131">percentComplete</span></span>|<span data-ttu-id="1378a-132">string</span><span class="sxs-lookup"><span data-stu-id="1378a-132">string</span></span>|<span data-ttu-id="1378a-133">Процент завершения операции, если операция в состоянии `running`.</span><span class="sxs-lookup"><span data-stu-id="1378a-133">The operation percent complete if the operation is still in `running` status</span></span>

## <a name="relationships"></a><span data-ttu-id="1378a-134">Связи</span><span class="sxs-lookup"><span data-stu-id="1378a-134">Relationships</span></span>
<span data-ttu-id="1378a-135">Нет</span><span class="sxs-lookup"><span data-stu-id="1378a-135">None</span></span>


## <a name="methods"></a><span data-ttu-id="1378a-136">Методы</span><span class="sxs-lookup"><span data-stu-id="1378a-136">Methods</span></span>

| <span data-ttu-id="1378a-137">Метод</span><span class="sxs-lookup"><span data-stu-id="1378a-137">Method</span></span>           | <span data-ttu-id="1378a-138">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="1378a-138">Return Type</span></span>    |<span data-ttu-id="1378a-139">Описание</span><span class="sxs-lookup"><span data-stu-id="1378a-139">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="1378a-140">Получение операции</span><span class="sxs-lookup"><span data-stu-id="1378a-140">Get operation</span></span>](../api/onenoteoperation_get.md) | [<span data-ttu-id="1378a-141">onenoteOperation</span><span class="sxs-lookup"><span data-stu-id="1378a-141">onenoteOperation</span></span>](onenoteoperation.md) |<span data-ttu-id="1378a-142">Получение состояния операции.</span><span class="sxs-lookup"><span data-stu-id="1378a-142">Get the status of the operation.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onenoteOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

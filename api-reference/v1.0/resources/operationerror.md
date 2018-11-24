# <a name="operationerror-resource-type"></a><span data-ttu-id="5b9e7-101">Тип ресурса operationError</span><span class="sxs-lookup"><span data-stu-id="5b9e7-101">operationError resource type</span></span>



<span data-ttu-id="5b9e7-102">Описание ошибки в [teamsAsyncOperation](teamsasyncoperation.md).</span><span class="sxs-lookup"><span data-stu-id="5b9e7-102">Describes errors in [teamsAsyncOperation](teamsasyncoperation.md).</span></span>

## <a name="operationerror-properties"></a><span data-ttu-id="5b9e7-103">operationError свойства</span><span class="sxs-lookup"><span data-stu-id="5b9e7-103">operationError Properties</span></span>
| <span data-ttu-id="5b9e7-104">Свойство</span><span class="sxs-lookup"><span data-stu-id="5b9e7-104">Property</span></span>     | <span data-ttu-id="5b9e7-105">Тип</span><span class="sxs-lookup"><span data-stu-id="5b9e7-105">Type</span></span>   |<span data-ttu-id="5b9e7-106">Описание</span><span class="sxs-lookup"><span data-stu-id="5b9e7-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5b9e7-107">code</span><span class="sxs-lookup"><span data-stu-id="5b9e7-107">code</span></span>|<span data-ttu-id="5b9e7-108">String (только для чтения)</span><span class="sxs-lookup"><span data-stu-id="5b9e7-108">string (readonly)</span></span>|<span data-ttu-id="5b9e7-109">Код ошибки операции.</span><span class="sxs-lookup"><span data-stu-id="5b9e7-109">Operation error code.</span></span>|
|<span data-ttu-id="5b9e7-110">message</span><span class="sxs-lookup"><span data-stu-id="5b9e7-110">message</span></span>|<span data-ttu-id="5b9e7-111">String (только для чтения)</span><span class="sxs-lookup"><span data-stu-id="5b9e7-111">string (readonly)</span></span>|<span data-ttu-id="5b9e7-112">Сообщение об ошибке операции.</span><span class="sxs-lookup"><span data-stu-id="5b9e7-112">Operation error message.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5b9e7-113">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5b9e7-113">JSON representation</span></span>

<span data-ttu-id="5b9e7-114">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5b9e7-114">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.operationError"
}-->

```json
{
    "code": "TeamUnavailable",
    "message": "The team was not found."
}
```

<!-- uuid: 069fadaa-52db-4ced-85d5-74f7caa2c66f
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "operation error resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

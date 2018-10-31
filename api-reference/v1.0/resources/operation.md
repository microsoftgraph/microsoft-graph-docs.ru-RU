# <a name="operation-resource-type"></a><span data-ttu-id="433bc-101">тип ресурса операции</span><span class="sxs-lookup"><span data-stu-id="433bc-101">operation resource type</span></span>

<span data-ttu-id="433bc-102">Состояние долго выполняемой операции.</span><span class="sxs-lookup"><span data-stu-id="433bc-102">The status of a long-running operation.</span></span>

## <a name="json-representation"></a><span data-ttu-id="433bc-103">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="433bc-103">JSON representation</span></span>

<span data-ttu-id="433bc-104">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="433bc-104">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.operation"
}-->

```json
{
  "createdDateTime": "String (timestamp)",
  "lastActionDateTime": "String (timestamp)",
  "status": "notStarted | running | completed | failed"
}

```
## <a name="properties"></a><span data-ttu-id="433bc-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="433bc-105">Properties</span></span>
| <span data-ttu-id="433bc-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="433bc-106">Property</span></span>     | <span data-ttu-id="433bc-107">Тип</span><span class="sxs-lookup"><span data-stu-id="433bc-107">Type</span></span>   |<span data-ttu-id="433bc-108">Описание</span><span class="sxs-lookup"><span data-stu-id="433bc-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="433bc-109">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="433bc-109">createdDateTime</span></span>| <span data-ttu-id="433bc-110">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="433bc-110">DateTimeOffset</span></span> |<span data-ttu-id="433bc-111">Время начала операции.</span><span class="sxs-lookup"><span data-stu-id="433bc-111">The start time of the operation.</span></span>|
|<span data-ttu-id="433bc-112">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="433bc-112">lastActionDateTime</span></span>| <span data-ttu-id="433bc-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="433bc-113">DateTimeOffset</span></span> |<span data-ttu-id="433bc-114">Время последнего действия операции.</span><span class="sxs-lookup"><span data-stu-id="433bc-114">The time of the last action of the operation.</span></span>|
|<span data-ttu-id="433bc-115">статус</span><span class="sxs-lookup"><span data-stu-id="433bc-115">status</span></span>|<span data-ttu-id="433bc-116">operationStatus</span><span class="sxs-lookup"><span data-stu-id="433bc-116">operationStatus</span></span>|<span data-ttu-id="433bc-117">Текущее состояние операции: `notStarted`, `running`, `completed`, `failed`</span><span class="sxs-lookup"><span data-stu-id="433bc-117">The current status of the operation: `notStarted`, `running`, `completed`, `failed`</span></span> |

<!-- uuid: 13fa92b1-3b41-498b-aab1-f943464a124f
2018-03-30 10:29:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "operation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

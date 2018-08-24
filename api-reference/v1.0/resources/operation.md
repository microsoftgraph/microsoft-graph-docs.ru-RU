# <a name="operation-resource-type"></a><span data-ttu-id="f6ccb-101">тип ресурса операции</span><span class="sxs-lookup"><span data-stu-id="f6ccb-101">operation resource type</span></span>

<span data-ttu-id="f6ccb-102">Состояние долго выполняемой операции.</span><span class="sxs-lookup"><span data-stu-id="f6ccb-102">The status of a long-running operation.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f6ccb-103">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f6ccb-103">JSON representation</span></span>

<span data-ttu-id="f6ccb-104">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f6ccb-104">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="f6ccb-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="f6ccb-105">Properties</span></span>
| <span data-ttu-id="f6ccb-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="f6ccb-106">Property</span></span>     | <span data-ttu-id="f6ccb-107">Тип</span><span class="sxs-lookup"><span data-stu-id="f6ccb-107">Type</span></span>   |<span data-ttu-id="f6ccb-108">Описание</span><span class="sxs-lookup"><span data-stu-id="f6ccb-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f6ccb-109">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f6ccb-109">createdDateTime</span></span>| <span data-ttu-id="f6ccb-110">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f6ccb-110">DateTimeOffset</span></span> |<span data-ttu-id="f6ccb-111">Время начала операции.</span><span class="sxs-lookup"><span data-stu-id="f6ccb-111">The start time of the operation.</span></span>|
|<span data-ttu-id="f6ccb-112">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="f6ccb-112">lastActionDateTime</span></span>| <span data-ttu-id="f6ccb-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f6ccb-113">DateTimeOffset</span></span> |<span data-ttu-id="f6ccb-114">Время последнего действия операции.</span><span class="sxs-lookup"><span data-stu-id="f6ccb-114">The time of the last action of the operation.</span></span>|
|<span data-ttu-id="f6ccb-115">статус</span><span class="sxs-lookup"><span data-stu-id="f6ccb-115">status</span></span>|<span data-ttu-id="f6ccb-116">operationStatus</span><span class="sxs-lookup"><span data-stu-id="f6ccb-116">operationStatus</span></span>|<span data-ttu-id="f6ccb-117">|||UNTRANSLATED_CONTENT_START|||The current status of the operation: `notStarted`, `running`, `completed`,|||UNTRANSLATED_CONTENT_END||| `failed`</span><span class="sxs-lookup"><span data-stu-id="f6ccb-117">The current status of the operation: `notStarted`, `running`, `completed`, `failed`</span></span> |

<!-- uuid: 13fa92b1-3b41-498b-aab1-f943464a124f
2018-03-30 10:29:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "operation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

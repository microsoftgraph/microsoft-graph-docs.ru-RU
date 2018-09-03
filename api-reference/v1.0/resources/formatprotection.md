# <a name="formatprotection-resource-type"></a><span data-ttu-id="848e3-101">Тип ресурса FormatProtection</span><span class="sxs-lookup"><span data-stu-id="848e3-101">FormatProtection resource type</span></span>

<span data-ttu-id="848e3-102">Представляет защиту формата объекта Range.</span><span class="sxs-lookup"><span data-stu-id="848e3-102">Represents the format protection of a range object.</span></span>


## <a name="methods"></a><span data-ttu-id="848e3-103">Методы</span><span class="sxs-lookup"><span data-stu-id="848e3-103">Methods</span></span>

| <span data-ttu-id="848e3-104">Метод</span><span class="sxs-lookup"><span data-stu-id="848e3-104">Method</span></span>           | <span data-ttu-id="848e3-105">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="848e3-105">Return Type</span></span>    |<span data-ttu-id="848e3-106">Описание</span><span class="sxs-lookup"><span data-stu-id="848e3-106">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="848e3-107">Получение объекта FormatProtection</span><span class="sxs-lookup"><span data-stu-id="848e3-107">Get FormatProtection</span></span>](../api/formatprotection_get.md) | [<span data-ttu-id="848e3-108">FormatProtection</span><span class="sxs-lookup"><span data-stu-id="848e3-108">FormatProtection</span></span>](formatprotection.md) |<span data-ttu-id="848e3-109">Чтение свойств и связей объекта formatProtection.</span><span class="sxs-lookup"><span data-stu-id="848e3-109">Read properties and relationships of formatProtection object.</span></span>|
|[<span data-ttu-id="848e3-110">Обновление</span><span class="sxs-lookup"><span data-stu-id="848e3-110">Update</span></span>](../api/formatprotection_update.md) | [<span data-ttu-id="848e3-111">FormatProtection</span><span class="sxs-lookup"><span data-stu-id="848e3-111">FormatProtection</span></span>](formatprotection.md)  |<span data-ttu-id="848e3-112">Обновление объекта FormatProtection.</span><span class="sxs-lookup"><span data-stu-id="848e3-112">Update FormatProtection object.</span></span> |

## <a name="properties"></a><span data-ttu-id="848e3-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="848e3-113">Properties</span></span>
| <span data-ttu-id="848e3-114">Свойство</span><span class="sxs-lookup"><span data-stu-id="848e3-114">Property</span></span>     | <span data-ttu-id="848e3-115">Тип</span><span class="sxs-lookup"><span data-stu-id="848e3-115">Type</span></span>   |<span data-ttu-id="848e3-116">Описание</span><span class="sxs-lookup"><span data-stu-id="848e3-116">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="848e3-117">formulaHidden</span><span class="sxs-lookup"><span data-stu-id="848e3-117">formulaHidden</span></span>|<span data-ttu-id="848e3-118">логический</span><span class="sxs-lookup"><span data-stu-id="848e3-118">boolean</span></span>|<span data-ttu-id="848e3-p101">Указывает, скрывает ли Excel формулу для ячеек в диапазоне. Значение NULL указывает, что для всего диапазона не задан единый параметр скрытия формулы.</span><span class="sxs-lookup"><span data-stu-id="848e3-p101">Indicates if Excel hides the formula for the cells in the range. A null value indicates that the entire range doesn't have uniform formula hidden setting.</span></span>|
|<span data-ttu-id="848e3-121">locked</span><span class="sxs-lookup"><span data-stu-id="848e3-121">locked</span></span>|<span data-ttu-id="848e3-122">логический</span><span class="sxs-lookup"><span data-stu-id="848e3-122">boolean</span></span>|<span data-ttu-id="848e3-p102">Указывает, блокирует ли Excel ячейки в объекте. Значение NULL указывает, что для всего диапазона не задан единый параметр блокировки.</span><span class="sxs-lookup"><span data-stu-id="848e3-p102">Indicates if Excel locks the cells in the object. A null value indicates that the entire range doesn't have uniform lock setting.</span></span>|

## <a name="relationships"></a><span data-ttu-id="848e3-125">Связи</span><span class="sxs-lookup"><span data-stu-id="848e3-125">Relationships</span></span>
<span data-ttu-id="848e3-126">Нет</span><span class="sxs-lookup"><span data-stu-id="848e3-126">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="848e3-127">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="848e3-127">JSON representation</span></span>

<span data-ttu-id="848e3-128">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="848e3-128">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookFormatProtection"
}-->

```json
{
  "formulaHidden": true,
  "locked": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "FormatProtection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
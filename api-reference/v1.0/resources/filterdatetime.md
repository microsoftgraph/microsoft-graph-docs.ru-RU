# <a name="filterdatetime-resource-type"></a><span data-ttu-id="b7e2c-101">Тип ресурса FilterDatetime</span><span class="sxs-lookup"><span data-stu-id="b7e2c-101">FilterDatetime resource type</span></span>

<span data-ttu-id="b7e2c-102">Представляет способ фильтрации даты при фильтрации по значениям.</span><span class="sxs-lookup"><span data-stu-id="b7e2c-102">Represents how to filter a date when filtering on values.</span></span>

## <a name="properties"></a><span data-ttu-id="b7e2c-103">Свойства</span><span class="sxs-lookup"><span data-stu-id="b7e2c-103">Properties</span></span>
| <span data-ttu-id="b7e2c-104">Свойство</span><span class="sxs-lookup"><span data-stu-id="b7e2c-104">Property</span></span>     | <span data-ttu-id="b7e2c-105">Тип</span><span class="sxs-lookup"><span data-stu-id="b7e2c-105">Type</span></span>   |<span data-ttu-id="b7e2c-106">Описание</span><span class="sxs-lookup"><span data-stu-id="b7e2c-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b7e2c-107">дата</span><span class="sxs-lookup"><span data-stu-id="b7e2c-107">date</span></span>|<span data-ttu-id="b7e2c-108">string (строка)</span><span class="sxs-lookup"><span data-stu-id="b7e2c-108">string</span></span>|<span data-ttu-id="b7e2c-109">Дата в формате ISO8601, используемая для фильтрации данных.</span><span class="sxs-lookup"><span data-stu-id="b7e2c-109">The date in ISO8601 format used to filter data.</span></span>|
|<span data-ttu-id="b7e2c-110">specificity</span><span class="sxs-lookup"><span data-stu-id="b7e2c-110">specificity</span></span>|<span data-ttu-id="b7e2c-111">string (строка)</span><span class="sxs-lookup"><span data-stu-id="b7e2c-111">string</span></span>|<span data-ttu-id="b7e2c-112">Точность, с которой производится фильтрация данных на основе даты.</span><span class="sxs-lookup"><span data-stu-id="b7e2c-112">How specific the date should be used to keep data.</span></span> <span data-ttu-id="b7e2c-113">Например, если указана дата 02.04.2005 а для свойства specificity задано значение month, после фильтрации останутся все строки, датированные апрелем 2009 г.</span><span class="sxs-lookup"><span data-stu-id="b7e2c-113">How specific the date should be used to keep data. For example, if the date is 2005-04-02 and the specifity is set to "month", the filter operation will keep all rows with a date in the month of april 2009. Possible values are: , , , , , .</span></span> <span data-ttu-id="b7e2c-114">Возможные значения: `Year`, `Monday`, `Day`, `Hour`, `Minute`, `Second`.</span><span class="sxs-lookup"><span data-stu-id="b7e2c-114">The possible values are `Year`, `Monday`, `Day`, `Hour`, `Minute`, `Second`, , , , , , or .</span></span>|

## <a name="relationships"></a><span data-ttu-id="b7e2c-115">Связи</span><span class="sxs-lookup"><span data-stu-id="b7e2c-115">Relationships</span></span>
<span data-ttu-id="b7e2c-116">Нет</span><span class="sxs-lookup"><span data-stu-id="b7e2c-116">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="b7e2c-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b7e2c-117">JSON representation</span></span>

<span data-ttu-id="b7e2c-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b7e2c-118">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookFilterDateTime"
}-->

```json
{
  "date": "string",
  "specificity": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "FilterDatetime resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
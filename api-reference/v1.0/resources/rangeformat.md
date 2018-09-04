# <a name="rangeformat-resource-type"></a><span data-ttu-id="80cf6-101">Тип ресурса RangeFormat</span><span class="sxs-lookup"><span data-stu-id="80cf6-101">RangeFormat resource type</span></span>

<span data-ttu-id="80cf6-102">Объект формата, в который включены шрифт, заливка, границы, выравнивание и другие свойства диапазона.</span><span class="sxs-lookup"><span data-stu-id="80cf6-102">A format object encapsulating the range's font, fill, borders, alignment, and other properties.</span></span>


## <a name="methods"></a><span data-ttu-id="80cf6-103">Методы</span><span class="sxs-lookup"><span data-stu-id="80cf6-103">Methods</span></span>

| <span data-ttu-id="80cf6-104">Метод</span><span class="sxs-lookup"><span data-stu-id="80cf6-104">Method</span></span>           | <span data-ttu-id="80cf6-105">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="80cf6-105">Return Type</span></span>    |<span data-ttu-id="80cf6-106">Описание</span><span class="sxs-lookup"><span data-stu-id="80cf6-106">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="80cf6-107">Получение объекта RangeFormat</span><span class="sxs-lookup"><span data-stu-id="80cf6-107">Get RangeFormat</span></span>](../api/rangeformat_get.md) | [<span data-ttu-id="80cf6-108">WorkbookRangeFormat</span><span class="sxs-lookup"><span data-stu-id="80cf6-108">WorkbookRangeFormat</span></span>](rangeformat.md) |<span data-ttu-id="80cf6-109">Чтение свойств и связей объекта rangeFormat.</span><span class="sxs-lookup"><span data-stu-id="80cf6-109">Read properties and relationships of rangeFormat object.</span></span>|
|[<span data-ttu-id="80cf6-110">Создание объекта RangeBorder</span><span class="sxs-lookup"><span data-stu-id="80cf6-110">Create RangeBorder</span></span>](../api/rangeformat_post_borders.md) |[<span data-ttu-id="80cf6-111">WorkbookRangeBorder</span><span class="sxs-lookup"><span data-stu-id="80cf6-111">WorkbookRangeBorder</span></span>](rangeborder.md)| <span data-ttu-id="80cf6-112">Создание объекта RangeBorder путем добавления в коллекцию границ.</span><span class="sxs-lookup"><span data-stu-id="80cf6-112">Create a new RangeBorder by posting to the borders collection.</span></span>|
|[<span data-ttu-id="80cf6-113">Список границ</span><span class="sxs-lookup"><span data-stu-id="80cf6-113">List borders</span></span>](../api/rangeformat_list_borders.md) |<span data-ttu-id="80cf6-114">Коллекция [WorkbookRangeBorder](rangeborder.md)</span><span class="sxs-lookup"><span data-stu-id="80cf6-114">[WorkbookRangeBorder](rangeborder.md) collection</span></span>| <span data-ttu-id="80cf6-115">Получение коллекции объектов RangeBorder.</span><span class="sxs-lookup"><span data-stu-id="80cf6-115">Get a RangeBorder object collection.</span></span>|
|[<span data-ttu-id="80cf6-116">Обновление</span><span class="sxs-lookup"><span data-stu-id="80cf6-116">Update</span></span>](../api/rangeformat_update.md) | [<span data-ttu-id="80cf6-117">WorkbookRangeFormat</span><span class="sxs-lookup"><span data-stu-id="80cf6-117">WorkbookRangeFormat</span></span>](rangeformat.md) |<span data-ttu-id="80cf6-118">Обновление объекта RangeFormat.</span><span class="sxs-lookup"><span data-stu-id="80cf6-118">Update RangeFormat object.</span></span> |
|[<span data-ttu-id="80cf6-119">Autofitcolumns</span><span class="sxs-lookup"><span data-stu-id="80cf6-119">Autofitcolumns</span></span>](../api/rangeformat_autofitcolumns.md)|<span data-ttu-id="80cf6-120">Нет</span><span class="sxs-lookup"><span data-stu-id="80cf6-120">None</span></span>|<span data-ttu-id="80cf6-121">Изменяет ширину столбцов текущего диапазона на оптимальную с учетом текущих данных в столбцах.</span><span class="sxs-lookup"><span data-stu-id="80cf6-121">Changes the width of the columns of the current range to achieve the best fit, based on the current data in the columns.</span></span>|
|[<span data-ttu-id="80cf6-122">Autofitrows</span><span class="sxs-lookup"><span data-stu-id="80cf6-122">Autofitrows</span></span>](../api/rangeformat_autofitrows.md)|<span data-ttu-id="80cf6-123">Нет</span><span class="sxs-lookup"><span data-stu-id="80cf6-123">None</span></span>|<span data-ttu-id="80cf6-124">Изменяет высоту строк текущего диапазона на оптимальную с учетом текущих данных в столбцах.</span><span class="sxs-lookup"><span data-stu-id="80cf6-124">Changes the height of the rows of the current range to achieve the best fit, based on the current data in the columns.</span></span>|

## <a name="properties"></a><span data-ttu-id="80cf6-125">Свойства</span><span class="sxs-lookup"><span data-stu-id="80cf6-125">Properties</span></span>
| <span data-ttu-id="80cf6-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="80cf6-126">Property</span></span>     | <span data-ttu-id="80cf6-127">Тип</span><span class="sxs-lookup"><span data-stu-id="80cf6-127">Type</span></span>   |<span data-ttu-id="80cf6-128">Описание</span><span class="sxs-lookup"><span data-stu-id="80cf6-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="80cf6-129">columnWidth</span><span class="sxs-lookup"><span data-stu-id="80cf6-129">columnWidth</span></span>|<span data-ttu-id="80cf6-130">double</span><span class="sxs-lookup"><span data-stu-id="80cf6-130">double</span></span>|<span data-ttu-id="80cf6-p101">Возвращает или задает ширину всех столбцов в пределах диапазона. Если столбцы разной ширины, будет возвращено значение NULL.</span><span class="sxs-lookup"><span data-stu-id="80cf6-p101">Gets or sets the width of all colums within the range. If the column widths are not uniform, null will be returned.</span></span>|
|<span data-ttu-id="80cf6-133">horizontalAlignment</span><span class="sxs-lookup"><span data-stu-id="80cf6-133">horizontalAlignment</span></span>|<span data-ttu-id="80cf6-134">строка</span><span class="sxs-lookup"><span data-stu-id="80cf6-134">string</span></span>|<span data-ttu-id="80cf6-135">Представляет горизонтальное выравнивание для указанного объекта.</span><span class="sxs-lookup"><span data-stu-id="80cf6-135">Represents the horizontal alignment for the specified object. Possible values are: , , , , , , , .</span></span> <span data-ttu-id="80cf6-136">Возможные значения: `General`, `Left`, `Center`, `Right`, `Fill`, `Justify`, `CenterAcrossSelection`, `Distributed`.</span><span class="sxs-lookup"><span data-stu-id="80cf6-136">The possible values are `General`, `Left`, `Center`, `Right`, `Fill`, `Justify`, `CenterAcrossSelection`, `Distributed`, , , , or .</span></span>|
|<span data-ttu-id="80cf6-137">rowHeight</span><span class="sxs-lookup"><span data-stu-id="80cf6-137">rowHeight</span></span>|<span data-ttu-id="80cf6-138">double</span><span class="sxs-lookup"><span data-stu-id="80cf6-138">double</span></span>|<span data-ttu-id="80cf6-p103">Возвращает или задает высоту всех строк в диапазоне. Если строки разной высоты, будет возвращено значение NULL.</span><span class="sxs-lookup"><span data-stu-id="80cf6-p103">Gets or sets the height of all rows in the range. If the row heights are not uniform null will be returned.</span></span>|
|<span data-ttu-id="80cf6-141">verticalAlignment</span><span class="sxs-lookup"><span data-stu-id="80cf6-141">verticalAlignment</span></span>|<span data-ttu-id="80cf6-142">строка</span><span class="sxs-lookup"><span data-stu-id="80cf6-142">string</span></span>|<span data-ttu-id="80cf6-143">Представляет вертикальное выравнивание для указанного объекта.</span><span class="sxs-lookup"><span data-stu-id="80cf6-143">Represents the vertical alignment for the specified object. Possible values are: , , , , .</span></span> <span data-ttu-id="80cf6-144">Возможные значения: `Top`, `Center`, `Bottom`, `Justify`, `Distributed`.</span><span class="sxs-lookup"><span data-stu-id="80cf6-144">The possible values are `Top`, `Center`, `Bottom`, `Justify`, `Distributed`, , , , , , , or .</span></span>|
|<span data-ttu-id="80cf6-145">wrapText</span><span class="sxs-lookup"><span data-stu-id="80cf6-145">wrapText</span></span>|<span data-ttu-id="80cf6-146">логический</span><span class="sxs-lookup"><span data-stu-id="80cf6-146">boolean</span></span>|<span data-ttu-id="80cf6-p105">Указывает, использует ли Excel обтекание текстом для объекта. Значение null указывает, что для диапазона в целом не применяется согласованный параметр обтекания.</span><span class="sxs-lookup"><span data-stu-id="80cf6-p105">Indicates if Excel wraps the text in the object. A null value indicates that the entire range doesn't have uniform wrap setting</span></span>|

## <a name="relationships"></a><span data-ttu-id="80cf6-149">Связи</span><span class="sxs-lookup"><span data-stu-id="80cf6-149">Relationships</span></span>
| <span data-ttu-id="80cf6-150">Связь</span><span class="sxs-lookup"><span data-stu-id="80cf6-150">Relationship</span></span> | <span data-ttu-id="80cf6-151">Тип</span><span class="sxs-lookup"><span data-stu-id="80cf6-151">Type</span></span>   |<span data-ttu-id="80cf6-152">Описание</span><span class="sxs-lookup"><span data-stu-id="80cf6-152">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="80cf6-153">borders</span><span class="sxs-lookup"><span data-stu-id="80cf6-153">borders</span></span>|<span data-ttu-id="80cf6-154">Коллекция [WorkbookRangeBorder](rangeborder.md)</span><span class="sxs-lookup"><span data-stu-id="80cf6-154">[WorkbookRangeBorder](rangeborder.md) collection</span></span>|<span data-ttu-id="80cf6-155">Коллекция объектов границ, которые применяются к общему выделенному диапазону. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="80cf6-155">Collection of border objects that apply to the overall range selected Read-only.</span></span>|
|<span data-ttu-id="80cf6-156">fill</span><span class="sxs-lookup"><span data-stu-id="80cf6-156">fill</span></span>|[<span data-ttu-id="80cf6-157">WorkbookRangeFill</span><span class="sxs-lookup"><span data-stu-id="80cf6-157">WorkbookRangeFill</span></span>](rangefill.md)|<span data-ttu-id="80cf6-p106">Возвращает объект заливки, определенный для всего диапазона. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="80cf6-p106">Returns the fill object defined on the overall range. Read-only.</span></span>|
|<span data-ttu-id="80cf6-160">font</span><span class="sxs-lookup"><span data-stu-id="80cf6-160">font</span></span>|[<span data-ttu-id="80cf6-161">WorkbookRangeFont</span><span class="sxs-lookup"><span data-stu-id="80cf6-161">WorkbookRangeFont</span></span>](rangefont.md)|<span data-ttu-id="80cf6-162">Возвращает объект шрифта, определенный для общего выбранного диапазона. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="80cf6-162">Returns the font object defined on the overall range selected Read-only.</span></span>|
|<span data-ttu-id="80cf6-163">protection</span><span class="sxs-lookup"><span data-stu-id="80cf6-163">protection</span></span>|[<span data-ttu-id="80cf6-164">WorkbookFormatProtection</span><span class="sxs-lookup"><span data-stu-id="80cf6-164">WorkbookFormatProtection</span></span>](formatprotection.md)|<span data-ttu-id="80cf6-p107">Возвращает объект защиты формата для диапазона. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="80cf6-p107">Returns the format protection object for a range. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="80cf6-167">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="80cf6-167">JSON representation</span></span>

<span data-ttu-id="80cf6-168">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="80cf6-168">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookRangeFormat"
}-->

```json
{
  "columnWidth": 1024,
  "horizontalAlignment": "string",
  "rowHeight": 1024,
  "verticalAlignment": "string",
  "wrapText": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "RangeFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
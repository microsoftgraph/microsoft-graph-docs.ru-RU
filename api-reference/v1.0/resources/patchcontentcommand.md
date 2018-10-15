# <a name="patchcontentcommand-resource-type"></a><span data-ttu-id="1a741-101">Тип ресурса patchContentCommand</span><span class="sxs-lookup"><span data-stu-id="1a741-101">patchContentCommand resource type</span></span>

<span data-ttu-id="1a741-102">Изменения, которые необходимо внести на страницу OneNote в запросе PATCH.</span><span class="sxs-lookup"><span data-stu-id="1a741-102">The changes to make to a OneNote page in a PATCH request.</span></span>

## <a name="json-representation"></a><span data-ttu-id="1a741-103">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1a741-103">JSON representation</span></span>

<span data-ttu-id="1a741-104">Ниже показано представление ресурса в формате JSON, которое отправляется в тексте запроса [PATCH pages/{id}\`](../api/page_update.md).</span><span class="sxs-lookup"><span data-stu-id="1a741-104">Here is a JSON representation of the resource, which is sent in the body of the [PATCH pages/{id}\`](../api/page_update.md) request.</span></span> 

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onenotePatchContentCommand"
}-->

```json
{
  "action": "String",
  "content": "string",
  "position": "String",
  "target": "string"
}

```

## <a name="properties"></a><span data-ttu-id="1a741-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="1a741-105">Properties</span></span>
| <span data-ttu-id="1a741-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="1a741-106">Property</span></span>     | <span data-ttu-id="1a741-107">Тип</span><span class="sxs-lookup"><span data-stu-id="1a741-107">Type</span></span>   |<span data-ttu-id="1a741-108">Описание</span><span class="sxs-lookup"><span data-stu-id="1a741-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1a741-109">action</span><span class="sxs-lookup"><span data-stu-id="1a741-109">action</span></span>|<span data-ttu-id="1a741-110">onenotePatchActionType</span><span class="sxs-lookup"><span data-stu-id="1a741-110">onenotePatchActionType values</span></span>|<span data-ttu-id="1a741-111">Действие, которое требуется выполнить с целевым элементом.</span><span class="sxs-lookup"><span data-stu-id="1a741-111">The action to perform on the target element.</span></span> <span data-ttu-id="1a741-112">Допустимые значения: `replace`, `append`, `delete`, `insert` или `prepend`.</span><span class="sxs-lookup"><span data-stu-id="1a741-112">The possible values are `replace`, `append`, `delete`, `insert`, , , , , , , , or `prepend`.</span></span>|
|<span data-ttu-id="1a741-113">content</span><span class="sxs-lookup"><span data-stu-id="1a741-113">content</span></span>|<span data-ttu-id="1a741-114">String (строка)</span><span class="sxs-lookup"><span data-stu-id="1a741-114">String</span></span>|<span data-ttu-id="1a741-p102">Строка правильно оформленного HTML-кода, который необходимо добавить на страницу, а также двоичные данные любого изображения или файла. Если контент содержит двоичные данные, необходимо отправить запрос с использованием типа контента `multipart/form-data` с частью Commands.</span><span class="sxs-lookup"><span data-stu-id="1a741-p102">A string of well-formed HTML to add to the page, and any image or file binary data. If the content contains binary data, the request must be sent using the `multipart/form-data` content type with a "Commands" part.</span></span> |
|<span data-ttu-id="1a741-117">position</span><span class="sxs-lookup"><span data-stu-id="1a741-117">position</span></span>|<span data-ttu-id="1a741-118">onenotePatchInsertPosition</span><span class="sxs-lookup"><span data-stu-id="1a741-118">onenotePatchInsertPosition values</span></span>|<span data-ttu-id="1a741-119">Расположение относительно целевого элемента, куда нужно добавить указанное содержимое.</span><span class="sxs-lookup"><span data-stu-id="1a741-119">The location to add the supplied content, relative to the target element.</span></span> <span data-ttu-id="1a741-120">Возможные значения: `after` (по умолчанию) или `before`.</span><span class="sxs-lookup"><span data-stu-id="1a741-120">The possible values are , , , , , , , , , , , or .</span></span>|
|<span data-ttu-id="1a741-121">target</span><span class="sxs-lookup"><span data-stu-id="1a741-121">target</span></span>|<span data-ttu-id="1a741-122">String (строка)</span><span class="sxs-lookup"><span data-stu-id="1a741-122">String</span></span>|<span data-ttu-id="1a741-p104">Элемент для обновления. Значение этого свойства должно представлять собой `#<data-id>`, созданный идентификатор `<id>` элемента либо ключевое слово `body` или `title`.</span><span class="sxs-lookup"><span data-stu-id="1a741-p104">The element to update. Must be the `#<data-id>` or the generated `<id>` of the element, or the `body` or `title` keyword.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "patchContentCommand resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

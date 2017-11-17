# <a name="page-resource-type"></a><span data-ttu-id="b67de-101">Тип ресурса page</span><span class="sxs-lookup"><span data-stu-id="b67de-101">page resource type</span></span>

<span data-ttu-id="b67de-102">Страница в записной книжке OneNote.</span><span class="sxs-lookup"><span data-stu-id="b67de-102">A page in a OneNote notebook.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b67de-103">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="b67de-103">JSON representation</span></span>

<span data-ttu-id="b67de-104">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b67de-104">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "parentNotebook",
    "parentSection"
  ],
  "@odata.type": "microsoft.graph.onenotePage"
}-->

```json
{
  "content": "stream",
  "contentUrl": "string",
  "createdByAppId": "string",
  "createdDateTime": "String (timestamp)",
  "id": "string (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "level": 1024,
  "links": {"@odata.type": "microsoft.graph.pageLinks"},
  "order": 1024,
  "self": "string",
  "title": "string"
}

```
## <a name="properties"></a><span data-ttu-id="b67de-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="b67de-105">Properties</span></span>
| <span data-ttu-id="b67de-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="b67de-106">Property</span></span>     | <span data-ttu-id="b67de-107">Тип</span><span class="sxs-lookup"><span data-stu-id="b67de-107">Type</span></span>   |<span data-ttu-id="b67de-108">Описание</span><span class="sxs-lookup"><span data-stu-id="b67de-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b67de-109">content</span><span class="sxs-lookup"><span data-stu-id="b67de-109">content</span></span>|<span data-ttu-id="b67de-110">Поток</span><span class="sxs-lookup"><span data-stu-id="b67de-110">Stream</span></span>|<span data-ttu-id="b67de-111">HTML-содержимое страницы.</span><span class="sxs-lookup"><span data-stu-id="b67de-111">The page's HTML content.</span></span>|
|<span data-ttu-id="b67de-112">contentUrl</span><span class="sxs-lookup"><span data-stu-id="b67de-112">contentUrl</span></span>|<span data-ttu-id="b67de-113">String</span><span class="sxs-lookup"><span data-stu-id="b67de-113">String</span></span>|<span data-ttu-id="b67de-p101">URL-адрес HTML-содержимого страницы.  Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b67de-p101">The URL for the page's HTML content.  Read-only.</span></span>|
|<span data-ttu-id="b67de-116">createdByAppId</span><span class="sxs-lookup"><span data-stu-id="b67de-116">createdByAppId</span></span>|<span data-ttu-id="b67de-117">String</span><span class="sxs-lookup"><span data-stu-id="b67de-117">String</span></span>|<span data-ttu-id="b67de-p102">Уникальный идентификатор приложения, которое создало страницу. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b67de-p102">The unique identifier of the application that created the page. Read-only.</span></span>|
|<span data-ttu-id="b67de-120">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b67de-120">createdDateTime</span></span>|<span data-ttu-id="b67de-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b67de-121">DateTimeOffset</span></span>|<span data-ttu-id="b67de-p103">Дата и время создания страницы. Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b67de-p103">The date and time when the page was created. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|
|<span data-ttu-id="b67de-126">id</span><span class="sxs-lookup"><span data-stu-id="b67de-126">id</span></span>|<span data-ttu-id="b67de-127">String</span><span class="sxs-lookup"><span data-stu-id="b67de-127">String</span></span>|<span data-ttu-id="b67de-p104">Уникальный идентификатор страницы.  Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b67de-p104">The unique identifier of the page.  Read-only.</span></span>|
|<span data-ttu-id="b67de-130">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b67de-130">lastModifiedDateTime</span></span>|<span data-ttu-id="b67de-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b67de-131">DateTimeOffset</span></span>|<span data-ttu-id="b67de-p105">Дата и время последнего изменения страницы. Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b67de-p105">The date and time when the page was last modified. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|
|<span data-ttu-id="b67de-136">level</span><span class="sxs-lookup"><span data-stu-id="b67de-136">level</span></span>|<span data-ttu-id="b67de-137">Int32</span><span class="sxs-lookup"><span data-stu-id="b67de-137">Int32</span></span>|<span data-ttu-id="b67de-p106">Уровень отступа для страницы. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b67de-p106">The indentation level of the page. Read-only.</span></span>|
|<span data-ttu-id="b67de-140">links</span><span class="sxs-lookup"><span data-stu-id="b67de-140">links</span></span>|[<span data-ttu-id="b67de-141">PageLinks</span><span class="sxs-lookup"><span data-stu-id="b67de-141">PageLinks</span></span>](pagelinks.md)|<span data-ttu-id="b67de-p107">Ссылки для открытия страницы. Ссылка `oneNoteClientURL` открывает страницу в клиенте OneNote, если он установлен. Ссылка `oneNoteWebUrl` открывает страницу в OneNote Online. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b67de-p107">Links for opening the page. The `oneNoteClientURL` link opens the page in the OneNote native client if it 's installed. The `oneNoteWebUrl` link opens the page in OneNote Online. Read-only.</span></span>|
|<span data-ttu-id="b67de-146">order</span><span class="sxs-lookup"><span data-stu-id="b67de-146">order</span></span>|<span data-ttu-id="b67de-147">Int32</span><span class="sxs-lookup"><span data-stu-id="b67de-147">Int32</span></span>|<span data-ttu-id="b67de-p108">Расположение страницы в родительском разделе. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b67de-p108">The order of the page within its parent section. Read-only.</span></span>|
|<span data-ttu-id="b67de-150">self</span><span class="sxs-lookup"><span data-stu-id="b67de-150">self</span></span>|<span data-ttu-id="b67de-151">String</span><span class="sxs-lookup"><span data-stu-id="b67de-151">String</span></span>|<span data-ttu-id="b67de-p109">Конечная точка, в которой можно получить сведения о странице. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b67de-p109">The endpoint where you can get details about the page. Read-only.</span></span>|
|<span data-ttu-id="b67de-154">title</span><span class="sxs-lookup"><span data-stu-id="b67de-154">title</span></span>|<span data-ttu-id="b67de-155">Строка</span><span class="sxs-lookup"><span data-stu-id="b67de-155">String</span></span>|<span data-ttu-id="b67de-156">Заголовок страницы.</span><span class="sxs-lookup"><span data-stu-id="b67de-156">The title of the page.</span></span> |

## <a name="relationships"></a><span data-ttu-id="b67de-157">Отношения</span><span class="sxs-lookup"><span data-stu-id="b67de-157">Relationships</span></span>
| <span data-ttu-id="b67de-158">Связь</span><span class="sxs-lookup"><span data-stu-id="b67de-158">Relationship</span></span> | <span data-ttu-id="b67de-159">Тип</span><span class="sxs-lookup"><span data-stu-id="b67de-159">Type</span></span>   |<span data-ttu-id="b67de-160">Описание</span><span class="sxs-lookup"><span data-stu-id="b67de-160">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b67de-161">parentNotebook</span><span class="sxs-lookup"><span data-stu-id="b67de-161">parentNotebook</span></span>|[<span data-ttu-id="b67de-162">Notebook</span><span class="sxs-lookup"><span data-stu-id="b67de-162">Notebook</span></span>](notebook.md)|<span data-ttu-id="b67de-p110">Записная книжка, содержащая страницу.  Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b67de-p110">The notebook that contains the page.  Read-only.</span></span>|
|<span data-ttu-id="b67de-165">parentSection</span><span class="sxs-lookup"><span data-stu-id="b67de-165">parentSection</span></span>|[<span data-ttu-id="b67de-166">Section</span><span class="sxs-lookup"><span data-stu-id="b67de-166">Section</span></span>](section.md)|<span data-ttu-id="b67de-p111">Раздел, содержащий страницу. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b67de-p111">The section that contains the page. Read-only.</span></span>|

## <a name="methods"></a><span data-ttu-id="b67de-169">Методы</span><span class="sxs-lookup"><span data-stu-id="b67de-169">Methods</span></span>

| <span data-ttu-id="b67de-170">Метод</span><span class="sxs-lookup"><span data-stu-id="b67de-170">Method</span></span>           | <span data-ttu-id="b67de-171">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="b67de-171">Return Type</span></span>    |<span data-ttu-id="b67de-172">Описание</span><span class="sxs-lookup"><span data-stu-id="b67de-172">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b67de-173">Получение страницы</span><span class="sxs-lookup"><span data-stu-id="b67de-173">Get page</span></span>](../api/page_get.md) | [<span data-ttu-id="b67de-174">Page</span><span class="sxs-lookup"><span data-stu-id="b67de-174">Page</span></span>](page.md) |<span data-ttu-id="b67de-175">Чтение свойств и отношений страницы.</span><span class="sxs-lookup"><span data-stu-id="b67de-175">Read the properties and relationships of the page.</span></span>|
|[<span data-ttu-id="b67de-176">Обновление содержимого страницы</span><span class="sxs-lookup"><span data-stu-id="b67de-176">Update page content</span></span>](../api/page_update.md) | <span data-ttu-id="b67de-177">Нет</span><span class="sxs-lookup"><span data-stu-id="b67de-177">None</span></span> |<span data-ttu-id="b67de-178">Обновление HTML-содержимого страницы.</span><span class="sxs-lookup"><span data-stu-id="b67de-178">Update the HTML content of the page.</span></span> |
|[<span data-ttu-id="b67de-179">Удаление страницы</span><span class="sxs-lookup"><span data-stu-id="b67de-179">Delete page</span></span>](../api/page_delete.md) | <span data-ttu-id="b67de-180">Нет</span><span class="sxs-lookup"><span data-stu-id="b67de-180">None</span></span> |<span data-ttu-id="b67de-181">Удаление страницы.</span><span class="sxs-lookup"><span data-stu-id="b67de-181">Delete the page.</span></span> |
|[<span data-ttu-id="b67de-182">copyToSection</span><span class="sxs-lookup"><span data-stu-id="b67de-182">copyToSection</span></span>](../api/page_copytosection.md)| <span data-ttu-id="b67de-183">Нет</span><span class="sxs-lookup"><span data-stu-id="b67de-183">None</span></span> |<span data-ttu-id="b67de-184">Копирование страницы в определенный раздел.</span><span class="sxs-lookup"><span data-stu-id="b67de-184">Copies the page to a specific section.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "page resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
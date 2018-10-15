# <a name="page-resource-type"></a><span data-ttu-id="4fd4a-101">Тип ресурса page</span><span class="sxs-lookup"><span data-stu-id="4fd4a-101">page resource type</span></span>

<span data-ttu-id="4fd4a-102">Страница в записной книжке OneNote.</span><span class="sxs-lookup"><span data-stu-id="4fd4a-102">A page in a OneNote notebook.</span></span>

## <a name="json-representation"></a><span data-ttu-id="4fd4a-103">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="4fd4a-103">JSON representation</span></span>

<span data-ttu-id="4fd4a-104">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4fd4a-104">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.onenoteEntitySchemaObjectModel",
  "optionalProperties": [
    "parentNotebook",
    "parentSection"
  ],
  "isMediaEntity": true,
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
## <a name="properties"></a><span data-ttu-id="4fd4a-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="4fd4a-105">Properties</span></span>
| <span data-ttu-id="4fd4a-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="4fd4a-106">Property</span></span>     | <span data-ttu-id="4fd4a-107">Тип</span><span class="sxs-lookup"><span data-stu-id="4fd4a-107">Type</span></span>   |<span data-ttu-id="4fd4a-108">Описание</span><span class="sxs-lookup"><span data-stu-id="4fd4a-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4fd4a-109">content</span><span class="sxs-lookup"><span data-stu-id="4fd4a-109">content</span></span>|<span data-ttu-id="4fd4a-110">Поток</span><span class="sxs-lookup"><span data-stu-id="4fd4a-110">Stream</span></span>|<span data-ttu-id="4fd4a-111">HTML-содержимое страницы.</span><span class="sxs-lookup"><span data-stu-id="4fd4a-111">The page's HTML content.</span></span>|
|<span data-ttu-id="4fd4a-112">contentUrl</span><span class="sxs-lookup"><span data-stu-id="4fd4a-112">contentUrl</span></span>|<span data-ttu-id="4fd4a-113">String (строка)</span><span class="sxs-lookup"><span data-stu-id="4fd4a-113">String</span></span>|<span data-ttu-id="4fd4a-p101">URL-адрес HTML-содержимого страницы.  Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4fd4a-p101">The URL for the page's HTML content.  Read-only.</span></span>|
|<span data-ttu-id="4fd4a-116">createdByAppId</span><span class="sxs-lookup"><span data-stu-id="4fd4a-116">createdByAppId</span></span>|<span data-ttu-id="4fd4a-117">String (строка)</span><span class="sxs-lookup"><span data-stu-id="4fd4a-117">String</span></span>|<span data-ttu-id="4fd4a-p102">Уникальный идентификатор приложения, которое создало страницу. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4fd4a-p102">The unique identifier of the application that created the page. Read-only.</span></span>|
|<span data-ttu-id="4fd4a-120">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4fd4a-120">createdDateTime</span></span>|<span data-ttu-id="4fd4a-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4fd4a-121">DateTimeOffset</span></span>|<span data-ttu-id="4fd4a-p103">Дата и время создания страницы. Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4fd4a-p103">The date and time when the page was created. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|
|<span data-ttu-id="4fd4a-126">id</span><span class="sxs-lookup"><span data-stu-id="4fd4a-126">id</span></span>|<span data-ttu-id="4fd4a-127">String (строка)</span><span class="sxs-lookup"><span data-stu-id="4fd4a-127">String</span></span>|<span data-ttu-id="4fd4a-p104">Уникальный идентификатор страницы.  Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4fd4a-p104">The unique identifier of the page.  Read-only.</span></span>|
|<span data-ttu-id="4fd4a-130">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4fd4a-130">lastModifiedDateTime</span></span>|<span data-ttu-id="4fd4a-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4fd4a-131">DateTimeOffset</span></span>|<span data-ttu-id="4fd4a-p105">Дата и время последнего изменения страницы. Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4fd4a-p105">The date and time when the page was last modified. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|
|<span data-ttu-id="4fd4a-136">level</span><span class="sxs-lookup"><span data-stu-id="4fd4a-136">level</span></span>|<span data-ttu-id="4fd4a-137">Int32</span><span class="sxs-lookup"><span data-stu-id="4fd4a-137">Int32</span></span>|<span data-ttu-id="4fd4a-p106">Уровень отступа для страницы. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4fd4a-p106">The indentation level of the page. Read-only.</span></span>|
|<span data-ttu-id="4fd4a-140">links</span><span class="sxs-lookup"><span data-stu-id="4fd4a-140">links</span></span>|[<span data-ttu-id="4fd4a-141">PageLinks</span><span class="sxs-lookup"><span data-stu-id="4fd4a-141">PageLinks</span></span>](pagelinks.md)|<span data-ttu-id="4fd4a-p107">Ссылки для открытия страницы. Ссылка `oneNoteClientURL` открывает страницу в клиенте OneNote, если он установлен. Ссылка `oneNoteWebUrl` открывает страницу в OneNote Online. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4fd4a-p107">Links for opening the page. The `oneNoteClientURL` link opens the page in the OneNote native client if it 's installed. The `oneNoteWebUrl` link opens the page in OneNote Online. Read-only.</span></span>|
|<span data-ttu-id="4fd4a-146">order</span><span class="sxs-lookup"><span data-stu-id="4fd4a-146">order</span></span>|<span data-ttu-id="4fd4a-147">Int32</span><span class="sxs-lookup"><span data-stu-id="4fd4a-147">Int32</span></span>|<span data-ttu-id="4fd4a-p108">Расположение страницы в родительском разделе. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4fd4a-p108">The order of the page within its parent section. Read-only.</span></span>|
|<span data-ttu-id="4fd4a-150">self</span><span class="sxs-lookup"><span data-stu-id="4fd4a-150">self</span></span>|<span data-ttu-id="4fd4a-151">String (строка)</span><span class="sxs-lookup"><span data-stu-id="4fd4a-151">String</span></span>|<span data-ttu-id="4fd4a-p109">Конечная точка, в которой можно получить сведения о странице. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4fd4a-p109">The endpoint where you can get details about the page. Read-only.</span></span>|
|<span data-ttu-id="4fd4a-154">title</span><span class="sxs-lookup"><span data-stu-id="4fd4a-154">title</span></span>|<span data-ttu-id="4fd4a-155">String (строка)</span><span class="sxs-lookup"><span data-stu-id="4fd4a-155">String</span></span>|<span data-ttu-id="4fd4a-156">Заголовок страницы.</span><span class="sxs-lookup"><span data-stu-id="4fd4a-156">The title of the page.</span></span> |

## <a name="relationships"></a><span data-ttu-id="4fd4a-157">Отношения</span><span class="sxs-lookup"><span data-stu-id="4fd4a-157">Relationships</span></span>
| <span data-ttu-id="4fd4a-158">Связь</span><span class="sxs-lookup"><span data-stu-id="4fd4a-158">Relationship</span></span> | <span data-ttu-id="4fd4a-159">Тип</span><span class="sxs-lookup"><span data-stu-id="4fd4a-159">Type</span></span>   |<span data-ttu-id="4fd4a-160">Описание</span><span class="sxs-lookup"><span data-stu-id="4fd4a-160">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4fd4a-161">parentNotebook</span><span class="sxs-lookup"><span data-stu-id="4fd4a-161">parentNotebook</span></span>|[<span data-ttu-id="4fd4a-162">Notebook</span><span class="sxs-lookup"><span data-stu-id="4fd4a-162">Notebook</span></span>](notebook.md)|<span data-ttu-id="4fd4a-p110">Записная книжка, содержащая страницу.  Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4fd4a-p110">The notebook that contains the page.  Read-only.</span></span>|
|<span data-ttu-id="4fd4a-165">parentSection</span><span class="sxs-lookup"><span data-stu-id="4fd4a-165">parentSection</span></span>|[<span data-ttu-id="4fd4a-166">OnenoteSection</span><span class="sxs-lookup"><span data-stu-id="4fd4a-166">OnenoteSection</span></span>](section.md)|<span data-ttu-id="4fd4a-p111">Раздел, содержащий страницу. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4fd4a-p111">The section that contains the page. Read-only.</span></span>|

## <a name="methods"></a><span data-ttu-id="4fd4a-169">Методы</span><span class="sxs-lookup"><span data-stu-id="4fd4a-169">Methods</span></span>

| <span data-ttu-id="4fd4a-170">Метод</span><span class="sxs-lookup"><span data-stu-id="4fd4a-170">Method</span></span>           | <span data-ttu-id="4fd4a-171">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="4fd4a-171">Return Type</span></span>    |<span data-ttu-id="4fd4a-172">Описание</span><span class="sxs-lookup"><span data-stu-id="4fd4a-172">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="4fd4a-173">Получение страницы</span><span class="sxs-lookup"><span data-stu-id="4fd4a-173">Get page</span></span>](../api/page_get.md) | [<span data-ttu-id="4fd4a-174">Page</span><span class="sxs-lookup"><span data-stu-id="4fd4a-174">Page</span></span>](page.md) |<span data-ttu-id="4fd4a-175">Чтение свойств и отношений страницы.</span><span class="sxs-lookup"><span data-stu-id="4fd4a-175">Read the properties and relationships of the page.</span></span>|
|[<span data-ttu-id="4fd4a-176">Обновление содержимого страницы</span><span class="sxs-lookup"><span data-stu-id="4fd4a-176">Update page content</span></span>](../api/page_update.md) | <span data-ttu-id="4fd4a-177">Нет</span><span class="sxs-lookup"><span data-stu-id="4fd4a-177">None</span></span> |<span data-ttu-id="4fd4a-178">Обновление HTML-содержимого страницы.</span><span class="sxs-lookup"><span data-stu-id="4fd4a-178">Update the HTML content of the page.</span></span> |
|[<span data-ttu-id="4fd4a-179">Удаление страницы</span><span class="sxs-lookup"><span data-stu-id="4fd4a-179">Delete page</span></span>](../api/page_delete.md) | <span data-ttu-id="4fd4a-180">Нет</span><span class="sxs-lookup"><span data-stu-id="4fd4a-180">None</span></span> |<span data-ttu-id="4fd4a-181">Удаление страницы.</span><span class="sxs-lookup"><span data-stu-id="4fd4a-181">Delete the page.</span></span> |
|[<span data-ttu-id="4fd4a-182">copyToSection</span><span class="sxs-lookup"><span data-stu-id="4fd4a-182">copyToSection</span></span>](../api/page_copytosection.md)| <span data-ttu-id="4fd4a-183">Нет</span><span class="sxs-lookup"><span data-stu-id="4fd4a-183">None</span></span> |<span data-ttu-id="4fd4a-184">Копирование страницы в определенный раздел.</span><span class="sxs-lookup"><span data-stu-id="4fd4a-184">Copies the page to a specific section.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "page resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
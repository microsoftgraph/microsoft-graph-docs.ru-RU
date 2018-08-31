# <a name="section-resource-type"></a><span data-ttu-id="12765-101">Тип ресурса section</span><span class="sxs-lookup"><span data-stu-id="12765-101">section resource type</span></span>

<span data-ttu-id="12765-p101">Раздел в записной книжке OneNote. Разделы могут содержать страницы.</span><span class="sxs-lookup"><span data-stu-id="12765-p101">A section in a OneNote notebook. Sections can contain pages.</span></span>

## <a name="json-representation"></a><span data-ttu-id="12765-104">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="12765-104">JSON representation</span></span>

<span data-ttu-id="12765-105">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="12765-105">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.onenoteEntityHierarchyModel",
  "optionalProperties": [
    "pages",
    "parentNotebook",
    "parentSectionGroup"
  ],
  "@odata.type": "microsoft.graph.onenoteSection"
}-->

```json
{
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "createdDateTime": "String (timestamp)",
  "id": "string (identifier)",
  "isDefault": true,
  "lastModifiedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "lastModifiedDateTime": "String (timestamp)",
  "links": {"@odata.type": "microsoft.graph.sectionLinks"},
  "displayName": "string",
  "pagesUrl": "string",
  "self": "string"
}

```
## <a name="properties"></a><span data-ttu-id="12765-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="12765-106">Properties</span></span>
| <span data-ttu-id="12765-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="12765-107">Property</span></span>     | <span data-ttu-id="12765-108">Тип</span><span class="sxs-lookup"><span data-stu-id="12765-108">Type</span></span>   |<span data-ttu-id="12765-109">Описание</span><span class="sxs-lookup"><span data-stu-id="12765-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="12765-110">createdBy</span><span class="sxs-lookup"><span data-stu-id="12765-110">createdBy</span></span>|[<span data-ttu-id="12765-111">identitySet</span><span class="sxs-lookup"><span data-stu-id="12765-111">identitySet</span></span>](identityset.md)|<span data-ttu-id="12765-p102">Идентификатор пользователя, устройства или приложения, создавшего элемент. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="12765-p102">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="12765-114">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="12765-114">createdDateTime</span></span>|<span data-ttu-id="12765-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="12765-115">DateTimeOffset</span></span>|<span data-ttu-id="12765-p103">Дата и время создания раздела. Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="12765-p103">The date and time when the section was created. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|
|<span data-ttu-id="12765-120">id</span><span class="sxs-lookup"><span data-stu-id="12765-120">id</span></span>|<span data-ttu-id="12765-121">String (строка)</span><span class="sxs-lookup"><span data-stu-id="12765-121">String</span></span>|<span data-ttu-id="12765-p104">Уникальный идентификатор раздела.  Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="12765-p104">The unique identifier of the section.  Read-only.</span></span>|
|<span data-ttu-id="12765-124">isDefault</span><span class="sxs-lookup"><span data-stu-id="12765-124">isDefault</span></span>|<span data-ttu-id="12765-125">Boolean (логический)</span><span class="sxs-lookup"><span data-stu-id="12765-125">Boolean</span></span>|<span data-ttu-id="12765-p105">Указывает, является ли этот раздел разделом пользователя по умолчанию. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="12765-p105">Indicates whether this is the user's default section. Read-only.</span></span>|
|<span data-ttu-id="12765-128">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="12765-128">lastModifiedBy</span></span>|[<span data-ttu-id="12765-129">identitySet</span><span class="sxs-lookup"><span data-stu-id="12765-129">identitySet</span></span>](identityset.md)|<span data-ttu-id="12765-p106">Идентификатор пользователя, устройства или приложения, создавшего элемент. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="12765-p106">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="12765-132">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="12765-132">lastModifiedDateTime</span></span>|<span data-ttu-id="12765-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="12765-133">DateTimeOffset</span></span>|<span data-ttu-id="12765-p107">Дата и время последнего изменения раздела. Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="12765-p107">The date and time when the section was last modified. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|
|<span data-ttu-id="12765-138">links</span><span class="sxs-lookup"><span data-stu-id="12765-138">links</span></span>|[<span data-ttu-id="12765-139">SectionLinks</span><span class="sxs-lookup"><span data-stu-id="12765-139">SectionLinks</span></span>](sectionlinks.md)|<span data-ttu-id="12765-p108">Ссылки для открытия раздела. Ссылка `oneNoteClientURL` открывает раздел в клиенте OneNote, если он установлен. Ссылка `oneNoteWebURL` открывает раздел в OneNote Online.</span><span class="sxs-lookup"><span data-stu-id="12765-p108">Links for opening the section. The `oneNoteClientURL` link opens the section in the OneNote native client if it's installed. The `oneNoteWebURL` link opens the section in OneNote Online.</span></span>|
|<span data-ttu-id="12765-143">displayName</span><span class="sxs-lookup"><span data-stu-id="12765-143">displayName</span></span>|<span data-ttu-id="12765-144">String (строка)</span><span class="sxs-lookup"><span data-stu-id="12765-144">String</span></span>|<span data-ttu-id="12765-145">Имя раздела.</span><span class="sxs-lookup"><span data-stu-id="12765-145">The name of the section.</span></span> |
|<span data-ttu-id="12765-146">pagesUrl</span><span class="sxs-lookup"><span data-stu-id="12765-146">pagesUrl</span></span>|<span data-ttu-id="12765-147">String (строка)</span><span class="sxs-lookup"><span data-stu-id="12765-147">String</span></span>|<span data-ttu-id="12765-p109">— конечная точка, в которой можно получить сведения обо всех страницах в разделе. Только для чтения.`pages`</span><span class="sxs-lookup"><span data-stu-id="12765-p109">The `pages` endpoint where you can get details for all the pages in the section. Read-only.</span></span>|
|<span data-ttu-id="12765-150">self</span><span class="sxs-lookup"><span data-stu-id="12765-150">self</span></span>|<span data-ttu-id="12765-151">String (строка)</span><span class="sxs-lookup"><span data-stu-id="12765-151">String</span></span>|<span data-ttu-id="12765-p110">Конечная точка, в которой можно получить сведения о разделе. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="12765-p110">The endpoint where you can get details about the section. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="12765-154">Связи</span><span class="sxs-lookup"><span data-stu-id="12765-154">Relationships</span></span>
| <span data-ttu-id="12765-155">Связь</span><span class="sxs-lookup"><span data-stu-id="12765-155">Relationship</span></span> | <span data-ttu-id="12765-156">Тип</span><span class="sxs-lookup"><span data-stu-id="12765-156">Type</span></span>   |<span data-ttu-id="12765-157">Описание</span><span class="sxs-lookup"><span data-stu-id="12765-157">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="12765-158">pages</span><span class="sxs-lookup"><span data-stu-id="12765-158">pages</span></span>|<span data-ttu-id="12765-159">Коллекция [OnenotePage](page.md)</span><span class="sxs-lookup"><span data-stu-id="12765-159">[OnenotePage](page.md) collection</span></span>|<span data-ttu-id="12765-p111">Коллекция страниц в разделе.  Только для чтения. Допускает значение null.</span><span class="sxs-lookup"><span data-stu-id="12765-p111">The collection of pages in the section.  Read-only. Nullable.</span></span>|
|<span data-ttu-id="12765-163">parentNotebook</span><span class="sxs-lookup"><span data-stu-id="12765-163">parentNotebook</span></span>|[<span data-ttu-id="12765-164">Notebook</span><span class="sxs-lookup"><span data-stu-id="12765-164">Notebook</span></span>](notebook.md)|<span data-ttu-id="12765-p112">Записная книжка, содержащая раздел.  Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="12765-p112">The notebook that contains the section.  Read-only.</span></span>|
|<span data-ttu-id="12765-167">parentSectionGroup</span><span class="sxs-lookup"><span data-stu-id="12765-167">parentSectionGroup</span></span>|[<span data-ttu-id="12765-168">SectionGroup</span><span class="sxs-lookup"><span data-stu-id="12765-168">SectionGroup</span></span>](sectiongroup.md)|<span data-ttu-id="12765-p113">Группа объектов, содержащая раздел.  Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="12765-p113">The section group that contains the section.  Read-only.</span></span>|

## <a name="methods"></a><span data-ttu-id="12765-171">Методы</span><span class="sxs-lookup"><span data-stu-id="12765-171">Methods</span></span>

| <span data-ttu-id="12765-172">Метод</span><span class="sxs-lookup"><span data-stu-id="12765-172">Method</span></span>           | <span data-ttu-id="12765-173">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="12765-173">Return Type</span></span>    |<span data-ttu-id="12765-174">Описание</span><span class="sxs-lookup"><span data-stu-id="12765-174">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="12765-175">Получение раздела</span><span class="sxs-lookup"><span data-stu-id="12765-175">Get section</span></span>](../api/section_get.md) | [<span data-ttu-id="12765-176">OnenoteSection</span><span class="sxs-lookup"><span data-stu-id="12765-176">OnenoteSection</span></span>](section.md) |<span data-ttu-id="12765-177">Чтение свойств и отношений раздела.</span><span class="sxs-lookup"><span data-stu-id="12765-177">Read the properties and relationships of the section.</span></span>|
|[<span data-ttu-id="12765-178">Создание страницы</span><span class="sxs-lookup"><span data-stu-id="12765-178">Create page</span></span>](../api/section_post_pages.md) |[<span data-ttu-id="12765-179">Page</span><span class="sxs-lookup"><span data-stu-id="12765-179">Page</span></span>](page.md)| <span data-ttu-id="12765-180">Создайте страницу, отправив запрос POST в коллекцию pages в указанном разделе.</span><span class="sxs-lookup"><span data-stu-id="12765-180">Create a page by posting to the pages collection in the specified section.</span></span>|
|[<span data-ttu-id="12765-181">Перечисление страниц</span><span class="sxs-lookup"><span data-stu-id="12765-181">List pages</span></span>](../api/section_list_pages.md) |<span data-ttu-id="12765-182">Коллекция объектов [Page](page.md)</span><span class="sxs-lookup"><span data-stu-id="12765-182">[Page](page.md) collection</span></span>| <span data-ttu-id="12765-183">Получение коллекции страниц в указанном разделе.</span><span class="sxs-lookup"><span data-stu-id="12765-183">Get a collection of pages in the specified section.</span></span>|
|[<span data-ttu-id="12765-184">copyToNotebook</span><span class="sxs-lookup"><span data-stu-id="12765-184">copyToNotebook</span></span>](../api/section_copytonotebook.md)|<span data-ttu-id="12765-185">Нет</span><span class="sxs-lookup"><span data-stu-id="12765-185">None</span></span>|<span data-ttu-id="12765-186">Копирование раздела в указанную записную книжку.</span><span class="sxs-lookup"><span data-stu-id="12765-186">Copy the section to a specific notebook.</span></span>|
|[<span data-ttu-id="12765-187">copyToSectionGroup</span><span class="sxs-lookup"><span data-stu-id="12765-187">copyToSectionGroup</span></span>](../api/section_copytosectiongroup.md)|<span data-ttu-id="12765-188">Нет</span><span class="sxs-lookup"><span data-stu-id="12765-188">None</span></span>|<span data-ttu-id="12765-189">Копирование раздела в указанную группу разделов.</span><span class="sxs-lookup"><span data-stu-id="12765-189">Copy the section to a specific section group.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onenoteSection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

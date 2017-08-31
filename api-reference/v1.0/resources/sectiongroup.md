# <a name="sectiongroup-resource-type"></a><span data-ttu-id="bae37-101">Тип ресурса sectionGroup</span><span class="sxs-lookup"><span data-stu-id="bae37-101">sectionGroup resource type</span></span>

<span data-ttu-id="bae37-p101">Группа разделов в записной книжке OneNote. Группы разделов могут содержать разделы и группы разделов.</span><span class="sxs-lookup"><span data-stu-id="bae37-p101">A section group in a OneNote notebook. Section groups can contain sections and section groups.</span></span>

## <a name="json-representation"></a><span data-ttu-id="bae37-104">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bae37-104">JSON representation</span></span>

<span data-ttu-id="bae37-105">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bae37-105">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "parentNotebook",
    "parentSectionGroup",
    "sectionGroups",
    "sections"
  ],
  "@odata.type": "microsoft.graph.sectiongroup"
}-->

```json
{
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "createdDateTime": "String (timestamp)",
  "id": "string (identifier)",
  "lastModifiedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "string",
  "sectionGroupsUrl": "string",
  "sectionsUrl": "string",
  "self": "string"
}

```
## <a name="properties"></a><span data-ttu-id="bae37-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="bae37-106">Properties</span></span>
| <span data-ttu-id="bae37-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="bae37-107">Property</span></span>     | <span data-ttu-id="bae37-108">Тип</span><span class="sxs-lookup"><span data-stu-id="bae37-108">Type</span></span>   |<span data-ttu-id="bae37-109">Описание</span><span class="sxs-lookup"><span data-stu-id="bae37-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bae37-110">createdBy</span><span class="sxs-lookup"><span data-stu-id="bae37-110">createdBy</span></span>|[<span data-ttu-id="bae37-111">identitySet</span><span class="sxs-lookup"><span data-stu-id="bae37-111">identitySet</span></span>](identityset.md)|<span data-ttu-id="bae37-p102">Идентификатор пользователя, устройства или приложения, создавшего элемент. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="bae37-p102">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="bae37-114">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="bae37-114">createdDateTime</span></span>|<span data-ttu-id="bae37-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bae37-115">DateTimeOffset</span></span>|<span data-ttu-id="bae37-p103">Дата и время создания группы разделов. Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="bae37-p103">The date and time when the section group was created. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|
|<span data-ttu-id="bae37-120">id</span><span class="sxs-lookup"><span data-stu-id="bae37-120">id</span></span>|<span data-ttu-id="bae37-121">String</span><span class="sxs-lookup"><span data-stu-id="bae37-121">String</span></span>|<span data-ttu-id="bae37-p104">Уникальный идентификатор группы разделов. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="bae37-p104">The unique identifier of the section group. Read-only.</span></span>|
|<span data-ttu-id="bae37-124">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="bae37-124">lastModifiedBy</span></span>|[<span data-ttu-id="bae37-125">identitySet</span><span class="sxs-lookup"><span data-stu-id="bae37-125">identitySet</span></span>](identityset.md)|<span data-ttu-id="bae37-p105">Идентификатор пользователя, устройства или приложения, создавшего элемент. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="bae37-p105">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="bae37-128">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bae37-128">lastModifiedDateTime</span></span>|<span data-ttu-id="bae37-129">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bae37-129">DateTimeOffset</span></span>|<span data-ttu-id="bae37-p106">Дата и время последнего изменения группы разделов. Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="bae37-p106">The date and time when the section group was last modified. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|
|<span data-ttu-id="bae37-134">displayName</span><span class="sxs-lookup"><span data-stu-id="bae37-134">displayName</span></span>|<span data-ttu-id="bae37-135">Строка</span><span class="sxs-lookup"><span data-stu-id="bae37-135">String</span></span>|<span data-ttu-id="bae37-136">Имя группы разделов.</span><span class="sxs-lookup"><span data-stu-id="bae37-136">The name of the section group.</span></span>|
|<span data-ttu-id="bae37-137">sectionGroupsUrl</span><span class="sxs-lookup"><span data-stu-id="bae37-137">sectionGroupsUrl</span></span>|<span data-ttu-id="bae37-138">Строка</span><span class="sxs-lookup"><span data-stu-id="bae37-138">String</span></span>|<span data-ttu-id="bae37-p107">URL-адрес для свойства навигации `sectionGroups`, который возвращает все группы разделов в группе разделов. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="bae37-p107">The URL for the `sectionGroups` navigation property, which returns all the section groups in the section group. Read-only.</span></span>|
|<span data-ttu-id="bae37-141">sectionsUrl</span><span class="sxs-lookup"><span data-stu-id="bae37-141">sectionsUrl</span></span>|<span data-ttu-id="bae37-142">Строка</span><span class="sxs-lookup"><span data-stu-id="bae37-142">String</span></span>|<span data-ttu-id="bae37-p108">URL-адрес для свойства навигации `sections`, который возвращает все разделы в группе разделов. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="bae37-p108">The URL for the `sections` navigation property, which returns all the sections in the section group. Read-only.</span></span>|
|<span data-ttu-id="bae37-145">self</span><span class="sxs-lookup"><span data-stu-id="bae37-145">self</span></span>|<span data-ttu-id="bae37-146">String</span><span class="sxs-lookup"><span data-stu-id="bae37-146">String</span></span>|<span data-ttu-id="bae37-p109">Конечная точка, в которой можно получить сведения о группе разделов. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="bae37-p109">The endpoint where you can get details about the section group. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bae37-149">Связи</span><span class="sxs-lookup"><span data-stu-id="bae37-149">Relationships</span></span>
| <span data-ttu-id="bae37-150">Связь</span><span class="sxs-lookup"><span data-stu-id="bae37-150">Relationship</span></span> | <span data-ttu-id="bae37-151">Тип</span><span class="sxs-lookup"><span data-stu-id="bae37-151">Type</span></span>   |<span data-ttu-id="bae37-152">Описание</span><span class="sxs-lookup"><span data-stu-id="bae37-152">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bae37-153">parentNotebook</span><span class="sxs-lookup"><span data-stu-id="bae37-153">parentNotebook</span></span>|[<span data-ttu-id="bae37-154">Notebook</span><span class="sxs-lookup"><span data-stu-id="bae37-154">Notebook</span></span>](notebook.md)|<span data-ttu-id="bae37-p110">Записная книжка, содержащая группу разделов. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="bae37-p110">The notebook that contains the section group. Read-only.</span></span>|
|<span data-ttu-id="bae37-157">parentSectionGroup</span><span class="sxs-lookup"><span data-stu-id="bae37-157">parentSectionGroup</span></span>|[<span data-ttu-id="bae37-158">SectionGroup</span><span class="sxs-lookup"><span data-stu-id="bae37-158">SectionGroup</span></span>](sectiongroup.md)|<span data-ttu-id="bae37-p111">Группа разделов, содержащая группу разделов. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="bae37-p111">The section group that contains the section group. Read-only.</span></span>|
|<span data-ttu-id="bae37-161">sectionGroups</span><span class="sxs-lookup"><span data-stu-id="bae37-161">sectionGroups</span></span>|<span data-ttu-id="bae37-162">Коллекция объектов [SectionGroup](sectiongroup.md)</span><span class="sxs-lookup"><span data-stu-id="bae37-162">[SectionGroup](sectiongroup.md) collection</span></span>|<span data-ttu-id="bae37-p112">Группы разделов в разделе. Только для чтения. Допускает значение null.</span><span class="sxs-lookup"><span data-stu-id="bae37-p112">The section groups in the section. Read-only. Nullable.</span></span>|
|<span data-ttu-id="bae37-166">sections</span><span class="sxs-lookup"><span data-stu-id="bae37-166">sections</span></span>|<span data-ttu-id="bae37-167">Коллекция объектов [Section](section.md)</span><span class="sxs-lookup"><span data-stu-id="bae37-167">[Section](section.md) collection</span></span>|<span data-ttu-id="bae37-p113">Разделы в группе разделов. Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="bae37-p113">The sections in the section group. Read-only. Nullable.</span></span>|

## <a name="methods"></a><span data-ttu-id="bae37-171">Методы</span><span class="sxs-lookup"><span data-stu-id="bae37-171">Methods</span></span>

| <span data-ttu-id="bae37-172">Метод</span><span class="sxs-lookup"><span data-stu-id="bae37-172">Method</span></span>           | <span data-ttu-id="bae37-173">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="bae37-173">Return Type</span></span>    |<span data-ttu-id="bae37-174">Описание</span><span class="sxs-lookup"><span data-stu-id="bae37-174">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="bae37-175">Получение группы разделов</span><span class="sxs-lookup"><span data-stu-id="bae37-175">Get section group</span></span>](../api/sectiongroup_get.md) | [<span data-ttu-id="bae37-176">SectionGroup</span><span class="sxs-lookup"><span data-stu-id="bae37-176">SectionGroup</span></span>](sectiongroup.md) |<span data-ttu-id="bae37-177">Чтение свойств и отношений группы разделов.</span><span class="sxs-lookup"><span data-stu-id="bae37-177">Read the properties and relationships of the section group.</span></span>|
|[<span data-ttu-id="bae37-178">Создание группы разделов</span><span class="sxs-lookup"><span data-stu-id="bae37-178">Create section group</span></span>](../api/sectiongroup_post_sectiongroups.md) |[<span data-ttu-id="bae37-179">SectionGroup</span><span class="sxs-lookup"><span data-stu-id="bae37-179">SectionGroup</span></span>](sectiongroup.md)| <span data-ttu-id="bae37-180">Создайте группу разделов, отправив запрос POST в коллекцию sectionGroups в указанной группе разделов.</span><span class="sxs-lookup"><span data-stu-id="bae37-180">Create a section group by posting to the sectionGroups collection in the specified section group.</span></span>|
|[<span data-ttu-id="bae37-181">Перечисление групп разделов</span><span class="sxs-lookup"><span data-stu-id="bae37-181">List section groups</span></span>](../api/sectiongroup_list_sectiongroups.md) |<span data-ttu-id="bae37-182">Коллекция объектов [SectionGroup](sectiongroup.md)</span><span class="sxs-lookup"><span data-stu-id="bae37-182">[SectionGroup](sectiongroup.md) collection</span></span>| <span data-ttu-id="bae37-183">Получение коллекции групп разделов в указанной группе разделов.</span><span class="sxs-lookup"><span data-stu-id="bae37-183">Get collection of section groups in the specified section group.</span></span>|
|[<span data-ttu-id="bae37-184">Создание раздела</span><span class="sxs-lookup"><span data-stu-id="bae37-184">Create section</span></span>](../api/sectiongroup_post_sections.md) |[<span data-ttu-id="bae37-185">Section</span><span class="sxs-lookup"><span data-stu-id="bae37-185">Section</span></span>](section.md)| <span data-ttu-id="bae37-186">Создайте раздел, отправив запрос POST в коллекцию sections в указанной группе разделов.</span><span class="sxs-lookup"><span data-stu-id="bae37-186">Create a section by posting to the sections collection in the specified section group.</span></span>|
|[<span data-ttu-id="bae37-187">Перечисление разделов</span><span class="sxs-lookup"><span data-stu-id="bae37-187">List sections</span></span>](../api/sectiongroup_list_sections.md) |<span data-ttu-id="bae37-188">Коллекция объектов [Section](section.md)</span><span class="sxs-lookup"><span data-stu-id="bae37-188">[Section](section.md) collection</span></span>| <span data-ttu-id="bae37-189">Получение коллекции разделов в указанной группе разделов.</span><span class="sxs-lookup"><span data-stu-id="bae37-189">Get a collection of sections in the specified section group.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "sectionGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

# <a name="calendargroup-resource-type"></a><span data-ttu-id="e1eee-101">Тип ресурса calendarGroup</span><span class="sxs-lookup"><span data-stu-id="e1eee-101">calendarGroup resource type</span></span>

<span data-ttu-id="e1eee-102">Группа календарей.</span><span class="sxs-lookup"><span data-stu-id="e1eee-102">A group of calendars.</span></span>

<span data-ttu-id="e1eee-p101">**Примечание**. Outlook.com поддерживает только группу календарей по умолчанию, доступную по ссылке ../me/calendars. Удалить эту группу календарей невозможно.</span><span class="sxs-lookup"><span data-stu-id="e1eee-p101">**Note** Outlook.com supports only the default calendar group which is accessible by the ../me/calendars shortcut. You cannot delete that calendar group.</span></span>

## <a name="methods"></a><span data-ttu-id="e1eee-105">Методы</span><span class="sxs-lookup"><span data-stu-id="e1eee-105">Methods</span></span>

| <span data-ttu-id="e1eee-106">Метод</span><span class="sxs-lookup"><span data-stu-id="e1eee-106">Method</span></span>       | <span data-ttu-id="e1eee-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="e1eee-107">Return Type</span></span>  |<span data-ttu-id="e1eee-108">Описание</span><span class="sxs-lookup"><span data-stu-id="e1eee-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e1eee-109">Список групп календарей</span><span class="sxs-lookup"><span data-stu-id="e1eee-109">List calendar groups</span></span>](../api/user_list_calendargroups.md) |<span data-ttu-id="e1eee-110">Коллекция объектов [Calendar](calendar.md)</span><span class="sxs-lookup"><span data-stu-id="e1eee-110">[Calendar](calendar.md) collection</span></span>| <span data-ttu-id="e1eee-111">Получение групп календарей пользователя.</span><span class="sxs-lookup"><span data-stu-id="e1eee-111">Get the user's calendar groups.</span></span>|
|[<span data-ttu-id="e1eee-112">Создание группы календарей</span><span class="sxs-lookup"><span data-stu-id="e1eee-112">Create calendar group</span></span>](../api/user_post_calendargroups.md) |[<span data-ttu-id="e1eee-113">Calendar</span><span class="sxs-lookup"><span data-stu-id="e1eee-113">Calendar</span></span>](calendar.md)| <span data-ttu-id="e1eee-114">Создание группы календарей.</span><span class="sxs-lookup"><span data-stu-id="e1eee-114">Create a new calendar group.</span></span>|
|[<span data-ttu-id="e1eee-115">Получение группы календарей</span><span class="sxs-lookup"><span data-stu-id="e1eee-115">Get calendar group</span></span>](../api/calendargroup_get.md) | [<span data-ttu-id="e1eee-116">calendarGroup</span><span class="sxs-lookup"><span data-stu-id="e1eee-116">calendarGroup</span></span>](calendargroup.md) |<span data-ttu-id="e1eee-117">Чтение свойств и связей, принадлежащих объекту группы календарей.</span><span class="sxs-lookup"><span data-stu-id="e1eee-117">Read properties and relationships of a calendar group object.</span></span>|
|[<span data-ttu-id="e1eee-118">Обновление</span><span class="sxs-lookup"><span data-stu-id="e1eee-118">Update</span></span>](../api/calendargroup_update.md) | [<span data-ttu-id="e1eee-119">calendarGroup</span><span class="sxs-lookup"><span data-stu-id="e1eee-119">calendarGroup</span></span>](calendargroup.md) |<span data-ttu-id="e1eee-120">Обновление объекта calendarGroup.</span><span class="sxs-lookup"><span data-stu-id="e1eee-120">Update calendarGroup object.</span></span> |
|[<span data-ttu-id="e1eee-121">Удаление</span><span class="sxs-lookup"><span data-stu-id="e1eee-121">Delete</span></span>](../api/calendargroup_delete.md) | <span data-ttu-id="e1eee-122">Нет</span><span class="sxs-lookup"><span data-stu-id="e1eee-122">None</span></span> |<span data-ttu-id="e1eee-123">Удаление объекта calendarGroup.</span><span class="sxs-lookup"><span data-stu-id="e1eee-123">Delete calendarGroup object.</span></span> |
|[<span data-ttu-id="e1eee-124">Список календарей</span><span class="sxs-lookup"><span data-stu-id="e1eee-124">List calendars</span></span>](../api/calendargroup_list_calendars.md) |<span data-ttu-id="e1eee-125">Коллекция объектов [Calendar](calendar.md)</span><span class="sxs-lookup"><span data-stu-id="e1eee-125">[Calendar](calendar.md) collection</span></span>| <span data-ttu-id="e1eee-126">Список календарей в группе календарей.</span><span class="sxs-lookup"><span data-stu-id="e1eee-126">List calendars in a calendar group.</span></span>|
|[<span data-ttu-id="e1eee-127">Создание объекта Calendar</span><span class="sxs-lookup"><span data-stu-id="e1eee-127">Create Calendar</span></span>](../api/calendargroup_post_calendars.md) |[<span data-ttu-id="e1eee-128">Calendar</span><span class="sxs-lookup"><span data-stu-id="e1eee-128">Calendar</span></span>](calendar.md)| <span data-ttu-id="e1eee-129">Создание календаря в группе календарей.</span><span class="sxs-lookup"><span data-stu-id="e1eee-129">Create a new Calendar in a calendar group.</span></span>|

## <a name="properties"></a><span data-ttu-id="e1eee-130">Свойства</span><span class="sxs-lookup"><span data-stu-id="e1eee-130">Properties</span></span>
| <span data-ttu-id="e1eee-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="e1eee-131">Property</span></span>     | <span data-ttu-id="e1eee-132">Тип</span><span class="sxs-lookup"><span data-stu-id="e1eee-132">Type</span></span>   |<span data-ttu-id="e1eee-133">Описание</span><span class="sxs-lookup"><span data-stu-id="e1eee-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e1eee-134">name</span><span class="sxs-lookup"><span data-stu-id="e1eee-134">name</span></span>|<span data-ttu-id="e1eee-135">String</span><span class="sxs-lookup"><span data-stu-id="e1eee-135">String</span></span>|<span data-ttu-id="e1eee-136">Имя группы.</span><span class="sxs-lookup"><span data-stu-id="e1eee-136">The group name.</span></span>|
|<span data-ttu-id="e1eee-137">changeKey</span><span class="sxs-lookup"><span data-stu-id="e1eee-137">changeKey</span></span>|<span data-ttu-id="e1eee-138">Строка</span><span class="sxs-lookup"><span data-stu-id="e1eee-138">String</span></span>|<span data-ttu-id="e1eee-p102">Указывает версию группы календарей. При каждом изменении группы календарей также меняется значение ChangeKey. Благодаря этому Exchange может применять изменения к правильной версии объекта. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e1eee-p102">Identifies the version of the calendar group. Every time the calendar group is changed, ChangeKey changes as well. This allows Exchange to apply changes to the correct version of the object. Read-only.</span></span>|
|<span data-ttu-id="e1eee-143">classId</span><span class="sxs-lookup"><span data-stu-id="e1eee-143">classId</span></span>|<span data-ttu-id="e1eee-144">Guid</span><span class="sxs-lookup"><span data-stu-id="e1eee-144">Guid</span></span>|<span data-ttu-id="e1eee-p103">Идентификатор класса. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e1eee-p103">The class identifier. Read-only.</span></span>|
|<span data-ttu-id="e1eee-147">id</span><span class="sxs-lookup"><span data-stu-id="e1eee-147">id</span></span>|<span data-ttu-id="e1eee-148">Строка</span><span class="sxs-lookup"><span data-stu-id="e1eee-148">String</span></span>|<span data-ttu-id="e1eee-p104">Уникальный идентификатор группы. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e1eee-p104">The group's unique identifier. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e1eee-151">Связи</span><span class="sxs-lookup"><span data-stu-id="e1eee-151">Relationships</span></span>
| <span data-ttu-id="e1eee-152">Связь</span><span class="sxs-lookup"><span data-stu-id="e1eee-152">Relationship</span></span> | <span data-ttu-id="e1eee-153">Тип</span><span class="sxs-lookup"><span data-stu-id="e1eee-153">Type</span></span>   |<span data-ttu-id="e1eee-154">Описание</span><span class="sxs-lookup"><span data-stu-id="e1eee-154">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e1eee-155">calendars</span><span class="sxs-lookup"><span data-stu-id="e1eee-155">calendars</span></span>|<span data-ttu-id="e1eee-156">Коллекция объектов [Calendar](calendar.md)</span><span class="sxs-lookup"><span data-stu-id="e1eee-156">[Calendar](calendar.md) collection</span></span>|<span data-ttu-id="e1eee-p105">Календари в группе календарей. Свойство навигации. Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="e1eee-p105">The calendars in the calendar group. Navigation property. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e1eee-161">Описание в формате JSON</span><span class="sxs-lookup"><span data-stu-id="e1eee-161">JSON representation</span></span>

<span data-ttu-id="e1eee-162">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e1eee-162">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "calendars"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.calendarGroup"
}-->

```json
{
  "changeKey": "string",
  "classId": "guid",
  "id": "string (identifier)",
  "name": "string"
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "calendarGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

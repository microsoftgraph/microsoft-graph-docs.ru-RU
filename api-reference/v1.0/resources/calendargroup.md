# <a name="calendargroup-resource-type"></a><span data-ttu-id="ecbb9-101">Тип ресурса calendarGroup</span><span class="sxs-lookup"><span data-stu-id="ecbb9-101">calendarGroup resource type</span></span>

<span data-ttu-id="ecbb9-102">Группа календарей.</span><span class="sxs-lookup"><span data-stu-id="ecbb9-102">A group of calendars.</span></span>

## <a name="methods"></a><span data-ttu-id="ecbb9-103">Методы</span><span class="sxs-lookup"><span data-stu-id="ecbb9-103">Methods</span></span>

| <span data-ttu-id="ecbb9-104">Метод</span><span class="sxs-lookup"><span data-stu-id="ecbb9-104">Method</span></span>                                                      | <span data-ttu-id="ecbb9-105">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="ecbb9-105">Return Type</span></span>                        | <span data-ttu-id="ecbb9-106">Описание</span><span class="sxs-lookup"><span data-stu-id="ecbb9-106">Description</span></span>                                                   |
| :---------------------------------------------------------- | :--------------------------------- | :------------------------------------------------------------ |
| [<span data-ttu-id="ecbb9-107">Список групп календарей</span><span class="sxs-lookup"><span data-stu-id="ecbb9-107">List calendar groups</span></span>](../api/user_list_calendargroups.md)  | <span data-ttu-id="ecbb9-108">Коллекция объектов [Calendar](calendar.md)</span><span class="sxs-lookup"><span data-stu-id="ecbb9-108">[Calendar](calendar.md) collection</span></span> | <span data-ttu-id="ecbb9-109">Получение групп календарей пользователя.</span><span class="sxs-lookup"><span data-stu-id="ecbb9-109">Get the user's calendar groups.</span></span>                               |
| [<span data-ttu-id="ecbb9-110">Создание группы календарей</span><span class="sxs-lookup"><span data-stu-id="ecbb9-110">Create calendar group</span></span>](../api/user_post_calendargroups.md) | [<span data-ttu-id="ecbb9-111">Календарь</span><span class="sxs-lookup"><span data-stu-id="ecbb9-111">Calendar</span></span>](calendar.md)            | <span data-ttu-id="ecbb9-112">Создание группы календарей.</span><span class="sxs-lookup"><span data-stu-id="ecbb9-112">Create a new calendar group.</span></span>                                  |
| [<span data-ttu-id="ecbb9-113">Получение группы календарей</span><span class="sxs-lookup"><span data-stu-id="ecbb9-113">Get calendar group</span></span>](../api/calendargroup_get.md)           | [<span data-ttu-id="ecbb9-114">calendarGroup</span><span class="sxs-lookup"><span data-stu-id="ecbb9-114">calendarGroup</span></span>](calendargroup.md)  | <span data-ttu-id="ecbb9-115">Чтение свойств и связей, принадлежащих объекту группы календарей.</span><span class="sxs-lookup"><span data-stu-id="ecbb9-115">Read properties and relationships of a calendar group object.</span></span> |
| [<span data-ttu-id="ecbb9-116">Обновление</span><span class="sxs-lookup"><span data-stu-id="ecbb9-116">Update</span></span>](../api/calendargroup_update.md)                    | [<span data-ttu-id="ecbb9-117">calendarGroup</span><span class="sxs-lookup"><span data-stu-id="ecbb9-117">calendarGroup</span></span>](calendargroup.md)  | <span data-ttu-id="ecbb9-118">Обновление объекта calendarGroup.</span><span class="sxs-lookup"><span data-stu-id="ecbb9-118">Update calendarGroup object.</span></span>                                  |
| [<span data-ttu-id="ecbb9-119">Удаление</span><span class="sxs-lookup"><span data-stu-id="ecbb9-119">Delete</span></span>](../api/calendargroup_delete.md)                    | <span data-ttu-id="ecbb9-120">Нет</span><span class="sxs-lookup"><span data-stu-id="ecbb9-120">None</span></span>                               | <span data-ttu-id="ecbb9-121">Удаление объекта calendarGroup.</span><span class="sxs-lookup"><span data-stu-id="ecbb9-121">Delete calendarGroup object.</span></span>                                  |
| [<span data-ttu-id="ecbb9-122">Список календарей</span><span class="sxs-lookup"><span data-stu-id="ecbb9-122">List calendars</span></span>](../api/calendargroup_list_calendars.md)    | <span data-ttu-id="ecbb9-123">Коллекция объектов [Calendar](calendar.md)</span><span class="sxs-lookup"><span data-stu-id="ecbb9-123">[Calendar](calendar.md) collection</span></span> | <span data-ttu-id="ecbb9-124">Список календарей в группе календарей.</span><span class="sxs-lookup"><span data-stu-id="ecbb9-124">List calendars in a calendar group.</span></span>                           |
| [<span data-ttu-id="ecbb9-125">Создание объекта Calendar</span><span class="sxs-lookup"><span data-stu-id="ecbb9-125">Create Calendar</span></span>](../api/calendargroup_post_calendars.md)   | [<span data-ttu-id="ecbb9-126">Календарь</span><span class="sxs-lookup"><span data-stu-id="ecbb9-126">Calendar</span></span>](calendar.md)            | <span data-ttu-id="ecbb9-127">Создание календаря в группе календарей.</span><span class="sxs-lookup"><span data-stu-id="ecbb9-127">Create a new Calendar in a calendar group.</span></span>                    |

## <a name="properties"></a><span data-ttu-id="ecbb9-128">Свойства</span><span class="sxs-lookup"><span data-stu-id="ecbb9-128">Properties</span></span>

| <span data-ttu-id="ecbb9-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="ecbb9-129">Property</span></span>  | <span data-ttu-id="ecbb9-130">Тип</span><span class="sxs-lookup"><span data-stu-id="ecbb9-130">Type</span></span>   | <span data-ttu-id="ecbb9-131">Описание</span><span class="sxs-lookup"><span data-stu-id="ecbb9-131">Description</span></span>                                                                                                                                                                                               |
| :-------- | :----- | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="ecbb9-132">name</span><span class="sxs-lookup"><span data-stu-id="ecbb9-132">name</span></span>      | <span data-ttu-id="ecbb9-133">Строка​</span><span class="sxs-lookup"><span data-stu-id="ecbb9-133">String</span></span> | <span data-ttu-id="ecbb9-134">Имя группы.</span><span class="sxs-lookup"><span data-stu-id="ecbb9-134">The group name.</span></span>                                                                                                                                                                                           |
| <span data-ttu-id="ecbb9-135">changeKey</span><span class="sxs-lookup"><span data-stu-id="ecbb9-135">changeKey</span></span> | <span data-ttu-id="ecbb9-136">Строка​</span><span class="sxs-lookup"><span data-stu-id="ecbb9-136">String</span></span> | <span data-ttu-id="ecbb9-p101">Указывает версию группы календарей. При каждом изменении группы календарей также меняется значение ChangeKey. Благодаря этому Exchange может применять изменения к правильной версии объекта. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ecbb9-p101">Identifies the version of the calendar group. Every time the calendar group is changed, ChangeKey changes as well. This allows Exchange to apply changes to the correct version of the object. Read-only.</span></span> |
| <span data-ttu-id="ecbb9-141">classId</span><span class="sxs-lookup"><span data-stu-id="ecbb9-141">classId</span></span>   | <span data-ttu-id="ecbb9-142">Guid</span><span class="sxs-lookup"><span data-stu-id="ecbb9-142">Guid</span></span>   | <span data-ttu-id="ecbb9-p102">Идентификатор класса. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ecbb9-p102">The class identifier. Read-only.</span></span>                                                                                                                                                                          |
| <span data-ttu-id="ecbb9-145">id</span><span class="sxs-lookup"><span data-stu-id="ecbb9-145">id</span></span>        | <span data-ttu-id="ecbb9-146">Строка​</span><span class="sxs-lookup"><span data-stu-id="ecbb9-146">String</span></span> | <span data-ttu-id="ecbb9-p103">Уникальный идентификатор группы. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ecbb9-p103">The group's unique identifier. Read-only.</span></span>                                                                                                                                                                 |

## <a name="relationships"></a><span data-ttu-id="ecbb9-149">Связи</span><span class="sxs-lookup"><span data-stu-id="ecbb9-149">Relationships</span></span>

| <span data-ttu-id="ecbb9-150">Связь</span><span class="sxs-lookup"><span data-stu-id="ecbb9-150">Relationship</span></span> | <span data-ttu-id="ecbb9-151">Тип</span><span class="sxs-lookup"><span data-stu-id="ecbb9-151">Type</span></span>                               | <span data-ttu-id="ecbb9-152">Описание</span><span class="sxs-lookup"><span data-stu-id="ecbb9-152">Description</span></span>                                                                    |
| :----------- | :--------------------------------- | :----------------------------------------------------------------------------- |
| <span data-ttu-id="ecbb9-153">calendars</span><span class="sxs-lookup"><span data-stu-id="ecbb9-153">calendars</span></span>    | <span data-ttu-id="ecbb9-154">Коллекция [Calendar](calendar.md)</span><span class="sxs-lookup"><span data-stu-id="ecbb9-154">[Calendar](calendar.md) collection</span></span> | <span data-ttu-id="ecbb9-p104">Календари в группе календарей. Свойство навигации. Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="ecbb9-p104">The calendars in the calendar group. Navigation property. Read-only. Nullable.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="ecbb9-159">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ecbb9-159">JSON representation</span></span>

<span data-ttu-id="ecbb9-160">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ecbb9-160">Here is a JSON representation of the resource</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "calendars"
  ],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.calendarGroup",
  "@odata.annotations": [
    {
      "property": "calendars",
      "capabilities": {
        "changeTracking": false,
        "expandable": false,
        "navigability": "single",
        "searchable": false
      }
    }
  ]
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

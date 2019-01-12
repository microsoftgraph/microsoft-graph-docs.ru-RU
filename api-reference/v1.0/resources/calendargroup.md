---
title: Тип ресурса calendarGroup
description: Группа пользователей календарей.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 5b75ebf253276876129859be7d37ecb6748fc0d9
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27949628"
---
# <a name="calendargroup-resource-type"></a><span data-ttu-id="6b05b-103">Тип ресурса calendarGroup</span><span class="sxs-lookup"><span data-stu-id="6b05b-103">calendarGroup resource type</span></span>

<span data-ttu-id="6b05b-104">Группа пользователей календарей.</span><span class="sxs-lookup"><span data-stu-id="6b05b-104">A group of user calendars.</span></span>

## <a name="methods"></a><span data-ttu-id="6b05b-105">Методы</span><span class="sxs-lookup"><span data-stu-id="6b05b-105">Methods</span></span>

| <span data-ttu-id="6b05b-106">Метод</span><span class="sxs-lookup"><span data-stu-id="6b05b-106">Method</span></span>                                                      | <span data-ttu-id="6b05b-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="6b05b-107">Return Type</span></span>                        | <span data-ttu-id="6b05b-108">Описание</span><span class="sxs-lookup"><span data-stu-id="6b05b-108">Description</span></span>                                                   |
| :---------------------------------------------------------- | :--------------------------------- | :------------------------------------------------------------ |
| [<span data-ttu-id="6b05b-109">Список групп календарей</span><span class="sxs-lookup"><span data-stu-id="6b05b-109">List calendar groups</span></span>](../api/user-list-calendargroups.md)  | <span data-ttu-id="6b05b-110">Коллекция объектов [Calendar](calendar.md)</span><span class="sxs-lookup"><span data-stu-id="6b05b-110">[Calendar](calendar.md) collection</span></span> | <span data-ttu-id="6b05b-111">Получение групп календарей пользователя.</span><span class="sxs-lookup"><span data-stu-id="6b05b-111">Get the user's calendar groups.</span></span>                               |
| [<span data-ttu-id="6b05b-112">Создание группы календарей</span><span class="sxs-lookup"><span data-stu-id="6b05b-112">Create calendar group</span></span>](../api/user-post-calendargroups.md) | [<span data-ttu-id="6b05b-113">Calendar</span><span class="sxs-lookup"><span data-stu-id="6b05b-113">Calendar</span></span>](calendar.md)            | <span data-ttu-id="6b05b-114">Создание группы календарей.</span><span class="sxs-lookup"><span data-stu-id="6b05b-114">Create a new calendar group.</span></span>                                  |
| [<span data-ttu-id="6b05b-115">Получение группы календарей</span><span class="sxs-lookup"><span data-stu-id="6b05b-115">Get calendar group</span></span>](../api/calendargroup-get.md)           | [<span data-ttu-id="6b05b-116">calendarGroup</span><span class="sxs-lookup"><span data-stu-id="6b05b-116">calendarGroup</span></span>](calendargroup.md)  | <span data-ttu-id="6b05b-117">Чтение свойств и связей, принадлежащих объекту группы календарей.</span><span class="sxs-lookup"><span data-stu-id="6b05b-117">Read properties and relationships of a calendar group object.</span></span> |
| [<span data-ttu-id="6b05b-118">Обновление</span><span class="sxs-lookup"><span data-stu-id="6b05b-118">Update</span></span>](../api/calendargroup-update.md)                    | [<span data-ttu-id="6b05b-119">calendarGroup</span><span class="sxs-lookup"><span data-stu-id="6b05b-119">calendarGroup</span></span>](calendargroup.md)  | <span data-ttu-id="6b05b-120">Обновление объекта calendarGroup.</span><span class="sxs-lookup"><span data-stu-id="6b05b-120">Update calendarGroup object.</span></span>                                  |
| [<span data-ttu-id="6b05b-121">Удаление</span><span class="sxs-lookup"><span data-stu-id="6b05b-121">Delete</span></span>](../api/calendargroup-delete.md)                    | <span data-ttu-id="6b05b-122">Нет</span><span class="sxs-lookup"><span data-stu-id="6b05b-122">None</span></span>                               | <span data-ttu-id="6b05b-123">Удаление объекта calendarGroup.</span><span class="sxs-lookup"><span data-stu-id="6b05b-123">Delete calendarGroup object.</span></span>                                  |
| [<span data-ttu-id="6b05b-124">Список календарей</span><span class="sxs-lookup"><span data-stu-id="6b05b-124">List calendars</span></span>](../api/calendargroup-list-calendars.md)    | <span data-ttu-id="6b05b-125">Коллекция объектов [Calendar](calendar.md)</span><span class="sxs-lookup"><span data-stu-id="6b05b-125">[Calendar](calendar.md) collection</span></span> | <span data-ttu-id="6b05b-126">Список календарей в группе календарей.</span><span class="sxs-lookup"><span data-stu-id="6b05b-126">List calendars in a calendar group.</span></span>                           |
| [<span data-ttu-id="6b05b-127">Создание объекта Calendar</span><span class="sxs-lookup"><span data-stu-id="6b05b-127">Create Calendar</span></span>](../api/calendargroup-post-calendars.md)   | [<span data-ttu-id="6b05b-128">Calendar</span><span class="sxs-lookup"><span data-stu-id="6b05b-128">Calendar</span></span>](calendar.md)            | <span data-ttu-id="6b05b-129">Создание календаря в группе календарей.</span><span class="sxs-lookup"><span data-stu-id="6b05b-129">Create a new Calendar in a calendar group.</span></span>                    |

## <a name="properties"></a><span data-ttu-id="6b05b-130">Свойства</span><span class="sxs-lookup"><span data-stu-id="6b05b-130">Properties</span></span>

| <span data-ttu-id="6b05b-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="6b05b-131">Property</span></span>  | <span data-ttu-id="6b05b-132">Тип</span><span class="sxs-lookup"><span data-stu-id="6b05b-132">Type</span></span>   | <span data-ttu-id="6b05b-133">Описание</span><span class="sxs-lookup"><span data-stu-id="6b05b-133">Description</span></span>                                                                                                                                                                                               |
| :-------- | :----- | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="6b05b-134">name</span><span class="sxs-lookup"><span data-stu-id="6b05b-134">name</span></span>      | <span data-ttu-id="6b05b-135">String</span><span class="sxs-lookup"><span data-stu-id="6b05b-135">String</span></span> | <span data-ttu-id="6b05b-136">Имя группы.</span><span class="sxs-lookup"><span data-stu-id="6b05b-136">The group name.</span></span>                                                                                                                                                                                           |
| <span data-ttu-id="6b05b-137">changeKey</span><span class="sxs-lookup"><span data-stu-id="6b05b-137">changeKey</span></span> | <span data-ttu-id="6b05b-138">Строка</span><span class="sxs-lookup"><span data-stu-id="6b05b-138">String</span></span> | <span data-ttu-id="6b05b-p101">Указывает версию группы календарей. При каждом изменении группы календарей также меняется значение ChangeKey. Благодаря этому Exchange может применять изменения к правильной версии объекта. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6b05b-p101">Identifies the version of the calendar group. Every time the calendar group is changed, ChangeKey changes as well. This allows Exchange to apply changes to the correct version of the object. Read-only.</span></span> |
| <span data-ttu-id="6b05b-143">classId</span><span class="sxs-lookup"><span data-stu-id="6b05b-143">classId</span></span>   | <span data-ttu-id="6b05b-144">Guid</span><span class="sxs-lookup"><span data-stu-id="6b05b-144">Guid</span></span>   | <span data-ttu-id="6b05b-p102">Идентификатор класса. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6b05b-p102">The class identifier. Read-only.</span></span>                                                                                                                                                                          |
| <span data-ttu-id="6b05b-147">id</span><span class="sxs-lookup"><span data-stu-id="6b05b-147">id</span></span>        | <span data-ttu-id="6b05b-148">Строка</span><span class="sxs-lookup"><span data-stu-id="6b05b-148">String</span></span> | <span data-ttu-id="6b05b-p103">Уникальный идентификатор группы. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6b05b-p103">The group's unique identifier. Read-only.</span></span>                                                                                                                                                                 |

## <a name="relationships"></a><span data-ttu-id="6b05b-151">Связи</span><span class="sxs-lookup"><span data-stu-id="6b05b-151">Relationships</span></span>

| <span data-ttu-id="6b05b-152">Связь</span><span class="sxs-lookup"><span data-stu-id="6b05b-152">Relationship</span></span> | <span data-ttu-id="6b05b-153">Тип</span><span class="sxs-lookup"><span data-stu-id="6b05b-153">Type</span></span>                               | <span data-ttu-id="6b05b-154">Описание</span><span class="sxs-lookup"><span data-stu-id="6b05b-154">Description</span></span>                                                                    |
| :----------- | :--------------------------------- | :----------------------------------------------------------------------------- |
| <span data-ttu-id="6b05b-155">calendars</span><span class="sxs-lookup"><span data-stu-id="6b05b-155">calendars</span></span>    | <span data-ttu-id="6b05b-156">Коллекция [Calendar](calendar.md)</span><span class="sxs-lookup"><span data-stu-id="6b05b-156">[Calendar](calendar.md) collection</span></span> | <span data-ttu-id="6b05b-p104">Календари в группе календарей. Свойство навигации. Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="6b05b-p104">The calendars in the calendar group. Navigation property. Read-only. Nullable.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="6b05b-161">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6b05b-161">JSON representation</span></span>

<span data-ttu-id="6b05b-162">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6b05b-162">Here is a JSON representation of the resource</span></span>

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

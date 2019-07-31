---
title: Тип ресурса calendarGroup
description: Группа пользовательских календарей.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: e556743517436950e3608247b537307e5bb97e3d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36013047"
---
# <a name="calendargroup-resource-type"></a><span data-ttu-id="f5513-103">Тип ресурса calendarGroup</span><span class="sxs-lookup"><span data-stu-id="f5513-103">calendarGroup resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f5513-104">Группа пользовательских календарей.</span><span class="sxs-lookup"><span data-stu-id="f5513-104">A group of user calendars.</span></span>

## <a name="methods"></a><span data-ttu-id="f5513-105">Методы</span><span class="sxs-lookup"><span data-stu-id="f5513-105">Methods</span></span>

| <span data-ttu-id="f5513-106">Метод</span><span class="sxs-lookup"><span data-stu-id="f5513-106">Method</span></span>                                                      | <span data-ttu-id="f5513-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="f5513-107">Return Type</span></span>                        | <span data-ttu-id="f5513-108">Описание</span><span class="sxs-lookup"><span data-stu-id="f5513-108">Description</span></span>                                                   |
| :---------------------------------------------------------- | :--------------------------------- | :------------------------------------------------------------ |
| [<span data-ttu-id="f5513-109">Список групп календарей</span><span class="sxs-lookup"><span data-stu-id="f5513-109">List calendar groups</span></span>](../api/user-list-calendargroups.md)  | <span data-ttu-id="f5513-110">Коллекция [Calendar](calendar.md)</span><span class="sxs-lookup"><span data-stu-id="f5513-110">[Calendar](calendar.md) collection</span></span> | <span data-ttu-id="f5513-111">Получение групп календарей пользователя.</span><span class="sxs-lookup"><span data-stu-id="f5513-111">Get the user's calendar groups.</span></span>                               |
| [<span data-ttu-id="f5513-112">Создание группы календарей</span><span class="sxs-lookup"><span data-stu-id="f5513-112">Create calendar group</span></span>](../api/user-post-calendargroups.md) | [<span data-ttu-id="f5513-113">Calendar</span><span class="sxs-lookup"><span data-stu-id="f5513-113">Calendar</span></span>](calendar.md)            | <span data-ttu-id="f5513-114">Создание группы календарей.</span><span class="sxs-lookup"><span data-stu-id="f5513-114">Create a new calendar group.</span></span>                                  |
| [<span data-ttu-id="f5513-115">Получение группы календарей</span><span class="sxs-lookup"><span data-stu-id="f5513-115">Get calendar group</span></span>](../api/calendargroup-get.md)           | [<span data-ttu-id="f5513-116">calendarGroup</span><span class="sxs-lookup"><span data-stu-id="f5513-116">calendarGroup</span></span>](calendargroup.md)  | <span data-ttu-id="f5513-117">Чтение свойств и связей, принадлежащих объекту группы календарей.</span><span class="sxs-lookup"><span data-stu-id="f5513-117">Read properties and relationships of a calendar group object.</span></span> |
| [<span data-ttu-id="f5513-118">Обновление</span><span class="sxs-lookup"><span data-stu-id="f5513-118">Update</span></span>](../api/calendargroup-update.md)                    | [<span data-ttu-id="f5513-119">calendarGroup</span><span class="sxs-lookup"><span data-stu-id="f5513-119">calendarGroup</span></span>](calendargroup.md)  | <span data-ttu-id="f5513-120">Обновление объекта calendarGroup.</span><span class="sxs-lookup"><span data-stu-id="f5513-120">Update calendarGroup object.</span></span>                                  |
| [<span data-ttu-id="f5513-121">Удаление</span><span class="sxs-lookup"><span data-stu-id="f5513-121">Delete</span></span>](../api/calendargroup-delete.md)                    | <span data-ttu-id="f5513-122">Нет</span><span class="sxs-lookup"><span data-stu-id="f5513-122">None</span></span>                               | <span data-ttu-id="f5513-123">Удаление объекта calendarGroup.</span><span class="sxs-lookup"><span data-stu-id="f5513-123">Delete calendarGroup object.</span></span>                                  |
| [<span data-ttu-id="f5513-124">Список календарей</span><span class="sxs-lookup"><span data-stu-id="f5513-124">List calendars</span></span>](../api/calendargroup-list-calendars.md)    | <span data-ttu-id="f5513-125">Коллекция объектов [Calendar](calendar.md)</span><span class="sxs-lookup"><span data-stu-id="f5513-125">[Calendar](calendar.md) collection</span></span> | <span data-ttu-id="f5513-126">Список календарей в группе календарей.</span><span class="sxs-lookup"><span data-stu-id="f5513-126">List calendars in a calendar group.</span></span>                           |
| [<span data-ttu-id="f5513-127">Создание объекта Calendar</span><span class="sxs-lookup"><span data-stu-id="f5513-127">Create Calendar</span></span>](../api/calendargroup-post-calendars.md)   | [<span data-ttu-id="f5513-128">Calendar</span><span class="sxs-lookup"><span data-stu-id="f5513-128">Calendar</span></span>](calendar.md)            | <span data-ttu-id="f5513-129">Создание календаря в группе календарей.</span><span class="sxs-lookup"><span data-stu-id="f5513-129">Create a new Calendar in a calendar group.</span></span>                    |

## <a name="properties"></a><span data-ttu-id="f5513-130">Свойства</span><span class="sxs-lookup"><span data-stu-id="f5513-130">Properties</span></span>

| <span data-ttu-id="f5513-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="f5513-131">Property</span></span>  | <span data-ttu-id="f5513-132">Тип</span><span class="sxs-lookup"><span data-stu-id="f5513-132">Type</span></span>   | <span data-ttu-id="f5513-133">Описание</span><span class="sxs-lookup"><span data-stu-id="f5513-133">Description</span></span>                                                                                                                                                                                               |
| :-------- | :----- | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="f5513-134">name</span><span class="sxs-lookup"><span data-stu-id="f5513-134">name</span></span>      | <span data-ttu-id="f5513-135">String</span><span class="sxs-lookup"><span data-stu-id="f5513-135">String</span></span> | <span data-ttu-id="f5513-136">Имя группы.</span><span class="sxs-lookup"><span data-stu-id="f5513-136">The group name.</span></span>                                                                                                                                                                                           |
| <span data-ttu-id="f5513-137">changeKey</span><span class="sxs-lookup"><span data-stu-id="f5513-137">changeKey</span></span> | <span data-ttu-id="f5513-138">String</span><span class="sxs-lookup"><span data-stu-id="f5513-138">String</span></span> | <span data-ttu-id="f5513-p101">Указывает версию группы календарей. При каждом изменении группы календарей также меняется значение ChangeKey. Благодаря этому Exchange может применять изменения к правильной версии объекта. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f5513-p101">Identifies the version of the calendar group. Every time the calendar group is changed, ChangeKey changes as well. This allows Exchange to apply changes to the correct version of the object. Read-only.</span></span> |
| <span data-ttu-id="f5513-143">classId</span><span class="sxs-lookup"><span data-stu-id="f5513-143">classId</span></span>   | <span data-ttu-id="f5513-144">Guid</span><span class="sxs-lookup"><span data-stu-id="f5513-144">Guid</span></span>   | <span data-ttu-id="f5513-p102">Идентификатор класса. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f5513-p102">The class identifier. Read-only.</span></span>                                                                                                                                                                          |
| <span data-ttu-id="f5513-147">id</span><span class="sxs-lookup"><span data-stu-id="f5513-147">id</span></span>        | <span data-ttu-id="f5513-148">Строка</span><span class="sxs-lookup"><span data-stu-id="f5513-148">String</span></span> | <span data-ttu-id="f5513-p103">Уникальный идентификатор группы. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f5513-p103">The group's unique identifier. Read-only.</span></span>                                                                                                                                                                 |

## <a name="relationships"></a><span data-ttu-id="f5513-151">Отношения</span><span class="sxs-lookup"><span data-stu-id="f5513-151">Relationships</span></span>

| <span data-ttu-id="f5513-152">Отношение</span><span class="sxs-lookup"><span data-stu-id="f5513-152">Relationship</span></span> | <span data-ttu-id="f5513-153">Тип</span><span class="sxs-lookup"><span data-stu-id="f5513-153">Type</span></span>                               | <span data-ttu-id="f5513-154">Описание</span><span class="sxs-lookup"><span data-stu-id="f5513-154">Description</span></span>                                                                    |
| :----------- | :--------------------------------- | :----------------------------------------------------------------------------- |
| <span data-ttu-id="f5513-155">calendars</span><span class="sxs-lookup"><span data-stu-id="f5513-155">calendars</span></span>    | <span data-ttu-id="f5513-156">Коллекция [Calendar](calendar.md)</span><span class="sxs-lookup"><span data-stu-id="f5513-156">[Calendar](calendar.md) collection</span></span> | <span data-ttu-id="f5513-p104">Календари в группе календарей. Свойство навигации. Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="f5513-p104">The calendars in the calendar group. Navigation property. Read-only. Nullable.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="f5513-161">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f5513-161">JSON representation</span></span>

<span data-ttu-id="f5513-162">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f5513-162">Here is a JSON representation of the resource</span></span>

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

<!--
{
  "type": "#page.annotation",
  "description": "calendarGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

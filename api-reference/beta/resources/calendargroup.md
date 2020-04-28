---
title: Тип ресурса calendarGroup
description: Группа пользовательских календарей.
author: harini84
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: a630d35f5527494ce4cf477219dfd1f22547c490
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43471498"
---
# <a name="calendargroup-resource-type"></a><span data-ttu-id="aa949-103">Тип ресурса calendarGroup</span><span class="sxs-lookup"><span data-stu-id="aa949-103">calendarGroup resource type</span></span>

<span data-ttu-id="aa949-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aa949-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aa949-105">Группа пользовательских календарей.</span><span class="sxs-lookup"><span data-stu-id="aa949-105">A group of user calendars.</span></span>

## <a name="methods"></a><span data-ttu-id="aa949-106">Методы</span><span class="sxs-lookup"><span data-stu-id="aa949-106">Methods</span></span>

| <span data-ttu-id="aa949-107">Метод</span><span class="sxs-lookup"><span data-stu-id="aa949-107">Method</span></span>                                                      | <span data-ttu-id="aa949-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="aa949-108">Return Type</span></span>                        | <span data-ttu-id="aa949-109">Описание</span><span class="sxs-lookup"><span data-stu-id="aa949-109">Description</span></span>                                                   |
| :---------------------------------------------------------- | :--------------------------------- | :------------------------------------------------------------ |
| [<span data-ttu-id="aa949-110">Список групп календарей</span><span class="sxs-lookup"><span data-stu-id="aa949-110">List calendar groups</span></span>](../api/user-list-calendargroups.md)  | <span data-ttu-id="aa949-111">Коллекция [Calendar](calendar.md)</span><span class="sxs-lookup"><span data-stu-id="aa949-111">[Calendar](calendar.md) collection</span></span> | <span data-ttu-id="aa949-112">Получение групп календарей пользователя.</span><span class="sxs-lookup"><span data-stu-id="aa949-112">Get the user's calendar groups.</span></span>                               |
| [<span data-ttu-id="aa949-113">Создание группы календарей</span><span class="sxs-lookup"><span data-stu-id="aa949-113">Create calendar group</span></span>](../api/user-post-calendargroups.md) | [<span data-ttu-id="aa949-114">Календарь</span><span class="sxs-lookup"><span data-stu-id="aa949-114">Calendar</span></span>](calendar.md)            | <span data-ttu-id="aa949-115">Создание группы календарей.</span><span class="sxs-lookup"><span data-stu-id="aa949-115">Create a new calendar group.</span></span>                                  |
| [<span data-ttu-id="aa949-116">Получение группы календарей</span><span class="sxs-lookup"><span data-stu-id="aa949-116">Get calendar group</span></span>](../api/calendargroup-get.md)           | [<span data-ttu-id="aa949-117">calendarGroup</span><span class="sxs-lookup"><span data-stu-id="aa949-117">calendarGroup</span></span>](calendargroup.md)  | <span data-ttu-id="aa949-118">Чтение свойств и связей, принадлежащих объекту группы календарей.</span><span class="sxs-lookup"><span data-stu-id="aa949-118">Read properties and relationships of a calendar group object.</span></span> |
| [<span data-ttu-id="aa949-119">Обновление</span><span class="sxs-lookup"><span data-stu-id="aa949-119">Update</span></span>](../api/calendargroup-update.md)                    | [<span data-ttu-id="aa949-120">calendarGroup</span><span class="sxs-lookup"><span data-stu-id="aa949-120">calendarGroup</span></span>](calendargroup.md)  | <span data-ttu-id="aa949-121">Обновление объекта calendarGroup.</span><span class="sxs-lookup"><span data-stu-id="aa949-121">Update calendarGroup object.</span></span>                                  |
| <span data-ttu-id="aa949-122">[удаление](../api/calendargroup-delete.md);</span><span class="sxs-lookup"><span data-stu-id="aa949-122">[Delete](../api/calendargroup-delete.md)</span></span>                    | <span data-ttu-id="aa949-123">Нет</span><span class="sxs-lookup"><span data-stu-id="aa949-123">None</span></span>                               | <span data-ttu-id="aa949-124">Удаление объекта calendarGroup.</span><span class="sxs-lookup"><span data-stu-id="aa949-124">Delete calendarGroup object.</span></span>                                  |
| [<span data-ttu-id="aa949-125">Список календарей</span><span class="sxs-lookup"><span data-stu-id="aa949-125">List calendars</span></span>](../api/calendargroup-list-calendars.md)    | <span data-ttu-id="aa949-126">Коллекция объектов [Calendar](calendar.md)</span><span class="sxs-lookup"><span data-stu-id="aa949-126">[Calendar](calendar.md) collection</span></span> | <span data-ttu-id="aa949-127">Список календарей в группе календарей.</span><span class="sxs-lookup"><span data-stu-id="aa949-127">List calendars in a calendar group.</span></span>                           |
| [<span data-ttu-id="aa949-128">Создание объекта Calendar</span><span class="sxs-lookup"><span data-stu-id="aa949-128">Create Calendar</span></span>](../api/calendargroup-post-calendars.md)   | [<span data-ttu-id="aa949-129">Calendar</span><span class="sxs-lookup"><span data-stu-id="aa949-129">Calendar</span></span>](calendar.md)            | <span data-ttu-id="aa949-130">Создание календаря в группе календарей.</span><span class="sxs-lookup"><span data-stu-id="aa949-130">Create a new Calendar in a calendar group.</span></span>                    |

## <a name="properties"></a><span data-ttu-id="aa949-131">Свойства</span><span class="sxs-lookup"><span data-stu-id="aa949-131">Properties</span></span>

| <span data-ttu-id="aa949-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="aa949-132">Property</span></span>  | <span data-ttu-id="aa949-133">Тип</span><span class="sxs-lookup"><span data-stu-id="aa949-133">Type</span></span>   | <span data-ttu-id="aa949-134">Описание</span><span class="sxs-lookup"><span data-stu-id="aa949-134">Description</span></span>                                                                                                                                                                                               |
| :-------- | :----- | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="aa949-135">name</span><span class="sxs-lookup"><span data-stu-id="aa949-135">name</span></span>      | <span data-ttu-id="aa949-136">String</span><span class="sxs-lookup"><span data-stu-id="aa949-136">String</span></span> | <span data-ttu-id="aa949-137">Имя группы.</span><span class="sxs-lookup"><span data-stu-id="aa949-137">The group name.</span></span>                                                                                                                                                                                           |
| <span data-ttu-id="aa949-138">changeKey</span><span class="sxs-lookup"><span data-stu-id="aa949-138">changeKey</span></span> | <span data-ttu-id="aa949-139">String</span><span class="sxs-lookup"><span data-stu-id="aa949-139">String</span></span> | <span data-ttu-id="aa949-p101">Указывает версию группы календарей. При каждом изменении группы календарей также меняется значение ChangeKey. Благодаря этому Exchange может применять изменения к правильной версии объекта. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="aa949-p101">Identifies the version of the calendar group. Every time the calendar group is changed, ChangeKey changes as well. This allows Exchange to apply changes to the correct version of the object. Read-only.</span></span> |
| <span data-ttu-id="aa949-144">classId</span><span class="sxs-lookup"><span data-stu-id="aa949-144">classId</span></span>   | <span data-ttu-id="aa949-145">Guid</span><span class="sxs-lookup"><span data-stu-id="aa949-145">Guid</span></span>   | <span data-ttu-id="aa949-p102">Идентификатор класса. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="aa949-p102">The class identifier. Read-only.</span></span>                                                                                                                                                                          |
| <span data-ttu-id="aa949-148">id</span><span class="sxs-lookup"><span data-stu-id="aa949-148">id</span></span>        | <span data-ttu-id="aa949-149">Строка</span><span class="sxs-lookup"><span data-stu-id="aa949-149">String</span></span> | <span data-ttu-id="aa949-p103">Уникальный идентификатор группы. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="aa949-p103">The group's unique identifier. Read-only.</span></span>                                                                                                                                                                 |

## <a name="relationships"></a><span data-ttu-id="aa949-152">Связи</span><span class="sxs-lookup"><span data-stu-id="aa949-152">Relationships</span></span>

| <span data-ttu-id="aa949-153">Связь</span><span class="sxs-lookup"><span data-stu-id="aa949-153">Relationship</span></span> | <span data-ttu-id="aa949-154">Тип</span><span class="sxs-lookup"><span data-stu-id="aa949-154">Type</span></span>                               | <span data-ttu-id="aa949-155">Описание</span><span class="sxs-lookup"><span data-stu-id="aa949-155">Description</span></span>                                                                    |
| :----------- | :--------------------------------- | :----------------------------------------------------------------------------- |
| <span data-ttu-id="aa949-156">calendars</span><span class="sxs-lookup"><span data-stu-id="aa949-156">calendars</span></span>    | <span data-ttu-id="aa949-157">Коллекция [Calendar](calendar.md)</span><span class="sxs-lookup"><span data-stu-id="aa949-157">[Calendar](calendar.md) collection</span></span> | <span data-ttu-id="aa949-p104">Календари в группе календарей. Свойство навигации. Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="aa949-p104">The calendars in the calendar group. Navigation property. Read-only. Nullable.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="aa949-162">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="aa949-162">JSON representation</span></span>

<span data-ttu-id="aa949-163">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="aa949-163">Here is a JSON representation of the resource</span></span>

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

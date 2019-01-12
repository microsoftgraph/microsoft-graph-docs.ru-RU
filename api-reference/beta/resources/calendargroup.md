---
title: Тип ресурса calendarGroup
description: Группа пользователей календарей.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 10a840fd9ae9835eb5ca6a96b88719605f89245b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27985293"
---
# <a name="calendargroup-resource-type"></a><span data-ttu-id="a4e63-103">Тип ресурса calendarGroup</span><span class="sxs-lookup"><span data-stu-id="a4e63-103">calendarGroup resource type</span></span>

> <span data-ttu-id="a4e63-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="a4e63-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a4e63-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a4e63-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a4e63-106">Группа пользователей календарей.</span><span class="sxs-lookup"><span data-stu-id="a4e63-106">A group of user calendars.</span></span>

## <a name="methods"></a><span data-ttu-id="a4e63-107">Методы</span><span class="sxs-lookup"><span data-stu-id="a4e63-107">Methods</span></span>

| <span data-ttu-id="a4e63-108">Метод</span><span class="sxs-lookup"><span data-stu-id="a4e63-108">Method</span></span>                                                      | <span data-ttu-id="a4e63-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="a4e63-109">Return Type</span></span>                        | <span data-ttu-id="a4e63-110">Описание</span><span class="sxs-lookup"><span data-stu-id="a4e63-110">Description</span></span>                                                   |
| :---------------------------------------------------------- | :--------------------------------- | :------------------------------------------------------------ |
| [<span data-ttu-id="a4e63-111">Список групп календарей</span><span class="sxs-lookup"><span data-stu-id="a4e63-111">List calendar groups</span></span>](../api/user-list-calendargroups.md)  | <span data-ttu-id="a4e63-112">Коллекция объектов [Calendar](calendar.md)</span><span class="sxs-lookup"><span data-stu-id="a4e63-112">[Calendar](calendar.md) collection</span></span> | <span data-ttu-id="a4e63-113">Получение групп календарей пользователя.</span><span class="sxs-lookup"><span data-stu-id="a4e63-113">Get the user's calendar groups.</span></span>                               |
| [<span data-ttu-id="a4e63-114">Создание группы календарей</span><span class="sxs-lookup"><span data-stu-id="a4e63-114">Create calendar group</span></span>](../api/user-post-calendargroups.md) | [<span data-ttu-id="a4e63-115">Calendar</span><span class="sxs-lookup"><span data-stu-id="a4e63-115">Calendar</span></span>](calendar.md)            | <span data-ttu-id="a4e63-116">Создание группы календарей.</span><span class="sxs-lookup"><span data-stu-id="a4e63-116">Create a new calendar group.</span></span>                                  |
| [<span data-ttu-id="a4e63-117">Получение группы календарей</span><span class="sxs-lookup"><span data-stu-id="a4e63-117">Get calendar group</span></span>](../api/calendargroup-get.md)           | [<span data-ttu-id="a4e63-118">calendarGroup</span><span class="sxs-lookup"><span data-stu-id="a4e63-118">calendarGroup</span></span>](calendargroup.md)  | <span data-ttu-id="a4e63-119">Чтение свойств и связей, принадлежащих объекту группы календарей.</span><span class="sxs-lookup"><span data-stu-id="a4e63-119">Read properties and relationships of a calendar group object.</span></span> |
| [<span data-ttu-id="a4e63-120">Обновление</span><span class="sxs-lookup"><span data-stu-id="a4e63-120">Update</span></span>](../api/calendargroup-update.md)                    | [<span data-ttu-id="a4e63-121">calendarGroup</span><span class="sxs-lookup"><span data-stu-id="a4e63-121">calendarGroup</span></span>](calendargroup.md)  | <span data-ttu-id="a4e63-122">Обновление объекта calendarGroup.</span><span class="sxs-lookup"><span data-stu-id="a4e63-122">Update calendarGroup object.</span></span>                                  |
| [<span data-ttu-id="a4e63-123">Удаление</span><span class="sxs-lookup"><span data-stu-id="a4e63-123">Delete</span></span>](../api/calendargroup-delete.md)                    | <span data-ttu-id="a4e63-124">Нет</span><span class="sxs-lookup"><span data-stu-id="a4e63-124">None</span></span>                               | <span data-ttu-id="a4e63-125">Удаление объекта calendarGroup.</span><span class="sxs-lookup"><span data-stu-id="a4e63-125">Delete calendarGroup object.</span></span>                                  |
| [<span data-ttu-id="a4e63-126">Список календарей</span><span class="sxs-lookup"><span data-stu-id="a4e63-126">List calendars</span></span>](../api/calendargroup-list-calendars.md)    | <span data-ttu-id="a4e63-127">Коллекция объектов [Calendar](calendar.md)</span><span class="sxs-lookup"><span data-stu-id="a4e63-127">[Calendar](calendar.md) collection</span></span> | <span data-ttu-id="a4e63-128">Список календарей в группе календарей.</span><span class="sxs-lookup"><span data-stu-id="a4e63-128">List calendars in a calendar group.</span></span>                           |
| [<span data-ttu-id="a4e63-129">Создание объекта Calendar</span><span class="sxs-lookup"><span data-stu-id="a4e63-129">Create Calendar</span></span>](../api/calendargroup-post-calendars.md)   | [<span data-ttu-id="a4e63-130">Calendar</span><span class="sxs-lookup"><span data-stu-id="a4e63-130">Calendar</span></span>](calendar.md)            | <span data-ttu-id="a4e63-131">Создание календаря в группе календарей.</span><span class="sxs-lookup"><span data-stu-id="a4e63-131">Create a new Calendar in a calendar group.</span></span>                    |

## <a name="properties"></a><span data-ttu-id="a4e63-132">Свойства</span><span class="sxs-lookup"><span data-stu-id="a4e63-132">Properties</span></span>

| <span data-ttu-id="a4e63-133">Свойство</span><span class="sxs-lookup"><span data-stu-id="a4e63-133">Property</span></span>  | <span data-ttu-id="a4e63-134">Тип</span><span class="sxs-lookup"><span data-stu-id="a4e63-134">Type</span></span>   | <span data-ttu-id="a4e63-135">Описание</span><span class="sxs-lookup"><span data-stu-id="a4e63-135">Description</span></span>                                                                                                                                                                                               |
| :-------- | :----- | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="a4e63-136">name</span><span class="sxs-lookup"><span data-stu-id="a4e63-136">name</span></span>      | <span data-ttu-id="a4e63-137">String</span><span class="sxs-lookup"><span data-stu-id="a4e63-137">String</span></span> | <span data-ttu-id="a4e63-138">Имя группы.</span><span class="sxs-lookup"><span data-stu-id="a4e63-138">The group name.</span></span>                                                                                                                                                                                           |
| <span data-ttu-id="a4e63-139">changeKey</span><span class="sxs-lookup"><span data-stu-id="a4e63-139">changeKey</span></span> | <span data-ttu-id="a4e63-140">String</span><span class="sxs-lookup"><span data-stu-id="a4e63-140">String</span></span> | <span data-ttu-id="a4e63-p102">Указывает версию группы календарей. При каждом изменении группы календарей также меняется значение ChangeKey. Благодаря этому Exchange может применять изменения к правильной версии объекта. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a4e63-p102">Identifies the version of the calendar group. Every time the calendar group is changed, ChangeKey changes as well. This allows Exchange to apply changes to the correct version of the object. Read-only.</span></span> |
| <span data-ttu-id="a4e63-145">classId</span><span class="sxs-lookup"><span data-stu-id="a4e63-145">classId</span></span>   | <span data-ttu-id="a4e63-146">Guid</span><span class="sxs-lookup"><span data-stu-id="a4e63-146">Guid</span></span>   | <span data-ttu-id="a4e63-p103">Идентификатор класса. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a4e63-p103">The class identifier. Read-only.</span></span>                                                                                                                                                                          |
| <span data-ttu-id="a4e63-149">id</span><span class="sxs-lookup"><span data-stu-id="a4e63-149">id</span></span>        | <span data-ttu-id="a4e63-150">String</span><span class="sxs-lookup"><span data-stu-id="a4e63-150">String</span></span> | <span data-ttu-id="a4e63-p104">Уникальный идентификатор группы. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a4e63-p104">The group's unique identifier. Read-only.</span></span>                                                                                                                                                                 |

## <a name="relationships"></a><span data-ttu-id="a4e63-153">Связи</span><span class="sxs-lookup"><span data-stu-id="a4e63-153">Relationships</span></span>

| <span data-ttu-id="a4e63-154">Связь</span><span class="sxs-lookup"><span data-stu-id="a4e63-154">Relationship</span></span> | <span data-ttu-id="a4e63-155">Тип</span><span class="sxs-lookup"><span data-stu-id="a4e63-155">Type</span></span>                               | <span data-ttu-id="a4e63-156">Описание</span><span class="sxs-lookup"><span data-stu-id="a4e63-156">Description</span></span>                                                                    |
| :----------- | :--------------------------------- | :----------------------------------------------------------------------------- |
| <span data-ttu-id="a4e63-157">calendars</span><span class="sxs-lookup"><span data-stu-id="a4e63-157">calendars</span></span>    | <span data-ttu-id="a4e63-158">Коллекция [Calendar](calendar.md)</span><span class="sxs-lookup"><span data-stu-id="a4e63-158">[Calendar](calendar.md) collection</span></span> | <span data-ttu-id="a4e63-p105">Календари в группе календарей. Свойство навигации. Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="a4e63-p105">The calendars in the calendar group. Navigation property. Read-only. Nullable.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="a4e63-163">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a4e63-163">JSON representation</span></span>

<span data-ttu-id="a4e63-164">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a4e63-164">Here is a JSON representation of the resource</span></span>

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

---
title: Тип ресурса calendarGroup
description: Группа пользователей календарей.
author: angelgolfer-ms
localization_priority: Normal
ms.openlocfilehash: 4d141b63b840daa7730d17f9dcfc2e527c1ed66b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27810327"
---
# <a name="calendargroup-resource-type"></a><span data-ttu-id="db9aa-103">Тип ресурса calendarGroup</span><span class="sxs-lookup"><span data-stu-id="db9aa-103">calendarGroup resource type</span></span>

> <span data-ttu-id="db9aa-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="db9aa-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="db9aa-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="db9aa-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="db9aa-106">Группа пользователей календарей.</span><span class="sxs-lookup"><span data-stu-id="db9aa-106">A group of user calendars.</span></span>

## <a name="methods"></a><span data-ttu-id="db9aa-107">Методы</span><span class="sxs-lookup"><span data-stu-id="db9aa-107">Methods</span></span>

| <span data-ttu-id="db9aa-108">Метод</span><span class="sxs-lookup"><span data-stu-id="db9aa-108">Method</span></span>                                                      | <span data-ttu-id="db9aa-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="db9aa-109">Return Type</span></span>                        | <span data-ttu-id="db9aa-110">Описание</span><span class="sxs-lookup"><span data-stu-id="db9aa-110">Description</span></span>                                                   |
| :---------------------------------------------------------- | :--------------------------------- | :------------------------------------------------------------ |
| [<span data-ttu-id="db9aa-111">Список групп календарей</span><span class="sxs-lookup"><span data-stu-id="db9aa-111">List calendar groups</span></span>](../api/user-list-calendargroups.md)  | <span data-ttu-id="db9aa-112">Коллекция объектов [Calendar](calendar.md)</span><span class="sxs-lookup"><span data-stu-id="db9aa-112">[Calendar](calendar.md) collection</span></span> | <span data-ttu-id="db9aa-113">Получение групп календарей пользователя.</span><span class="sxs-lookup"><span data-stu-id="db9aa-113">Get the user's calendar groups.</span></span>                               |
| [<span data-ttu-id="db9aa-114">Создание группы календарей</span><span class="sxs-lookup"><span data-stu-id="db9aa-114">Create calendar group</span></span>](../api/user-post-calendargroups.md) | [<span data-ttu-id="db9aa-115">Calendar</span><span class="sxs-lookup"><span data-stu-id="db9aa-115">Calendar</span></span>](calendar.md)            | <span data-ttu-id="db9aa-116">Создание группы календарей.</span><span class="sxs-lookup"><span data-stu-id="db9aa-116">Create a new calendar group.</span></span>                                  |
| [<span data-ttu-id="db9aa-117">Получение группы календарей</span><span class="sxs-lookup"><span data-stu-id="db9aa-117">Get calendar group</span></span>](../api/calendargroup-get.md)           | [<span data-ttu-id="db9aa-118">calendarGroup</span><span class="sxs-lookup"><span data-stu-id="db9aa-118">calendarGroup</span></span>](calendargroup.md)  | <span data-ttu-id="db9aa-119">Чтение свойств и связей, принадлежащих объекту группы календарей.</span><span class="sxs-lookup"><span data-stu-id="db9aa-119">Read properties and relationships of a calendar group object.</span></span> |
| [<span data-ttu-id="db9aa-120">Обновление</span><span class="sxs-lookup"><span data-stu-id="db9aa-120">Update</span></span>](../api/calendargroup-update.md)                    | [<span data-ttu-id="db9aa-121">calendarGroup</span><span class="sxs-lookup"><span data-stu-id="db9aa-121">calendarGroup</span></span>](calendargroup.md)  | <span data-ttu-id="db9aa-122">Обновление объекта calendarGroup.</span><span class="sxs-lookup"><span data-stu-id="db9aa-122">Update calendarGroup object.</span></span>                                  |
| [<span data-ttu-id="db9aa-123">Удаление</span><span class="sxs-lookup"><span data-stu-id="db9aa-123">Delete</span></span>](../api/calendargroup-delete.md)                    | <span data-ttu-id="db9aa-124">Нет</span><span class="sxs-lookup"><span data-stu-id="db9aa-124">None</span></span>                               | <span data-ttu-id="db9aa-125">Удаление объекта calendarGroup.</span><span class="sxs-lookup"><span data-stu-id="db9aa-125">Delete calendarGroup object.</span></span>                                  |
| [<span data-ttu-id="db9aa-126">Список календарей</span><span class="sxs-lookup"><span data-stu-id="db9aa-126">List calendars</span></span>](../api/calendargroup-list-calendars.md)    | <span data-ttu-id="db9aa-127">Коллекция объектов [Calendar](calendar.md)</span><span class="sxs-lookup"><span data-stu-id="db9aa-127">[Calendar](calendar.md) collection</span></span> | <span data-ttu-id="db9aa-128">Список календарей в группе календарей.</span><span class="sxs-lookup"><span data-stu-id="db9aa-128">List calendars in a calendar group.</span></span>                           |
| [<span data-ttu-id="db9aa-129">Создание объекта Calendar</span><span class="sxs-lookup"><span data-stu-id="db9aa-129">Create Calendar</span></span>](../api/calendargroup-post-calendars.md)   | [<span data-ttu-id="db9aa-130">Calendar</span><span class="sxs-lookup"><span data-stu-id="db9aa-130">Calendar</span></span>](calendar.md)            | <span data-ttu-id="db9aa-131">Создание календаря в группе календарей.</span><span class="sxs-lookup"><span data-stu-id="db9aa-131">Create a new Calendar in a calendar group.</span></span>                    |

## <a name="properties"></a><span data-ttu-id="db9aa-132">Свойства</span><span class="sxs-lookup"><span data-stu-id="db9aa-132">Properties</span></span>

| <span data-ttu-id="db9aa-133">Свойство</span><span class="sxs-lookup"><span data-stu-id="db9aa-133">Property</span></span>  | <span data-ttu-id="db9aa-134">Тип</span><span class="sxs-lookup"><span data-stu-id="db9aa-134">Type</span></span>   | <span data-ttu-id="db9aa-135">Описание</span><span class="sxs-lookup"><span data-stu-id="db9aa-135">Description</span></span>                                                                                                                                                                                               |
| :-------- | :----- | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="db9aa-136">name</span><span class="sxs-lookup"><span data-stu-id="db9aa-136">name</span></span>      | <span data-ttu-id="db9aa-137">String</span><span class="sxs-lookup"><span data-stu-id="db9aa-137">String</span></span> | <span data-ttu-id="db9aa-138">Имя группы.</span><span class="sxs-lookup"><span data-stu-id="db9aa-138">The group name.</span></span>                                                                                                                                                                                           |
| <span data-ttu-id="db9aa-139">changeKey</span><span class="sxs-lookup"><span data-stu-id="db9aa-139">changeKey</span></span> | <span data-ttu-id="db9aa-140">Строка</span><span class="sxs-lookup"><span data-stu-id="db9aa-140">String</span></span> | <span data-ttu-id="db9aa-p102">Указывает версию группы календарей. При каждом изменении группы календарей также меняется значение ChangeKey. Благодаря этому Exchange может применять изменения к правильной версии объекта. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="db9aa-p102">Identifies the version of the calendar group. Every time the calendar group is changed, ChangeKey changes as well. This allows Exchange to apply changes to the correct version of the object. Read-only.</span></span> |
| <span data-ttu-id="db9aa-145">classId</span><span class="sxs-lookup"><span data-stu-id="db9aa-145">classId</span></span>   | <span data-ttu-id="db9aa-146">Guid</span><span class="sxs-lookup"><span data-stu-id="db9aa-146">Guid</span></span>   | <span data-ttu-id="db9aa-p103">Идентификатор класса. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="db9aa-p103">The class identifier. Read-only.</span></span>                                                                                                                                                                          |
| <span data-ttu-id="db9aa-149">id</span><span class="sxs-lookup"><span data-stu-id="db9aa-149">id</span></span>        | <span data-ttu-id="db9aa-150">Строка</span><span class="sxs-lookup"><span data-stu-id="db9aa-150">String</span></span> | <span data-ttu-id="db9aa-p104">Уникальный идентификатор группы. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="db9aa-p104">The group's unique identifier. Read-only.</span></span>                                                                                                                                                                 |

## <a name="relationships"></a><span data-ttu-id="db9aa-153">Связи</span><span class="sxs-lookup"><span data-stu-id="db9aa-153">Relationships</span></span>

| <span data-ttu-id="db9aa-154">Связь</span><span class="sxs-lookup"><span data-stu-id="db9aa-154">Relationship</span></span> | <span data-ttu-id="db9aa-155">Тип</span><span class="sxs-lookup"><span data-stu-id="db9aa-155">Type</span></span>                               | <span data-ttu-id="db9aa-156">Описание</span><span class="sxs-lookup"><span data-stu-id="db9aa-156">Description</span></span>                                                                    |
| :----------- | :--------------------------------- | :----------------------------------------------------------------------------- |
| <span data-ttu-id="db9aa-157">calendars</span><span class="sxs-lookup"><span data-stu-id="db9aa-157">calendars</span></span>    | <span data-ttu-id="db9aa-158">Коллекция [Calendar](calendar.md)</span><span class="sxs-lookup"><span data-stu-id="db9aa-158">[Calendar](calendar.md) collection</span></span> | <span data-ttu-id="db9aa-p105">Календари в группе календарей. Свойство навигации. Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="db9aa-p105">The calendars in the calendar group. Navigation property. Read-only. Nullable.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="db9aa-163">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="db9aa-163">JSON representation</span></span>

<span data-ttu-id="db9aa-164">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="db9aa-164">Here is a JSON representation of the resource</span></span>

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

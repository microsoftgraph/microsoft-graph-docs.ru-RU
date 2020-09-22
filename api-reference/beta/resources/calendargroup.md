---
title: Тип ресурса calendarGroup
description: Группа пользовательских календарей.
author: harini84
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 89a0a8176936654e287399c51c45e9ae55f46f23
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48071621"
---
# <a name="calendargroup-resource-type"></a><span data-ttu-id="2c973-103">Тип ресурса calendarGroup</span><span class="sxs-lookup"><span data-stu-id="2c973-103">calendarGroup resource type</span></span>

<span data-ttu-id="2c973-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2c973-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2c973-105">Группа пользовательских календарей.</span><span class="sxs-lookup"><span data-stu-id="2c973-105">A group of user calendars.</span></span>

## <a name="methods"></a><span data-ttu-id="2c973-106">Методы</span><span class="sxs-lookup"><span data-stu-id="2c973-106">Methods</span></span>

| <span data-ttu-id="2c973-107">Метод</span><span class="sxs-lookup"><span data-stu-id="2c973-107">Method</span></span>                                                      | <span data-ttu-id="2c973-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="2c973-108">Return Type</span></span>                        | <span data-ttu-id="2c973-109">Описание</span><span class="sxs-lookup"><span data-stu-id="2c973-109">Description</span></span>                                                   |
| :---------------------------------------------------------- | :--------------------------------- | :------------------------------------------------------------ |
| [<span data-ttu-id="2c973-110">Список групп календарей</span><span class="sxs-lookup"><span data-stu-id="2c973-110">List calendar groups</span></span>](../api/user-list-calendargroups.md)  | <span data-ttu-id="2c973-111">Коллекция объектов [Calendar](calendar.md)</span><span class="sxs-lookup"><span data-stu-id="2c973-111">[Calendar](calendar.md) collection</span></span> | <span data-ttu-id="2c973-112">Получение групп календарей пользователя.</span><span class="sxs-lookup"><span data-stu-id="2c973-112">Get the user's calendar groups.</span></span>                               |
| [<span data-ttu-id="2c973-113">Создание группы календарей</span><span class="sxs-lookup"><span data-stu-id="2c973-113">Create calendar group</span></span>](../api/user-post-calendargroups.md) | [<span data-ttu-id="2c973-114">Calendar</span><span class="sxs-lookup"><span data-stu-id="2c973-114">Calendar</span></span>](calendar.md)            | <span data-ttu-id="2c973-115">Создание группы календарей.</span><span class="sxs-lookup"><span data-stu-id="2c973-115">Create a new calendar group.</span></span>                                  |
| [<span data-ttu-id="2c973-116">Получение группы календарей</span><span class="sxs-lookup"><span data-stu-id="2c973-116">Get calendar group</span></span>](../api/calendargroup-get.md)           | [<span data-ttu-id="2c973-117">calendarGroup</span><span class="sxs-lookup"><span data-stu-id="2c973-117">calendarGroup</span></span>](calendargroup.md)  | <span data-ttu-id="2c973-118">Чтение свойств и связей, принадлежащих объекту группы календарей.</span><span class="sxs-lookup"><span data-stu-id="2c973-118">Read properties and relationships of a calendar group object.</span></span> |
| [<span data-ttu-id="2c973-119">Обновление</span><span class="sxs-lookup"><span data-stu-id="2c973-119">Update</span></span>](../api/calendargroup-update.md)                    | [<span data-ttu-id="2c973-120">calendarGroup</span><span class="sxs-lookup"><span data-stu-id="2c973-120">calendarGroup</span></span>](calendargroup.md)  | <span data-ttu-id="2c973-121">Обновление объекта calendarGroup.</span><span class="sxs-lookup"><span data-stu-id="2c973-121">Update calendarGroup object.</span></span>                                  |
| [<span data-ttu-id="2c973-122">Удаление</span><span class="sxs-lookup"><span data-stu-id="2c973-122">Delete</span></span>](../api/calendargroup-delete.md)                    | <span data-ttu-id="2c973-123">Нет</span><span class="sxs-lookup"><span data-stu-id="2c973-123">None</span></span>                               | <span data-ttu-id="2c973-124">Удаление объекта calendarGroup.</span><span class="sxs-lookup"><span data-stu-id="2c973-124">Delete calendarGroup object.</span></span>                                  |
| [<span data-ttu-id="2c973-125">Список календарей</span><span class="sxs-lookup"><span data-stu-id="2c973-125">List calendars</span></span>](../api/calendargroup-list-calendars.md)    | <span data-ttu-id="2c973-126">Коллекция [Calendar](calendar.md)</span><span class="sxs-lookup"><span data-stu-id="2c973-126">[Calendar](calendar.md) collection</span></span> | <span data-ttu-id="2c973-127">Список календарей в группе календарей.</span><span class="sxs-lookup"><span data-stu-id="2c973-127">List calendars in a calendar group.</span></span>                           |
| [<span data-ttu-id="2c973-128">Создание объекта Calendar</span><span class="sxs-lookup"><span data-stu-id="2c973-128">Create Calendar</span></span>](../api/calendargroup-post-calendars.md)   | [<span data-ttu-id="2c973-129">Calendar</span><span class="sxs-lookup"><span data-stu-id="2c973-129">Calendar</span></span>](calendar.md)            | <span data-ttu-id="2c973-130">Создание календаря в группе календарей.</span><span class="sxs-lookup"><span data-stu-id="2c973-130">Create a new Calendar in a calendar group.</span></span>                    |

## <a name="properties"></a><span data-ttu-id="2c973-131">Свойства</span><span class="sxs-lookup"><span data-stu-id="2c973-131">Properties</span></span>

| <span data-ttu-id="2c973-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="2c973-132">Property</span></span>  | <span data-ttu-id="2c973-133">Тип</span><span class="sxs-lookup"><span data-stu-id="2c973-133">Type</span></span>   | <span data-ttu-id="2c973-134">Описание</span><span class="sxs-lookup"><span data-stu-id="2c973-134">Description</span></span>                                                                                                                                                                                               |
| :-------- | :----- | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="2c973-135">name</span><span class="sxs-lookup"><span data-stu-id="2c973-135">name</span></span>      | <span data-ttu-id="2c973-136">String</span><span class="sxs-lookup"><span data-stu-id="2c973-136">String</span></span> | <span data-ttu-id="2c973-137">Имя группы.</span><span class="sxs-lookup"><span data-stu-id="2c973-137">The group name.</span></span>                                                                                                                                                                                           |
| <span data-ttu-id="2c973-138">changeKey</span><span class="sxs-lookup"><span data-stu-id="2c973-138">changeKey</span></span> | <span data-ttu-id="2c973-139">String</span><span class="sxs-lookup"><span data-stu-id="2c973-139">String</span></span> | <span data-ttu-id="2c973-p101">Указывает версию группы календарей. При каждом изменении группы календарей также меняется значение ChangeKey. Благодаря этому Exchange может применять изменения к правильной версии объекта. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2c973-p101">Identifies the version of the calendar group. Every time the calendar group is changed, ChangeKey changes as well. This allows Exchange to apply changes to the correct version of the object. Read-only.</span></span> |
| <span data-ttu-id="2c973-144">classId</span><span class="sxs-lookup"><span data-stu-id="2c973-144">classId</span></span>   | <span data-ttu-id="2c973-145">Guid</span><span class="sxs-lookup"><span data-stu-id="2c973-145">Guid</span></span>   | <span data-ttu-id="2c973-p102">Идентификатор класса. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2c973-p102">The class identifier. Read-only.</span></span>                                                                                                                                                                          |
| <span data-ttu-id="2c973-148">id</span><span class="sxs-lookup"><span data-stu-id="2c973-148">id</span></span>        | <span data-ttu-id="2c973-149">Строка</span><span class="sxs-lookup"><span data-stu-id="2c973-149">String</span></span> | <span data-ttu-id="2c973-p103">Уникальный идентификатор группы. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2c973-p103">The group's unique identifier. Read-only.</span></span>                                                                                                                                                                 |

## <a name="relationships"></a><span data-ttu-id="2c973-152">Отношения</span><span class="sxs-lookup"><span data-stu-id="2c973-152">Relationships</span></span>

| <span data-ttu-id="2c973-153">Связь</span><span class="sxs-lookup"><span data-stu-id="2c973-153">Relationship</span></span> | <span data-ttu-id="2c973-154">Тип</span><span class="sxs-lookup"><span data-stu-id="2c973-154">Type</span></span>                               | <span data-ttu-id="2c973-155">Описание</span><span class="sxs-lookup"><span data-stu-id="2c973-155">Description</span></span>                                                                    |
| :----------- | :--------------------------------- | :----------------------------------------------------------------------------- |
| <span data-ttu-id="2c973-156">calendars</span><span class="sxs-lookup"><span data-stu-id="2c973-156">calendars</span></span>    | <span data-ttu-id="2c973-157">Коллекция [Calendar](calendar.md)</span><span class="sxs-lookup"><span data-stu-id="2c973-157">[Calendar](calendar.md) collection</span></span> | <span data-ttu-id="2c973-p104">Календари в группе календарей. Свойство навигации. Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="2c973-p104">The calendars in the calendar group. Navigation property. Read-only. Nullable.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="2c973-162">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2c973-162">JSON representation</span></span>

<span data-ttu-id="2c973-163">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2c973-163">Here is a JSON representation of the resource</span></span>

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



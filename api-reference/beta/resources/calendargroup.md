---
title: Тип ресурса calendarGroup
description: Группа пользовательских календарей.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 175b3b8372214851ef62cf0740779b19fd2d4ce1
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507833"
---
# <a name="calendargroup-resource-type"></a><span data-ttu-id="57f33-103">Тип ресурса calendarGroup</span><span class="sxs-lookup"><span data-stu-id="57f33-103">calendarGroup resource type</span></span>

<span data-ttu-id="57f33-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="57f33-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="57f33-105">Группа пользовательских календарей.</span><span class="sxs-lookup"><span data-stu-id="57f33-105">A group of user calendars.</span></span>

## <a name="methods"></a><span data-ttu-id="57f33-106">Методы</span><span class="sxs-lookup"><span data-stu-id="57f33-106">Methods</span></span>

| <span data-ttu-id="57f33-107">Метод</span><span class="sxs-lookup"><span data-stu-id="57f33-107">Method</span></span>                                                      | <span data-ttu-id="57f33-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="57f33-108">Return Type</span></span>                        | <span data-ttu-id="57f33-109">Описание</span><span class="sxs-lookup"><span data-stu-id="57f33-109">Description</span></span>                                                   |
| :---------------------------------------------------------- | :--------------------------------- | :------------------------------------------------------------ |
| [<span data-ttu-id="57f33-110">Список групп календарей</span><span class="sxs-lookup"><span data-stu-id="57f33-110">List calendar groups</span></span>](../api/user-list-calendargroups.md)  | <span data-ttu-id="57f33-111">Коллекция [Calendar](calendar.md)</span><span class="sxs-lookup"><span data-stu-id="57f33-111">[Calendar](calendar.md) collection</span></span> | <span data-ttu-id="57f33-112">Получение групп календарей пользователя.</span><span class="sxs-lookup"><span data-stu-id="57f33-112">Get the user's calendar groups.</span></span>                               |
| [<span data-ttu-id="57f33-113">Создание группы календарей</span><span class="sxs-lookup"><span data-stu-id="57f33-113">Create calendar group</span></span>](../api/user-post-calendargroups.md) | [<span data-ttu-id="57f33-114">Календарь</span><span class="sxs-lookup"><span data-stu-id="57f33-114">Calendar</span></span>](calendar.md)            | <span data-ttu-id="57f33-115">Создание группы календарей.</span><span class="sxs-lookup"><span data-stu-id="57f33-115">Create a new calendar group.</span></span>                                  |
| [<span data-ttu-id="57f33-116">Получение группы календарей</span><span class="sxs-lookup"><span data-stu-id="57f33-116">Get calendar group</span></span>](../api/calendargroup-get.md)           | [<span data-ttu-id="57f33-117">calendarGroup</span><span class="sxs-lookup"><span data-stu-id="57f33-117">calendarGroup</span></span>](calendargroup.md)  | <span data-ttu-id="57f33-118">Чтение свойств и связей, принадлежащих объекту группы календарей.</span><span class="sxs-lookup"><span data-stu-id="57f33-118">Read properties and relationships of a calendar group object.</span></span> |
| [<span data-ttu-id="57f33-119">Обновление</span><span class="sxs-lookup"><span data-stu-id="57f33-119">Update</span></span>](../api/calendargroup-update.md)                    | [<span data-ttu-id="57f33-120">calendarGroup</span><span class="sxs-lookup"><span data-stu-id="57f33-120">calendarGroup</span></span>](calendargroup.md)  | <span data-ttu-id="57f33-121">Обновление объекта calendarGroup.</span><span class="sxs-lookup"><span data-stu-id="57f33-121">Update calendarGroup object.</span></span>                                  |
| <span data-ttu-id="57f33-122">[удаление](../api/calendargroup-delete.md);</span><span class="sxs-lookup"><span data-stu-id="57f33-122">[Delete](../api/calendargroup-delete.md)</span></span>                    | <span data-ttu-id="57f33-123">Нет</span><span class="sxs-lookup"><span data-stu-id="57f33-123">None</span></span>                               | <span data-ttu-id="57f33-124">Удаление объекта calendarGroup.</span><span class="sxs-lookup"><span data-stu-id="57f33-124">Delete calendarGroup object.</span></span>                                  |
| [<span data-ttu-id="57f33-125">Список календарей</span><span class="sxs-lookup"><span data-stu-id="57f33-125">List calendars</span></span>](../api/calendargroup-list-calendars.md)    | <span data-ttu-id="57f33-126">Коллекция объектов [Calendar](calendar.md)</span><span class="sxs-lookup"><span data-stu-id="57f33-126">[Calendar](calendar.md) collection</span></span> | <span data-ttu-id="57f33-127">Список календарей в группе календарей.</span><span class="sxs-lookup"><span data-stu-id="57f33-127">List calendars in a calendar group.</span></span>                           |
| [<span data-ttu-id="57f33-128">Создание объекта Calendar</span><span class="sxs-lookup"><span data-stu-id="57f33-128">Create Calendar</span></span>](../api/calendargroup-post-calendars.md)   | [<span data-ttu-id="57f33-129">Calendar</span><span class="sxs-lookup"><span data-stu-id="57f33-129">Calendar</span></span>](calendar.md)            | <span data-ttu-id="57f33-130">Создание календаря в группе календарей.</span><span class="sxs-lookup"><span data-stu-id="57f33-130">Create a new Calendar in a calendar group.</span></span>                    |

## <a name="properties"></a><span data-ttu-id="57f33-131">Свойства</span><span class="sxs-lookup"><span data-stu-id="57f33-131">Properties</span></span>

| <span data-ttu-id="57f33-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="57f33-132">Property</span></span>  | <span data-ttu-id="57f33-133">Тип</span><span class="sxs-lookup"><span data-stu-id="57f33-133">Type</span></span>   | <span data-ttu-id="57f33-134">Описание</span><span class="sxs-lookup"><span data-stu-id="57f33-134">Description</span></span>                                                                                                                                                                                               |
| :-------- | :----- | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="57f33-135">name</span><span class="sxs-lookup"><span data-stu-id="57f33-135">name</span></span>      | <span data-ttu-id="57f33-136">String</span><span class="sxs-lookup"><span data-stu-id="57f33-136">String</span></span> | <span data-ttu-id="57f33-137">Имя группы.</span><span class="sxs-lookup"><span data-stu-id="57f33-137">The group name.</span></span>                                                                                                                                                                                           |
| <span data-ttu-id="57f33-138">changeKey</span><span class="sxs-lookup"><span data-stu-id="57f33-138">changeKey</span></span> | <span data-ttu-id="57f33-139">String</span><span class="sxs-lookup"><span data-stu-id="57f33-139">String</span></span> | <span data-ttu-id="57f33-p101">Указывает версию группы календарей. При каждом изменении группы календарей также меняется значение ChangeKey. Благодаря этому Exchange может применять изменения к правильной версии объекта. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="57f33-p101">Identifies the version of the calendar group. Every time the calendar group is changed, ChangeKey changes as well. This allows Exchange to apply changes to the correct version of the object. Read-only.</span></span> |
| <span data-ttu-id="57f33-144">classId</span><span class="sxs-lookup"><span data-stu-id="57f33-144">classId</span></span>   | <span data-ttu-id="57f33-145">Guid</span><span class="sxs-lookup"><span data-stu-id="57f33-145">Guid</span></span>   | <span data-ttu-id="57f33-p102">Идентификатор класса. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="57f33-p102">The class identifier. Read-only.</span></span>                                                                                                                                                                          |
| <span data-ttu-id="57f33-148">id</span><span class="sxs-lookup"><span data-stu-id="57f33-148">id</span></span>        | <span data-ttu-id="57f33-149">Строка</span><span class="sxs-lookup"><span data-stu-id="57f33-149">String</span></span> | <span data-ttu-id="57f33-p103">Уникальный идентификатор группы. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="57f33-p103">The group's unique identifier. Read-only.</span></span>                                                                                                                                                                 |

## <a name="relationships"></a><span data-ttu-id="57f33-152">Связи</span><span class="sxs-lookup"><span data-stu-id="57f33-152">Relationships</span></span>

| <span data-ttu-id="57f33-153">Связь</span><span class="sxs-lookup"><span data-stu-id="57f33-153">Relationship</span></span> | <span data-ttu-id="57f33-154">Тип</span><span class="sxs-lookup"><span data-stu-id="57f33-154">Type</span></span>                               | <span data-ttu-id="57f33-155">Описание</span><span class="sxs-lookup"><span data-stu-id="57f33-155">Description</span></span>                                                                    |
| :----------- | :--------------------------------- | :----------------------------------------------------------------------------- |
| <span data-ttu-id="57f33-156">calendars</span><span class="sxs-lookup"><span data-stu-id="57f33-156">calendars</span></span>    | <span data-ttu-id="57f33-157">Коллекция [Calendar](calendar.md)</span><span class="sxs-lookup"><span data-stu-id="57f33-157">[Calendar](calendar.md) collection</span></span> | <span data-ttu-id="57f33-p104">Календари в группе календарей. Свойство навигации. Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="57f33-p104">The calendars in the calendar group. Navigation property. Read-only. Nullable.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="57f33-162">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="57f33-162">JSON representation</span></span>

<span data-ttu-id="57f33-163">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="57f33-163">Here is a JSON representation of the resource</span></span>

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

---
title: Тип ресурса calendarGroup
description: Группа пользователей календарей.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: cea68da3a91396972c4e237d1fdaf0e16d65e3a3
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/30/2019
ms.locfileid: "29643715"
---
# <a name="calendargroup-resource-type"></a><span data-ttu-id="e9e31-103">Тип ресурса calendarGroup</span><span class="sxs-lookup"><span data-stu-id="e9e31-103">calendarGroup resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e9e31-104">Группа пользователей календарей.</span><span class="sxs-lookup"><span data-stu-id="e9e31-104">A group of user calendars.</span></span>

## <a name="methods"></a><span data-ttu-id="e9e31-105">Методы</span><span class="sxs-lookup"><span data-stu-id="e9e31-105">Methods</span></span>

| <span data-ttu-id="e9e31-106">Метод</span><span class="sxs-lookup"><span data-stu-id="e9e31-106">Method</span></span>                                                      | <span data-ttu-id="e9e31-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="e9e31-107">Return Type</span></span>                        | <span data-ttu-id="e9e31-108">Описание</span><span class="sxs-lookup"><span data-stu-id="e9e31-108">Description</span></span>                                                   |
| :---------------------------------------------------------- | :--------------------------------- | :------------------------------------------------------------ |
| [<span data-ttu-id="e9e31-109">Список групп календарей</span><span class="sxs-lookup"><span data-stu-id="e9e31-109">List calendar groups</span></span>](../api/user-list-calendargroups.md)  | <span data-ttu-id="e9e31-110">Коллекция объектов [Calendar](calendar.md)</span><span class="sxs-lookup"><span data-stu-id="e9e31-110">[Calendar](calendar.md) collection</span></span> | <span data-ttu-id="e9e31-111">Получение групп календарей пользователя.</span><span class="sxs-lookup"><span data-stu-id="e9e31-111">Get the user's calendar groups.</span></span>                               |
| [<span data-ttu-id="e9e31-112">Создание группы календарей</span><span class="sxs-lookup"><span data-stu-id="e9e31-112">Create calendar group</span></span>](../api/user-post-calendargroups.md) | [<span data-ttu-id="e9e31-113">Calendar</span><span class="sxs-lookup"><span data-stu-id="e9e31-113">Calendar</span></span>](calendar.md)            | <span data-ttu-id="e9e31-114">Создание группы календарей.</span><span class="sxs-lookup"><span data-stu-id="e9e31-114">Create a new calendar group.</span></span>                                  |
| [<span data-ttu-id="e9e31-115">Получение группы календарей</span><span class="sxs-lookup"><span data-stu-id="e9e31-115">Get calendar group</span></span>](../api/calendargroup-get.md)           | [<span data-ttu-id="e9e31-116">calendarGroup</span><span class="sxs-lookup"><span data-stu-id="e9e31-116">calendarGroup</span></span>](calendargroup.md)  | <span data-ttu-id="e9e31-117">Чтение свойств и связей, принадлежащих объекту группы календарей.</span><span class="sxs-lookup"><span data-stu-id="e9e31-117">Read properties and relationships of a calendar group object.</span></span> |
| [<span data-ttu-id="e9e31-118">Обновление</span><span class="sxs-lookup"><span data-stu-id="e9e31-118">Update</span></span>](../api/calendargroup-update.md)                    | [<span data-ttu-id="e9e31-119">calendarGroup</span><span class="sxs-lookup"><span data-stu-id="e9e31-119">calendarGroup</span></span>](calendargroup.md)  | <span data-ttu-id="e9e31-120">Обновление объекта calendarGroup.</span><span class="sxs-lookup"><span data-stu-id="e9e31-120">Update calendarGroup object.</span></span>                                  |
| [<span data-ttu-id="e9e31-121">Удаление</span><span class="sxs-lookup"><span data-stu-id="e9e31-121">Delete</span></span>](../api/calendargroup-delete.md)                    | <span data-ttu-id="e9e31-122">Нет</span><span class="sxs-lookup"><span data-stu-id="e9e31-122">None</span></span>                               | <span data-ttu-id="e9e31-123">Удаление объекта calendarGroup.</span><span class="sxs-lookup"><span data-stu-id="e9e31-123">Delete calendarGroup object.</span></span>                                  |
| [<span data-ttu-id="e9e31-124">Список календарей</span><span class="sxs-lookup"><span data-stu-id="e9e31-124">List calendars</span></span>](../api/calendargroup-list-calendars.md)    | <span data-ttu-id="e9e31-125">Коллекция объектов [Calendar](calendar.md)</span><span class="sxs-lookup"><span data-stu-id="e9e31-125">[Calendar](calendar.md) collection</span></span> | <span data-ttu-id="e9e31-126">Список календарей в группе календарей.</span><span class="sxs-lookup"><span data-stu-id="e9e31-126">List calendars in a calendar group.</span></span>                           |
| [<span data-ttu-id="e9e31-127">Создание объекта Calendar</span><span class="sxs-lookup"><span data-stu-id="e9e31-127">Create Calendar</span></span>](../api/calendargroup-post-calendars.md)   | [<span data-ttu-id="e9e31-128">Calendar</span><span class="sxs-lookup"><span data-stu-id="e9e31-128">Calendar</span></span>](calendar.md)            | <span data-ttu-id="e9e31-129">Создание календаря в группе календарей.</span><span class="sxs-lookup"><span data-stu-id="e9e31-129">Create a new Calendar in a calendar group.</span></span>                    |

## <a name="properties"></a><span data-ttu-id="e9e31-130">Свойства</span><span class="sxs-lookup"><span data-stu-id="e9e31-130">Properties</span></span>

| <span data-ttu-id="e9e31-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="e9e31-131">Property</span></span>  | <span data-ttu-id="e9e31-132">Тип</span><span class="sxs-lookup"><span data-stu-id="e9e31-132">Type</span></span>   | <span data-ttu-id="e9e31-133">Описание</span><span class="sxs-lookup"><span data-stu-id="e9e31-133">Description</span></span>                                                                                                                                                                                               |
| :-------- | :----- | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="e9e31-134">name</span><span class="sxs-lookup"><span data-stu-id="e9e31-134">name</span></span>      | <span data-ttu-id="e9e31-135">String</span><span class="sxs-lookup"><span data-stu-id="e9e31-135">String</span></span> | <span data-ttu-id="e9e31-136">Имя группы.</span><span class="sxs-lookup"><span data-stu-id="e9e31-136">The group name.</span></span>                                                                                                                                                                                           |
| <span data-ttu-id="e9e31-137">changeKey</span><span class="sxs-lookup"><span data-stu-id="e9e31-137">changeKey</span></span> | <span data-ttu-id="e9e31-138">String</span><span class="sxs-lookup"><span data-stu-id="e9e31-138">String</span></span> | <span data-ttu-id="e9e31-p101">Указывает версию группы календарей. При каждом изменении группы календарей также меняется значение ChangeKey. Благодаря этому Exchange может применять изменения к правильной версии объекта. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e9e31-p101">Identifies the version of the calendar group. Every time the calendar group is changed, ChangeKey changes as well. This allows Exchange to apply changes to the correct version of the object. Read-only.</span></span> |
| <span data-ttu-id="e9e31-143">classId</span><span class="sxs-lookup"><span data-stu-id="e9e31-143">classId</span></span>   | <span data-ttu-id="e9e31-144">Guid</span><span class="sxs-lookup"><span data-stu-id="e9e31-144">Guid</span></span>   | <span data-ttu-id="e9e31-p102">Идентификатор класса. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e9e31-p102">The class identifier. Read-only.</span></span>                                                                                                                                                                          |
| <span data-ttu-id="e9e31-147">id</span><span class="sxs-lookup"><span data-stu-id="e9e31-147">id</span></span>        | <span data-ttu-id="e9e31-148">String</span><span class="sxs-lookup"><span data-stu-id="e9e31-148">String</span></span> | <span data-ttu-id="e9e31-p103">Уникальный идентификатор группы. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e9e31-p103">The group's unique identifier. Read-only.</span></span>                                                                                                                                                                 |

## <a name="relationships"></a><span data-ttu-id="e9e31-151">Связи</span><span class="sxs-lookup"><span data-stu-id="e9e31-151">Relationships</span></span>

| <span data-ttu-id="e9e31-152">Связь</span><span class="sxs-lookup"><span data-stu-id="e9e31-152">Relationship</span></span> | <span data-ttu-id="e9e31-153">Тип</span><span class="sxs-lookup"><span data-stu-id="e9e31-153">Type</span></span>                               | <span data-ttu-id="e9e31-154">Описание</span><span class="sxs-lookup"><span data-stu-id="e9e31-154">Description</span></span>                                                                    |
| :----------- | :--------------------------------- | :----------------------------------------------------------------------------- |
| <span data-ttu-id="e9e31-155">calendars</span><span class="sxs-lookup"><span data-stu-id="e9e31-155">calendars</span></span>    | <span data-ttu-id="e9e31-156">Коллекция [Calendar](calendar.md)</span><span class="sxs-lookup"><span data-stu-id="e9e31-156">[Calendar](calendar.md) collection</span></span> | <span data-ttu-id="e9e31-p104">Календари в группе календарей. Свойство навигации. Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="e9e31-p104">The calendars in the calendar group. Navigation property. Read-only. Nullable.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="e9e31-161">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e9e31-161">JSON representation</span></span>

<span data-ttu-id="e9e31-162">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e9e31-162">Here is a JSON representation of the resource</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/calendargroup.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

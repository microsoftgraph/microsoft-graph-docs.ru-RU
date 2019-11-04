---
title: Тип ресурса Календарпермиссион
description: Разрешения пользователя, к которому открыт общий доступ к календарю.
localization_priority: Normal
author: sochowdh
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 5d19a1738d3369f2d910dd590062016acf3047ab
ms.sourcegitcommit: dd94c3a0f7663699825b6dbc119cdcef494cd130
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/04/2019
ms.locfileid: "37950453"
---
# <a name="calendarpermission-resource-type"></a><span data-ttu-id="71d63-103">Тип ресурса Календарпермиссион</span><span class="sxs-lookup"><span data-stu-id="71d63-103">calendarPermission resource type</span></span>

<span data-ttu-id="71d63-104">Разрешения пользователя, к которому открыт общий доступ к календарю.</span><span class="sxs-lookup"><span data-stu-id="71d63-104">The permissions of a user with whom the calendar is shared.</span></span> 

## <a name="methods"></a><span data-ttu-id="71d63-105">Методы</span><span class="sxs-lookup"><span data-stu-id="71d63-105">Methods</span></span>

| <span data-ttu-id="71d63-106">Метод</span><span class="sxs-lookup"><span data-stu-id="71d63-106">Method</span></span>       | <span data-ttu-id="71d63-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="71d63-107">Return Type</span></span> | <span data-ttu-id="71d63-108">Описание</span><span class="sxs-lookup"><span data-stu-id="71d63-108">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="71d63-109">Получение Календарпермиссион</span><span class="sxs-lookup"><span data-stu-id="71d63-109">Get calendarPermission</span></span>](../api/calendarpermission-get.md) | [<span data-ttu-id="71d63-110">календарпермиссион</span><span class="sxs-lookup"><span data-stu-id="71d63-110">calendarPermission</span></span>](calendarpermission.md) | <span data-ttu-id="71d63-111">Чтение свойств и связей объекта Календарпермиссион.</span><span class="sxs-lookup"><span data-stu-id="71d63-111">Read properties and relationships of calendarPermission object.</span></span> |
| [<span data-ttu-id="71d63-112">Update</span><span class="sxs-lookup"><span data-stu-id="71d63-112">Update</span></span>](../api/calendarpermission-update.md) | [<span data-ttu-id="71d63-113">календарпермиссион</span><span class="sxs-lookup"><span data-stu-id="71d63-113">calendarPermission</span></span>](calendarpermission.md) | <span data-ttu-id="71d63-114">Обновление объекта Календарпермиссион.</span><span class="sxs-lookup"><span data-stu-id="71d63-114">Update calendarPermission object.</span></span> |
| [<span data-ttu-id="71d63-115">Delete</span><span class="sxs-lookup"><span data-stu-id="71d63-115">Delete</span></span>](../api/calendarpermission-delete.md) | <span data-ttu-id="71d63-116">Нет.</span><span class="sxs-lookup"><span data-stu-id="71d63-116">None</span></span> | <span data-ttu-id="71d63-117">Удаление объекта Календарпермиссион.</span><span class="sxs-lookup"><span data-stu-id="71d63-117">Delete calendarPermission object.</span></span> |

## <a name="properties"></a><span data-ttu-id="71d63-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="71d63-118">Properties</span></span>

| <span data-ttu-id="71d63-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="71d63-119">Property</span></span>     | <span data-ttu-id="71d63-120">Тип</span><span class="sxs-lookup"><span data-stu-id="71d63-120">Type</span></span>        | <span data-ttu-id="71d63-121">Описание</span><span class="sxs-lookup"><span data-stu-id="71d63-121">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="71d63-122">алловедролес</span><span class="sxs-lookup"><span data-stu-id="71d63-122">allowedRoles</span></span>|<span data-ttu-id="71d63-123">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="71d63-123">string collection</span></span>| <span data-ttu-id="71d63-124">Список разрешенных для общего доступа уровней разрешений для календаря.</span><span class="sxs-lookup"><span data-stu-id="71d63-124">List of allowed sharing permission levels for the calendar.</span></span> <span data-ttu-id="71d63-125">Возможные значения: `none`, `freeBusyRead`, `limitedRead`, `read`, `write`, `delegateWithoutPrivateEventAccess`, `delegateWithPrivateEventAccess`, `custom`.</span><span class="sxs-lookup"><span data-stu-id="71d63-125">Possible values are: `none`, `freeBusyRead`, `limitedRead`, `read`, `write`, `delegateWithoutPrivateEventAccess`, `delegateWithPrivateEventAccess`, `custom`.</span></span>|
|<span data-ttu-id="71d63-126">emailAddress</span><span class="sxs-lookup"><span data-stu-id="71d63-126">emailAddress</span></span>|[<span data-ttu-id="71d63-127">emailAddress</span><span class="sxs-lookup"><span data-stu-id="71d63-127">emailAddress</span></span>](emailaddress.md)| <span data-ttu-id="71d63-128">Представляет общую папку, у которой есть доступ к календарю.</span><span class="sxs-lookup"><span data-stu-id="71d63-128">Represents a sharee who has access to the calendar.</span></span> <span data-ttu-id="71d63-129">Для общего доступа к общему ресурсу "Моя организация" свойство **Address** имеет значение null.</span><span class="sxs-lookup"><span data-stu-id="71d63-129">For the "My Organization" sharee, the **address** property is null.</span></span> |
|<span data-ttu-id="71d63-130">id</span><span class="sxs-lookup"><span data-stu-id="71d63-130">id</span></span>|<span data-ttu-id="71d63-131">String</span><span class="sxs-lookup"><span data-stu-id="71d63-131">String</span></span>| <span data-ttu-id="71d63-132">Уникальный идентификатор пользователя (общего доступа), с которым открыт общий доступ к календарю.</span><span class="sxs-lookup"><span data-stu-id="71d63-132">The unique identifier of the user (sharee) with whom the calendar has been shared.</span></span> <span data-ttu-id="71d63-133">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="71d63-133">Read-only.</span></span>|
|<span data-ttu-id="71d63-134">исинсидеорганизатион</span><span class="sxs-lookup"><span data-stu-id="71d63-134">isInsideOrganization</span></span>|<span data-ttu-id="71d63-135">Логический</span><span class="sxs-lookup"><span data-stu-id="71d63-135">Boolean</span></span>| <span data-ttu-id="71d63-136">Значение true, если пользователь в контексте (Share) находится в той же организации, что и владелец календаря.</span><span class="sxs-lookup"><span data-stu-id="71d63-136">True if the user in context (sharee) is inside the same organization as the calendar owner.</span></span>|
|<span data-ttu-id="71d63-137">"несъемный"</span><span class="sxs-lookup"><span data-stu-id="71d63-137">isRemovable</span></span>|<span data-ttu-id="71d63-138">Логический</span><span class="sxs-lookup"><span data-stu-id="71d63-138">Boolean</span></span>| <span data-ttu-id="71d63-139">`True`, если пользователь может быть удален из списка общих папок для указанного календаря, `false` в противном случае.</span><span class="sxs-lookup"><span data-stu-id="71d63-139">`True` if the user can be removed from the list of sharees for the specified calendar, `false` otherwise.</span></span> <span data-ttu-id="71d63-140">Пользователь "Моя организация" определяет разрешения, которые пользователи в организации имеют в указанном календаре.</span><span class="sxs-lookup"><span data-stu-id="71d63-140">The "My organization" user determines the permissions other people within your organization have to the given calendar.</span></span> <span data-ttu-id="71d63-141">Вы не можете удалить "Моя организация" как общий доступ к календарю.</span><span class="sxs-lookup"><span data-stu-id="71d63-141">You cannot remove "My organization" as a sharee to a calendar.</span></span>|
|<span data-ttu-id="71d63-142">role</span><span class="sxs-lookup"><span data-stu-id="71d63-142">role</span></span>|<span data-ttu-id="71d63-143">календарролетипе</span><span class="sxs-lookup"><span data-stu-id="71d63-143">calendarRoleType</span></span>| <span data-ttu-id="71d63-144">Текущий уровень разрешений общего календаря.</span><span class="sxs-lookup"><span data-stu-id="71d63-144">Current permission level of the calendar sharee.</span></span> <span data-ttu-id="71d63-145">Возможные значения: `none`, `freeBusyRead`, `limitedRead`, `read`, `write`, `delegateWithoutPrivateEventAccess`, `delegateWithPrivateEventAccess`, `custom`.</span><span class="sxs-lookup"><span data-stu-id="71d63-145">Possible values are: `none`, `freeBusyRead`, `limitedRead`, `read`, `write`, `delegateWithoutPrivateEventAccess`, `delegateWithPrivateEventAccess`, `custom`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="71d63-146">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="71d63-146">JSON representation</span></span>

<span data-ttu-id="71d63-147">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="71d63-147">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.calendarPermission",
  "keyProperty": "id"
}-->

```json
{
  "allowedRoles": ["string"],
  "emailAddress": {"@odata.type": "microsoft.graph.emailAddress"},
  "id": "String (identifier)",
  "isInsideOrganization": "boolean",
  "isRemovable": "boolean",
  "role": "string"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "calendarPermission resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
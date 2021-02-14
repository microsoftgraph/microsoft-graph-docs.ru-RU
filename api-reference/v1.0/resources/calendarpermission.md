---
title: Тип ресурса calendarPermission
description: Разрешения пользователя, которому совместно передается календарь.
localization_priority: Normal
author: sochowdh
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 8162220df0ebf6973f1b317c1e4c063dbc98de3e
ms.sourcegitcommit: 48fff935d56fe96e97577a80a3a0aa15c45419ba
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/10/2021
ms.locfileid: "50176705"
---
# <a name="calendarpermission-resource-type"></a><span data-ttu-id="8f3df-103">Тип ресурса calendarPermission</span><span class="sxs-lookup"><span data-stu-id="8f3df-103">calendarPermission resource type</span></span>

<span data-ttu-id="8f3df-104">Разрешения пользователя, которому был передан календарь или которому делегирован доступ в клиенте Outlook.</span><span class="sxs-lookup"><span data-stu-id="8f3df-104">The permissions of a user with whom the calendar has been shared or delegated in an Outlook client.</span></span>

<span data-ttu-id="8f3df-105">Получать, обновлять и удалять разрешения календаря можно только от имени владельца календаря.</span><span class="sxs-lookup"><span data-stu-id="8f3df-105">Get, update, and delete of calendar permissions is supported on behalf of only the calendar owner.</span></span>

<span data-ttu-id="8f3df-106">Получение разрешений календаря от имени пользователя или делегата возвращает пустую коллекцию разрешений календаря.</span><span class="sxs-lookup"><span data-stu-id="8f3df-106">Getting the calendar permissions of a calendar on behalf of a sharee or delegate returns an empty calendar permissions collection.</span></span>

<span data-ttu-id="8f3df-107">После того как для календаря настроены объекты [](../api/calendarpermission-update.md) sharee  или delegate, можно обновить только свойство роли, чтобы изменить разрешения sharee или delegate.</span><span class="sxs-lookup"><span data-stu-id="8f3df-107">Once a sharee or delegate has been set up for a calendar, you can [update](../api/calendarpermission-update.md) only the **role** property to change the permissions of a sharee or delegate.</span></span> <span data-ttu-id="8f3df-108">Вы не **можете обновить** **свойство allowedRoles,** **emailAddress,** **isInsideOrganization** или **isRemovable.**</span><span class="sxs-lookup"><span data-stu-id="8f3df-108">You cannot **update** the **allowedRoles**, **emailAddress**, **isInsideOrganization**, or **isRemovable** property.</span></span> <span data-ttu-id="8f3df-109">Чтобы изменить эти свойства, [](../api/calendarpermission-delete.md) необходимо удалить соответствующий объект **calendarPermission** и создать в клиенте Outlook другого представителя или представителя.</span><span class="sxs-lookup"><span data-stu-id="8f3df-109">To change these properties, you should [delete](../api/calendarpermission-delete.md) the corresponding **calendarPermission** object and create another sharee or delegate in an Outlook client.</span></span>

## <a name="methods"></a><span data-ttu-id="8f3df-110">Методы</span><span class="sxs-lookup"><span data-stu-id="8f3df-110">Methods</span></span>

| <span data-ttu-id="8f3df-111">Метод</span><span class="sxs-lookup"><span data-stu-id="8f3df-111">Method</span></span>       | <span data-ttu-id="8f3df-112">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="8f3df-112">Return Type</span></span> | <span data-ttu-id="8f3df-113">Описание</span><span class="sxs-lookup"><span data-stu-id="8f3df-113">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="8f3df-114">Get calendarPermission</span><span class="sxs-lookup"><span data-stu-id="8f3df-114">Get calendarPermission</span></span>](../api/calendarpermission-get.md) | [<span data-ttu-id="8f3df-115">calendarPermission</span><span class="sxs-lookup"><span data-stu-id="8f3df-115">calendarPermission</span></span>](calendarpermission.md) | <span data-ttu-id="8f3df-116">Чтение свойств и связей объекта calendarPermission.</span><span class="sxs-lookup"><span data-stu-id="8f3df-116">Read properties and relationships of calendarPermission object.</span></span> |
| [<span data-ttu-id="8f3df-117">Обновление</span><span class="sxs-lookup"><span data-stu-id="8f3df-117">Update</span></span>](../api/calendarpermission-update.md) | [<span data-ttu-id="8f3df-118">calendarPermission</span><span class="sxs-lookup"><span data-stu-id="8f3df-118">calendarPermission</span></span>](calendarpermission.md) | <span data-ttu-id="8f3df-119">Обновление объекта calendarPermission.</span><span class="sxs-lookup"><span data-stu-id="8f3df-119">Update calendarPermission object.</span></span> |
| <span data-ttu-id="8f3df-120">[удаление](../api/calendarpermission-delete.md);</span><span class="sxs-lookup"><span data-stu-id="8f3df-120">[Delete](../api/calendarpermission-delete.md)</span></span> | <span data-ttu-id="8f3df-121">Нет</span><span class="sxs-lookup"><span data-stu-id="8f3df-121">None</span></span> | <span data-ttu-id="8f3df-122">Удаление объекта calendarPermission.</span><span class="sxs-lookup"><span data-stu-id="8f3df-122">Delete calendarPermission object.</span></span> |

## <a name="properties"></a><span data-ttu-id="8f3df-123">Свойства</span><span class="sxs-lookup"><span data-stu-id="8f3df-123">Properties</span></span>

| <span data-ttu-id="8f3df-124">Свойство</span><span class="sxs-lookup"><span data-stu-id="8f3df-124">Property</span></span>     | <span data-ttu-id="8f3df-125">Тип</span><span class="sxs-lookup"><span data-stu-id="8f3df-125">Type</span></span>        | <span data-ttu-id="8f3df-126">Описание</span><span class="sxs-lookup"><span data-stu-id="8f3df-126">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="8f3df-127">allowedRoles</span><span class="sxs-lookup"><span data-stu-id="8f3df-127">allowedRoles</span></span>|<span data-ttu-id="8f3df-128">[Коллекция calendarRoleType](#calendarroletype-values)</span><span class="sxs-lookup"><span data-stu-id="8f3df-128">[calendarRoleType](#calendarroletype-values) collection</span></span>| <span data-ttu-id="8f3df-129">Список разрешенных уровней разрешений общего доступа или делегирование для календаря.</span><span class="sxs-lookup"><span data-stu-id="8f3df-129">List of allowed sharing or delegating permission levels for the calendar.</span></span> <span data-ttu-id="8f3df-130">Возможные значения: `none`, `freeBusyRead`, `limitedRead`, `read`, `write`, `delegateWithoutPrivateEventAccess`, `delegateWithPrivateEventAccess`, `custom`.</span><span class="sxs-lookup"><span data-stu-id="8f3df-130">Possible values are: `none`, `freeBusyRead`, `limitedRead`, `read`, `write`, `delegateWithoutPrivateEventAccess`, `delegateWithPrivateEventAccess`, `custom`.</span></span>|
|<span data-ttu-id="8f3df-131">emailAddress</span><span class="sxs-lookup"><span data-stu-id="8f3df-131">emailAddress</span></span>|[<span data-ttu-id="8f3df-132">emailAddress</span><span class="sxs-lookup"><span data-stu-id="8f3df-132">emailAddress</span></span>](emailaddress.md)| <span data-ttu-id="8f3df-133">Представляет делиться данными или делегатами, у которых есть доступ к календарю.</span><span class="sxs-lookup"><span data-stu-id="8f3df-133">Represents a sharee or delegate who has access to the calendar.</span></span> <span data-ttu-id="8f3df-134">Для обоймы "Моя организация" свойство **адреса** имеет null.</span><span class="sxs-lookup"><span data-stu-id="8f3df-134">For the "My Organization" sharee, the **address** property is null.</span></span> <span data-ttu-id="8f3df-135">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8f3df-135">Read-only.</span></span> |
|<span data-ttu-id="8f3df-136">id</span><span class="sxs-lookup"><span data-stu-id="8f3df-136">id</span></span>|<span data-ttu-id="8f3df-137">String</span><span class="sxs-lookup"><span data-stu-id="8f3df-137">String</span></span>| <span data-ttu-id="8f3df-138">Уникальный идентификатор пользователя (общего доступа или делегата), которому был передан календарь.</span><span class="sxs-lookup"><span data-stu-id="8f3df-138">The unique identifier of the user (sharee or delegate) with whom the calendar has been shared.</span></span> <span data-ttu-id="8f3df-139">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8f3df-139">Read-only.</span></span>|
|<span data-ttu-id="8f3df-140">isInsideOrganization</span><span class="sxs-lookup"><span data-stu-id="8f3df-140">isInsideOrganization</span></span>|<span data-ttu-id="8f3df-141">Логический</span><span class="sxs-lookup"><span data-stu-id="8f3df-141">Boolean</span></span>| <span data-ttu-id="8f3df-142">Имеет true, если пользователь в контексте (пользователь или делегат) находится в той же организации, что и владелец календаря.</span><span class="sxs-lookup"><span data-stu-id="8f3df-142">True if the user in context (sharee or delegate) is inside the same organization as the calendar owner.</span></span>|
|<span data-ttu-id="8f3df-143">isRemovable</span><span class="sxs-lookup"><span data-stu-id="8f3df-143">isRemovable</span></span>|<span data-ttu-id="8f3df-144">Логический</span><span class="sxs-lookup"><span data-stu-id="8f3df-144">Boolean</span></span>| <span data-ttu-id="8f3df-145">`True` если пользователь может быть удален из списка sharees или делегатов для указанного календаря, в противном `false` случае.</span><span class="sxs-lookup"><span data-stu-id="8f3df-145">`True` if the user can be removed from the list of sharees or delegates for the specified calendar, `false` otherwise.</span></span> <span data-ttu-id="8f3df-146">Пользователь "Моя организация" определяет разрешения, которые другие пользователи в организации имеют для данного календаря.</span><span class="sxs-lookup"><span data-stu-id="8f3df-146">The "My organization" user determines the permissions other people within your organization have to the given calendar.</span></span> <span data-ttu-id="8f3df-147">Невозможно удалить "Моя организация" в качестве делиться в календаре.</span><span class="sxs-lookup"><span data-stu-id="8f3df-147">You cannot remove "My organization" as a sharee to a calendar.</span></span>|
|<span data-ttu-id="8f3df-148">role</span><span class="sxs-lookup"><span data-stu-id="8f3df-148">role</span></span>|[<span data-ttu-id="8f3df-149">calendarRoleType</span><span class="sxs-lookup"><span data-stu-id="8f3df-149">calendarRoleType</span></span>](#calendarroletype-values)| <span data-ttu-id="8f3df-150">Текущий уровень разрешений для доступа к календарю или делегата.</span><span class="sxs-lookup"><span data-stu-id="8f3df-150">Current permission level of the calendar sharee or delegate.</span></span> |

### <a name="calendarroletype-values"></a><span data-ttu-id="8f3df-151">Значения calendarRoleType</span><span class="sxs-lookup"><span data-stu-id="8f3df-151">calendarRoleType values</span></span>

| <span data-ttu-id="8f3df-152">Member</span><span class="sxs-lookup"><span data-stu-id="8f3df-152">Member</span></span>        | <span data-ttu-id="8f3df-153">Описание</span><span class="sxs-lookup"><span data-stu-id="8f3df-153">Description</span></span> |
|:--------------|:------------|
| <span data-ttu-id="8f3df-154">Нет</span><span class="sxs-lookup"><span data-stu-id="8f3df-154">none</span></span> | <span data-ttu-id="8f3df-155">Календарь не является общим для пользователя.</span><span class="sxs-lookup"><span data-stu-id="8f3df-155">Calendar is not shared with the user.</span></span> |
| <span data-ttu-id="8f3df-156">freeBusyRead</span><span class="sxs-lookup"><span data-stu-id="8f3df-156">freeBusyRead</span></span> | <span data-ttu-id="8f3df-157">Пользователь — это пользователь, который может просматривать состояние занятости владельца в календаре.</span><span class="sxs-lookup"><span data-stu-id="8f3df-157">User is a sharee who can view free/busy status of the owner on the calendar.</span></span> |
| <span data-ttu-id="8f3df-158">limitedRead</span><span class="sxs-lookup"><span data-stu-id="8f3df-158">limitedRead</span></span> | <span data-ttu-id="8f3df-159">Пользователь — это пользователь, который может просматривать состояние занятости, а также заголовки и расположения событий в календаре.</span><span class="sxs-lookup"><span data-stu-id="8f3df-159">User is a sharee who can view free/busy status, and titles and locations of the events on the calendar.</span></span> |
| <span data-ttu-id="8f3df-160">read</span><span class="sxs-lookup"><span data-stu-id="8f3df-160">read</span></span> | <span data-ttu-id="8f3df-161">Пользователь — это пользователь, который может просматривать все сведения о событиях в календаре, кроме частных событий владельца.</span><span class="sxs-lookup"><span data-stu-id="8f3df-161">User is a sharee who can view all the details of the events on the calendar, except for the owner's private events.</span></span> |
| <span data-ttu-id="8f3df-162">write</span><span class="sxs-lookup"><span data-stu-id="8f3df-162">write</span></span> | <span data-ttu-id="8f3df-163">Пользователь — это пользователь, который может просматривать все сведения (кроме частных событий) и редактировать события в календаре.</span><span class="sxs-lookup"><span data-stu-id="8f3df-163">User is a sharee who can view all the details (except for private events) and edit events on the calendar.</span></span> |
| <span data-ttu-id="8f3df-164">delegateWithoutPrivateEventAccess</span><span class="sxs-lookup"><span data-stu-id="8f3df-164">delegateWithoutPrivateEventAccess</span></span> | <span data-ttu-id="8f3df-165">Пользователь является делегатом, который имеет доступ на записи, но не может просматривать сведения о частных событиях владельца в календаре.</span><span class="sxs-lookup"><span data-stu-id="8f3df-165">User is a delegate who has write access but cannot view information of the owner's private events on the calendar.</span></span> |
| <span data-ttu-id="8f3df-166">delegateWithPrivateEventAccess</span><span class="sxs-lookup"><span data-stu-id="8f3df-166">delegateWithPrivateEventAccess</span></span> | <span data-ttu-id="8f3df-167">Пользователь — это делегат, который имеет доступ на записи и может просматривать сведения о частных событиях владельца в календаре.</span><span class="sxs-lookup"><span data-stu-id="8f3df-167">User is a delegate who has write access and can view information of the owner's private events on the calendar.</span></span> |
| <span data-ttu-id="8f3df-168">custom</span><span class="sxs-lookup"><span data-stu-id="8f3df-168">custom</span></span> | <span data-ttu-id="8f3df-169">Пользователь имеет настраиваемые разрешения на доступ к календарю.</span><span class="sxs-lookup"><span data-stu-id="8f3df-169">User has custom permissions to the calendar.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="8f3df-170">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8f3df-170">JSON representation</span></span>

<span data-ttu-id="8f3df-171">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8f3df-171">The following is a JSON representation of the resource.</span></span>

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

---
title: Тип ресурса calendarPermission
description: Разрешения пользователя, которому совместно передается календарь.
localization_priority: Normal
author: sochowdh
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 0c8cf612827819370a43b02dbb7064d03530a5d1
ms.sourcegitcommit: 48fff935d56fe96e97577a80a3a0aa15c45419ba
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/10/2021
ms.locfileid: "50177097"
---
# <a name="calendarpermission-resource-type"></a><span data-ttu-id="dbe82-103">Тип ресурса calendarPermission</span><span class="sxs-lookup"><span data-stu-id="dbe82-103">calendarPermission resource type</span></span>

<span data-ttu-id="dbe82-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dbe82-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="dbe82-105">Разрешения пользователя, которому был передан календарь или которому делегирован доступ в клиенте Outlook.</span><span class="sxs-lookup"><span data-stu-id="dbe82-105">The permissions of a user with whom the calendar has been shared or delegated in an Outlook client.</span></span>

<span data-ttu-id="dbe82-106">Получать, обновлять и удалять разрешения календаря можно только от имени владельца календаря.</span><span class="sxs-lookup"><span data-stu-id="dbe82-106">Get, update, and delete of calendar permissions is supported on behalf of only the calendar owner.</span></span>

<span data-ttu-id="dbe82-107">Получение разрешений календаря от имени пользователя или делегата возвращает пустую коллекцию разрешений календаря.</span><span class="sxs-lookup"><span data-stu-id="dbe82-107">Getting the calendar permissions of a calendar on behalf of a sharee or delegate returns an empty calendar permissions collection.</span></span>

<span data-ttu-id="dbe82-108">После того как для календаря настроены обилие или делегат, вы можете обновить только свойство **роли,** чтобы изменить разрешения sharee или делегата. [](../api/calendarpermission-update.md)</span><span class="sxs-lookup"><span data-stu-id="dbe82-108">Once a sharee or delegate has been set up for a calendar, you can [update](../api/calendarpermission-update.md) only the **role** property to change the permissions of a sharee or delegate.</span></span> <span data-ttu-id="dbe82-109">Вы не **можете обновить** **свойство allowedRoles,** **emailAddress,** **isInsideOrganization** или **isRemovable.**</span><span class="sxs-lookup"><span data-stu-id="dbe82-109">You cannot **update** the **allowedRoles**, **emailAddress**, **isInsideOrganization**, or **isRemovable** property.</span></span> <span data-ttu-id="dbe82-110">Чтобы изменить эти свойства, [](../api/calendarpermission-delete.md) необходимо удалить соответствующий объект **calendarPermission** и создать в клиенте Outlook другого представителя или представителя.</span><span class="sxs-lookup"><span data-stu-id="dbe82-110">To change these properties, you should [delete](../api/calendarpermission-delete.md) the corresponding **calendarPermission** object and create another sharee or delegate in an Outlook client.</span></span>

## <a name="methods"></a><span data-ttu-id="dbe82-111">Методы</span><span class="sxs-lookup"><span data-stu-id="dbe82-111">Methods</span></span>

| <span data-ttu-id="dbe82-112">Метод</span><span class="sxs-lookup"><span data-stu-id="dbe82-112">Method</span></span>       | <span data-ttu-id="dbe82-113">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="dbe82-113">Return Type</span></span> | <span data-ttu-id="dbe82-114">Описание</span><span class="sxs-lookup"><span data-stu-id="dbe82-114">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="dbe82-115">Get calendarPermission</span><span class="sxs-lookup"><span data-stu-id="dbe82-115">Get calendarPermission</span></span>](../api/calendarpermission-get.md) | [<span data-ttu-id="dbe82-116">calendarPermission</span><span class="sxs-lookup"><span data-stu-id="dbe82-116">calendarPermission</span></span>](calendarpermission.md) | <span data-ttu-id="dbe82-117">Чтение свойств и связей объекта calendarPermission.</span><span class="sxs-lookup"><span data-stu-id="dbe82-117">Read properties and relationships of calendarPermission object.</span></span> |
| [<span data-ttu-id="dbe82-118">Обновление</span><span class="sxs-lookup"><span data-stu-id="dbe82-118">Update</span></span>](../api/calendarpermission-update.md) | [<span data-ttu-id="dbe82-119">calendarPermission</span><span class="sxs-lookup"><span data-stu-id="dbe82-119">calendarPermission</span></span>](calendarpermission.md) | <span data-ttu-id="dbe82-120">Обновление объекта calendarPermission.</span><span class="sxs-lookup"><span data-stu-id="dbe82-120">Update calendarPermission object.</span></span> |
| <span data-ttu-id="dbe82-121">[удаление](../api/calendarpermission-delete.md);</span><span class="sxs-lookup"><span data-stu-id="dbe82-121">[Delete](../api/calendarpermission-delete.md)</span></span> | <span data-ttu-id="dbe82-122">Нет</span><span class="sxs-lookup"><span data-stu-id="dbe82-122">None</span></span> | <span data-ttu-id="dbe82-123">Удаление объекта calendarPermission.</span><span class="sxs-lookup"><span data-stu-id="dbe82-123">Delete calendarPermission object.</span></span> |

## <a name="properties"></a><span data-ttu-id="dbe82-124">Свойства</span><span class="sxs-lookup"><span data-stu-id="dbe82-124">Properties</span></span>

| <span data-ttu-id="dbe82-125">Свойство</span><span class="sxs-lookup"><span data-stu-id="dbe82-125">Property</span></span>     | <span data-ttu-id="dbe82-126">Тип</span><span class="sxs-lookup"><span data-stu-id="dbe82-126">Type</span></span>        | <span data-ttu-id="dbe82-127">Описание</span><span class="sxs-lookup"><span data-stu-id="dbe82-127">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="dbe82-128">allowedRoles</span><span class="sxs-lookup"><span data-stu-id="dbe82-128">allowedRoles</span></span>|<span data-ttu-id="dbe82-129">[Коллекция calendarRoleType](#calendarroletype-values)</span><span class="sxs-lookup"><span data-stu-id="dbe82-129">[calendarRoleType](#calendarroletype-values) collection</span></span>| <span data-ttu-id="dbe82-130">Список разрешенных уровней разрешений общего доступа или делегирование для календаря.</span><span class="sxs-lookup"><span data-stu-id="dbe82-130">List of allowed sharing or delegating permission levels for the calendar.</span></span> <span data-ttu-id="dbe82-131">Возможные значения: `none`, `freeBusyRead`, `limitedRead`, `read`, `write`, `delegateWithoutPrivateEventAccess`, `delegateWithPrivateEventAccess`, `custom`.</span><span class="sxs-lookup"><span data-stu-id="dbe82-131">Possible values are: `none`, `freeBusyRead`, `limitedRead`, `read`, `write`, `delegateWithoutPrivateEventAccess`, `delegateWithPrivateEventAccess`, `custom`.</span></span>|
|<span data-ttu-id="dbe82-132">emailAddress</span><span class="sxs-lookup"><span data-stu-id="dbe82-132">emailAddress</span></span>|[<span data-ttu-id="dbe82-133">emailAddress</span><span class="sxs-lookup"><span data-stu-id="dbe82-133">emailAddress</span></span>](emailaddress.md)| <span data-ttu-id="dbe82-134">Представляет делиться данными или делегатами, у которых есть доступ к календарю.</span><span class="sxs-lookup"><span data-stu-id="dbe82-134">Represents a sharee or delegate who has access to the calendar.</span></span> <span data-ttu-id="dbe82-135">Для обоймы "Моя организация" свойство **адреса** имеет null.</span><span class="sxs-lookup"><span data-stu-id="dbe82-135">For the "My Organization" sharee, the **address** property is null.</span></span> <span data-ttu-id="dbe82-136">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="dbe82-136">Read-only.</span></span> |
|<span data-ttu-id="dbe82-137">id</span><span class="sxs-lookup"><span data-stu-id="dbe82-137">id</span></span>|<span data-ttu-id="dbe82-138">String</span><span class="sxs-lookup"><span data-stu-id="dbe82-138">String</span></span>| <span data-ttu-id="dbe82-139">Уникальный идентификатор пользователя (общего доступа или делегата), которому был передан календарь.</span><span class="sxs-lookup"><span data-stu-id="dbe82-139">The unique identifier of the user (sharee or delegate) with whom the calendar has been shared.</span></span> <span data-ttu-id="dbe82-140">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="dbe82-140">Read-only.</span></span>|
|<span data-ttu-id="dbe82-141">isInsideOrganization</span><span class="sxs-lookup"><span data-stu-id="dbe82-141">isInsideOrganization</span></span>|<span data-ttu-id="dbe82-142">Логическое</span><span class="sxs-lookup"><span data-stu-id="dbe82-142">Boolean</span></span>| <span data-ttu-id="dbe82-143">Имеет true, если пользователь в контексте (пользователь или делегат) находится в той же организации, что и владелец календаря.</span><span class="sxs-lookup"><span data-stu-id="dbe82-143">True if the user in context (sharee or delegate) is inside the same organization as the calendar owner.</span></span>|
|<span data-ttu-id="dbe82-144">isRemovable</span><span class="sxs-lookup"><span data-stu-id="dbe82-144">isRemovable</span></span>|<span data-ttu-id="dbe82-145">Логический</span><span class="sxs-lookup"><span data-stu-id="dbe82-145">Boolean</span></span>| <span data-ttu-id="dbe82-146">`True` если пользователь может быть удален из списка sharees или делегатов для указанного календаря, в противном `false` случае.</span><span class="sxs-lookup"><span data-stu-id="dbe82-146">`True` if the user can be removed from the list of sharees or delegates for the specified calendar, `false` otherwise.</span></span> <span data-ttu-id="dbe82-147">Пользователь "Моя организация" определяет разрешения, которые другие пользователи в организации имеют для данного календаря.</span><span class="sxs-lookup"><span data-stu-id="dbe82-147">The "My organization" user determines the permissions other people within your organization have to the given calendar.</span></span> <span data-ttu-id="dbe82-148">Невозможно удалить "Моя организация" в качестве делиться в календаре.</span><span class="sxs-lookup"><span data-stu-id="dbe82-148">You cannot remove "My organization" as a sharee to a calendar.</span></span>|
|<span data-ttu-id="dbe82-149">role</span><span class="sxs-lookup"><span data-stu-id="dbe82-149">role</span></span>|[<span data-ttu-id="dbe82-150">calendarRoleType</span><span class="sxs-lookup"><span data-stu-id="dbe82-150">calendarRoleType</span></span>](#calendarroletype-values)| <span data-ttu-id="dbe82-151">Текущий уровень разрешений для доступа к календарю или делегата.</span><span class="sxs-lookup"><span data-stu-id="dbe82-151">Current permission level of the calendar sharee or delegate.</span></span> |

### <a name="calendarroletype-values"></a><span data-ttu-id="dbe82-152">Значения calendarRoleType</span><span class="sxs-lookup"><span data-stu-id="dbe82-152">calendarRoleType values</span></span>

| <span data-ttu-id="dbe82-153">Member</span><span class="sxs-lookup"><span data-stu-id="dbe82-153">Member</span></span>        | <span data-ttu-id="dbe82-154">Описание</span><span class="sxs-lookup"><span data-stu-id="dbe82-154">Description</span></span> |
|:--------------|:------------|
| <span data-ttu-id="dbe82-155">Нет</span><span class="sxs-lookup"><span data-stu-id="dbe82-155">none</span></span> | <span data-ttu-id="dbe82-156">Календарь не является общим для пользователя.</span><span class="sxs-lookup"><span data-stu-id="dbe82-156">Calendar is not shared with the user.</span></span> |
| <span data-ttu-id="dbe82-157">freeBusyRead</span><span class="sxs-lookup"><span data-stu-id="dbe82-157">freeBusyRead</span></span> | <span data-ttu-id="dbe82-158">Пользователь — это пользователь, который может просматривать состояние занятости владельца в календаре.</span><span class="sxs-lookup"><span data-stu-id="dbe82-158">User is a sharee who can view free/busy status of the owner on the calendar.</span></span> |
| <span data-ttu-id="dbe82-159">limitedRead</span><span class="sxs-lookup"><span data-stu-id="dbe82-159">limitedRead</span></span> | <span data-ttu-id="dbe82-160">Пользователь — это пользователь, который может просматривать состояние занятости, а также заголовки и расположения событий в календаре.</span><span class="sxs-lookup"><span data-stu-id="dbe82-160">User is a sharee who can view free/busy status, and titles and locations of the events on the calendar.</span></span> |
| <span data-ttu-id="dbe82-161">read</span><span class="sxs-lookup"><span data-stu-id="dbe82-161">read</span></span> | <span data-ttu-id="dbe82-162">Пользователь — это пользователь, который может просматривать все сведения о событиях в календаре, кроме частных событий владельца.</span><span class="sxs-lookup"><span data-stu-id="dbe82-162">User is a sharee who can view all the details of the events on the calendar, except for the owner's private events.</span></span> |
| <span data-ttu-id="dbe82-163">write</span><span class="sxs-lookup"><span data-stu-id="dbe82-163">write</span></span> | <span data-ttu-id="dbe82-164">Пользователь — это пользователь, который может просматривать все сведения (кроме частных событий) и редактировать события в календаре.</span><span class="sxs-lookup"><span data-stu-id="dbe82-164">User is a sharee who can view all the details (except for private events) and edit events on the calendar.</span></span> |
| <span data-ttu-id="dbe82-165">delegateWithoutPrivateEventAccess</span><span class="sxs-lookup"><span data-stu-id="dbe82-165">delegateWithoutPrivateEventAccess</span></span> | <span data-ttu-id="dbe82-166">Пользователь является делегатом, который имеет доступ на записи, но не может просматривать сведения о частных событиях владельца в календаре.</span><span class="sxs-lookup"><span data-stu-id="dbe82-166">User is a delegate who has write access but cannot view information of the owner's private events on the calendar.</span></span> |
| <span data-ttu-id="dbe82-167">delegateWithPrivateEventAccess</span><span class="sxs-lookup"><span data-stu-id="dbe82-167">delegateWithPrivateEventAccess</span></span> | <span data-ttu-id="dbe82-168">Пользователь — это делегат, который имеет доступ на записи и может просматривать сведения о частных событиях владельца в календаре.</span><span class="sxs-lookup"><span data-stu-id="dbe82-168">User is a delegate who has write access and can view information of the owner's private events on the calendar.</span></span> |
| <span data-ttu-id="dbe82-169">custom</span><span class="sxs-lookup"><span data-stu-id="dbe82-169">custom</span></span> | <span data-ttu-id="dbe82-170">Пользователь имеет настраиваемые разрешения на доступ к календарю.</span><span class="sxs-lookup"><span data-stu-id="dbe82-170">User has custom permissions to the calendar.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="dbe82-171">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="dbe82-171">JSON representation</span></span>

<span data-ttu-id="dbe82-172">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="dbe82-172">The following is a JSON representation of the resource.</span></span>

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


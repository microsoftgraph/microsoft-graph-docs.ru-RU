---
title: Тип ресурса Календарпермиссион
description: Разрешения пользователя, к которому открыт общий доступ к календарю.
localization_priority: Normal
author: sochowdh
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 80c704dbb3e50d3f4d0ba586a40f06f74f032321
ms.sourcegitcommit: 9a6ce4ddf75beead19b7c35a1949cf4d105b9b29
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2020
ms.locfileid: "43229467"
---
# <a name="calendarpermission-resource-type"></a><span data-ttu-id="cc2d2-103">Тип ресурса Календарпермиссион</span><span class="sxs-lookup"><span data-stu-id="cc2d2-103">calendarPermission resource type</span></span>

<span data-ttu-id="cc2d2-104">Разрешения пользователя, к которому открыт общий доступ к календарю или который был делегирован в клиенте Outlook.</span><span class="sxs-lookup"><span data-stu-id="cc2d2-104">The permissions of a user with whom the calendar has been shared or delegated in an Outlook client.</span></span>

<span data-ttu-id="cc2d2-105">Получение, обновление и удаление разрешений календаря поддерживается только от имени владельца календаря.</span><span class="sxs-lookup"><span data-stu-id="cc2d2-105">Get, update, and delete of calendar permissions is supported on behalf of only the calendar owner.</span></span>

<span data-ttu-id="cc2d2-106">Получение разрешений календаря для календаря от имени объекта Share или делегата возвращает пустой набор разрешений календаря.</span><span class="sxs-lookup"><span data-stu-id="cc2d2-106">Getting the calendar permissions of a calendar on behalf of a sharee or delegate returns an empty calendar permissions collection.</span></span>

<span data-ttu-id="cc2d2-107">После настройки общего доступа или делегирования для календаря можно [Обновить](../api/calendarpermission-update.md) только свойство **Role** , чтобы изменить разрешения для общего доступа или делегата.</span><span class="sxs-lookup"><span data-stu-id="cc2d2-107">Once a sharee or delegate has been set up for a calendar, you can [update](../api/calendarpermission-update.md) only the **role** property to change the permissions of a sharee or delegate.</span></span> <span data-ttu-id="cc2d2-108">Невозможно **Обновить** свойства **алловедролес**, **EmailAddress**, **исинсидеорганизатион и**. **isRemovable**</span><span class="sxs-lookup"><span data-stu-id="cc2d2-108">You cannot **update** the **allowedRoles**, **emailAddress**, **isInsideOrganization**, or **isRemovable** property.</span></span> <span data-ttu-id="cc2d2-109">Чтобы изменить эти свойства, необходимо [Удалить](../api/calendarpermission-delete.md) соответствующий объект **календарпермиссион** и создать еще одну общую папку или делегат в клиенте Outlook.</span><span class="sxs-lookup"><span data-stu-id="cc2d2-109">To change these properties, you should [delete](../api/calendarpermission-delete.md) the corresponding **calendarPermission** object and create another sharee or delegate in an Outlook client.</span></span>

## <a name="methods"></a><span data-ttu-id="cc2d2-110">Методы</span><span class="sxs-lookup"><span data-stu-id="cc2d2-110">Methods</span></span>

| <span data-ttu-id="cc2d2-111">Метод</span><span class="sxs-lookup"><span data-stu-id="cc2d2-111">Method</span></span>       | <span data-ttu-id="cc2d2-112">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="cc2d2-112">Return Type</span></span> | <span data-ttu-id="cc2d2-113">Описание</span><span class="sxs-lookup"><span data-stu-id="cc2d2-113">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="cc2d2-114">Получение Календарпермиссион</span><span class="sxs-lookup"><span data-stu-id="cc2d2-114">Get calendarPermission</span></span>](../api/calendarpermission-get.md) | [<span data-ttu-id="cc2d2-115">календарпермиссион</span><span class="sxs-lookup"><span data-stu-id="cc2d2-115">calendarPermission</span></span>](calendarpermission.md) | <span data-ttu-id="cc2d2-116">Чтение свойств и связей объекта Календарпермиссион.</span><span class="sxs-lookup"><span data-stu-id="cc2d2-116">Read properties and relationships of calendarPermission object.</span></span> |
| <span data-ttu-id="cc2d2-117">[обновление](../api/calendarpermission-update.md).</span><span class="sxs-lookup"><span data-stu-id="cc2d2-117">[Update](../api/calendarpermission-update.md)</span></span> | [<span data-ttu-id="cc2d2-118">календарпермиссион</span><span class="sxs-lookup"><span data-stu-id="cc2d2-118">calendarPermission</span></span>](calendarpermission.md) | <span data-ttu-id="cc2d2-119">Обновление объекта Календарпермиссион.</span><span class="sxs-lookup"><span data-stu-id="cc2d2-119">Update calendarPermission object.</span></span> |
| <span data-ttu-id="cc2d2-120">[удаление](../api/calendarpermission-delete.md);</span><span class="sxs-lookup"><span data-stu-id="cc2d2-120">[Delete](../api/calendarpermission-delete.md)</span></span> | <span data-ttu-id="cc2d2-121">Нет</span><span class="sxs-lookup"><span data-stu-id="cc2d2-121">None</span></span> | <span data-ttu-id="cc2d2-122">Удаление объекта Календарпермиссион.</span><span class="sxs-lookup"><span data-stu-id="cc2d2-122">Delete calendarPermission object.</span></span> |

## <a name="properties"></a><span data-ttu-id="cc2d2-123">Свойства</span><span class="sxs-lookup"><span data-stu-id="cc2d2-123">Properties</span></span>

| <span data-ttu-id="cc2d2-124">Свойство</span><span class="sxs-lookup"><span data-stu-id="cc2d2-124">Property</span></span>     | <span data-ttu-id="cc2d2-125">Тип</span><span class="sxs-lookup"><span data-stu-id="cc2d2-125">Type</span></span>        | <span data-ttu-id="cc2d2-126">Описание</span><span class="sxs-lookup"><span data-stu-id="cc2d2-126">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="cc2d2-127">алловедролес</span><span class="sxs-lookup"><span data-stu-id="cc2d2-127">allowedRoles</span></span>|<span data-ttu-id="cc2d2-128">Коллекция [календарролетипе](#calendarroletype-values)</span><span class="sxs-lookup"><span data-stu-id="cc2d2-128">[calendarRoleType](#calendarroletype-values) collection</span></span>| <span data-ttu-id="cc2d2-129">Список разрешенных для общего доступа или делегирования уровней разрешений для календаря.</span><span class="sxs-lookup"><span data-stu-id="cc2d2-129">List of allowed sharing or delegating permission levels for the calendar.</span></span> <span data-ttu-id="cc2d2-130">Возможные значения: `none`, `freeBusyRead`, `limitedRead`, `read`, `write`, `delegateWithoutPrivateEventAccess`, `delegateWithPrivateEventAccess`, `custom`.</span><span class="sxs-lookup"><span data-stu-id="cc2d2-130">Possible values are: `none`, `freeBusyRead`, `limitedRead`, `read`, `write`, `delegateWithoutPrivateEventAccess`, `delegateWithPrivateEventAccess`, `custom`.</span></span>|
|<span data-ttu-id="cc2d2-131">emailAddress</span><span class="sxs-lookup"><span data-stu-id="cc2d2-131">emailAddress</span></span>|[<span data-ttu-id="cc2d2-132">emailAddress</span><span class="sxs-lookup"><span data-stu-id="cc2d2-132">emailAddress</span></span>](emailaddress.md)| <span data-ttu-id="cc2d2-133">Представляет общий доступ или представитель, имеющий доступ к календарю.</span><span class="sxs-lookup"><span data-stu-id="cc2d2-133">Represents a sharee or delegate who has access to the calendar.</span></span> <span data-ttu-id="cc2d2-134">Для общего доступа к общему ресурсу "Моя организация" свойство **Address** имеет значение null.</span><span class="sxs-lookup"><span data-stu-id="cc2d2-134">For the "My Organization" sharee, the **address** property is null.</span></span> <span data-ttu-id="cc2d2-135">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="cc2d2-135">Read-only.</span></span> |
|<span data-ttu-id="cc2d2-136">id</span><span class="sxs-lookup"><span data-stu-id="cc2d2-136">id</span></span>|<span data-ttu-id="cc2d2-137">String</span><span class="sxs-lookup"><span data-stu-id="cc2d2-137">String</span></span>| <span data-ttu-id="cc2d2-138">Уникальный идентификатор пользователя (общего доступа или представителя), к которому открыт общий доступ к календарю.</span><span class="sxs-lookup"><span data-stu-id="cc2d2-138">The unique identifier of the user (sharee or delegate) with whom the calendar has been shared.</span></span> <span data-ttu-id="cc2d2-139">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="cc2d2-139">Read-only.</span></span>|
|<span data-ttu-id="cc2d2-140">исинсидеорганизатион</span><span class="sxs-lookup"><span data-stu-id="cc2d2-140">isInsideOrganization</span></span>|<span data-ttu-id="cc2d2-141">Boolean</span><span class="sxs-lookup"><span data-stu-id="cc2d2-141">Boolean</span></span>| <span data-ttu-id="cc2d2-142">Имеет значение true, если пользователь в контексте (общий доступ или представитель) находится в той же организации, что и владелец календаря.</span><span class="sxs-lookup"><span data-stu-id="cc2d2-142">True if the user in context (sharee or delegate) is inside the same organization as the calendar owner.</span></span>|
|<span data-ttu-id="cc2d2-143">isRemovable</span><span class="sxs-lookup"><span data-stu-id="cc2d2-143">isRemovable</span></span>|<span data-ttu-id="cc2d2-144">Логический</span><span class="sxs-lookup"><span data-stu-id="cc2d2-144">Boolean</span></span>| <span data-ttu-id="cc2d2-145">`True`, если пользователь может быть удален из списка общих или делегатов для указанного календаря, `false` в противном случае.</span><span class="sxs-lookup"><span data-stu-id="cc2d2-145">`True` if the user can be removed from the list of sharees or delegates for the specified calendar, `false` otherwise.</span></span> <span data-ttu-id="cc2d2-146">Пользователь "Моя организация" определяет разрешения, которые пользователи в организации имеют в указанном календаре.</span><span class="sxs-lookup"><span data-stu-id="cc2d2-146">The "My organization" user determines the permissions other people within your organization have to the given calendar.</span></span> <span data-ttu-id="cc2d2-147">Вы не можете удалить "Моя организация" как общий доступ к календарю.</span><span class="sxs-lookup"><span data-stu-id="cc2d2-147">You cannot remove "My organization" as a sharee to a calendar.</span></span>|
|<span data-ttu-id="cc2d2-148">role</span><span class="sxs-lookup"><span data-stu-id="cc2d2-148">role</span></span>|[<span data-ttu-id="cc2d2-149">календарролетипе</span><span class="sxs-lookup"><span data-stu-id="cc2d2-149">calendarRoleType</span></span>](#calendarroletype-values)| <span data-ttu-id="cc2d2-150">Текущий уровень разрешений для общего доступа к календарю или представителем.</span><span class="sxs-lookup"><span data-stu-id="cc2d2-150">Current permission level of the calendar sharee or delegate.</span></span> |

### <a name="calendarroletype-values"></a><span data-ttu-id="cc2d2-151">значения Календарролетипе</span><span class="sxs-lookup"><span data-stu-id="cc2d2-151">calendarRoleType values</span></span>

| <span data-ttu-id="cc2d2-152">Значения</span><span class="sxs-lookup"><span data-stu-id="cc2d2-152">Values</span></span>        | <span data-ttu-id="cc2d2-153">Описание</span><span class="sxs-lookup"><span data-stu-id="cc2d2-153">Description</span></span> |
|:--------------|:------------|
| <span data-ttu-id="cc2d2-154">Нет</span><span class="sxs-lookup"><span data-stu-id="cc2d2-154">none</span></span> | <span data-ttu-id="cc2d2-155">Доступ к календарю для пользователя не предоставляется.</span><span class="sxs-lookup"><span data-stu-id="cc2d2-155">Calendar is not shared with the user.</span></span> |
| <span data-ttu-id="cc2d2-156">фрибусиреад</span><span class="sxs-lookup"><span data-stu-id="cc2d2-156">freeBusyRead</span></span> | <span data-ttu-id="cc2d2-157">Пользователь — это общий доступ, который может просматривать сведения о доступности владельца в календаре.</span><span class="sxs-lookup"><span data-stu-id="cc2d2-157">User is a sharee who can view free/busy status of the owner on the calendar.</span></span> |
| <span data-ttu-id="cc2d2-158">лимитедреад</span><span class="sxs-lookup"><span data-stu-id="cc2d2-158">limitedRead</span></span> | <span data-ttu-id="cc2d2-159">Пользователь предоставляет доступ к сведениям о доступности, а также заголовках и расположениях событий в календаре.</span><span class="sxs-lookup"><span data-stu-id="cc2d2-159">User is a sharee who can view free/busy status, and titles and locations of the events on the calendar.</span></span> |
| <span data-ttu-id="cc2d2-160">прочитан</span><span class="sxs-lookup"><span data-stu-id="cc2d2-160">read</span></span> | <span data-ttu-id="cc2d2-161">Пользователь предоставляет общий доступ, который может просматривать все сведения о событиях в календаре, за исключением частных событий владельца.</span><span class="sxs-lookup"><span data-stu-id="cc2d2-161">User is a sharee who can view all the details of the events on the calendar, except for the owner's private events.</span></span> |
| <span data-ttu-id="cc2d2-162">понижен</span><span class="sxs-lookup"><span data-stu-id="cc2d2-162">write</span></span> | <span data-ttu-id="cc2d2-163">Пользователь — это общий доступ, который может просматривать все сведения (кроме частных событий) и изменять события в календаре.</span><span class="sxs-lookup"><span data-stu-id="cc2d2-163">User is a sharee who can view all the details (except for private events) and edit events on the calendar.</span></span> |
| <span data-ttu-id="cc2d2-164">делегатевисаутпривативентакцесс</span><span class="sxs-lookup"><span data-stu-id="cc2d2-164">delegateWithoutPrivateEventAccess</span></span> | <span data-ttu-id="cc2d2-165">Пользователь — это делегат с доступом для записи, но не может просматривать сведения о закрытых событиях владельца в календаре.</span><span class="sxs-lookup"><span data-stu-id="cc2d2-165">User is a delegate who has write access but cannot view information of the owner's private events on the calendar.</span></span> |
| <span data-ttu-id="cc2d2-166">делегатевиспривативентакцесс</span><span class="sxs-lookup"><span data-stu-id="cc2d2-166">delegateWithPrivateEventAccess</span></span> | <span data-ttu-id="cc2d2-167">Пользователь — это представитель, имеющий доступ на запись и позволяющий просматривать сведения о частных событиях владельца в календаре.</span><span class="sxs-lookup"><span data-stu-id="cc2d2-167">User is a delegate who has write access and can view information of the owner's private events on the calendar.</span></span> |
| <span data-ttu-id="cc2d2-168">собственный</span><span class="sxs-lookup"><span data-stu-id="cc2d2-168">custom</span></span> | <span data-ttu-id="cc2d2-169">Пользователь обладает пользовательскими разрешениями на доступ к календарю.</span><span class="sxs-lookup"><span data-stu-id="cc2d2-169">User has custom permissions to the calendar.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="cc2d2-170">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="cc2d2-170">JSON representation</span></span>

<span data-ttu-id="cc2d2-171">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cc2d2-171">The following is a JSON representation of the resource.</span></span>

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
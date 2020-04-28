---
title: Тип ресурса Календарпермиссион
description: Разрешения пользователя, к которому открыт общий доступ к календарю.
localization_priority: Normal
author: sochowdh
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: c038ccd69cefa66c4fd57f4b09273662320f2640
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507840"
---
# <a name="calendarpermission-resource-type"></a><span data-ttu-id="a626b-103">Тип ресурса Календарпермиссион</span><span class="sxs-lookup"><span data-stu-id="a626b-103">calendarPermission resource type</span></span>

<span data-ttu-id="a626b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a626b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a626b-105">Разрешения пользователя, к которому открыт общий доступ к календарю или который был делегирован в клиенте Outlook.</span><span class="sxs-lookup"><span data-stu-id="a626b-105">The permissions of a user with whom the calendar has been shared or delegated in an Outlook client.</span></span>

<span data-ttu-id="a626b-106">Получение, обновление и удаление разрешений календаря поддерживается только от имени владельца календаря.</span><span class="sxs-lookup"><span data-stu-id="a626b-106">Get, update, and delete of calendar permissions is supported on behalf of only the calendar owner.</span></span>

<span data-ttu-id="a626b-107">Получение разрешений календаря для календаря от имени объекта Share или делегата возвращает пустой набор разрешений календаря.</span><span class="sxs-lookup"><span data-stu-id="a626b-107">Getting the calendar permissions of a calendar on behalf of a sharee or delegate returns an empty calendar permissions collection.</span></span>

<span data-ttu-id="a626b-108">После настройки общего доступа или делегирования для календаря можно [Обновить](../api/calendarpermission-update.md) только свойство **Role** , чтобы изменить разрешения для общего доступа или делегата.</span><span class="sxs-lookup"><span data-stu-id="a626b-108">Once a sharee or delegate has been set up for a calendar, you can [update](../api/calendarpermission-update.md) only the **role** property to change the permissions of a sharee or delegate.</span></span> <span data-ttu-id="a626b-109">Невозможно **Обновить** свойства **алловедролес**, **EmailAddress**, **исинсидеорганизатион и**. **isRemovable**</span><span class="sxs-lookup"><span data-stu-id="a626b-109">You cannot **update** the **allowedRoles**, **emailAddress**, **isInsideOrganization**, or **isRemovable** property.</span></span> <span data-ttu-id="a626b-110">Чтобы изменить эти свойства, необходимо [Удалить](../api/calendarpermission-delete.md) соответствующий объект **календарпермиссион** и создать еще одну общую папку или делегат в клиенте Outlook.</span><span class="sxs-lookup"><span data-stu-id="a626b-110">To change these properties, you should [delete](../api/calendarpermission-delete.md) the corresponding **calendarPermission** object and create another sharee or delegate in an Outlook client.</span></span>

## <a name="methods"></a><span data-ttu-id="a626b-111">Методы</span><span class="sxs-lookup"><span data-stu-id="a626b-111">Methods</span></span>

| <span data-ttu-id="a626b-112">Метод</span><span class="sxs-lookup"><span data-stu-id="a626b-112">Method</span></span>       | <span data-ttu-id="a626b-113">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="a626b-113">Return Type</span></span> | <span data-ttu-id="a626b-114">Описание</span><span class="sxs-lookup"><span data-stu-id="a626b-114">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="a626b-115">Получение Календарпермиссион</span><span class="sxs-lookup"><span data-stu-id="a626b-115">Get calendarPermission</span></span>](../api/calendarpermission-get.md) | [<span data-ttu-id="a626b-116">календарпермиссион</span><span class="sxs-lookup"><span data-stu-id="a626b-116">calendarPermission</span></span>](calendarpermission.md) | <span data-ttu-id="a626b-117">Чтение свойств и связей объекта Календарпермиссион.</span><span class="sxs-lookup"><span data-stu-id="a626b-117">Read properties and relationships of calendarPermission object.</span></span> |
| <span data-ttu-id="a626b-118">[обновление](../api/calendarpermission-update.md).</span><span class="sxs-lookup"><span data-stu-id="a626b-118">[Update](../api/calendarpermission-update.md)</span></span> | [<span data-ttu-id="a626b-119">календарпермиссион</span><span class="sxs-lookup"><span data-stu-id="a626b-119">calendarPermission</span></span>](calendarpermission.md) | <span data-ttu-id="a626b-120">Обновление объекта Календарпермиссион.</span><span class="sxs-lookup"><span data-stu-id="a626b-120">Update calendarPermission object.</span></span> |
| <span data-ttu-id="a626b-121">[удаление](../api/calendarpermission-delete.md);</span><span class="sxs-lookup"><span data-stu-id="a626b-121">[Delete](../api/calendarpermission-delete.md)</span></span> | <span data-ttu-id="a626b-122">Нет</span><span class="sxs-lookup"><span data-stu-id="a626b-122">None</span></span> | <span data-ttu-id="a626b-123">Удаление объекта Календарпермиссион.</span><span class="sxs-lookup"><span data-stu-id="a626b-123">Delete calendarPermission object.</span></span> |

## <a name="properties"></a><span data-ttu-id="a626b-124">Свойства</span><span class="sxs-lookup"><span data-stu-id="a626b-124">Properties</span></span>

| <span data-ttu-id="a626b-125">Свойство</span><span class="sxs-lookup"><span data-stu-id="a626b-125">Property</span></span>     | <span data-ttu-id="a626b-126">Тип</span><span class="sxs-lookup"><span data-stu-id="a626b-126">Type</span></span>        | <span data-ttu-id="a626b-127">Описание</span><span class="sxs-lookup"><span data-stu-id="a626b-127">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="a626b-128">алловедролес</span><span class="sxs-lookup"><span data-stu-id="a626b-128">allowedRoles</span></span>|<span data-ttu-id="a626b-129">Коллекция [календарролетипе](#calendarroletype-values)</span><span class="sxs-lookup"><span data-stu-id="a626b-129">[calendarRoleType](#calendarroletype-values) collection</span></span>| <span data-ttu-id="a626b-130">Список разрешенных для общего доступа или делегирования уровней разрешений для календаря.</span><span class="sxs-lookup"><span data-stu-id="a626b-130">List of allowed sharing or delegating permission levels for the calendar.</span></span> <span data-ttu-id="a626b-131">Возможные значения: `none`, `freeBusyRead`, `limitedRead`, `read`, `write`, `delegateWithoutPrivateEventAccess`, `delegateWithPrivateEventAccess`, `custom`.</span><span class="sxs-lookup"><span data-stu-id="a626b-131">Possible values are: `none`, `freeBusyRead`, `limitedRead`, `read`, `write`, `delegateWithoutPrivateEventAccess`, `delegateWithPrivateEventAccess`, `custom`.</span></span>|
|<span data-ttu-id="a626b-132">emailAddress</span><span class="sxs-lookup"><span data-stu-id="a626b-132">emailAddress</span></span>|[<span data-ttu-id="a626b-133">emailAddress</span><span class="sxs-lookup"><span data-stu-id="a626b-133">emailAddress</span></span>](emailaddress.md)| <span data-ttu-id="a626b-134">Представляет общий доступ или представитель, имеющий доступ к календарю.</span><span class="sxs-lookup"><span data-stu-id="a626b-134">Represents a sharee or delegate who has access to the calendar.</span></span> <span data-ttu-id="a626b-135">Для общего доступа к общему ресурсу "Моя организация" свойство **Address** имеет значение null.</span><span class="sxs-lookup"><span data-stu-id="a626b-135">For the "My Organization" sharee, the **address** property is null.</span></span> <span data-ttu-id="a626b-136">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a626b-136">Read-only.</span></span> |
|<span data-ttu-id="a626b-137">id</span><span class="sxs-lookup"><span data-stu-id="a626b-137">id</span></span>|<span data-ttu-id="a626b-138">String</span><span class="sxs-lookup"><span data-stu-id="a626b-138">String</span></span>| <span data-ttu-id="a626b-139">Уникальный идентификатор пользователя (общего доступа или представителя), к которому открыт общий доступ к календарю.</span><span class="sxs-lookup"><span data-stu-id="a626b-139">The unique identifier of the user (sharee or delegate) with whom the calendar has been shared.</span></span> <span data-ttu-id="a626b-140">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a626b-140">Read-only.</span></span>|
|<span data-ttu-id="a626b-141">исинсидеорганизатион</span><span class="sxs-lookup"><span data-stu-id="a626b-141">isInsideOrganization</span></span>|<span data-ttu-id="a626b-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="a626b-142">Boolean</span></span>| <span data-ttu-id="a626b-143">Имеет значение true, если пользователь в контексте (общий доступ или представитель) находится в той же организации, что и владелец календаря.</span><span class="sxs-lookup"><span data-stu-id="a626b-143">True if the user in context (sharee or delegate) is inside the same organization as the calendar owner.</span></span>|
|<span data-ttu-id="a626b-144">isRemovable</span><span class="sxs-lookup"><span data-stu-id="a626b-144">isRemovable</span></span>|<span data-ttu-id="a626b-145">Логический</span><span class="sxs-lookup"><span data-stu-id="a626b-145">Boolean</span></span>| <span data-ttu-id="a626b-146">`True`, если пользователь может быть удален из списка общих или делегатов для указанного календаря, `false` в противном случае.</span><span class="sxs-lookup"><span data-stu-id="a626b-146">`True` if the user can be removed from the list of sharees or delegates for the specified calendar, `false` otherwise.</span></span> <span data-ttu-id="a626b-147">Пользователь "Моя организация" определяет разрешения, которые пользователи в организации имеют в указанном календаре.</span><span class="sxs-lookup"><span data-stu-id="a626b-147">The "My organization" user determines the permissions other people within your organization have to the given calendar.</span></span> <span data-ttu-id="a626b-148">Вы не можете удалить "Моя организация" как общий доступ к календарю.</span><span class="sxs-lookup"><span data-stu-id="a626b-148">You cannot remove "My organization" as a sharee to a calendar.</span></span>|
|<span data-ttu-id="a626b-149">role</span><span class="sxs-lookup"><span data-stu-id="a626b-149">role</span></span>|[<span data-ttu-id="a626b-150">календарролетипе</span><span class="sxs-lookup"><span data-stu-id="a626b-150">calendarRoleType</span></span>](#calendarroletype-values)| <span data-ttu-id="a626b-151">Текущий уровень разрешений для общего доступа к календарю или представителем.</span><span class="sxs-lookup"><span data-stu-id="a626b-151">Current permission level of the calendar sharee or delegate.</span></span> |

### <a name="calendarroletype-values"></a><span data-ttu-id="a626b-152">значения Календарролетипе</span><span class="sxs-lookup"><span data-stu-id="a626b-152">calendarRoleType values</span></span>

| <span data-ttu-id="a626b-153">Значения</span><span class="sxs-lookup"><span data-stu-id="a626b-153">Values</span></span>        | <span data-ttu-id="a626b-154">Описание</span><span class="sxs-lookup"><span data-stu-id="a626b-154">Description</span></span> |
|:--------------|:------------|
| <span data-ttu-id="a626b-155">Нет</span><span class="sxs-lookup"><span data-stu-id="a626b-155">none</span></span> | <span data-ttu-id="a626b-156">Доступ к календарю для пользователя не предоставляется.</span><span class="sxs-lookup"><span data-stu-id="a626b-156">Calendar is not shared with the user.</span></span> |
| <span data-ttu-id="a626b-157">фрибусиреад</span><span class="sxs-lookup"><span data-stu-id="a626b-157">freeBusyRead</span></span> | <span data-ttu-id="a626b-158">Пользователь — это общий доступ, который может просматривать сведения о доступности владельца в календаре.</span><span class="sxs-lookup"><span data-stu-id="a626b-158">User is a sharee who can view free/busy status of the owner on the calendar.</span></span> |
| <span data-ttu-id="a626b-159">лимитедреад</span><span class="sxs-lookup"><span data-stu-id="a626b-159">limitedRead</span></span> | <span data-ttu-id="a626b-160">Пользователь предоставляет доступ к сведениям о доступности, а также заголовках и расположениях событий в календаре.</span><span class="sxs-lookup"><span data-stu-id="a626b-160">User is a sharee who can view free/busy status, and titles and locations of the events on the calendar.</span></span> |
| <span data-ttu-id="a626b-161">прочитан</span><span class="sxs-lookup"><span data-stu-id="a626b-161">read</span></span> | <span data-ttu-id="a626b-162">Пользователь предоставляет общий доступ, который может просматривать все сведения о событиях в календаре, за исключением частных событий владельца.</span><span class="sxs-lookup"><span data-stu-id="a626b-162">User is a sharee who can view all the details of the events on the calendar, except for the owner's private events.</span></span> |
| <span data-ttu-id="a626b-163">понижен</span><span class="sxs-lookup"><span data-stu-id="a626b-163">write</span></span> | <span data-ttu-id="a626b-164">Пользователь — это общий доступ, который может просматривать все сведения (кроме частных событий) и изменять события в календаре.</span><span class="sxs-lookup"><span data-stu-id="a626b-164">User is a sharee who can view all the details (except for private events) and edit events on the calendar.</span></span> |
| <span data-ttu-id="a626b-165">делегатевисаутпривативентакцесс</span><span class="sxs-lookup"><span data-stu-id="a626b-165">delegateWithoutPrivateEventAccess</span></span> | <span data-ttu-id="a626b-166">Пользователь — это делегат с доступом для записи, но не может просматривать сведения о закрытых событиях владельца в календаре.</span><span class="sxs-lookup"><span data-stu-id="a626b-166">User is a delegate who has write access but cannot view information of the owner's private events on the calendar.</span></span> |
| <span data-ttu-id="a626b-167">делегатевиспривативентакцесс</span><span class="sxs-lookup"><span data-stu-id="a626b-167">delegateWithPrivateEventAccess</span></span> | <span data-ttu-id="a626b-168">Пользователь — это представитель, имеющий доступ на запись и позволяющий просматривать сведения о частных событиях владельца в календаре.</span><span class="sxs-lookup"><span data-stu-id="a626b-168">User is a delegate who has write access and can view information of the owner's private events on the calendar.</span></span> |
| <span data-ttu-id="a626b-169">собственный</span><span class="sxs-lookup"><span data-stu-id="a626b-169">custom</span></span> | <span data-ttu-id="a626b-170">Пользователь обладает пользовательскими разрешениями на доступ к календарю.</span><span class="sxs-lookup"><span data-stu-id="a626b-170">User has custom permissions to the calendar.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="a626b-171">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a626b-171">JSON representation</span></span>

<span data-ttu-id="a626b-172">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a626b-172">The following is a JSON representation of the resource.</span></span>

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
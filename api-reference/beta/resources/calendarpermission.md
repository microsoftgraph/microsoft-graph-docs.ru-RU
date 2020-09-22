---
title: Тип ресурса Календарпермиссион
description: Разрешения пользователя, к которому открыт общий доступ к календарю.
localization_priority: Normal
author: sochowdh
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 5ba8b0021a815f6c1ae329523741b7d536994ca1
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48071614"
---
# <a name="calendarpermission-resource-type"></a><span data-ttu-id="be82c-103">Тип ресурса Календарпермиссион</span><span class="sxs-lookup"><span data-stu-id="be82c-103">calendarPermission resource type</span></span>

<span data-ttu-id="be82c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="be82c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="be82c-105">Разрешения пользователя, к которому открыт общий доступ к календарю или который был делегирован в клиенте Outlook.</span><span class="sxs-lookup"><span data-stu-id="be82c-105">The permissions of a user with whom the calendar has been shared or delegated in an Outlook client.</span></span>

<span data-ttu-id="be82c-106">Получение, обновление и удаление разрешений календаря поддерживается только от имени владельца календаря.</span><span class="sxs-lookup"><span data-stu-id="be82c-106">Get, update, and delete of calendar permissions is supported on behalf of only the calendar owner.</span></span>

<span data-ttu-id="be82c-107">Получение разрешений календаря для календаря от имени объекта Share или делегата возвращает пустой набор разрешений календаря.</span><span class="sxs-lookup"><span data-stu-id="be82c-107">Getting the calendar permissions of a calendar on behalf of a sharee or delegate returns an empty calendar permissions collection.</span></span>

<span data-ttu-id="be82c-108">После настройки общего доступа или делегирования для календаря можно [Обновить](../api/calendarpermission-update.md) только свойство **Role** , чтобы изменить разрешения для общего доступа или делегата.</span><span class="sxs-lookup"><span data-stu-id="be82c-108">Once a sharee or delegate has been set up for a calendar, you can [update](../api/calendarpermission-update.md) only the **role** property to change the permissions of a sharee or delegate.</span></span> <span data-ttu-id="be82c-109">Невозможно **Обновить** свойства **алловедролес**, **EmailAddress**, **исинсидеорганизатион и**. **isRemovable**</span><span class="sxs-lookup"><span data-stu-id="be82c-109">You cannot **update** the **allowedRoles**, **emailAddress**, **isInsideOrganization**, or **isRemovable** property.</span></span> <span data-ttu-id="be82c-110">Чтобы изменить эти свойства, необходимо [Удалить](../api/calendarpermission-delete.md) соответствующий объект **календарпермиссион** и создать еще одну общую папку или делегат в клиенте Outlook.</span><span class="sxs-lookup"><span data-stu-id="be82c-110">To change these properties, you should [delete](../api/calendarpermission-delete.md) the corresponding **calendarPermission** object and create another sharee or delegate in an Outlook client.</span></span>

## <a name="methods"></a><span data-ttu-id="be82c-111">Методы</span><span class="sxs-lookup"><span data-stu-id="be82c-111">Methods</span></span>

| <span data-ttu-id="be82c-112">Метод</span><span class="sxs-lookup"><span data-stu-id="be82c-112">Method</span></span>       | <span data-ttu-id="be82c-113">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="be82c-113">Return Type</span></span> | <span data-ttu-id="be82c-114">Описание</span><span class="sxs-lookup"><span data-stu-id="be82c-114">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="be82c-115">Получение Календарпермиссион</span><span class="sxs-lookup"><span data-stu-id="be82c-115">Get calendarPermission</span></span>](../api/calendarpermission-get.md) | [<span data-ttu-id="be82c-116">календарпермиссион</span><span class="sxs-lookup"><span data-stu-id="be82c-116">calendarPermission</span></span>](calendarpermission.md) | <span data-ttu-id="be82c-117">Чтение свойств и связей объекта Календарпермиссион.</span><span class="sxs-lookup"><span data-stu-id="be82c-117">Read properties and relationships of calendarPermission object.</span></span> |
| [<span data-ttu-id="be82c-118">Обновление</span><span class="sxs-lookup"><span data-stu-id="be82c-118">Update</span></span>](../api/calendarpermission-update.md) | [<span data-ttu-id="be82c-119">календарпермиссион</span><span class="sxs-lookup"><span data-stu-id="be82c-119">calendarPermission</span></span>](calendarpermission.md) | <span data-ttu-id="be82c-120">Обновление объекта Календарпермиссион.</span><span class="sxs-lookup"><span data-stu-id="be82c-120">Update calendarPermission object.</span></span> |
| [<span data-ttu-id="be82c-121">Удаление</span><span class="sxs-lookup"><span data-stu-id="be82c-121">Delete</span></span>](../api/calendarpermission-delete.md) | <span data-ttu-id="be82c-122">Нет</span><span class="sxs-lookup"><span data-stu-id="be82c-122">None</span></span> | <span data-ttu-id="be82c-123">Удаление объекта Календарпермиссион.</span><span class="sxs-lookup"><span data-stu-id="be82c-123">Delete calendarPermission object.</span></span> |

## <a name="properties"></a><span data-ttu-id="be82c-124">Свойства</span><span class="sxs-lookup"><span data-stu-id="be82c-124">Properties</span></span>

| <span data-ttu-id="be82c-125">Свойство</span><span class="sxs-lookup"><span data-stu-id="be82c-125">Property</span></span>     | <span data-ttu-id="be82c-126">Тип</span><span class="sxs-lookup"><span data-stu-id="be82c-126">Type</span></span>        | <span data-ttu-id="be82c-127">Описание</span><span class="sxs-lookup"><span data-stu-id="be82c-127">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="be82c-128">алловедролес</span><span class="sxs-lookup"><span data-stu-id="be82c-128">allowedRoles</span></span>|<span data-ttu-id="be82c-129">Коллекция [календарролетипе](#calendarroletype-values)</span><span class="sxs-lookup"><span data-stu-id="be82c-129">[calendarRoleType](#calendarroletype-values) collection</span></span>| <span data-ttu-id="be82c-130">Список разрешенных для общего доступа или делегирования уровней разрешений для календаря.</span><span class="sxs-lookup"><span data-stu-id="be82c-130">List of allowed sharing or delegating permission levels for the calendar.</span></span> <span data-ttu-id="be82c-131">Возможные значения: `none`, `freeBusyRead`, `limitedRead`, `read`, `write`, `delegateWithoutPrivateEventAccess`, `delegateWithPrivateEventAccess`, `custom`.</span><span class="sxs-lookup"><span data-stu-id="be82c-131">Possible values are: `none`, `freeBusyRead`, `limitedRead`, `read`, `write`, `delegateWithoutPrivateEventAccess`, `delegateWithPrivateEventAccess`, `custom`.</span></span>|
|<span data-ttu-id="be82c-132">emailAddress</span><span class="sxs-lookup"><span data-stu-id="be82c-132">emailAddress</span></span>|[<span data-ttu-id="be82c-133">emailAddress</span><span class="sxs-lookup"><span data-stu-id="be82c-133">emailAddress</span></span>](emailaddress.md)| <span data-ttu-id="be82c-134">Представляет общий доступ или представитель, имеющий доступ к календарю.</span><span class="sxs-lookup"><span data-stu-id="be82c-134">Represents a sharee or delegate who has access to the calendar.</span></span> <span data-ttu-id="be82c-135">Для общего доступа к общему ресурсу "Моя организация" свойство **Address** имеет значение null.</span><span class="sxs-lookup"><span data-stu-id="be82c-135">For the "My Organization" sharee, the **address** property is null.</span></span> <span data-ttu-id="be82c-136">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="be82c-136">Read-only.</span></span> |
|<span data-ttu-id="be82c-137">id</span><span class="sxs-lookup"><span data-stu-id="be82c-137">id</span></span>|<span data-ttu-id="be82c-138">String</span><span class="sxs-lookup"><span data-stu-id="be82c-138">String</span></span>| <span data-ttu-id="be82c-139">Уникальный идентификатор пользователя (общего доступа или представителя), к которому открыт общий доступ к календарю.</span><span class="sxs-lookup"><span data-stu-id="be82c-139">The unique identifier of the user (sharee or delegate) with whom the calendar has been shared.</span></span> <span data-ttu-id="be82c-140">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="be82c-140">Read-only.</span></span>|
|<span data-ttu-id="be82c-141">исинсидеорганизатион</span><span class="sxs-lookup"><span data-stu-id="be82c-141">isInsideOrganization</span></span>|<span data-ttu-id="be82c-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="be82c-142">Boolean</span></span>| <span data-ttu-id="be82c-143">Имеет значение true, если пользователь в контексте (общий доступ или представитель) находится в той же организации, что и владелец календаря.</span><span class="sxs-lookup"><span data-stu-id="be82c-143">True if the user in context (sharee or delegate) is inside the same organization as the calendar owner.</span></span>|
|<span data-ttu-id="be82c-144">isRemovable</span><span class="sxs-lookup"><span data-stu-id="be82c-144">isRemovable</span></span>|<span data-ttu-id="be82c-145">Логический</span><span class="sxs-lookup"><span data-stu-id="be82c-145">Boolean</span></span>| <span data-ttu-id="be82c-146">`True` , если пользователь может быть удален из списка общих или делегатов для указанного календаря, `false` в противном случае.</span><span class="sxs-lookup"><span data-stu-id="be82c-146">`True` if the user can be removed from the list of sharees or delegates for the specified calendar, `false` otherwise.</span></span> <span data-ttu-id="be82c-147">Пользователь "Моя организация" определяет разрешения, которые пользователи в организации имеют в указанном календаре.</span><span class="sxs-lookup"><span data-stu-id="be82c-147">The "My organization" user determines the permissions other people within your organization have to the given calendar.</span></span> <span data-ttu-id="be82c-148">Вы не можете удалить "Моя организация" как общий доступ к календарю.</span><span class="sxs-lookup"><span data-stu-id="be82c-148">You cannot remove "My organization" as a sharee to a calendar.</span></span>|
|<span data-ttu-id="be82c-149">role</span><span class="sxs-lookup"><span data-stu-id="be82c-149">role</span></span>|[<span data-ttu-id="be82c-150">календарролетипе</span><span class="sxs-lookup"><span data-stu-id="be82c-150">calendarRoleType</span></span>](#calendarroletype-values)| <span data-ttu-id="be82c-151">Текущий уровень разрешений для общего доступа к календарю или представителем.</span><span class="sxs-lookup"><span data-stu-id="be82c-151">Current permission level of the calendar sharee or delegate.</span></span> |

### <a name="calendarroletype-values"></a><span data-ttu-id="be82c-152">значения Календарролетипе</span><span class="sxs-lookup"><span data-stu-id="be82c-152">calendarRoleType values</span></span>

| <span data-ttu-id="be82c-153">Значения</span><span class="sxs-lookup"><span data-stu-id="be82c-153">Values</span></span>        | <span data-ttu-id="be82c-154">Описание</span><span class="sxs-lookup"><span data-stu-id="be82c-154">Description</span></span> |
|:--------------|:------------|
| <span data-ttu-id="be82c-155">Нет</span><span class="sxs-lookup"><span data-stu-id="be82c-155">none</span></span> | <span data-ttu-id="be82c-156">Доступ к календарю для пользователя не предоставляется.</span><span class="sxs-lookup"><span data-stu-id="be82c-156">Calendar is not shared with the user.</span></span> |
| <span data-ttu-id="be82c-157">фрибусиреад</span><span class="sxs-lookup"><span data-stu-id="be82c-157">freeBusyRead</span></span> | <span data-ttu-id="be82c-158">Пользователь — это общий доступ, который может просматривать сведения о доступности владельца в календаре.</span><span class="sxs-lookup"><span data-stu-id="be82c-158">User is a sharee who can view free/busy status of the owner on the calendar.</span></span> |
| <span data-ttu-id="be82c-159">лимитедреад</span><span class="sxs-lookup"><span data-stu-id="be82c-159">limitedRead</span></span> | <span data-ttu-id="be82c-160">Пользователь предоставляет доступ к сведениям о доступности, а также заголовках и расположениях событий в календаре.</span><span class="sxs-lookup"><span data-stu-id="be82c-160">User is a sharee who can view free/busy status, and titles and locations of the events on the calendar.</span></span> |
| <span data-ttu-id="be82c-161">read</span><span class="sxs-lookup"><span data-stu-id="be82c-161">read</span></span> | <span data-ttu-id="be82c-162">Пользователь предоставляет общий доступ, который может просматривать все сведения о событиях в календаре, за исключением частных событий владельца.</span><span class="sxs-lookup"><span data-stu-id="be82c-162">User is a sharee who can view all the details of the events on the calendar, except for the owner's private events.</span></span> |
| <span data-ttu-id="be82c-163">write</span><span class="sxs-lookup"><span data-stu-id="be82c-163">write</span></span> | <span data-ttu-id="be82c-164">Пользователь — это общий доступ, который может просматривать все сведения (кроме частных событий) и изменять события в календаре.</span><span class="sxs-lookup"><span data-stu-id="be82c-164">User is a sharee who can view all the details (except for private events) and edit events on the calendar.</span></span> |
| <span data-ttu-id="be82c-165">делегатевисаутпривативентакцесс</span><span class="sxs-lookup"><span data-stu-id="be82c-165">delegateWithoutPrivateEventAccess</span></span> | <span data-ttu-id="be82c-166">Пользователь — это делегат с доступом для записи, но не может просматривать сведения о закрытых событиях владельца в календаре.</span><span class="sxs-lookup"><span data-stu-id="be82c-166">User is a delegate who has write access but cannot view information of the owner's private events on the calendar.</span></span> |
| <span data-ttu-id="be82c-167">делегатевиспривативентакцесс</span><span class="sxs-lookup"><span data-stu-id="be82c-167">delegateWithPrivateEventAccess</span></span> | <span data-ttu-id="be82c-168">Пользователь — это представитель, имеющий доступ на запись и позволяющий просматривать сведения о частных событиях владельца в календаре.</span><span class="sxs-lookup"><span data-stu-id="be82c-168">User is a delegate who has write access and can view information of the owner's private events on the calendar.</span></span> |
| <span data-ttu-id="be82c-169">собственный</span><span class="sxs-lookup"><span data-stu-id="be82c-169">custom</span></span> | <span data-ttu-id="be82c-170">Пользователь обладает пользовательскими разрешениями на доступ к календарю.</span><span class="sxs-lookup"><span data-stu-id="be82c-170">User has custom permissions to the calendar.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="be82c-171">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="be82c-171">JSON representation</span></span>

<span data-ttu-id="be82c-172">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="be82c-172">The following is a JSON representation of the resource.</span></span>

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


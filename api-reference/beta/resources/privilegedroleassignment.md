---
title: Тип ресурса privilegedRoleAssignment
description: 'Представляет назначение привилегированной ролей для определенного пользователя. '
localization_priority: Normal
ms.openlocfilehash: ec6bc34ecd56839c764592ff298475e8648f300b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27823319"
---
# <a name="privilegedroleassignment-resource-type"></a><span data-ttu-id="cd84a-103">Тип ресурса privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="cd84a-103">privilegedRoleAssignment resource type</span></span>

> <span data-ttu-id="cd84a-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="cd84a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cd84a-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cd84a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="cd84a-106">Представляет назначение привилегированной ролей для определенного пользователя.</span><span class="sxs-lookup"><span data-stu-id="cd84a-106">Represents a privileged role assignment for a particular user.</span></span> 


## <a name="methods"></a><span data-ttu-id="cd84a-107">Методы</span><span class="sxs-lookup"><span data-stu-id="cd84a-107">Methods</span></span>

| <span data-ttu-id="cd84a-108">Метод</span><span class="sxs-lookup"><span data-stu-id="cd84a-108">Method</span></span>           | <span data-ttu-id="cd84a-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="cd84a-109">Return Type</span></span>    |<span data-ttu-id="cd84a-110">Описание</span><span class="sxs-lookup"><span data-stu-id="cd84a-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="cd84a-111">Список privilegedRoleAssignment коллекции</span><span class="sxs-lookup"><span data-stu-id="cd84a-111">List privilegedRoleAssignment collection</span></span>](../api/privilegedroleassignment-list.md) | <span data-ttu-id="cd84a-112">[privilegedRoleAssignment](privilegedroleassignment.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="cd84a-112">[privilegedRoleAssignment](privilegedroleassignment.md) collection</span></span>|<span data-ttu-id="cd84a-113">Получите коллекцию объектов privilegedRoleAssignment.</span><span class="sxs-lookup"><span data-stu-id="cd84a-113">Get the collection of privilegedRoleAssignment objects.</span></span>|
|[<span data-ttu-id="cd84a-114">Получение privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="cd84a-114">Get privilegedRoleAssignment</span></span>](../api/privilegedroleassignment-get.md) | [<span data-ttu-id="cd84a-115">privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="cd84a-115">privilegedRoleAssignment</span></span>](privilegedroleassignment.md) |<span data-ttu-id="cd84a-116">Чтение свойства и связи объекта privilegedRoleAssignment.</span><span class="sxs-lookup"><span data-stu-id="cd84a-116">Read properties and relationships of privilegedRoleAssignment object.</span></span>|
|[<span data-ttu-id="cd84a-117">Создание назначения</span><span class="sxs-lookup"><span data-stu-id="cd84a-117">Create assignment</span></span>](../api/privilegedroleassignment-post-privilegedroleassignments.md) |[<span data-ttu-id="cd84a-118">privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="cd84a-118">privilegedRoleAssignment</span></span>](privilegedroleassignment.md)| <span data-ttu-id="cd84a-119">Создание нового назначения путем учета к коллекции назначений.</span><span class="sxs-lookup"><span data-stu-id="cd84a-119">Create a new assignment by posting to the assignments collection.</span></span>|
|[<span data-ttu-id="cd84a-120">Delete</span><span class="sxs-lookup"><span data-stu-id="cd84a-120">Delete</span></span>](../api/privilegedroleassignment-delete.md) | <span data-ttu-id="cd84a-121">Нет</span><span class="sxs-lookup"><span data-stu-id="cd84a-121">None</span></span> |<span data-ttu-id="cd84a-122">Удалите объект privilegedRoleAssignment.</span><span class="sxs-lookup"><span data-stu-id="cd84a-122">Delete privilegedRoleAssignment object.</span></span> |
|[<span data-ttu-id="cd84a-123">makePermanent</span><span class="sxs-lookup"><span data-stu-id="cd84a-123">makePermanent</span></span>](../api/privilegedroleassignment-makepermanent.md)|[<span data-ttu-id="cd84a-124">privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="cd84a-124">privilegedRoleAssignment</span></span>](privilegedroleassignment.md)|<span data-ttu-id="cd84a-125">Сделайте как постоянное назначение ролей.</span><span class="sxs-lookup"><span data-stu-id="cd84a-125">Make the role assignment as permanent.</span></span>|
|[<span data-ttu-id="cd84a-126">makeEligible</span><span class="sxs-lookup"><span data-stu-id="cd84a-126">makeEligible</span></span>](../api/privilegedroleassignment-makeeligible.md)|[<span data-ttu-id="cd84a-127">privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="cd84a-127">privilegedRoleAssignment</span></span>](privilegedroleassignment.md)|<span data-ttu-id="cd84a-128">Сделайте назначения ролей как подходящими.</span><span class="sxs-lookup"><span data-stu-id="cd84a-128">Make the role assignment as eligible.</span></span>|
|[<span data-ttu-id="cd84a-129">Мои</span><span class="sxs-lookup"><span data-stu-id="cd84a-129">my</span></span>](../api/privilegedroleassignment-my.md)|<span data-ttu-id="cd84a-130">[privilegedRoleAssignment](privilegedroleassignment.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="cd84a-130">[privilegedRoleAssignment](privilegedroleassignment.md) collection</span></span>|<span data-ttu-id="cd84a-131">Получение назначения привилегированной роли текущего пользователя.</span><span class="sxs-lookup"><span data-stu-id="cd84a-131">Get the current user's privileged role assignments.</span></span>|

## <a name="properties"></a><span data-ttu-id="cd84a-132">Свойства</span><span class="sxs-lookup"><span data-stu-id="cd84a-132">Properties</span></span>
| <span data-ttu-id="cd84a-133">Свойство</span><span class="sxs-lookup"><span data-stu-id="cd84a-133">Property</span></span>     | <span data-ttu-id="cd84a-134">Тип</span><span class="sxs-lookup"><span data-stu-id="cd84a-134">Type</span></span>   |<span data-ttu-id="cd84a-135">Описание</span><span class="sxs-lookup"><span data-stu-id="cd84a-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cd84a-136">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="cd84a-136">expirationDateTime</span></span>|<span data-ttu-id="cd84a-137">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cd84a-137">dateTimeOffset</span></span>|<span data-ttu-id="cd84a-138">Даты-времени UTC при истечет назначения временные привилегированной роли.</span><span class="sxs-lookup"><span data-stu-id="cd84a-138">The UTC DateTime when the temporary privileged role assignment will be expired.</span></span> <span data-ttu-id="cd84a-139">Для назначения постоянной роли значение null.</span><span class="sxs-lookup"><span data-stu-id="cd84a-139">For permanent role assignment, the value is null.</span></span>|
|<span data-ttu-id="cd84a-140">id</span><span class="sxs-lookup"><span data-stu-id="cd84a-140">id</span></span>|<span data-ttu-id="cd84a-141">строка</span><span class="sxs-lookup"><span data-stu-id="cd84a-141">string</span></span>| <span data-ttu-id="cd84a-142">Уникальный идентификатор для назначения привилегированной роли.</span><span class="sxs-lookup"><span data-stu-id="cd84a-142">The unique identifier for the privileged role assignment.</span></span> <span data-ttu-id="cd84a-143">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="cd84a-143">Read-only.</span></span> <span data-ttu-id="cd84a-144">Это в формате «userId_roleId», где идентификатор пользователя — это строка идентификатора GUID для Azure AD идентификатор пользователя, а roleId — string GUID для идентификатора роль Azure администратора.</span><span class="sxs-lookup"><span data-stu-id="cd84a-144">It is in the format of 'userId_roleId', where userId is the GUID string for Azure AD user id, and roleId is the GUID string for Azure administrator role id.</span></span>|
|<span data-ttu-id="cd84a-145">isElevated</span><span class="sxs-lookup"><span data-stu-id="cd84a-145">isElevated</span></span>|<span data-ttu-id="cd84a-146">boolean</span><span class="sxs-lookup"><span data-stu-id="cd84a-146">boolean</span></span>|<span data-ttu-id="cd84a-147">**значение true,** если активирован назначения ролей.</span><span class="sxs-lookup"><span data-stu-id="cd84a-147">**true** if the role assignment is activated.</span></span> <span data-ttu-id="cd84a-148">**значение false,** Если назначения ролей отключена.</span><span class="sxs-lookup"><span data-stu-id="cd84a-148">**false** if the role assignment is deactivated.</span></span>|
|<span data-ttu-id="cd84a-149">resultMessage</span><span class="sxs-lookup"><span data-stu-id="cd84a-149">resultMessage</span></span>|<span data-ttu-id="cd84a-150">string</span><span class="sxs-lookup"><span data-stu-id="cd84a-150">string</span></span>|<span data-ttu-id="cd84a-151">Установка службы сообщения результата.</span><span class="sxs-lookup"><span data-stu-id="cd84a-151">Result message set by the service.</span></span>|
|<span data-ttu-id="cd84a-152">roleId</span><span class="sxs-lookup"><span data-stu-id="cd84a-152">roleId</span></span>|<span data-ttu-id="cd84a-153">string</span><span class="sxs-lookup"><span data-stu-id="cd84a-153">string</span></span>|<span data-ttu-id="cd84a-154">Идентификатор роли.</span><span class="sxs-lookup"><span data-stu-id="cd84a-154">Role identifier.</span></span> <span data-ttu-id="cd84a-155">В строковом формате GUID.</span><span class="sxs-lookup"><span data-stu-id="cd84a-155">In GUID string format.</span></span>|
|<span data-ttu-id="cd84a-156">userId</span><span class="sxs-lookup"><span data-stu-id="cd84a-156">userId</span></span>|<span data-ttu-id="cd84a-157">string</span><span class="sxs-lookup"><span data-stu-id="cd84a-157">string</span></span>|<span data-ttu-id="cd84a-158">Идентификатор пользователя.</span><span class="sxs-lookup"><span data-stu-id="cd84a-158">User identifier.</span></span> <span data-ttu-id="cd84a-159">В строковом формате GUID.</span><span class="sxs-lookup"><span data-stu-id="cd84a-159">In GUID string format.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cd84a-160">Связи</span><span class="sxs-lookup"><span data-stu-id="cd84a-160">Relationships</span></span>
| <span data-ttu-id="cd84a-161">Связь</span><span class="sxs-lookup"><span data-stu-id="cd84a-161">Relationship</span></span> | <span data-ttu-id="cd84a-162">Тип</span><span class="sxs-lookup"><span data-stu-id="cd84a-162">Type</span></span>   |<span data-ttu-id="cd84a-163">Описание</span><span class="sxs-lookup"><span data-stu-id="cd84a-163">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cd84a-164">roleInfo</span><span class="sxs-lookup"><span data-stu-id="cd84a-164">roleInfo</span></span>|[<span data-ttu-id="cd84a-165">privilegedRole</span><span class="sxs-lookup"><span data-stu-id="cd84a-165">privilegedRole</span></span>](privilegedrole.md)| <span data-ttu-id="cd84a-166">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="cd84a-166">Read-only.</span></span> <span data-ttu-id="cd84a-167">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="cd84a-167">Nullable.</span></span> <span data-ttu-id="cd84a-168">Сведения о связанных ролей.</span><span class="sxs-lookup"><span data-stu-id="cd84a-168">The associated role information.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="cd84a-169">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="cd84a-169">JSON representation</span></span>

<span data-ttu-id="cd84a-170">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cd84a-170">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.privilegedRoleAssignment"
}-->

```json
{
  "expirationDateTime": "String (timestamp)",
  "id": "string (identifier)",
  "isElevated": true,
  "resultMessage": "string",
  "roleId": "string",
  "userId": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "privilegedRoleAssignment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

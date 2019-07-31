---
title: Тип ресурса Привилежедролеассигнмент
description: 'Представляет назначение привилегированной роли для определенного пользователя. '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 010dbf110de414e5221873263ffb5bcffe30db48
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36008882"
---
# <a name="privilegedroleassignment-resource-type"></a><span data-ttu-id="1edc2-103">Тип ресурса Привилежедролеассигнмент</span><span class="sxs-lookup"><span data-stu-id="1edc2-103">privilegedRoleAssignment resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1edc2-104">Представляет назначение привилегированной роли для определенного пользователя.</span><span class="sxs-lookup"><span data-stu-id="1edc2-104">Represents a privileged role assignment for a particular user.</span></span> 


## <a name="methods"></a><span data-ttu-id="1edc2-105">Методы</span><span class="sxs-lookup"><span data-stu-id="1edc2-105">Methods</span></span>

| <span data-ttu-id="1edc2-106">Метод</span><span class="sxs-lookup"><span data-stu-id="1edc2-106">Method</span></span>           | <span data-ttu-id="1edc2-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="1edc2-107">Return Type</span></span>    |<span data-ttu-id="1edc2-108">Описание</span><span class="sxs-lookup"><span data-stu-id="1edc2-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="1edc2-109">Коллекция Привилежедролеассигнмент списка</span><span class="sxs-lookup"><span data-stu-id="1edc2-109">List privilegedRoleAssignment collection</span></span>](../api/privilegedroleassignment-list.md) | <span data-ttu-id="1edc2-110">Коллекция [privilegedRoleAssignment](privilegedroleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="1edc2-110">[privilegedRoleAssignment](privilegedroleassignment.md) collection</span></span>|<span data-ttu-id="1edc2-111">Получение коллекции объектов Привилежедролеассигнмент.</span><span class="sxs-lookup"><span data-stu-id="1edc2-111">Get the collection of privilegedRoleAssignment objects.</span></span>|
|[<span data-ttu-id="1edc2-112">Получение privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="1edc2-112">Get privilegedRoleAssignment</span></span>](../api/privilegedroleassignment-get.md) | [<span data-ttu-id="1edc2-113">privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="1edc2-113">privilegedRoleAssignment</span></span>](privilegedroleassignment.md) |<span data-ttu-id="1edc2-114">Чтение свойств и связей объекта Привилежедролеассигнмент.</span><span class="sxs-lookup"><span data-stu-id="1edc2-114">Read properties and relationships of privilegedRoleAssignment object.</span></span>|
|[<span data-ttu-id="1edc2-115">Создание задания</span><span class="sxs-lookup"><span data-stu-id="1edc2-115">Create assignment</span></span>](../api/privilegedroleassignment-post-privilegedroleassignments.md) |[<span data-ttu-id="1edc2-116">privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="1edc2-116">privilegedRoleAssignment</span></span>](privilegedroleassignment.md)| <span data-ttu-id="1edc2-117">Создайте новое назначение путем публикации в коллекции назначений.</span><span class="sxs-lookup"><span data-stu-id="1edc2-117">Create a new assignment by posting to the assignments collection.</span></span>|
|[<span data-ttu-id="1edc2-118">Удаление</span><span class="sxs-lookup"><span data-stu-id="1edc2-118">Delete</span></span>](../api/privilegedroleassignment-delete.md) | <span data-ttu-id="1edc2-119">Нет</span><span class="sxs-lookup"><span data-stu-id="1edc2-119">None</span></span> |<span data-ttu-id="1edc2-120">Удаление объекта privilegedRoleAssignment.</span><span class="sxs-lookup"><span data-stu-id="1edc2-120">Delete privilegedRoleAssignment object.</span></span> |
|[<span data-ttu-id="1edc2-121">makePermanent</span><span class="sxs-lookup"><span data-stu-id="1edc2-121">makePermanent</span></span>](../api/privilegedroleassignment-makepermanent.md)|[<span data-ttu-id="1edc2-122">privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="1edc2-122">privilegedRoleAssignment</span></span>](privilegedroleassignment.md)|<span data-ttu-id="1edc2-123">Выполнение назначения ролей как бессрочного.</span><span class="sxs-lookup"><span data-stu-id="1edc2-123">Make the role assignment as permanent.</span></span>|
|[<span data-ttu-id="1edc2-124">makeEligible</span><span class="sxs-lookup"><span data-stu-id="1edc2-124">makeEligible</span></span>](../api/privilegedroleassignment-makeeligible.md)|[<span data-ttu-id="1edc2-125">privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="1edc2-125">privilegedRoleAssignment</span></span>](privilegedroleassignment.md)|<span data-ttu-id="1edc2-126">Выполнение назначения ролей как соответствующего требованиям.</span><span class="sxs-lookup"><span data-stu-id="1edc2-126">Make the role assignment as eligible.</span></span>|
|[<span data-ttu-id="1edc2-127">my</span><span class="sxs-lookup"><span data-stu-id="1edc2-127">my</span></span>](../api/privilegedroleassignment-my.md)|<span data-ttu-id="1edc2-128">Коллекция [privilegedRoleAssignment](privilegedroleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="1edc2-128">[privilegedRoleAssignment](privilegedroleassignment.md) collection</span></span>|<span data-ttu-id="1edc2-129">Получение привилегированных назначений ролей текущего пользователя.</span><span class="sxs-lookup"><span data-stu-id="1edc2-129">Get the current user's privileged role assignments.</span></span>|

## <a name="properties"></a><span data-ttu-id="1edc2-130">Свойства</span><span class="sxs-lookup"><span data-stu-id="1edc2-130">Properties</span></span>
| <span data-ttu-id="1edc2-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="1edc2-131">Property</span></span>     | <span data-ttu-id="1edc2-132">Тип</span><span class="sxs-lookup"><span data-stu-id="1edc2-132">Type</span></span>   |<span data-ttu-id="1edc2-133">Описание</span><span class="sxs-lookup"><span data-stu-id="1edc2-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1edc2-134">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="1edc2-134">expirationDateTime</span></span>|<span data-ttu-id="1edc2-135">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1edc2-135">dateTimeOffset</span></span>|<span data-ttu-id="1edc2-136">Дата и время в формате UTC, когда истечет срок действия назначения роли Temporary privileged.</span><span class="sxs-lookup"><span data-stu-id="1edc2-136">The UTC DateTime when the temporary privileged role assignment will be expired.</span></span> <span data-ttu-id="1edc2-137">Для назначения постоянной роли значение равно null.</span><span class="sxs-lookup"><span data-stu-id="1edc2-137">For permanent role assignment, the value is null.</span></span>|
|<span data-ttu-id="1edc2-138">id</span><span class="sxs-lookup"><span data-stu-id="1edc2-138">id</span></span>|<span data-ttu-id="1edc2-139">string</span><span class="sxs-lookup"><span data-stu-id="1edc2-139">string</span></span>| <span data-ttu-id="1edc2-140">Уникальный идентификатор для назначения привилегированной роли.</span><span class="sxs-lookup"><span data-stu-id="1edc2-140">The unique identifier for the privileged role assignment.</span></span> <span data-ttu-id="1edc2-141">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1edc2-141">Read-only.</span></span> <span data-ttu-id="1edc2-142">Он указан в формате "Усерид_ролеид", где userId — это строка GUID для идентификатора пользователя Azure AD, а roleId — строка GUID для идентификатора роли администратора Azure.</span><span class="sxs-lookup"><span data-stu-id="1edc2-142">It is in the format of 'userId_roleId', where userId is the GUID string for Azure AD user id, and roleId is the GUID string for Azure administrator role id.</span></span>|
|<span data-ttu-id="1edc2-143">Повышенный уровень</span><span class="sxs-lookup"><span data-stu-id="1edc2-143">isElevated</span></span>|<span data-ttu-id="1edc2-144">boolean</span><span class="sxs-lookup"><span data-stu-id="1edc2-144">boolean</span></span>|<span data-ttu-id="1edc2-145">**значение true** , если назначение роли активировано.</span><span class="sxs-lookup"><span data-stu-id="1edc2-145">**true** if the role assignment is activated.</span></span> <span data-ttu-id="1edc2-146">**значение false** , если назначение роли отключено.</span><span class="sxs-lookup"><span data-stu-id="1edc2-146">**false** if the role assignment is deactivated.</span></span>|
|<span data-ttu-id="1edc2-147">Ресултмессаже</span><span class="sxs-lookup"><span data-stu-id="1edc2-147">resultMessage</span></span>|<span data-ttu-id="1edc2-148">string</span><span class="sxs-lookup"><span data-stu-id="1edc2-148">string</span></span>|<span data-ttu-id="1edc2-149">Результирующее сообщение, заданное службой.</span><span class="sxs-lookup"><span data-stu-id="1edc2-149">Result message set by the service.</span></span>|
|<span data-ttu-id="1edc2-150">roleId</span><span class="sxs-lookup"><span data-stu-id="1edc2-150">roleId</span></span>|<span data-ttu-id="1edc2-151">string</span><span class="sxs-lookup"><span data-stu-id="1edc2-151">string</span></span>|<span data-ttu-id="1edc2-152">Идентификатор роли.</span><span class="sxs-lookup"><span data-stu-id="1edc2-152">Role identifier.</span></span> <span data-ttu-id="1edc2-153">В формате строки GUID.</span><span class="sxs-lookup"><span data-stu-id="1edc2-153">In GUID string format.</span></span>|
|<span data-ttu-id="1edc2-154">userId</span><span class="sxs-lookup"><span data-stu-id="1edc2-154">userId</span></span>|<span data-ttu-id="1edc2-155">string</span><span class="sxs-lookup"><span data-stu-id="1edc2-155">string</span></span>|<span data-ttu-id="1edc2-156">Идентификатор пользователя.</span><span class="sxs-lookup"><span data-stu-id="1edc2-156">User identifier.</span></span> <span data-ttu-id="1edc2-157">В формате строки GUID.</span><span class="sxs-lookup"><span data-stu-id="1edc2-157">In GUID string format.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1edc2-158">Отношения</span><span class="sxs-lookup"><span data-stu-id="1edc2-158">Relationships</span></span>
| <span data-ttu-id="1edc2-159">Отношение</span><span class="sxs-lookup"><span data-stu-id="1edc2-159">Relationship</span></span> | <span data-ttu-id="1edc2-160">Тип</span><span class="sxs-lookup"><span data-stu-id="1edc2-160">Type</span></span>   |<span data-ttu-id="1edc2-161">Описание</span><span class="sxs-lookup"><span data-stu-id="1edc2-161">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1edc2-162">Ролеинфо</span><span class="sxs-lookup"><span data-stu-id="1edc2-162">roleInfo</span></span>|[<span data-ttu-id="1edc2-163">privilegedRole</span><span class="sxs-lookup"><span data-stu-id="1edc2-163">privilegedRole</span></span>](privilegedrole.md)| <span data-ttu-id="1edc2-164">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1edc2-164">Read-only.</span></span> <span data-ttu-id="1edc2-165">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="1edc2-165">Nullable.</span></span> <span data-ttu-id="1edc2-166">Сведения о связанной роли.</span><span class="sxs-lookup"><span data-stu-id="1edc2-166">The associated role information.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1edc2-167">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1edc2-167">JSON representation</span></span>

<span data-ttu-id="1edc2-168">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1edc2-168">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity",
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
<!--
{
  "type": "#page.annotation",
  "description": "privilegedRoleAssignment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

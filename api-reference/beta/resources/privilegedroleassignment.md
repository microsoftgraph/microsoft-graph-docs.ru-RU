---
title: Тип ресурса Привилежедролеассигнмент
description: 'Представляет назначение привилегированной роли для определенного пользователя. '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: shauliu
ms.openlocfilehash: aef2b3962601a20df30f27c19ccd1abf23b0c561
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/10/2020
ms.locfileid: "43217906"
---
# <a name="privilegedroleassignment-resource-type"></a><span data-ttu-id="b07cc-103">Тип ресурса Привилежедролеассигнмент</span><span class="sxs-lookup"><span data-stu-id="b07cc-103">privilegedRoleAssignment resource type</span></span>

<span data-ttu-id="b07cc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b07cc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b07cc-105">Представляет назначение привилегированной роли для определенного пользователя.</span><span class="sxs-lookup"><span data-stu-id="b07cc-105">Represents a privileged role assignment for a particular user.</span></span> 


## <a name="methods"></a><span data-ttu-id="b07cc-106">Методы</span><span class="sxs-lookup"><span data-stu-id="b07cc-106">Methods</span></span>

| <span data-ttu-id="b07cc-107">Метод</span><span class="sxs-lookup"><span data-stu-id="b07cc-107">Method</span></span>           | <span data-ttu-id="b07cc-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="b07cc-108">Return Type</span></span>    |<span data-ttu-id="b07cc-109">Описание</span><span class="sxs-lookup"><span data-stu-id="b07cc-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b07cc-110">Коллекция Привилежедролеассигнмент списка</span><span class="sxs-lookup"><span data-stu-id="b07cc-110">List privilegedRoleAssignment collection</span></span>](../api/privilegedroleassignment-list.md) | <span data-ttu-id="b07cc-111">Коллекция [privilegedRoleAssignment](privilegedroleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="b07cc-111">[privilegedRoleAssignment](privilegedroleassignment.md) collection</span></span>|<span data-ttu-id="b07cc-112">Получение коллекции объектов Привилежедролеассигнмент.</span><span class="sxs-lookup"><span data-stu-id="b07cc-112">Get the collection of privilegedRoleAssignment objects.</span></span>|
|[<span data-ttu-id="b07cc-113">Получение privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="b07cc-113">Get privilegedRoleAssignment</span></span>](../api/privilegedroleassignment-get.md) | [<span data-ttu-id="b07cc-114">privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="b07cc-114">privilegedRoleAssignment</span></span>](privilegedroleassignment.md) |<span data-ttu-id="b07cc-115">Чтение свойств и связей объекта Привилежедролеассигнмент.</span><span class="sxs-lookup"><span data-stu-id="b07cc-115">Read properties and relationships of privilegedRoleAssignment object.</span></span>|
|[<span data-ttu-id="b07cc-116">Создание задания</span><span class="sxs-lookup"><span data-stu-id="b07cc-116">Create assignment</span></span>](../api/privilegedroleassignment-post-privilegedroleassignments.md) |[<span data-ttu-id="b07cc-117">privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="b07cc-117">privilegedRoleAssignment</span></span>](privilegedroleassignment.md)| <span data-ttu-id="b07cc-118">Создайте новое назначение путем публикации в коллекции назначений.</span><span class="sxs-lookup"><span data-stu-id="b07cc-118">Create a new assignment by posting to the assignments collection.</span></span>|
|<span data-ttu-id="b07cc-119">[удаление](../api/privilegedroleassignment-delete.md);</span><span class="sxs-lookup"><span data-stu-id="b07cc-119">[Delete](../api/privilegedroleassignment-delete.md)</span></span> | <span data-ttu-id="b07cc-120">Нет</span><span class="sxs-lookup"><span data-stu-id="b07cc-120">None</span></span> |<span data-ttu-id="b07cc-121">Удаление объекта privilegedRoleAssignment.</span><span class="sxs-lookup"><span data-stu-id="b07cc-121">Delete privilegedRoleAssignment object.</span></span> |
|[<span data-ttu-id="b07cc-122">makePermanent</span><span class="sxs-lookup"><span data-stu-id="b07cc-122">makePermanent</span></span>](../api/privilegedroleassignment-makepermanent.md)|[<span data-ttu-id="b07cc-123">privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="b07cc-123">privilegedRoleAssignment</span></span>](privilegedroleassignment.md)|<span data-ttu-id="b07cc-124">Выполнение назначения ролей как бессрочного.</span><span class="sxs-lookup"><span data-stu-id="b07cc-124">Make the role assignment as permanent.</span></span>|
|[<span data-ttu-id="b07cc-125">makeEligible</span><span class="sxs-lookup"><span data-stu-id="b07cc-125">makeEligible</span></span>](../api/privilegedroleassignment-makeeligible.md)|[<span data-ttu-id="b07cc-126">privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="b07cc-126">privilegedRoleAssignment</span></span>](privilegedroleassignment.md)|<span data-ttu-id="b07cc-127">Выполнение назначения ролей как соответствующего требованиям.</span><span class="sxs-lookup"><span data-stu-id="b07cc-127">Make the role assignment as eligible.</span></span>|
|[<span data-ttu-id="b07cc-128">my</span><span class="sxs-lookup"><span data-stu-id="b07cc-128">my</span></span>](../api/privilegedroleassignment-my.md)|<span data-ttu-id="b07cc-129">Коллекция [privilegedRoleAssignment](privilegedroleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="b07cc-129">[privilegedRoleAssignment](privilegedroleassignment.md) collection</span></span>|<span data-ttu-id="b07cc-130">Получение привилегированных назначений ролей текущего пользователя.</span><span class="sxs-lookup"><span data-stu-id="b07cc-130">Get the current user's privileged role assignments.</span></span>|

## <a name="properties"></a><span data-ttu-id="b07cc-131">Свойства</span><span class="sxs-lookup"><span data-stu-id="b07cc-131">Properties</span></span>
| <span data-ttu-id="b07cc-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="b07cc-132">Property</span></span>     | <span data-ttu-id="b07cc-133">Тип</span><span class="sxs-lookup"><span data-stu-id="b07cc-133">Type</span></span>   |<span data-ttu-id="b07cc-134">Описание</span><span class="sxs-lookup"><span data-stu-id="b07cc-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b07cc-135">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="b07cc-135">expirationDateTime</span></span>|<span data-ttu-id="b07cc-136">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b07cc-136">dateTimeOffset</span></span>|<span data-ttu-id="b07cc-137">Дата и время в формате UTC, когда истечет срок действия назначения роли Temporary privileged.</span><span class="sxs-lookup"><span data-stu-id="b07cc-137">The UTC DateTime when the temporary privileged role assignment will be expired.</span></span> <span data-ttu-id="b07cc-138">Для назначения постоянной роли значение равно null.</span><span class="sxs-lookup"><span data-stu-id="b07cc-138">For permanent role assignment, the value is null.</span></span>|
|<span data-ttu-id="b07cc-139">id</span><span class="sxs-lookup"><span data-stu-id="b07cc-139">id</span></span>|<span data-ttu-id="b07cc-140">string</span><span class="sxs-lookup"><span data-stu-id="b07cc-140">string</span></span>| <span data-ttu-id="b07cc-141">Уникальный идентификатор для назначения привилегированной роли.</span><span class="sxs-lookup"><span data-stu-id="b07cc-141">The unique identifier for the privileged role assignment.</span></span> <span data-ttu-id="b07cc-142">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b07cc-142">Read-only.</span></span> <span data-ttu-id="b07cc-143">Он имеет формат "userId_roleId", где userId — это строка GUID для идентификатора пользователя Azure AD, а roleId — строка GUID для идентификатора роли администратора Azure.</span><span class="sxs-lookup"><span data-stu-id="b07cc-143">It is in the format of 'userId_roleId', where userId is the GUID string for Azure AD user id, and roleId is the GUID string for Azure administrator role id.</span></span>|
|<span data-ttu-id="b07cc-144">Повышенный уровень</span><span class="sxs-lookup"><span data-stu-id="b07cc-144">isElevated</span></span>|<span data-ttu-id="b07cc-145">boolean</span><span class="sxs-lookup"><span data-stu-id="b07cc-145">boolean</span></span>|<span data-ttu-id="b07cc-146">**значение true** , если назначение роли активировано.</span><span class="sxs-lookup"><span data-stu-id="b07cc-146">**true** if the role assignment is activated.</span></span> <span data-ttu-id="b07cc-147">**значение false** , если назначение роли отключено.</span><span class="sxs-lookup"><span data-stu-id="b07cc-147">**false** if the role assignment is deactivated.</span></span>|
|<span data-ttu-id="b07cc-148">ресултмессаже</span><span class="sxs-lookup"><span data-stu-id="b07cc-148">resultMessage</span></span>|<span data-ttu-id="b07cc-149">string</span><span class="sxs-lookup"><span data-stu-id="b07cc-149">string</span></span>|<span data-ttu-id="b07cc-150">Результирующее сообщение, заданное службой.</span><span class="sxs-lookup"><span data-stu-id="b07cc-150">Result message set by the service.</span></span>|
|<span data-ttu-id="b07cc-151">roleId</span><span class="sxs-lookup"><span data-stu-id="b07cc-151">roleId</span></span>|<span data-ttu-id="b07cc-152">string</span><span class="sxs-lookup"><span data-stu-id="b07cc-152">string</span></span>|<span data-ttu-id="b07cc-153">Идентификатор роли.</span><span class="sxs-lookup"><span data-stu-id="b07cc-153">Role identifier.</span></span> <span data-ttu-id="b07cc-154">В формате строки GUID.</span><span class="sxs-lookup"><span data-stu-id="b07cc-154">In GUID string format.</span></span>|
|<span data-ttu-id="b07cc-155">userId</span><span class="sxs-lookup"><span data-stu-id="b07cc-155">userId</span></span>|<span data-ttu-id="b07cc-156">строка</span><span class="sxs-lookup"><span data-stu-id="b07cc-156">string</span></span>|<span data-ttu-id="b07cc-157">Идентификатор пользователя.</span><span class="sxs-lookup"><span data-stu-id="b07cc-157">User identifier.</span></span> <span data-ttu-id="b07cc-158">В формате строки GUID.</span><span class="sxs-lookup"><span data-stu-id="b07cc-158">In GUID string format.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b07cc-159">Связи</span><span class="sxs-lookup"><span data-stu-id="b07cc-159">Relationships</span></span>
| <span data-ttu-id="b07cc-160">Связь</span><span class="sxs-lookup"><span data-stu-id="b07cc-160">Relationship</span></span> | <span data-ttu-id="b07cc-161">Тип</span><span class="sxs-lookup"><span data-stu-id="b07cc-161">Type</span></span>   |<span data-ttu-id="b07cc-162">Описание</span><span class="sxs-lookup"><span data-stu-id="b07cc-162">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b07cc-163">ролеинфо</span><span class="sxs-lookup"><span data-stu-id="b07cc-163">roleInfo</span></span>|[<span data-ttu-id="b07cc-164">privilegedRole</span><span class="sxs-lookup"><span data-stu-id="b07cc-164">privilegedRole</span></span>](privilegedrole.md)| <span data-ttu-id="b07cc-165">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b07cc-165">Read-only.</span></span> <span data-ttu-id="b07cc-166">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="b07cc-166">Nullable.</span></span> <span data-ttu-id="b07cc-167">Сведения о связанной роли.</span><span class="sxs-lookup"><span data-stu-id="b07cc-167">The associated role information.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b07cc-168">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b07cc-168">JSON representation</span></span>

<span data-ttu-id="b07cc-169">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b07cc-169">Here is a JSON representation of the resource.</span></span>

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

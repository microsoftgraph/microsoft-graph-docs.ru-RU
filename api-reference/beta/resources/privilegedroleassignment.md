---
title: тип ресурса privilegedRoleAssignment
description: 'Представляет привилегированное назначение роли для конкретного пользователя. '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: 55b37c195777659b172e668d4e02b60de4f78c0d
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50440166"
---
# <a name="privilegedroleassignment-resource-type"></a><span data-ttu-id="5bd9e-103">тип ресурса privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="5bd9e-103">privilegedRoleAssignment resource type</span></span>

<span data-ttu-id="5bd9e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5bd9e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5bd9e-105">Представляет привилегированное назначение роли для конкретного пользователя.</span><span class="sxs-lookup"><span data-stu-id="5bd9e-105">Represents a privileged role assignment for a particular user.</span></span> 


## <a name="methods"></a><span data-ttu-id="5bd9e-106">Методы</span><span class="sxs-lookup"><span data-stu-id="5bd9e-106">Methods</span></span>

| <span data-ttu-id="5bd9e-107">Метод</span><span class="sxs-lookup"><span data-stu-id="5bd9e-107">Method</span></span>           | <span data-ttu-id="5bd9e-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="5bd9e-108">Return Type</span></span>    |<span data-ttu-id="5bd9e-109">Описание</span><span class="sxs-lookup"><span data-stu-id="5bd9e-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="5bd9e-110">Список коллекции privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="5bd9e-110">List privilegedRoleAssignment collection</span></span>](../api/privilegedroleassignment-list.md) | <span data-ttu-id="5bd9e-111">Коллекция [privilegedRoleAssignment](privilegedroleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="5bd9e-111">[privilegedRoleAssignment](privilegedroleassignment.md) collection</span></span>|<span data-ttu-id="5bd9e-112">Получите коллекцию объектов privilegedRoleAssignment.</span><span class="sxs-lookup"><span data-stu-id="5bd9e-112">Get the collection of privilegedRoleAssignment objects.</span></span>|
|[<span data-ttu-id="5bd9e-113">Получение privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="5bd9e-113">Get privilegedRoleAssignment</span></span>](../api/privilegedroleassignment-get.md) | [<span data-ttu-id="5bd9e-114">privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="5bd9e-114">privilegedRoleAssignment</span></span>](privilegedroleassignment.md) |<span data-ttu-id="5bd9e-115">Чтение свойств и связей объекта privilegedRoleAssignment.</span><span class="sxs-lookup"><span data-stu-id="5bd9e-115">Read properties and relationships of privilegedRoleAssignment object.</span></span>|
|[<span data-ttu-id="5bd9e-116">Создание задания</span><span class="sxs-lookup"><span data-stu-id="5bd9e-116">Create assignment</span></span>](../api/privilegedroleassignment-post-privilegedroleassignments.md) |[<span data-ttu-id="5bd9e-117">privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="5bd9e-117">privilegedRoleAssignment</span></span>](privilegedroleassignment.md)| <span data-ttu-id="5bd9e-118">Создайте новое назначение, разместив в коллекции назначений.</span><span class="sxs-lookup"><span data-stu-id="5bd9e-118">Create a new assignment by posting to the assignments collection.</span></span>|
|<span data-ttu-id="5bd9e-119">[удаление](../api/privilegedroleassignment-delete.md);</span><span class="sxs-lookup"><span data-stu-id="5bd9e-119">[Delete](../api/privilegedroleassignment-delete.md)</span></span> | <span data-ttu-id="5bd9e-120">Нет</span><span class="sxs-lookup"><span data-stu-id="5bd9e-120">None</span></span> |<span data-ttu-id="5bd9e-121">Удаление объекта privilegedRoleAssignment.</span><span class="sxs-lookup"><span data-stu-id="5bd9e-121">Delete privilegedRoleAssignment object.</span></span> |
|[<span data-ttu-id="5bd9e-122">makePermanent</span><span class="sxs-lookup"><span data-stu-id="5bd9e-122">makePermanent</span></span>](../api/privilegedroleassignment-makepermanent.md)|[<span data-ttu-id="5bd9e-123">privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="5bd9e-123">privilegedRoleAssignment</span></span>](privilegedroleassignment.md)|<span data-ttu-id="5bd9e-124">Выполнение назначения ролей как бессрочного.</span><span class="sxs-lookup"><span data-stu-id="5bd9e-124">Make the role assignment as permanent.</span></span>|
|[<span data-ttu-id="5bd9e-125">makeEligible</span><span class="sxs-lookup"><span data-stu-id="5bd9e-125">makeEligible</span></span>](../api/privilegedroleassignment-makeeligible.md)|[<span data-ttu-id="5bd9e-126">privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="5bd9e-126">privilegedRoleAssignment</span></span>](privilegedroleassignment.md)|<span data-ttu-id="5bd9e-127">Выполнение назначения ролей как соответствующего требованиям.</span><span class="sxs-lookup"><span data-stu-id="5bd9e-127">Make the role assignment as eligible.</span></span>|
|[<span data-ttu-id="5bd9e-128">my</span><span class="sxs-lookup"><span data-stu-id="5bd9e-128">my</span></span>](../api/privilegedroleassignment-my.md)|<span data-ttu-id="5bd9e-129">Коллекция [privilegedRoleAssignment](privilegedroleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="5bd9e-129">[privilegedRoleAssignment](privilegedroleassignment.md) collection</span></span>|<span data-ttu-id="5bd9e-130">Получите привилегированные назначения ролей текущего пользователя.</span><span class="sxs-lookup"><span data-stu-id="5bd9e-130">Get the current user's privileged role assignments.</span></span>|

## <a name="properties"></a><span data-ttu-id="5bd9e-131">Свойства</span><span class="sxs-lookup"><span data-stu-id="5bd9e-131">Properties</span></span>
| <span data-ttu-id="5bd9e-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="5bd9e-132">Property</span></span>     | <span data-ttu-id="5bd9e-133">Тип</span><span class="sxs-lookup"><span data-stu-id="5bd9e-133">Type</span></span>   |<span data-ttu-id="5bd9e-134">Описание</span><span class="sxs-lookup"><span data-stu-id="5bd9e-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5bd9e-135">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="5bd9e-135">expirationDateTime</span></span>|<span data-ttu-id="5bd9e-136">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5bd9e-136">dateTimeOffset</span></span>|<span data-ttu-id="5bd9e-137">Время даты UTC, когда истекает срок действия временного назначения привилегированных ролей.</span><span class="sxs-lookup"><span data-stu-id="5bd9e-137">The UTC DateTime when the temporary privileged role assignment will be expired.</span></span> <span data-ttu-id="5bd9e-138">Для назначения постоянных ролей значение null.</span><span class="sxs-lookup"><span data-stu-id="5bd9e-138">For permanent role assignment, the value is null.</span></span>|
|<span data-ttu-id="5bd9e-139">id</span><span class="sxs-lookup"><span data-stu-id="5bd9e-139">id</span></span>|<span data-ttu-id="5bd9e-140">string</span><span class="sxs-lookup"><span data-stu-id="5bd9e-140">string</span></span>| <span data-ttu-id="5bd9e-141">Уникальный идентификатор для назначения привилегированных ролей.</span><span class="sxs-lookup"><span data-stu-id="5bd9e-141">The unique identifier for the privileged role assignment.</span></span> <span data-ttu-id="5bd9e-142">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5bd9e-142">Read-only.</span></span> <span data-ttu-id="5bd9e-143">Он находится в формате "userId_roleId", где userId — это строка GUID для пользовательского id azure AD, а roleId — строка GUID для id роли администратора Azure.</span><span class="sxs-lookup"><span data-stu-id="5bd9e-143">It is in the format of 'userId_roleId', where userId is the GUID string for Azure AD user id, and roleId is the GUID string for Azure administrator role id.</span></span>|
|<span data-ttu-id="5bd9e-144">isElevated</span><span class="sxs-lookup"><span data-stu-id="5bd9e-144">isElevated</span></span>|<span data-ttu-id="5bd9e-145">boolean</span><span class="sxs-lookup"><span data-stu-id="5bd9e-145">boolean</span></span>|<span data-ttu-id="5bd9e-146">**значение true,** если назначение роли активировано.</span><span class="sxs-lookup"><span data-stu-id="5bd9e-146">**true** if the role assignment is activated.</span></span> <span data-ttu-id="5bd9e-147">**false,** если назначение роли отключено.</span><span class="sxs-lookup"><span data-stu-id="5bd9e-147">**false** if the role assignment is deactivated.</span></span>|
|<span data-ttu-id="5bd9e-148">resultMessage</span><span class="sxs-lookup"><span data-stu-id="5bd9e-148">resultMessage</span></span>|<span data-ttu-id="5bd9e-149">string</span><span class="sxs-lookup"><span data-stu-id="5bd9e-149">string</span></span>|<span data-ttu-id="5bd9e-150">Сообщение результатов, за набором службы.</span><span class="sxs-lookup"><span data-stu-id="5bd9e-150">Result message set by the service.</span></span>|
|<span data-ttu-id="5bd9e-151">roleId</span><span class="sxs-lookup"><span data-stu-id="5bd9e-151">roleId</span></span>|<span data-ttu-id="5bd9e-152">string</span><span class="sxs-lookup"><span data-stu-id="5bd9e-152">string</span></span>|<span data-ttu-id="5bd9e-153">Идентификатор роли.</span><span class="sxs-lookup"><span data-stu-id="5bd9e-153">Role identifier.</span></span> <span data-ttu-id="5bd9e-154">В формате строк GUID.</span><span class="sxs-lookup"><span data-stu-id="5bd9e-154">In GUID string format.</span></span>|
|<span data-ttu-id="5bd9e-155">userId</span><span class="sxs-lookup"><span data-stu-id="5bd9e-155">userId</span></span>|<span data-ttu-id="5bd9e-156">строка</span><span class="sxs-lookup"><span data-stu-id="5bd9e-156">string</span></span>|<span data-ttu-id="5bd9e-157">Идентификатор пользователя.</span><span class="sxs-lookup"><span data-stu-id="5bd9e-157">User identifier.</span></span> <span data-ttu-id="5bd9e-158">В формате строк GUID.</span><span class="sxs-lookup"><span data-stu-id="5bd9e-158">In GUID string format.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5bd9e-159">Связи</span><span class="sxs-lookup"><span data-stu-id="5bd9e-159">Relationships</span></span>
| <span data-ttu-id="5bd9e-160">Связь</span><span class="sxs-lookup"><span data-stu-id="5bd9e-160">Relationship</span></span> | <span data-ttu-id="5bd9e-161">Тип</span><span class="sxs-lookup"><span data-stu-id="5bd9e-161">Type</span></span>   |<span data-ttu-id="5bd9e-162">Описание</span><span class="sxs-lookup"><span data-stu-id="5bd9e-162">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5bd9e-163">roleInfo</span><span class="sxs-lookup"><span data-stu-id="5bd9e-163">roleInfo</span></span>|[<span data-ttu-id="5bd9e-164">privilegedRole</span><span class="sxs-lookup"><span data-stu-id="5bd9e-164">privilegedRole</span></span>](privilegedrole.md)| <span data-ttu-id="5bd9e-165">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5bd9e-165">Read-only.</span></span> <span data-ttu-id="5bd9e-166">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="5bd9e-166">Nullable.</span></span> <span data-ttu-id="5bd9e-167">Связанные сведения о роли.</span><span class="sxs-lookup"><span data-stu-id="5bd9e-167">The associated role information.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5bd9e-168">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5bd9e-168">JSON representation</span></span>

<span data-ttu-id="5bd9e-169">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5bd9e-169">Here is a JSON representation of the resource.</span></span>

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



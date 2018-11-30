---
title: Тип ресурса appRoleAssignment
description: Используется для записи, когда пользователь или группа назначается приложения. В этом случае назначения роли приведет к плитки приложения отображается вверх на панели приложения доступа пользователя. Этот объект также могут быть использованы для предоставления другого приложения (смоделирован как основной службы) доступа к приложению ресурсов в определенной роли. Можно создавать, читать, обновление и удаление назначения ролей.
ms.openlocfilehash: 97155bde12735ebd8a7674e0dbf20dae30e53f14
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27076270"
---
# <a name="approleassignment-resource-type"></a><span data-ttu-id="8cc90-106">Тип ресурса appRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="8cc90-106">appRoleAssignment resource type</span></span>

> <span data-ttu-id="8cc90-107">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="8cc90-107">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8cc90-108">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8cc90-108">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8cc90-109">Используется для записи, когда пользователь или группа назначается приложения.</span><span class="sxs-lookup"><span data-stu-id="8cc90-109">Used to record when a user or group is assigned to an application.</span></span> <span data-ttu-id="8cc90-110">В этом случае назначения роли приведет к плитки приложения отображается вверх на панели приложения доступа пользователя.</span><span class="sxs-lookup"><span data-stu-id="8cc90-110">In this case, the role assignment will result in an application tile showing up on the user's app access panel.</span></span> <span data-ttu-id="8cc90-111">Этот объект также могут быть использованы для предоставления другого приложения (смоделирован как основной службы) доступа к приложению ресурсов в определенной роли.</span><span class="sxs-lookup"><span data-stu-id="8cc90-111">This entity may also be used to grant another application (modeled as a service principal) access to a resource application in a particular role.</span></span> <span data-ttu-id="8cc90-112">Можно создавать, читать, обновление и удаление назначения ролей.</span><span class="sxs-lookup"><span data-stu-id="8cc90-112">You can create, read, update, and delete role assignments.</span></span>


## <a name="json-representation"></a><span data-ttu-id="8cc90-113">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8cc90-113">JSON representation</span></span>

<span data-ttu-id="8cc90-114">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="8cc90-114">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.approleassignment"
}-->

```json
{
  "creationTimestamp": "String (timestamp)",
  "id": "guid (identifier)",
  "principalDisplayName": "string",
  "principalId": "guid",
  "principalType": "string",
  "resourceDisplayName": "string",
  "resourceId": "guid"
}

```
## <a name="properties"></a><span data-ttu-id="8cc90-115">Свойства</span><span class="sxs-lookup"><span data-stu-id="8cc90-115">Properties</span></span>
| <span data-ttu-id="8cc90-116">Свойство</span><span class="sxs-lookup"><span data-stu-id="8cc90-116">Property</span></span>     | <span data-ttu-id="8cc90-117">Тип</span><span class="sxs-lookup"><span data-stu-id="8cc90-117">Type</span></span>   |<span data-ttu-id="8cc90-118">Description</span><span class="sxs-lookup"><span data-stu-id="8cc90-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8cc90-119">creationTimestamp</span><span class="sxs-lookup"><span data-stu-id="8cc90-119">creationTimestamp</span></span>|<span data-ttu-id="8cc90-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8cc90-120">DateTimeOffset</span></span>|<span data-ttu-id="8cc90-121">Время создания разрешений. Тип метки времени представляет сведения даты и времени с использованием формата ISO 8601 и — это всегда в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="8cc90-121">The time when the grant was created.The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="8cc90-122">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="8cc90-122">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="8cc90-123">id</span><span class="sxs-lookup"><span data-stu-id="8cc90-123">id</span></span>|<span data-ttu-id="8cc90-124">Guid</span><span class="sxs-lookup"><span data-stu-id="8cc90-124">Guid</span></span>|<span data-ttu-id="8cc90-125">Идентификатор роли, которая была назначена субъекта.</span><span class="sxs-lookup"><span data-stu-id="8cc90-125">The role id that was assigned to the principal.</span></span>  <span data-ttu-id="8cc90-126">Эта роль должны быть объявлены с приложения ресурсов конечного **Ид_ресурса** в своем свойстве **appRoles** .</span><span class="sxs-lookup"><span data-stu-id="8cc90-126">This role must be declared by the target resource application **resourceId** in its **appRoles** property.</span></span> <span data-ttu-id="8cc90-127">Где ресурса не объявляет никаких разрешений, должен быть указан идентификатор по умолчанию (нулевое значение GUID).</span><span class="sxs-lookup"><span data-stu-id="8cc90-127">Where the resource does not declare any permissions, a default id (zero GUID) must be specified.</span></span> <span data-ttu-id="8cc90-128">Ключ.</span><span class="sxs-lookup"><span data-stu-id="8cc90-128">Key.</span></span> <span data-ttu-id="8cc90-129">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="8cc90-129">Not nullable.</span></span> |
|<span data-ttu-id="8cc90-130">principalDisplayName</span><span class="sxs-lookup"><span data-stu-id="8cc90-130">principalDisplayName</span></span>|<span data-ttu-id="8cc90-131">String</span><span class="sxs-lookup"><span data-stu-id="8cc90-131">String</span></span>|<span data-ttu-id="8cc90-132">Отображаемое имя субъекта, который был предоставлен доступ.</span><span class="sxs-lookup"><span data-stu-id="8cc90-132">The display name of the principal that was granted the access.</span></span>|
|<span data-ttu-id="8cc90-133">principalId</span><span class="sxs-lookup"><span data-stu-id="8cc90-133">principalId</span></span>|<span data-ttu-id="8cc90-134">Guid</span><span class="sxs-lookup"><span data-stu-id="8cc90-134">Guid</span></span>|<span data-ttu-id="8cc90-135">Уникальный идентификатор (**id**) для участника, которому предоставляется доступ.</span><span class="sxs-lookup"><span data-stu-id="8cc90-135">The unique identifier (**id**) for the principal being granted the access.</span></span> <span data-ttu-id="8cc90-136">Требуется при создании.</span><span class="sxs-lookup"><span data-stu-id="8cc90-136">Required on create.</span></span>            |
|<span data-ttu-id="8cc90-137">principalType</span><span class="sxs-lookup"><span data-stu-id="8cc90-137">principalType</span></span>|<span data-ttu-id="8cc90-138">String</span><span class="sxs-lookup"><span data-stu-id="8cc90-138">String</span></span>|<span data-ttu-id="8cc90-139">Тип субъекта.</span><span class="sxs-lookup"><span data-stu-id="8cc90-139">The type of principal.</span></span>  <span data-ttu-id="8cc90-140">Это может быть «User», «Группы» или «ServicePrincipal».</span><span class="sxs-lookup"><span data-stu-id="8cc90-140">This can either be "User", "Group" or "ServicePrincipal".</span></span>|
|<span data-ttu-id="8cc90-141">resourceDisplayName</span><span class="sxs-lookup"><span data-stu-id="8cc90-141">resourceDisplayName</span></span>|<span data-ttu-id="8cc90-142">String</span><span class="sxs-lookup"><span data-stu-id="8cc90-142">String</span></span>|<span data-ttu-id="8cc90-143">Отображаемое имя ресурса, к которому назначения.</span><span class="sxs-lookup"><span data-stu-id="8cc90-143">The display name of the resource to which the assignment was made.</span></span>|
|<span data-ttu-id="8cc90-144">resourceId</span><span class="sxs-lookup"><span data-stu-id="8cc90-144">resourceId</span></span>|<span data-ttu-id="8cc90-145">Guid</span><span class="sxs-lookup"><span data-stu-id="8cc90-145">Guid</span></span>|<span data-ttu-id="8cc90-146">Уникальный идентификатор (**id**) для целевой ресурс, для которого было выполнено назначение (участников-служб).</span><span class="sxs-lookup"><span data-stu-id="8cc90-146">The unique identifier (**id**) for the target resource (service principal) for which the assignment was made.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8cc90-147">Связи</span><span class="sxs-lookup"><span data-stu-id="8cc90-147">Relationships</span></span>
<span data-ttu-id="8cc90-148">Нет</span><span class="sxs-lookup"><span data-stu-id="8cc90-148">None</span></span>


## <a name="methods"></a><span data-ttu-id="8cc90-149">Методы</span><span class="sxs-lookup"><span data-stu-id="8cc90-149">Methods</span></span>

| <span data-ttu-id="8cc90-150">Метод</span><span class="sxs-lookup"><span data-stu-id="8cc90-150">Method</span></span>           | <span data-ttu-id="8cc90-151">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="8cc90-151">Return Type</span></span>    |<span data-ttu-id="8cc90-152">Описание</span><span class="sxs-lookup"><span data-stu-id="8cc90-152">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="8cc90-153">Получение appRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="8cc90-153">Get appRoleAssignment</span></span>](../api/approleassignment-get.md) | [<span data-ttu-id="8cc90-154">appRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="8cc90-154">appRoleAssignment</span></span>](approleassignment.md) |<span data-ttu-id="8cc90-155">Чтение свойства и связи объекта appRoleAssignment.</span><span class="sxs-lookup"><span data-stu-id="8cc90-155">Read properties and relationships of appRoleAssignment object.</span></span>|
|[<span data-ttu-id="8cc90-156">Update</span><span class="sxs-lookup"><span data-stu-id="8cc90-156">Update</span></span>](../api/approleassignment-update.md) | [<span data-ttu-id="8cc90-157">appRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="8cc90-157">appRoleAssignment</span></span>](approleassignment.md)   |<span data-ttu-id="8cc90-158">Обновление объекта appRoleAssignment.</span><span class="sxs-lookup"><span data-stu-id="8cc90-158">Update appRoleAssignment object.</span></span> |
|[<span data-ttu-id="8cc90-159">Delete</span><span class="sxs-lookup"><span data-stu-id="8cc90-159">Delete</span></span>](../api/approleassignment-delete.md) | <span data-ttu-id="8cc90-160">Нет</span><span class="sxs-lookup"><span data-stu-id="8cc90-160">None</span></span> |<span data-ttu-id="8cc90-161">Удалите объект appRoleAssignment.</span><span class="sxs-lookup"><span data-stu-id="8cc90-161">Delete appRoleAssignment object.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "appRoleAssignment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
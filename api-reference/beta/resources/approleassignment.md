---
title: Тип ресурса appRoleAssignment
description: Используется для записи при назначении пользователя или группы приложению. В этом случае после назначения роли будет отображаться плитка приложения на панели доступа к приложениям пользователя. Кроме того, с помощью этого объекта можно предоставить другому приложению (моделируемому как субъект-служба) доступ к приложению ресурса в определенной роли. Вы можете создавать, просматривать, обновлять и удалять назначенные роли.
localization_priority: Priority
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: psignoret
ms.openlocfilehash: 5a0b9faeb68e11f465e8b5ddb177351e9a0f44d6
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508242"
---
# <a name="approleassignment-resource-type"></a><span data-ttu-id="6af71-106">Тип ресурса appRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="6af71-106">appRoleAssignment resource type</span></span>

<span data-ttu-id="6af71-107">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6af71-107">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6af71-108">Используется для записи при назначении пользователя или группы приложению.</span><span class="sxs-lookup"><span data-stu-id="6af71-108">Used to record when a user or group is assigned to an application.</span></span> <span data-ttu-id="6af71-109">В этом случае после назначения роли будет отображаться плитка приложения на панели доступа к приложениям пользователя.</span><span class="sxs-lookup"><span data-stu-id="6af71-109">In this case, the role assignment will result in an application tile showing up on the user's app access panel.</span></span> <span data-ttu-id="6af71-110">Кроме того, с помощью этого объекта можно предоставить другому приложению (моделируемому как субъект-служба) доступ к приложению ресурса в определенной роли.</span><span class="sxs-lookup"><span data-stu-id="6af71-110">This entity may also be used to grant another application (modeled as a service principal) access to a resource application in a particular role.</span></span> <span data-ttu-id="6af71-111">Вы можете создавать, просматривать, обновлять и удалять назначенные роли.</span><span class="sxs-lookup"><span data-stu-id="6af71-111">You can create, read, update, and delete role assignments.</span></span>


## <a name="json-representation"></a><span data-ttu-id="6af71-112">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6af71-112">JSON representation</span></span>

<span data-ttu-id="6af71-113">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="6af71-113">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.appRoleAssignment"
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
## <a name="properties"></a><span data-ttu-id="6af71-114">Свойства</span><span class="sxs-lookup"><span data-stu-id="6af71-114">Properties</span></span>
| <span data-ttu-id="6af71-115">Свойство</span><span class="sxs-lookup"><span data-stu-id="6af71-115">Property</span></span>     | <span data-ttu-id="6af71-116">Тип</span><span class="sxs-lookup"><span data-stu-id="6af71-116">Type</span></span>   |<span data-ttu-id="6af71-117">Описание</span><span class="sxs-lookup"><span data-stu-id="6af71-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6af71-118">creationTimestamp</span><span class="sxs-lookup"><span data-stu-id="6af71-118">creationTimestamp</span></span>|<span data-ttu-id="6af71-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6af71-119">DateTimeOffset</span></span>|<span data-ttu-id="6af71-120">Время создания контакта. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: .</span><span class="sxs-lookup"><span data-stu-id="6af71-120">The time when the grant was created.The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="6af71-121">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="6af71-121">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="6af71-122">id</span><span class="sxs-lookup"><span data-stu-id="6af71-122">id</span></span>|<span data-ttu-id="6af71-123">GUID</span><span class="sxs-lookup"><span data-stu-id="6af71-123">Guid</span></span>|<span data-ttu-id="6af71-124">Идентификатор роли, назначенный субъекту.</span><span class="sxs-lookup"><span data-stu-id="6af71-124">The role id that was assigned to the principal.</span></span>  <span data-ttu-id="6af71-125">Эта роль должна быть объявлена в целевом приложении-ресурсе **resourceId** в свойстве **appRoles**.</span><span class="sxs-lookup"><span data-stu-id="6af71-125">This role must be declared by the target resource application **resourceId** in its **appRoles** property.</span></span> <span data-ttu-id="6af71-126">Если в ресурсе не объявлены разрешения, необходимо указать идентификатор по умолчанию (нулевой GUID).</span><span class="sxs-lookup"><span data-stu-id="6af71-126">Where the resource does not declare any permissions, a default id (zero GUID) must be specified.</span></span> <span data-ttu-id="6af71-127">Ключ.</span><span class="sxs-lookup"><span data-stu-id="6af71-127">Key.</span></span> <span data-ttu-id="6af71-128">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="6af71-128">Not nullable.</span></span> |
|<span data-ttu-id="6af71-129">principalDisplayName</span><span class="sxs-lookup"><span data-stu-id="6af71-129">principalDisplayName</span></span>|<span data-ttu-id="6af71-130">String</span><span class="sxs-lookup"><span data-stu-id="6af71-130">String</span></span>|<span data-ttu-id="6af71-131">Отображаемое имя субъекта, которому был предоставлен доступ.</span><span class="sxs-lookup"><span data-stu-id="6af71-131">The display name of the principal that was granted the access.</span></span>|
|<span data-ttu-id="6af71-132">principalId</span><span class="sxs-lookup"><span data-stu-id="6af71-132">principalId</span></span>|<span data-ttu-id="6af71-133">GUID</span><span class="sxs-lookup"><span data-stu-id="6af71-133">Guid</span></span>|<span data-ttu-id="6af71-134">Уникальный идентификатор (**id**) для субъекта, которому предоставлен доступ.</span><span class="sxs-lookup"><span data-stu-id="6af71-134">The unique identifier (**id**) for the principal being granted the access.</span></span> <span data-ttu-id="6af71-135">Требуется при создании.</span><span class="sxs-lookup"><span data-stu-id="6af71-135">Required on create.</span></span>            |
|<span data-ttu-id="6af71-136">principalType</span><span class="sxs-lookup"><span data-stu-id="6af71-136">principalType</span></span>|<span data-ttu-id="6af71-137">String</span><span class="sxs-lookup"><span data-stu-id="6af71-137">String</span></span>|<span data-ttu-id="6af71-138">Тип субъекта.</span><span class="sxs-lookup"><span data-stu-id="6af71-138">The type of principal.</span></span>  <span data-ttu-id="6af71-139">Это может "Пользователь", "Группа" или "Субъект-служба".</span><span class="sxs-lookup"><span data-stu-id="6af71-139">This can either be "User", "Group" or "ServicePrincipal".</span></span>|
|<span data-ttu-id="6af71-140">resourceDisplayName</span><span class="sxs-lookup"><span data-stu-id="6af71-140">resourceDisplayName</span></span>|<span data-ttu-id="6af71-141">String</span><span class="sxs-lookup"><span data-stu-id="6af71-141">String</span></span>|<span data-ttu-id="6af71-142">Отображаемое имя ресурса, для которого было выполнено назначение.</span><span class="sxs-lookup"><span data-stu-id="6af71-142">The display name of the resource to which the assignment was made.</span></span>|
|<span data-ttu-id="6af71-143">resourceId</span><span class="sxs-lookup"><span data-stu-id="6af71-143">resourceId</span></span>|<span data-ttu-id="6af71-144">GUID</span><span class="sxs-lookup"><span data-stu-id="6af71-144">Guid</span></span>|<span data-ttu-id="6af71-145">Уникальный идентификатор (**id**) для целевого ресурса (субъект-служба), для которого было выполнено назначение.</span><span class="sxs-lookup"><span data-stu-id="6af71-145">The unique identifier (**id**) for the target resource (service principal) for which the assignment was made.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6af71-146">Связи</span><span class="sxs-lookup"><span data-stu-id="6af71-146">Relationships</span></span>
<span data-ttu-id="6af71-147">Нет</span><span class="sxs-lookup"><span data-stu-id="6af71-147">None</span></span>


## <a name="methods"></a><span data-ttu-id="6af71-148">Методы</span><span class="sxs-lookup"><span data-stu-id="6af71-148">Methods</span></span>

| <span data-ttu-id="6af71-149">Метод</span><span class="sxs-lookup"><span data-stu-id="6af71-149">Method</span></span>           | <span data-ttu-id="6af71-150">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="6af71-150">Return Type</span></span>    |<span data-ttu-id="6af71-151">Описание</span><span class="sxs-lookup"><span data-stu-id="6af71-151">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="6af71-152">Получение объекта appRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="6af71-152">Get appRoleAssignment</span></span>](../api/approleassignment-get.md) | [<span data-ttu-id="6af71-153">appRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="6af71-153">appRoleAssignment</span></span>](approleassignment.md) |<span data-ttu-id="6af71-154">Чтение свойств и связей объекта appRoleAssignment.</span><span class="sxs-lookup"><span data-stu-id="6af71-154">Read properties and relationships of appRoleAssignment object.</span></span>|
|[<span data-ttu-id="6af71-155">Обновление</span><span class="sxs-lookup"><span data-stu-id="6af71-155">Update</span></span>](../api/approleassignment-update.md) | [<span data-ttu-id="6af71-156">appRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="6af71-156">appRoleAssignment</span></span>](approleassignment.md)   |<span data-ttu-id="6af71-157">Обновление объекта appRoleAssignment.</span><span class="sxs-lookup"><span data-stu-id="6af71-157">Update appRoleAssignment object.</span></span> |
|[<span data-ttu-id="6af71-158">Удаление</span><span class="sxs-lookup"><span data-stu-id="6af71-158">Delete</span></span>](../api/approleassignment-delete.md) | <span data-ttu-id="6af71-159">Нет</span><span class="sxs-lookup"><span data-stu-id="6af71-159">None</span></span> |<span data-ttu-id="6af71-160">Удаление объекта appRoleAssignment.</span><span class="sxs-lookup"><span data-stu-id="6af71-160">Delete appRoleAssignment object.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "appRoleAssignment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

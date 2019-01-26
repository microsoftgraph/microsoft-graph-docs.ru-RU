---
title: Тип ресурса appRoleAssignment
description: Используется для записи при назначении пользователя или группы приложению. В этом случае после назначения роли будет отображаться плитка приложения на панели доступа к приложениям пользователя. Кроме того, с помощью этого объекта можно предоставить другому приложению (моделируемому как субъект-служба) доступ к приложению ресурса в определенной роли. Вы можете создавать, просматривать, обновлять и удалять назначенные роли.
localization_priority: Priority
ms.openlocfilehash: 6255642f47f0e1454fb64440d4938605a2de5df4
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513902"
---
# <a name="approleassignment-resource-type"></a><span data-ttu-id="6d2cc-106">Тип ресурса appRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="6d2cc-106">appRoleAssignment resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6d2cc-107">Используется для записи при назначении пользователя или группы приложению.</span><span class="sxs-lookup"><span data-stu-id="6d2cc-107">Used to record when a user or group is assigned to an application.</span></span> <span data-ttu-id="6d2cc-108">В этом случае после назначения роли будет отображаться плитка приложения на панели доступа к приложениям пользователя.</span><span class="sxs-lookup"><span data-stu-id="6d2cc-108">In this case, the role assignment will result in an application tile showing up on the user's app access panel.</span></span> <span data-ttu-id="6d2cc-109">Кроме того, с помощью этого объекта можно предоставить другому приложению (моделируемому как субъект-служба) доступ к приложению ресурса в определенной роли.</span><span class="sxs-lookup"><span data-stu-id="6d2cc-109">This entity may also be used to grant another application (modeled as a service principal) access to a resource application in a particular role.</span></span> <span data-ttu-id="6d2cc-110">Вы можете создавать, просматривать, обновлять и удалять назначенные роли.</span><span class="sxs-lookup"><span data-stu-id="6d2cc-110">You can create, read, update, and delete role assignments.</span></span>


## <a name="json-representation"></a><span data-ttu-id="6d2cc-111">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6d2cc-111">JSON representation</span></span>

<span data-ttu-id="6d2cc-112">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="6d2cc-112">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="6d2cc-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="6d2cc-113">Properties</span></span>
| <span data-ttu-id="6d2cc-114">Свойство</span><span class="sxs-lookup"><span data-stu-id="6d2cc-114">Property</span></span>     | <span data-ttu-id="6d2cc-115">Тип</span><span class="sxs-lookup"><span data-stu-id="6d2cc-115">Type</span></span>   |<span data-ttu-id="6d2cc-116">Описание</span><span class="sxs-lookup"><span data-stu-id="6d2cc-116">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6d2cc-117">creationTimestamp</span><span class="sxs-lookup"><span data-stu-id="6d2cc-117">creationTimestamp</span></span>|<span data-ttu-id="6d2cc-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6d2cc-118">DateTimeOffset</span></span>|<span data-ttu-id="6d2cc-119">Время создания контакта. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: .</span><span class="sxs-lookup"><span data-stu-id="6d2cc-119">The time when the grant was created.The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="6d2cc-120">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="6d2cc-120">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="6d2cc-121">id</span><span class="sxs-lookup"><span data-stu-id="6d2cc-121">id</span></span>|<span data-ttu-id="6d2cc-122">GUID</span><span class="sxs-lookup"><span data-stu-id="6d2cc-122">Guid</span></span>|<span data-ttu-id="6d2cc-123">Идентификатор роли, назначенный субъекту.</span><span class="sxs-lookup"><span data-stu-id="6d2cc-123">The role id that was assigned to the principal.</span></span>  <span data-ttu-id="6d2cc-124">Эта роль должна быть объявлена в целевом приложении-ресурсе **resourceId** в свойстве **appRoles**.</span><span class="sxs-lookup"><span data-stu-id="6d2cc-124">This role must be declared by the target resource application **resourceId** in its **appRoles** property.</span></span> <span data-ttu-id="6d2cc-125">Если в ресурсе не объявлены разрешения, необходимо указать идентификатор по умолчанию (нулевой GUID).</span><span class="sxs-lookup"><span data-stu-id="6d2cc-125">Where the resource does not declare any permissions, a default id (zero GUID) must be specified.</span></span> <span data-ttu-id="6d2cc-126">Ключ.</span><span class="sxs-lookup"><span data-stu-id="6d2cc-126">Key.</span></span> <span data-ttu-id="6d2cc-127">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="6d2cc-127">Not nullable.</span></span> |
|<span data-ttu-id="6d2cc-128">principalDisplayName</span><span class="sxs-lookup"><span data-stu-id="6d2cc-128">principalDisplayName</span></span>|<span data-ttu-id="6d2cc-129">String</span><span class="sxs-lookup"><span data-stu-id="6d2cc-129">String</span></span>|<span data-ttu-id="6d2cc-130">Отображаемое имя субъекта, которому был предоставлен доступ.</span><span class="sxs-lookup"><span data-stu-id="6d2cc-130">The display name of the principal that was granted the access.</span></span>|
|<span data-ttu-id="6d2cc-131">principalId</span><span class="sxs-lookup"><span data-stu-id="6d2cc-131">principalId</span></span>|<span data-ttu-id="6d2cc-132">GUID</span><span class="sxs-lookup"><span data-stu-id="6d2cc-132">Guid</span></span>|<span data-ttu-id="6d2cc-133">Уникальный идентификатор (**id**) для субъекта, которому предоставлен доступ.</span><span class="sxs-lookup"><span data-stu-id="6d2cc-133">The unique identifier (**id**) for the principal being granted the access.</span></span> <span data-ttu-id="6d2cc-134">Требуется при создании.</span><span class="sxs-lookup"><span data-stu-id="6d2cc-134">Required on create.</span></span>            |
|<span data-ttu-id="6d2cc-135">principalType</span><span class="sxs-lookup"><span data-stu-id="6d2cc-135">principalType</span></span>|<span data-ttu-id="6d2cc-136">String</span><span class="sxs-lookup"><span data-stu-id="6d2cc-136">String</span></span>|<span data-ttu-id="6d2cc-137">Тип субъекта.</span><span class="sxs-lookup"><span data-stu-id="6d2cc-137">The type of principal.</span></span>  <span data-ttu-id="6d2cc-138">Это может "Пользователь", "Группа" или "Субъект-служба".</span><span class="sxs-lookup"><span data-stu-id="6d2cc-138">This can either be "User", "Group" or "ServicePrincipal".</span></span>|
|<span data-ttu-id="6d2cc-139">resourceDisplayName</span><span class="sxs-lookup"><span data-stu-id="6d2cc-139">resourceDisplayName</span></span>|<span data-ttu-id="6d2cc-140">String</span><span class="sxs-lookup"><span data-stu-id="6d2cc-140">String</span></span>|<span data-ttu-id="6d2cc-141">Отображаемое имя ресурса, для которого было выполнено назначение.</span><span class="sxs-lookup"><span data-stu-id="6d2cc-141">The display name of the resource to which the assignment was made.</span></span>|
|<span data-ttu-id="6d2cc-142">resourceId</span><span class="sxs-lookup"><span data-stu-id="6d2cc-142">resourceId</span></span>|<span data-ttu-id="6d2cc-143">GUID</span><span class="sxs-lookup"><span data-stu-id="6d2cc-143">Guid</span></span>|<span data-ttu-id="6d2cc-144">Уникальный идентификатор (**id**) для целевого ресурса (субъект-служба), для которого было выполнено назначение.</span><span class="sxs-lookup"><span data-stu-id="6d2cc-144">The unique identifier (**id**) for the target resource (service principal) for which the assignment was made.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6d2cc-145">Связи</span><span class="sxs-lookup"><span data-stu-id="6d2cc-145">Relationships</span></span>
<span data-ttu-id="6d2cc-146">Нет</span><span class="sxs-lookup"><span data-stu-id="6d2cc-146">None</span></span>


## <a name="methods"></a><span data-ttu-id="6d2cc-147">Методы</span><span class="sxs-lookup"><span data-stu-id="6d2cc-147">Methods</span></span>

| <span data-ttu-id="6d2cc-148">Метод</span><span class="sxs-lookup"><span data-stu-id="6d2cc-148">Method</span></span>           | <span data-ttu-id="6d2cc-149">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="6d2cc-149">Return Type</span></span>    |<span data-ttu-id="6d2cc-150">Описание</span><span class="sxs-lookup"><span data-stu-id="6d2cc-150">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="6d2cc-151">Получение объекта appRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="6d2cc-151">Get appRoleAssignment</span></span>](../api/approleassignment-get.md) | [<span data-ttu-id="6d2cc-152">appRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="6d2cc-152">appRoleAssignment</span></span>](approleassignment.md) |<span data-ttu-id="6d2cc-153">Чтение свойств и связей объекта appRoleAssignment.</span><span class="sxs-lookup"><span data-stu-id="6d2cc-153">Read properties and relationships of appRoleAssignment object.</span></span>|
|[<span data-ttu-id="6d2cc-154">Обновление</span><span class="sxs-lookup"><span data-stu-id="6d2cc-154">Update</span></span>](../api/approleassignment-update.md) | [<span data-ttu-id="6d2cc-155">appRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="6d2cc-155">appRoleAssignment</span></span>](approleassignment.md)   |<span data-ttu-id="6d2cc-156">Обновление объекта appRoleAssignment.</span><span class="sxs-lookup"><span data-stu-id="6d2cc-156">Update appRoleAssignment object.</span></span> |
|[<span data-ttu-id="6d2cc-157">Удаление</span><span class="sxs-lookup"><span data-stu-id="6d2cc-157">Delete</span></span>](../api/approleassignment-delete.md) | <span data-ttu-id="6d2cc-158">Нет</span><span class="sxs-lookup"><span data-stu-id="6d2cc-158">None</span></span> |<span data-ttu-id="6d2cc-159">Удаление объекта appRoleAssignment.</span><span class="sxs-lookup"><span data-stu-id="6d2cc-159">Delete appRoleAssignment object.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "appRoleAssignment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/approleassignment.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

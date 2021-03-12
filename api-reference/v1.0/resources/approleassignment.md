---
title: Тип ресурса appRoleAssignment
description: Используется, чтобы записать, когда пользователю, группе или субъекту-службе присваивается роль приложения в субъекте-службе приложения. Можно создавать, читать и удалять назначения ролей приложений.
localization_priority: Priority
doc_type: resourcePageType
ms.prod: applications
author: psignoret
ms.openlocfilehash: e224589453807ef86ba73410f7a9bb817495d9aa
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50721182"
---
# <a name="approleassignment-resource-type"></a><span data-ttu-id="7444d-104">Тип ресурса appRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="7444d-104">appRoleAssignment resource type</span></span>

<span data-ttu-id="7444d-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7444d-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7444d-106">Используется, чтобы записать, когда пользователю, группе или субъекту-службе присваивается роль приложения для какого-либо приложения.</span><span class="sxs-lookup"><span data-stu-id="7444d-106">Used to record when a user, group, or service principal is assigned an app role for an app.</span></span>

<span data-ttu-id="7444d-107">Назначение роли приложения — это отношение между назначенным субъектом (пользователь, группа или субъект-служба), приложением ресурса (субъект-служба приложения) и ролью приложения, определенной для приложения ресурса.</span><span class="sxs-lookup"><span data-stu-id="7444d-107">An app role assignment is a relationship between the assigned principal (a user, a group, or a service principal), a resource application (the app's service principal) and an app role defined on the resource application.</span></span>

<span data-ttu-id="7444d-108">Если у [роли приложения](approle.md), которая назначена субъекту, есть непустое свойство **value**, оно включается в утверждения **ролей** маркеров, где субъектом может быть назначенный субъект (например, отклики SAML, маркеры идентификаторов, маркеры доступа, определяющие вошедшего в систему пользователя, или маркер доступа, определяющий субъект-службу).</span><span class="sxs-lookup"><span data-stu-id="7444d-108">When the [app role](approle.md) which has been assigned to a principal has a non-empty **value** property, this will be included in the **roles** claim of tokens where the subject is the  assigned principal (e.g. SAML responses, ID tokens, access tokens identifying a signed-in user, or an access token identifying a service principal).</span></span> <span data-ttu-id="7444d-109">Приложения и API используют эти утверждения в логике авторизации.</span><span class="sxs-lookup"><span data-stu-id="7444d-109">Applications and APIs use these claims as part of their authorization logic.</span></span>

<span data-ttu-id="7444d-110">Пользователю можно назначить роль приложения напрямую.</span><span class="sxs-lookup"><span data-stu-id="7444d-110">A user can be assigned an app role directly.</span></span> <span data-ttu-id="7444d-111">Если роль приложения назначена группе, то эта роль приложения также считается назначенной непосредственным участникам этой группы.</span><span class="sxs-lookup"><span data-stu-id="7444d-111">If an app role is assigned to a group, direct members of the group are also considered to have been assigned the app role.</span></span> <span data-ttu-id="7444d-112">Когда пользователю назначается роль приложения для какого-либо приложения, название этого приложения отображается на [портале "Мои приложения](/azure/active-directory/user-help/my-apps-portal-end-user-access) этого пользователя и в [средстве запуска приложений Microsoft 365](https://support.office.com/article/meet-the-office-365-app-launcher-79f12104-6fed-442f-96a0-eb089a3f476a).</span><span class="sxs-lookup"><span data-stu-id="7444d-112">When a user is assigned an app role for an application, a tile for that application is displayed in the user's [MyApps portal](/azure/active-directory/user-help/my-apps-portal-end-user-access) and [Microsoft 365 app launcher](https://support.office.com/article/meet-the-office-365-app-launcher-79f12104-6fed-442f-96a0-eb089a3f476a).</span></span>

<span data-ttu-id="7444d-113">Если назначенный субъект является субъектом-службой, то предоставляется [доступ только к приложению](/azure/active-directory/develop/v2-permissions-and-consent#permission-types).</span><span class="sxs-lookup"><span data-stu-id="7444d-113">An app role assignment where the assigned principal is a service principal is an [app-only permission](/azure/active-directory/develop/v2-permissions-and-consent#permission-types) grant.</span></span> <span data-ttu-id="7444d-114">Когда пользователь или администратор принимает разрешение с доступом только к приложению, создается назначение роли приложения, в котором назначенный субъект является субъектом-службой для приложения клиента, а ресурс является субъектом-службой целевого API.</span><span class="sxs-lookup"><span data-stu-id="7444d-114">When a user or admin consents to an app-only permission, an app role assignment is created where the assigned principal is the service principal for the client application, and the resource is the target API's service principal.</span></span>

## <a name="properties"></a><span data-ttu-id="7444d-115">Свойства</span><span class="sxs-lookup"><span data-stu-id="7444d-115">Properties</span></span>

| <span data-ttu-id="7444d-116">Свойство</span><span class="sxs-lookup"><span data-stu-id="7444d-116">Property</span></span> | <span data-ttu-id="7444d-117">Тип</span><span class="sxs-lookup"><span data-stu-id="7444d-117">Type</span></span> | <span data-ttu-id="7444d-118">Описание</span><span class="sxs-lookup"><span data-stu-id="7444d-118">Description</span></span> |
|:---------------|:--------|:----------|
| <span data-ttu-id="7444d-119">id</span><span class="sxs-lookup"><span data-stu-id="7444d-119">id</span></span> | <span data-ttu-id="7444d-120">Строка</span><span class="sxs-lookup"><span data-stu-id="7444d-120">String</span></span> | <span data-ttu-id="7444d-121">Уникальный идентификатор ключа **appRoleAssignment**.</span><span class="sxs-lookup"><span data-stu-id="7444d-121">A unique identifier for the **appRoleAssignment** Key.</span></span> <span data-ttu-id="7444d-122">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="7444d-122">Not nullable.</span></span> <span data-ttu-id="7444d-123">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7444d-123">Read-only.</span></span> |
| <span data-ttu-id="7444d-124">creationTimestamp</span><span class="sxs-lookup"><span data-stu-id="7444d-124">creationTimestamp</span></span> | <span data-ttu-id="7444d-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7444d-125">DateTimeOffset</span></span> | <span data-ttu-id="7444d-126">Время создания назначения роли приложения. Тип Timestamp представляет сведения о времени и дате в формате ISO 8601 (всегда используется время в формате UTC).</span><span class="sxs-lookup"><span data-stu-id="7444d-126">The time when the app role assignment was created.The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="7444d-127">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="7444d-127">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="7444d-128">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7444d-128">Read-only.</span></span> <span data-ttu-id="7444d-129">Не поддерживает `$filter`.</span><span class="sxs-lookup"><span data-stu-id="7444d-129">Does not support `$filter`.</span></span> |
| <span data-ttu-id="7444d-130">principalId</span><span class="sxs-lookup"><span data-stu-id="7444d-130">principalId</span></span> | <span data-ttu-id="7444d-131">Guid</span><span class="sxs-lookup"><span data-stu-id="7444d-131">Guid</span></span> | <span data-ttu-id="7444d-132">Уникальный идентификатор (**ИД**) [пользователя](user.md), [группы](group.md) или [субъекта-службы](serviceprincipal.md), которым предоставляется роль приложения.</span><span class="sxs-lookup"><span data-stu-id="7444d-132">The unique identifier (**id**) for the [user](user.md), [group](group.md) or [service principal](serviceprincipal.md) being granted the app role.</span></span> <span data-ttu-id="7444d-133">Требуется при создании.</span><span class="sxs-lookup"><span data-stu-id="7444d-133">Required on create.</span></span> <span data-ttu-id="7444d-134">Не поддерживает `$filter`.</span><span class="sxs-lookup"><span data-stu-id="7444d-134">Does not support `$filter`.</span></span> |
| <span data-ttu-id="7444d-135">principalType</span><span class="sxs-lookup"><span data-stu-id="7444d-135">principalType</span></span> | <span data-ttu-id="7444d-136">Строка</span><span class="sxs-lookup"><span data-stu-id="7444d-136">String</span></span> | <span data-ttu-id="7444d-137">Тип назначенного субъекта.</span><span class="sxs-lookup"><span data-stu-id="7444d-137">The type of the assigned principal.</span></span> <span data-ttu-id="7444d-138">Это может "Пользователь", "Группа" или "Субъект-служба".</span><span class="sxs-lookup"><span data-stu-id="7444d-138">This can either be "User", "Group" or "ServicePrincipal".</span></span> <span data-ttu-id="7444d-139">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7444d-139">Read-only.</span></span> <span data-ttu-id="7444d-140">Не поддерживает `$filter`.</span><span class="sxs-lookup"><span data-stu-id="7444d-140">Does not support `$filter`.</span></span> |
| <span data-ttu-id="7444d-141">principalDisplayName</span><span class="sxs-lookup"><span data-stu-id="7444d-141">principalDisplayName</span></span> | <span data-ttu-id="7444d-142">Строка</span><span class="sxs-lookup"><span data-stu-id="7444d-142">String</span></span> |<span data-ttu-id="7444d-143">Отображаемое имя пользователя, группа или субъекта-службы, которым было предоставлено назначение роли приложения.</span><span class="sxs-lookup"><span data-stu-id="7444d-143">The display name of the user, group, or service principal that was granted the app role assignment.</span></span> <span data-ttu-id="7444d-144">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7444d-144">Read-only.</span></span> <span data-ttu-id="7444d-145">Поддерживает `$filter` (`eq` и `startswith`).</span><span class="sxs-lookup"><span data-stu-id="7444d-145">Supports `$filter` (`eq` and `startswith`).</span></span> |
| <span data-ttu-id="7444d-146">resourceId</span><span class="sxs-lookup"><span data-stu-id="7444d-146">resourceId</span></span> | <span data-ttu-id="7444d-147">Guid</span><span class="sxs-lookup"><span data-stu-id="7444d-147">Guid</span></span> |<span data-ttu-id="7444d-148">Уникальный идентификатор (**ИД**) ресурса [субъект-служба](serviceprincipal.md), для которого производится назначение.</span><span class="sxs-lookup"><span data-stu-id="7444d-148">The unique identifier (**id**) for the resource [service principal](serviceprincipal.md) for which the assignment is made.</span></span> <span data-ttu-id="7444d-149">Требуется при создании.</span><span class="sxs-lookup"><span data-stu-id="7444d-149">Required on create.</span></span> <span data-ttu-id="7444d-150">Поддерживает `$filter` (только `eq`).</span><span class="sxs-lookup"><span data-stu-id="7444d-150">Supports `$filter` (`eq` only).</span></span> |
| <span data-ttu-id="7444d-151">resourceDisplayName</span><span class="sxs-lookup"><span data-stu-id="7444d-151">resourceDisplayName</span></span> | <span data-ttu-id="7444d-152">Строка</span><span class="sxs-lookup"><span data-stu-id="7444d-152">String</span></span> | <span data-ttu-id="7444d-153">Отображаемое имя субъекта-службы приложения ресурса, для которого производится назначение.</span><span class="sxs-lookup"><span data-stu-id="7444d-153">The display name of the resource app's service principal to which the assignment is made.</span></span> <span data-ttu-id="7444d-154">Не поддерживает `$filter`.</span><span class="sxs-lookup"><span data-stu-id="7444d-154">Does not support `$filter`.</span></span> |
| <span data-ttu-id="7444d-155">appRoleId</span><span class="sxs-lookup"><span data-stu-id="7444d-155">appRoleId</span></span> | <span data-ttu-id="7444d-156">Guid</span><span class="sxs-lookup"><span data-stu-id="7444d-156">Guid</span></span> | <span data-ttu-id="7444d-157">Идентификатор (**ИД**) [роли приложения](approle.md), которая назначается субъекту.</span><span class="sxs-lookup"><span data-stu-id="7444d-157">The identifier (**id**) for the [app role](approle.md) which is assigned to the principal.</span></span> <span data-ttu-id="7444d-158">Эта роль приложения должна предоставляться в свойстве **appRoles** субъекта-службы приложения ресурса (**resourceId**).</span><span class="sxs-lookup"><span data-stu-id="7444d-158">This app role must be exposed in the **appRoles** property on the resource application's service principal (**resourceId**).</span></span> <span data-ttu-id="7444d-159">Если в приложении ресурса не объявлены никакие роли приложения, можно указать ИД роли приложения по умолчанию (`00000000-0000-0000-0000-000000000000`), чтобы указать, что субъект назначен приложению ресурса без каких-либо определенных ролей приложения.</span><span class="sxs-lookup"><span data-stu-id="7444d-159">If the resource application has not declared any app roles, a default app role ID of `00000000-0000-0000-0000-000000000000` can be specified to signal that the principal is assigned to the resource app without any specific app roles.</span></span> <span data-ttu-id="7444d-160">Требуется при создании.</span><span class="sxs-lookup"><span data-stu-id="7444d-160">Required on create.</span></span> <span data-ttu-id="7444d-161">Не поддерживает `$filter`.</span><span class="sxs-lookup"><span data-stu-id="7444d-161">Does not support `$filter`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="7444d-162">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7444d-162">JSON representation</span></span>

<span data-ttu-id="7444d-163">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7444d-163">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.appRoleAssignment"
}-->

```json
{
  "id": "string",
  "creationTimestamp": "String (timestamp)",
  "principalDisplayName": "string",
  "principalId": "guid",
  "principalType": "string",
  "resourceDisplayName": "string",
  "resourceId": "guid",
  "appRoleId": "guid"
}
```

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
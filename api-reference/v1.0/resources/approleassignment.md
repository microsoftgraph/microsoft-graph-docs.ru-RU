---
title: Тип ресурса appRoleAssignment
description: Используется для записи при назначении роли приложения для субъекта-службы приложения пользователя, группы или субъекта-службы. Вы можете создавать, читать и удалять назначения ролей приложений.
localization_priority: Priority
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: psignoret
ms.openlocfilehash: 98af5eb0812e0e3857e154bc51a663038b1230a7
ms.sourcegitcommit: 7a6231aeb570ff45d01b3db3df07a411f9f60fd1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/27/2020
ms.locfileid: "44383709"
---
# <a name="approleassignment-resource-type"></a><span data-ttu-id="3eb14-104">Тип ресурса appRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="3eb14-104">appRoleAssignment resource type</span></span>

<span data-ttu-id="3eb14-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3eb14-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3eb14-106">Используется для записи, когда пользователю, группе или участнику службы назначена роль приложения для приложения.</span><span class="sxs-lookup"><span data-stu-id="3eb14-106">Used to record when a user, group, or service principal is assigned an app role for an app.</span></span>

<span data-ttu-id="3eb14-107">Назначение роли приложения — это отношение между назначенным участником (пользователем, группой или субъектом-службой), приложением ресурсов (субъектом-службой приложения) и ролью приложения, определенной в приложении ресурса.</span><span class="sxs-lookup"><span data-stu-id="3eb14-107">An app role assignment is a relationship between the assigned principal (a user, a group, or a service principal), a resource application (the app's service principal) and an app role defined on the resource application.</span></span>

<span data-ttu-id="3eb14-108">Если [роль приложения](approle.md) , назначенная участнику, имеет непустое свойство **value** , она будет включена в утверждения **ролей** маркеров, в которых субъект является назначенным участником (например, ОТВЕТами SAML, маркерами идентификаторов, маркерами доступа, идентифицирующими вошедшего пользователя, или маркером доступа, идентифицирующим субъекта-службу).</span><span class="sxs-lookup"><span data-stu-id="3eb14-108">When the [app role](approle.md) which has been assigned to a principal has a non-empty **value** property, this will be included in the **roles** claim of tokens where the subject is the  assigned principal (e.g. SAML responses, ID tokens, access tokens identifying a signed-in user, or an access token identifying a service principal).</span></span> <span data-ttu-id="3eb14-109">Приложения и API используют эти утверждения в рамках логики авторизации.</span><span class="sxs-lookup"><span data-stu-id="3eb14-109">Applications and APIs use these claims as part of their authorization logic.</span></span>

<span data-ttu-id="3eb14-110">Пользователю может быть назначена роль приложения напрямую.</span><span class="sxs-lookup"><span data-stu-id="3eb14-110">A user can be assigned an app role directly.</span></span> <span data-ttu-id="3eb14-111">Если группе назначена роль приложения, то непосредственно членам группы также назначается роль приложения.</span><span class="sxs-lookup"><span data-stu-id="3eb14-111">If an app role is assigned to a group, direct members of the group are also considered to have been assigned the app role.</span></span> <span data-ttu-id="3eb14-112">Когда пользователю назначается роль приложения для приложения, плитка для этого приложения отображается на [портале](https://docs.microsoft.com/azure/active-directory/user-help/my-apps-portal-end-user-access) приложений пользователя и в средстве [запуска приложений Office 365](https://support.office.com/article/meet-the-office-365-app-launcher-79f12104-6fed-442f-96a0-eb089a3f476a).</span><span class="sxs-lookup"><span data-stu-id="3eb14-112">When a user is assigned an app role for an application, a tile for that application is displayed in the user's [MyApps portal](https://docs.microsoft.com/azure/active-directory/user-help/my-apps-portal-end-user-access) and [Office 365 app launcher](https://support.office.com/article/meet-the-office-365-app-launcher-79f12104-6fed-442f-96a0-eb089a3f476a).</span></span>

<span data-ttu-id="3eb14-113">Назначение роли приложения, когда назначенный участник является участником службы, представляет собой предоставление [разрешений только для приложения](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent#permission-types) .</span><span class="sxs-lookup"><span data-stu-id="3eb14-113">An app role assignment where the assigned principal is a service principal is an [app-only permission](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent#permission-types) grant.</span></span> <span data-ttu-id="3eb14-114">Если пользователь или администратор отправляет разрешение только для приложения, создается назначение роли приложения, в котором назначенный участник является субъектом-службой для клиентского приложения, а ресурс является субъектом-службой конечного API.</span><span class="sxs-lookup"><span data-stu-id="3eb14-114">When a user or admin consents to an app-only permission, an app role assignment is created where the assigned principal is the service principal for the client application, and the resource is the target API's service principal.</span></span>

## <a name="properties"></a><span data-ttu-id="3eb14-115">Свойства</span><span class="sxs-lookup"><span data-stu-id="3eb14-115">Properties</span></span>

| <span data-ttu-id="3eb14-116">Свойство</span><span class="sxs-lookup"><span data-stu-id="3eb14-116">Property</span></span> | <span data-ttu-id="3eb14-117">Тип</span><span class="sxs-lookup"><span data-stu-id="3eb14-117">Type</span></span> | <span data-ttu-id="3eb14-118">Описание</span><span class="sxs-lookup"><span data-stu-id="3eb14-118">Description</span></span> |
|:---------------|:--------|:----------|
| <span data-ttu-id="3eb14-119">id</span><span class="sxs-lookup"><span data-stu-id="3eb14-119">id</span></span> | <span data-ttu-id="3eb14-120">Строка</span><span class="sxs-lookup"><span data-stu-id="3eb14-120">String</span></span> | <span data-ttu-id="3eb14-121">Уникальный идентификатор для ключа **аппролеассигнмент** .</span><span class="sxs-lookup"><span data-stu-id="3eb14-121">A unique identifier for the **appRoleAssignment** Key.</span></span> <span data-ttu-id="3eb14-122">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="3eb14-122">Not nullable.</span></span> <span data-ttu-id="3eb14-123">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3eb14-123">Read-only.</span></span> |
| <span data-ttu-id="3eb14-124">creationTimestamp</span><span class="sxs-lookup"><span data-stu-id="3eb14-124">creationTimestamp</span></span> | <span data-ttu-id="3eb14-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3eb14-125">DateTimeOffset</span></span> | <span data-ttu-id="3eb14-126">Время создания назначения роли приложения. Тип timestamp представляет сведения о дате и времени с использованием формата ISO 8601 и всегда задается в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="3eb14-126">The time when the app role assignment was created.The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="3eb14-127">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="3eb14-127">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="3eb14-128">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3eb14-128">Read-only.</span></span> <span data-ttu-id="3eb14-129">Не поддерживает `$filter` .</span><span class="sxs-lookup"><span data-stu-id="3eb14-129">Does not support `$filter`.</span></span> |
| <span data-ttu-id="3eb14-130">principalId</span><span class="sxs-lookup"><span data-stu-id="3eb14-130">principalId</span></span> | <span data-ttu-id="3eb14-131">GUID</span><span class="sxs-lookup"><span data-stu-id="3eb14-131">Guid</span></span> | <span data-ttu-id="3eb14-132">Уникальный идентификатор (**ID**) для [пользователя](user.md), [группы](group.md) или [субъекта-службы](serviceprincipal.md) , которому назначена роль приложения.</span><span class="sxs-lookup"><span data-stu-id="3eb14-132">The unique identifier (**id**) for the [user](user.md), [group](group.md) or [service principal](serviceprincipal.md) being granted the app role.</span></span> <span data-ttu-id="3eb14-133">Требуется при создании.</span><span class="sxs-lookup"><span data-stu-id="3eb14-133">Required on create.</span></span> <span data-ttu-id="3eb14-134">Не поддерживает `$filter` .</span><span class="sxs-lookup"><span data-stu-id="3eb14-134">Does not support `$filter`.</span></span> |
| <span data-ttu-id="3eb14-135">principalType</span><span class="sxs-lookup"><span data-stu-id="3eb14-135">principalType</span></span> | <span data-ttu-id="3eb14-136">String</span><span class="sxs-lookup"><span data-stu-id="3eb14-136">String</span></span> | <span data-ttu-id="3eb14-137">Тип назначенного субъекта.</span><span class="sxs-lookup"><span data-stu-id="3eb14-137">The type of the assigned principal.</span></span> <span data-ttu-id="3eb14-138">Это может "Пользователь", "Группа" или "Субъект-служба".</span><span class="sxs-lookup"><span data-stu-id="3eb14-138">This can either be "User", "Group" or "ServicePrincipal".</span></span> <span data-ttu-id="3eb14-139">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3eb14-139">Read-only.</span></span> <span data-ttu-id="3eb14-140">Не поддерживает `$filter` .</span><span class="sxs-lookup"><span data-stu-id="3eb14-140">Does not support `$filter`.</span></span> |
| <span data-ttu-id="3eb14-141">principalDisplayName</span><span class="sxs-lookup"><span data-stu-id="3eb14-141">principalDisplayName</span></span> | <span data-ttu-id="3eb14-142">String</span><span class="sxs-lookup"><span data-stu-id="3eb14-142">String</span></span> |<span data-ttu-id="3eb14-143">Отображаемое имя пользователя, группы или субъекта службы, которым было предоставлено назначение роли приложения.</span><span class="sxs-lookup"><span data-stu-id="3eb14-143">The display name of the user, group, or service principal that was granted the app role assignment.</span></span> <span data-ttu-id="3eb14-144">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3eb14-144">Read-only.</span></span> <span data-ttu-id="3eb14-145">Поддерживает `$filter` ( `eq` и `startswith` ).</span><span class="sxs-lookup"><span data-stu-id="3eb14-145">Supports `$filter` (`eq` and `startswith`).</span></span> |
| <span data-ttu-id="3eb14-146">resourceId</span><span class="sxs-lookup"><span data-stu-id="3eb14-146">resourceId</span></span> | <span data-ttu-id="3eb14-147">GUID</span><span class="sxs-lookup"><span data-stu-id="3eb14-147">Guid</span></span> |<span data-ttu-id="3eb14-148">Уникальный**идентификатор** [субъекта службы](serviceprincipal.md) ресурсов, для которого выполняется назначение.</span><span class="sxs-lookup"><span data-stu-id="3eb14-148">The unique identifier (**id**) for the resource [service principal](serviceprincipal.md) for which the assignment is made.</span></span> <span data-ttu-id="3eb14-149">Требуется при создании.</span><span class="sxs-lookup"><span data-stu-id="3eb14-149">Required on create.</span></span> <span data-ttu-id="3eb14-150">Поддерживается `$filter` ( `eq` только).</span><span class="sxs-lookup"><span data-stu-id="3eb14-150">Supports `$filter` (`eq` only).</span></span> |
| <span data-ttu-id="3eb14-151">resourceDisplayName</span><span class="sxs-lookup"><span data-stu-id="3eb14-151">resourceDisplayName</span></span> | <span data-ttu-id="3eb14-152">String</span><span class="sxs-lookup"><span data-stu-id="3eb14-152">String</span></span> | <span data-ttu-id="3eb14-153">Отображаемое имя субъекта-службы приложения ресурсов, для которого выполняется назначение.</span><span class="sxs-lookup"><span data-stu-id="3eb14-153">The display name of the resource app's service principal to which the assignment is made.</span></span> <span data-ttu-id="3eb14-154">Не поддерживает `$filter` .</span><span class="sxs-lookup"><span data-stu-id="3eb14-154">Does not support `$filter`.</span></span> |
| <span data-ttu-id="3eb14-155">аппролеид</span><span class="sxs-lookup"><span data-stu-id="3eb14-155">appRoleId</span></span> | <span data-ttu-id="3eb14-156">Guid</span><span class="sxs-lookup"><span data-stu-id="3eb14-156">Guid</span></span> | <span data-ttu-id="3eb14-157">Идентификатор (**ID**) для [роли приложения](approle.md) , назначенный участнику.</span><span class="sxs-lookup"><span data-stu-id="3eb14-157">The identifier (**id**) for the [app role](approle.md) which is assigned to the principal.</span></span> <span data-ttu-id="3eb14-158">Эта роль приложения должна быть представлена в свойстве **appRoles** для субъекта-службы приложения ресурса (**resourceId**).</span><span class="sxs-lookup"><span data-stu-id="3eb14-158">This app role must be exposed in the **appRoles** property on the resource application's service principal (**resourceId**).</span></span> <span data-ttu-id="3eb14-159">Если приложение-ресурс не объявило роли приложений, идентификатор роли приложения по умолчанию `00000000-0000-0000-0000-000000000000` можно указать, чтобы сообщить, что участник назначен приложению ресурсов без каких-либо конкретных ролей приложения.</span><span class="sxs-lookup"><span data-stu-id="3eb14-159">If the resource application has not declared any app roles, a default app role ID of `00000000-0000-0000-0000-000000000000` can be specified to signal that the principal is assigned to the resource app without any specific app roles.</span></span> <span data-ttu-id="3eb14-160">Требуется при создании.</span><span class="sxs-lookup"><span data-stu-id="3eb14-160">Required on create.</span></span> <span data-ttu-id="3eb14-161">Не поддерживает `$filter` .</span><span class="sxs-lookup"><span data-stu-id="3eb14-161">Does not support `$filter`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="3eb14-162">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3eb14-162">JSON representation</span></span>

<span data-ttu-id="3eb14-163">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3eb14-163">Here is a JSON representation of the resource</span></span>

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

---
title: тип ресурса oAuth2PermissionGrant
description: Представляет делегированную разрешения (области OAuth 2.0), которые были предоставлены приложению, часто в результате процесса согласия пользователя или администратора.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: identity-and-sign-in
author: psignoret
ms.openlocfilehash: 27977a758e937312b2d0ea45c84902c275b035ab
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/19/2021
ms.locfileid: "52546884"
---
# <a name="oauth2permissiongrant-resource-type"></a><span data-ttu-id="827e2-103">тип ресурса oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="827e2-103">oAuth2PermissionGrant resource type</span></span>

<span data-ttu-id="827e2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="827e2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="827e2-105">Представляет делегированную лицензию, выданную директору службы приложения.</span><span class="sxs-lookup"><span data-stu-id="827e2-105">Represents the delegated permissions that have been granted to an application's service principal.</span></span>

<span data-ttu-id="827e2-106">Гранты на делегирование разрешений могут создаваться в результате согласия пользователя на запрос приложения на доступ к API или непосредственного создания.</span><span class="sxs-lookup"><span data-stu-id="827e2-106">Delegated permissions grants can be created as a result of a user consenting the an application's request to access an API, or created directly.</span></span>

<span data-ttu-id="827e2-107">Делегирование разрешений иногда называется "области OAuth 2.0" или "scopes".</span><span class="sxs-lookup"><span data-stu-id="827e2-107">Delegated permissions are sometimes referred to as "OAuth 2.0 scopes" or "scopes".</span></span>

## <a name="methods"></a><span data-ttu-id="827e2-108">Методы</span><span class="sxs-lookup"><span data-stu-id="827e2-108">Methods</span></span>

| <span data-ttu-id="827e2-109">Метод</span><span class="sxs-lookup"><span data-stu-id="827e2-109">Method</span></span> | <span data-ttu-id="827e2-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="827e2-110">Return Type</span></span> | <span data-ttu-id="827e2-111">Описание</span><span class="sxs-lookup"><span data-stu-id="827e2-111">Description</span></span> |
|:---------------|:--------|:----------|
| [<span data-ttu-id="827e2-112">Список oAuth2PermissionGrants</span><span class="sxs-lookup"><span data-stu-id="827e2-112">List oAuth2PermissionGrants</span></span>](../api/oauth2permissiongrant-list.md) | <span data-ttu-id="827e2-113">Коллекция [oAuth2PermissionGrant](oauth2permissiongrant.md)</span><span class="sxs-lookup"><span data-stu-id="827e2-113">[oAuth2PermissionGrant](oauth2permissiongrant.md) collection</span></span> | <span data-ttu-id="827e2-114">Получение списка делегирования разрешений.</span><span class="sxs-lookup"><span data-stu-id="827e2-114">Retrieve a list of delegated permission grants.</span></span> |
| [<span data-ttu-id="827e2-115">Получить oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="827e2-115">Get oAuth2PermissionGrant</span></span>](../api/oauth2permissiongrant-get.md) | [<span data-ttu-id="827e2-116">oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="827e2-116">oAuth2PermissionGrant</span></span>](oauth2permissiongrant.md)  | <span data-ttu-id="827e2-117">Ознакомьтесь с одним делегированным разрешением.</span><span class="sxs-lookup"><span data-stu-id="827e2-117">Read a single delegated permission grant.</span></span>|
| [<span data-ttu-id="827e2-118">Создание oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="827e2-118">Create oAuth2PermissionGrant</span></span>](../api/oauth2permissiongrant-post.md) | [<span data-ttu-id="827e2-119">oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="827e2-119">oAuth2PermissionGrant</span></span>](oauth2permissiongrant.md) | <span data-ttu-id="827e2-120">Создание делегированного разрешения.</span><span class="sxs-lookup"><span data-stu-id="827e2-120">Create a delegated permission grant.</span></span> |
| [<span data-ttu-id="827e2-121">Обновление oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="827e2-121">Update oAuth2PermissionGrant</span></span>](../api/oauth2permissiongrant-update.md) | <span data-ttu-id="827e2-122">Нет</span><span class="sxs-lookup"><span data-stu-id="827e2-122">None</span></span> | <span data-ttu-id="827e2-123">Обновление объекта oAuth2PermissionGrant.</span><span class="sxs-lookup"><span data-stu-id="827e2-123">Update oAuth2PermissionGrant object.</span></span> |
| [<span data-ttu-id="827e2-124">Удаление oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="827e2-124">Delete oAuth2PermissionGrant</span></span>](../api/oauth2permissiongrant-delete.md) | <span data-ttu-id="827e2-125">Нет</span><span class="sxs-lookup"><span data-stu-id="827e2-125">None</span></span>  | <span data-ttu-id="827e2-126">Удаление делегированного разрешения.</span><span class="sxs-lookup"><span data-stu-id="827e2-126">Delete a delegated permission grant.</span></span> |
| [<span data-ttu-id="827e2-127">Разность</span><span class="sxs-lookup"><span data-stu-id="827e2-127">Delta</span></span>](../api/oauth2permissiongrant-delta.md) | <span data-ttu-id="827e2-128">Коллекция [oAuth2PermissionGrant](oauth2permissiongrant.md)</span><span class="sxs-lookup"><span data-stu-id="827e2-128">[oAuth2PermissionGrant](oauth2permissiongrant.md) collection</span></span> |<span data-ttu-id="827e2-129">Получить вновь созданные, обновленные или удаленные **объекты oauth2permissiongrant** без полного чтения всей коллекции ресурсов.</span><span class="sxs-lookup"><span data-stu-id="827e2-129">Get newly created, updated, or deleted **oauth2permissiongrant** objects without performing a full read of the entire resource collection.</span></span> |

## <a name="properties"></a><span data-ttu-id="827e2-130">Свойства</span><span class="sxs-lookup"><span data-stu-id="827e2-130">Properties</span></span>

| <span data-ttu-id="827e2-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="827e2-131">Property</span></span> | <span data-ttu-id="827e2-132">Тип</span><span class="sxs-lookup"><span data-stu-id="827e2-132">Type</span></span> | <span data-ttu-id="827e2-133">Описание</span><span class="sxs-lookup"><span data-stu-id="827e2-133">Description</span></span> |
|:---------------|:--------|:----------|
| <span data-ttu-id="827e2-134">id</span><span class="sxs-lookup"><span data-stu-id="827e2-134">id</span></span> | <span data-ttu-id="827e2-135">String</span><span class="sxs-lookup"><span data-stu-id="827e2-135">String</span></span> | <span data-ttu-id="827e2-136">Уникальный идентификатор **для oAuth2PermissionGrant**.</span><span class="sxs-lookup"><span data-stu-id="827e2-136">Unique identifier for the **oAuth2PermissionGrant**.</span></span> <span data-ttu-id="827e2-137">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="827e2-137">Read-only.</span></span>|
| <span data-ttu-id="827e2-138">clientId</span><span class="sxs-lookup"><span data-stu-id="827e2-138">clientId</span></span> | <span data-ttu-id="827e2-139">String</span><span class="sxs-lookup"><span data-stu-id="827e2-139">String</span></span> | <span data-ttu-id="827e2-140">ID **директора** клиентской службы для приложения, которому разрешено действовать от имени пользователя, входишего в него, при доступе к API. [](serviceprincipal.md)</span><span class="sxs-lookup"><span data-stu-id="827e2-140">The **id** of the client [service principal](serviceprincipal.md) for the application which is authorized to act on behalf of a signed-in user when accessing an API.</span></span> <span data-ttu-id="827e2-141">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="827e2-141">Required.</span></span> <span data-ttu-id="827e2-142">Поддерживает `$filter` (только `eq`).</span><span class="sxs-lookup"><span data-stu-id="827e2-142">Supports `$filter` (`eq` only).</span></span> |
| <span data-ttu-id="827e2-143">consentType</span><span class="sxs-lookup"><span data-stu-id="827e2-143">consentType</span></span> | <span data-ttu-id="827e2-144">String</span><span class="sxs-lookup"><span data-stu-id="827e2-144">String</span></span> | <span data-ttu-id="827e2-145">Указывает, предоставляется ли авторизация клиентского приложения для выдают себя за всех пользователей или только определенного пользователя.</span><span class="sxs-lookup"><span data-stu-id="827e2-145">Indicates whether authorization is granted for the client application to impersonate all users or only a specific user.</span></span> <span data-ttu-id="827e2-146">*AllPrincipals* указывает авторизацию, чтобы выдать себя за всех пользователей.</span><span class="sxs-lookup"><span data-stu-id="827e2-146">*AllPrincipals* indicates authorization to impersonate all users.</span></span> <span data-ttu-id="827e2-147">*Principal* указывает авторизацию, чтобы выдать себя за конкретного пользователя.</span><span class="sxs-lookup"><span data-stu-id="827e2-147">*Principal* indicates authorization to impersonate a specific user.</span></span> <span data-ttu-id="827e2-148">Согласие от имени всех пользователей может быть предоставлено администратором.</span><span class="sxs-lookup"><span data-stu-id="827e2-148">Consent on behalf of all users can be granted by an administrator.</span></span> <span data-ttu-id="827e2-149">В некоторых случаях для некоторых делегированных разрешений пользователям, не относя правительственным администраторам, может быть разрешено согласие от имени самих себя.</span><span class="sxs-lookup"><span data-stu-id="827e2-149">Non-admin users may be authorized to consent on behalf of themselves in some cases, for some delegated permissions.</span></span> <span data-ttu-id="827e2-150">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="827e2-150">Required.</span></span> <span data-ttu-id="827e2-151">Поддерживает `$filter` (только `eq`).</span><span class="sxs-lookup"><span data-stu-id="827e2-151">Supports `$filter` (`eq` only).</span></span> |
| <span data-ttu-id="827e2-152">principalId</span><span class="sxs-lookup"><span data-stu-id="827e2-152">principalId</span></span> | <span data-ttu-id="827e2-153">String</span><span class="sxs-lookup"><span data-stu-id="827e2-153">String</span></span> | <span data-ttu-id="827e2-154">ID **пользователя,** от имени которого клиент уполномочен получать доступ к ресурсу, если **consentType** является [](user.md) *основным.*</span><span class="sxs-lookup"><span data-stu-id="827e2-154">The **id** of the [user](user.md) on behalf of whom the client is authorized to access the resource, when **consentType** is *Principal*.</span></span> <span data-ttu-id="827e2-155">Если **consentType** *— это AllPrincipals,* это значение является null.</span><span class="sxs-lookup"><span data-stu-id="827e2-155">If **consentType** is *AllPrincipals* this value is null.</span></span> <span data-ttu-id="827e2-156">Обязательно, когда **consentType** является *основным*.</span><span class="sxs-lookup"><span data-stu-id="827e2-156">Required when **consentType** is *Principal*.</span></span> |
| <span data-ttu-id="827e2-157">resourceId</span><span class="sxs-lookup"><span data-stu-id="827e2-157">resourceId</span></span> | <span data-ttu-id="827e2-158">String</span><span class="sxs-lookup"><span data-stu-id="827e2-158">String</span></span> | <span data-ttu-id="827e2-159">ID **главного** ресурса [службы,](serviceprincipal.md) к которому разрешен доступ.</span><span class="sxs-lookup"><span data-stu-id="827e2-159">The **id** of the resource [service principal](serviceprincipal.md) to which access is authorized.</span></span> <span data-ttu-id="827e2-160">При этом определяется API, который клиент уполномочен пытаться вызвать от имени подписанного пользователя.</span><span class="sxs-lookup"><span data-stu-id="827e2-160">This identifies the API which the client is authorized to attempt to call on behalf of a signed-in user.</span></span> |
| <span data-ttu-id="827e2-161">scope</span><span class="sxs-lookup"><span data-stu-id="827e2-161">scope</span></span> | <span data-ttu-id="827e2-162">String</span><span class="sxs-lookup"><span data-stu-id="827e2-162">String</span></span> | <span data-ttu-id="827e2-163">Разделенный пробелом список значений утверждений для делегирования разрешений, которые должны быть включены в маркеры доступа для приложения-ресурса (API).</span><span class="sxs-lookup"><span data-stu-id="827e2-163">A space-separated list of the claim values for delegated permissions which should be included in access tokens for the resource application (the API).</span></span> <span data-ttu-id="827e2-164">Например, `openid User.Read GroupMember.Read.All`.</span><span class="sxs-lookup"><span data-stu-id="827e2-164">For example, `openid User.Read GroupMember.Read.All`.</span></span> <span data-ttu-id="827e2-165">Каждое значение утверждения  должно совпадать с полем значения одного из делегированных разрешений, определенных API, перечисленным в свойстве **publishedPermissionScopes** директора [службы ресурсов.](serviceprincipal.md)</span><span class="sxs-lookup"><span data-stu-id="827e2-165">Each claim value should match the **value** field of one of the delegated permissions defined by the API, listed in the **publishedPermissionScopes** property of the resource [service principal](serviceprincipal.md).</span></span> |
| <span data-ttu-id="827e2-166">startTime</span><span class="sxs-lookup"><span data-stu-id="827e2-166">startTime</span></span> | <span data-ttu-id="827e2-167">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="827e2-167">DateTimeOffset</span></span> | <span data-ttu-id="827e2-168">В настоящее время значение времени начала игнорируется, но при создании **oAuth2PermissionGrant** требуется значение.</span><span class="sxs-lookup"><span data-stu-id="827e2-168">Currently, the start time value is ignored, but a value is required when creating an **oAuth2PermissionGrant**.</span></span> <span data-ttu-id="827e2-169">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="827e2-169">Required.</span></span> |
| <span data-ttu-id="827e2-170">expiryTime</span><span class="sxs-lookup"><span data-stu-id="827e2-170">expiryTime</span></span> | <span data-ttu-id="827e2-171">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="827e2-171">DateTimeOffset</span></span> | <span data-ttu-id="827e2-172">В настоящее время значение конца времени игнорируется, но при создании **oAuth2PermissionGrant** требуется значение.</span><span class="sxs-lookup"><span data-stu-id="827e2-172">Currently, the end time value is ignored, but a value is required when creating an **oAuth2PermissionGrant**.</span></span> <span data-ttu-id="827e2-173">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="827e2-173">Required.</span></span> |

## <a name="relationships"></a><span data-ttu-id="827e2-174">Связи</span><span class="sxs-lookup"><span data-stu-id="827e2-174">Relationships</span></span>
<span data-ttu-id="827e2-175">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="827e2-175">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="827e2-176">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="827e2-176">JSON representation</span></span>

<span data-ttu-id="827e2-177">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="827e2-177">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.oAuth2PermissionGrant"
}-->

```json
{
  "clientId": "string",
  "consentType": "string",
  "id": "string (identifier)",
  "principalId": "string",
  "resourceId": "string",
  "scope": "string",
  "startTime": "String (timestamp)",
  "expiryTime": "String (timestamp)"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "oAuth2PermissionGrant resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->



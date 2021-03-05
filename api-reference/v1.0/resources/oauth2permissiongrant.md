---
title: тип ресурса oAuth2PermissionGrant
description: Представляет делегированную разрешения (области OAuth 2.0), которые были предоставлены приложению, часто в результате процесса согласия пользователя или администратора.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: identity-and-sign-in
author: psignoret
ms.openlocfilehash: d0c9e78d22a882998c0e17ba521cc76a611697af
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50432846"
---
# <a name="oauth2permissiongrant-resource-type"></a><span data-ttu-id="bad5b-103">тип ресурса oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="bad5b-103">oAuth2PermissionGrant resource type</span></span>

<span data-ttu-id="bad5b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bad5b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="bad5b-105">Представляет делегированную лицензию, выданную директору службы приложения.</span><span class="sxs-lookup"><span data-stu-id="bad5b-105">Represents the delegated permissions that have been granted to an application's service principal.</span></span>

<span data-ttu-id="bad5b-106">Гранты на делегирование разрешений могут создаваться в результате согласия пользователя на запрос приложения на доступ к API или непосредственного создания.</span><span class="sxs-lookup"><span data-stu-id="bad5b-106">Delegated permissions grants can be created as a result of a user consenting the an application's request to access an API, or created directly.</span></span>

<span data-ttu-id="bad5b-107">Делегирование разрешений иногда называется "области OAuth 2.0" или "scopes".</span><span class="sxs-lookup"><span data-stu-id="bad5b-107">Delegated permissions are sometimes referred to as "OAuth 2.0 scopes" or "scopes".</span></span>

## <a name="methods"></a><span data-ttu-id="bad5b-108">Методы</span><span class="sxs-lookup"><span data-stu-id="bad5b-108">Methods</span></span>

| <span data-ttu-id="bad5b-109">Метод</span><span class="sxs-lookup"><span data-stu-id="bad5b-109">Method</span></span> | <span data-ttu-id="bad5b-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="bad5b-110">Return Type</span></span> | <span data-ttu-id="bad5b-111">Описание</span><span class="sxs-lookup"><span data-stu-id="bad5b-111">Description</span></span> |
|:---------------|:--------|:----------|
| [<span data-ttu-id="bad5b-112">Список oAuth2PermissionGrants</span><span class="sxs-lookup"><span data-stu-id="bad5b-112">List oAuth2PermissionGrants</span></span>](../api/oauth2permissiongrant-list.md) | <span data-ttu-id="bad5b-113">Коллекция [oAuth2PermissionGrant](oauth2permissiongrant.md)</span><span class="sxs-lookup"><span data-stu-id="bad5b-113">[oAuth2PermissionGrant](oauth2permissiongrant.md) collection</span></span> | <span data-ttu-id="bad5b-114">Получение списка делегирования разрешений.</span><span class="sxs-lookup"><span data-stu-id="bad5b-114">Retrieve a list of delegated permission grants.</span></span> |
| [<span data-ttu-id="bad5b-115">Получить oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="bad5b-115">Get oAuth2PermissionGrant</span></span>](../api/oauth2permissiongrant-get.md) | [<span data-ttu-id="bad5b-116">oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="bad5b-116">oAuth2PermissionGrant</span></span>](oauth2permissiongrant.md)  | <span data-ttu-id="bad5b-117">Ознакомьтесь с одним делегированным разрешением.</span><span class="sxs-lookup"><span data-stu-id="bad5b-117">Read a single delegated permission grant.</span></span>|
| [<span data-ttu-id="bad5b-118">Создание oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="bad5b-118">Create oAuth2PermissionGrant</span></span>](../api/oauth2permissiongrant-post.md) | [<span data-ttu-id="bad5b-119">oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="bad5b-119">oAuth2PermissionGrant</span></span>](oauth2permissiongrant.md) | <span data-ttu-id="bad5b-120">Создание делегированного разрешения.</span><span class="sxs-lookup"><span data-stu-id="bad5b-120">Create a delegated permission grant.</span></span> |
| [<span data-ttu-id="bad5b-121">Обновление oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="bad5b-121">Update oAuth2PermissionGrant</span></span>](../api/oauth2permissiongrant-update.md) | <span data-ttu-id="bad5b-122">Нет</span><span class="sxs-lookup"><span data-stu-id="bad5b-122">None</span></span> | <span data-ttu-id="bad5b-123">Обновление объекта oAuth2PermissionGrant.</span><span class="sxs-lookup"><span data-stu-id="bad5b-123">Update oAuth2PermissionGrant object.</span></span> |
| [<span data-ttu-id="bad5b-124">Удаление oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="bad5b-124">Delete oAuth2PermissionGrant</span></span>](../api/oauth2permissiongrant-delete.md) | <span data-ttu-id="bad5b-125">Нет</span><span class="sxs-lookup"><span data-stu-id="bad5b-125">None</span></span>  | <span data-ttu-id="bad5b-126">Удаление делегированного разрешения.</span><span class="sxs-lookup"><span data-stu-id="bad5b-126">Delete a delegated permission grant.</span></span> |
|[<span data-ttu-id="bad5b-127">Получение дельты</span><span class="sxs-lookup"><span data-stu-id="bad5b-127">Get delta</span></span>](../api/oauth2permissiongrant-delta.md)|[<span data-ttu-id="bad5b-128">oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="bad5b-128">oAuth2PermissionGrant</span></span>](oauth2permissiongrant.md)|<span data-ttu-id="bad5b-129">Получить вновь созданные, обновленные или удаленные **объекты oauth2permissiongrant** без полного чтения всей коллекции ресурсов.</span><span class="sxs-lookup"><span data-stu-id="bad5b-129">Get newly created, updated, or deleted **oauth2permissiongrant** objects without performing a full read of the entire resource collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="bad5b-130">Свойства</span><span class="sxs-lookup"><span data-stu-id="bad5b-130">Properties</span></span>

| <span data-ttu-id="bad5b-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="bad5b-131">Property</span></span> | <span data-ttu-id="bad5b-132">Тип</span><span class="sxs-lookup"><span data-stu-id="bad5b-132">Type</span></span> | <span data-ttu-id="bad5b-133">Описание</span><span class="sxs-lookup"><span data-stu-id="bad5b-133">Description</span></span> |
|:---------------|:--------|:----------|
| <span data-ttu-id="bad5b-134">id</span><span class="sxs-lookup"><span data-stu-id="bad5b-134">id</span></span> | <span data-ttu-id="bad5b-135">String</span><span class="sxs-lookup"><span data-stu-id="bad5b-135">String</span></span> | <span data-ttu-id="bad5b-136">Уникальный идентификатор **для oAuth2PermissionGrant**.</span><span class="sxs-lookup"><span data-stu-id="bad5b-136">Unique identifier for the **oAuth2PermissionGrant**.</span></span> <span data-ttu-id="bad5b-137">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="bad5b-137">Read-only.</span></span>|
| <span data-ttu-id="bad5b-138">clientId</span><span class="sxs-lookup"><span data-stu-id="bad5b-138">clientId</span></span> | <span data-ttu-id="bad5b-139">String</span><span class="sxs-lookup"><span data-stu-id="bad5b-139">String</span></span> | <span data-ttu-id="bad5b-140">ID **директора** клиентской службы для приложения, которому разрешено действовать от имени пользователя, входишего в него, при доступе к API. [](serviceprincipal.md)</span><span class="sxs-lookup"><span data-stu-id="bad5b-140">The **id** of the client [service principal](serviceprincipal.md) for the application which is authorized to act on behalf of a signed-in user when accessing an API.</span></span> <span data-ttu-id="bad5b-141">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="bad5b-141">Required.</span></span> <span data-ttu-id="bad5b-142">Поддерживает `$filter` (только `eq`).</span><span class="sxs-lookup"><span data-stu-id="bad5b-142">Supports `$filter` (`eq` only).</span></span> |
| <span data-ttu-id="bad5b-143">consentType</span><span class="sxs-lookup"><span data-stu-id="bad5b-143">consentType</span></span> | <span data-ttu-id="bad5b-144">String</span><span class="sxs-lookup"><span data-stu-id="bad5b-144">String</span></span> | <span data-ttu-id="bad5b-145">Указывает, предоставляется ли клиентской приложению авторизация, чтобы выдать себя за всех пользователей или только определенного пользователя.</span><span class="sxs-lookup"><span data-stu-id="bad5b-145">Indicates if authorization is granted for the client application to impersonate all users or only a specific user.</span></span> <span data-ttu-id="bad5b-146">*AllPrincipals* указывает авторизацию, чтобы выдать себя за всех пользователей.</span><span class="sxs-lookup"><span data-stu-id="bad5b-146">*AllPrincipals* indicates authorization to impersonate all users.</span></span> <span data-ttu-id="bad5b-147">*Principal* указывает авторизацию, чтобы выдать себя за конкретного пользователя.</span><span class="sxs-lookup"><span data-stu-id="bad5b-147">*Principal* indicates authorization to impersonate a specific user.</span></span> <span data-ttu-id="bad5b-148">Согласие от имени всех пользователей может быть предоставлено администратором.</span><span class="sxs-lookup"><span data-stu-id="bad5b-148">Consent on behalf of all users can be granted by an administrator.</span></span> <span data-ttu-id="bad5b-149">В некоторых случаях для некоторых делегированных разрешений пользователям, не относя правительственным администраторам, может быть разрешено согласие от имени самих себя.</span><span class="sxs-lookup"><span data-stu-id="bad5b-149">Non-admin users may be authorized to consent on behalf of themselves in some cases, for some delegated permissions.</span></span> <span data-ttu-id="bad5b-150">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="bad5b-150">Required.</span></span> <span data-ttu-id="bad5b-151">Поддерживает `$filter` (только `eq`).</span><span class="sxs-lookup"><span data-stu-id="bad5b-151">Supports `$filter` (`eq` only).</span></span> |
| <span data-ttu-id="bad5b-152">principalId</span><span class="sxs-lookup"><span data-stu-id="bad5b-152">principalId</span></span> | <span data-ttu-id="bad5b-153">String</span><span class="sxs-lookup"><span data-stu-id="bad5b-153">String</span></span> | <span data-ttu-id="bad5b-154">ID **пользователя,** от имени которого клиент уполномочен получать доступ к ресурсу, если **consentType** является [](user.md) *основным.*</span><span class="sxs-lookup"><span data-stu-id="bad5b-154">The **id** of the [user](user.md) on behalf of whom the client is authorized to access the resource, when **consentType** is *Principal*.</span></span> <span data-ttu-id="bad5b-155">Если **consentType** *— это AllPrincipals,* это значение является null.</span><span class="sxs-lookup"><span data-stu-id="bad5b-155">If **consentType** is *AllPrincipals* this value is null.</span></span> <span data-ttu-id="bad5b-156">Обязательно, когда **consentType** является *основным*.</span><span class="sxs-lookup"><span data-stu-id="bad5b-156">Required when **consentType** is *Principal*.</span></span> |
| <span data-ttu-id="bad5b-157">resourceId</span><span class="sxs-lookup"><span data-stu-id="bad5b-157">resourceId</span></span> | <span data-ttu-id="bad5b-158">String</span><span class="sxs-lookup"><span data-stu-id="bad5b-158">String</span></span> | <span data-ttu-id="bad5b-159">ID **главного** ресурса [службы,](serviceprincipal.md) к которому разрешен доступ.</span><span class="sxs-lookup"><span data-stu-id="bad5b-159">The **id** of the resource [service principal](serviceprincipal.md) to which access is authorized.</span></span> <span data-ttu-id="bad5b-160">При этом определяется API, который клиент уполномочен пытаться вызвать от имени подписанного пользователя.</span><span class="sxs-lookup"><span data-stu-id="bad5b-160">This identifies the API which the client is authorized to attempt to call on behalf of a signed-in user.</span></span> |
| <span data-ttu-id="bad5b-161">scope</span><span class="sxs-lookup"><span data-stu-id="bad5b-161">scope</span></span> | <span data-ttu-id="bad5b-162">String</span><span class="sxs-lookup"><span data-stu-id="bad5b-162">String</span></span> | <span data-ttu-id="bad5b-163">Разделенный пробелом список значений утверждений для делегирования разрешений, которые должны быть включены в маркеры доступа для приложения-ресурса (API).</span><span class="sxs-lookup"><span data-stu-id="bad5b-163">A space-separated list of the claim values for delegated permissions which should be included in access tokens for the resource application (the API).</span></span> <span data-ttu-id="bad5b-164">Например, `openid User.Read GroupMember.Read.All`.</span><span class="sxs-lookup"><span data-stu-id="bad5b-164">For example, `openid User.Read GroupMember.Read.All`.</span></span> <span data-ttu-id="bad5b-165">Каждое значение утверждения  должно совпадать с полем значения одного из делегированных разрешений, определенных API, перечисленным в свойстве **publishedPermissionScopes** директора [службы ресурсов.](serviceprincipal.md)</span><span class="sxs-lookup"><span data-stu-id="bad5b-165">Each claim value should match the **value** field of one of the delegated permissions defined by the API, listed in the **publishedPermissionScopes** property of the resource [service principal](serviceprincipal.md).</span></span> |

## <a name="relationships"></a><span data-ttu-id="bad5b-166">Связи</span><span class="sxs-lookup"><span data-stu-id="bad5b-166">Relationships</span></span>

<span data-ttu-id="bad5b-167">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="bad5b-167">None.</span></span>

<span data-ttu-id="bad5b-168">Этот ресурс поддерживает отслеживание добавлений, удалений и обновлений с помощью [разностного запроса](/graph/delta-query-overview) с функцией [delta](../api/oauth2permissiongrant-delta.md).</span><span class="sxs-lookup"><span data-stu-id="bad5b-168">This resource supports using [delta query](/graph/delta-query-overview) to track incremental additions, deletions, and updates, by providing a [delta](../api/oauth2permissiongrant-delta.md) function.</span></span>

## <a name="json-representation"></a><span data-ttu-id="bad5b-169">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bad5b-169">JSON representation</span></span>

<span data-ttu-id="bad5b-170">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bad5b-170">The following is a JSON representation of the resource.</span></span>

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
  "scope": "string"
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


---
title: Тип ресурса oAuth2PermissionGrant
description: Представляет делегированные разрешения (области OAuth 2,0), которые были предоставлены приложению, часто в результате процесса согласия пользователя или администратора.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: psignoret
ms.openlocfilehash: 557bd9973a3a04ffedb2104a480823de21c95499
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48041199"
---
# <a name="oauth2permissiongrant-resource-type"></a><span data-ttu-id="8e296-103">Тип ресурса oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="8e296-103">oAuth2PermissionGrant resource type</span></span>

<span data-ttu-id="8e296-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8e296-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8e296-105">Представляет делегированные разрешения, которые были предоставлены участнику службы приложения.</span><span class="sxs-lookup"><span data-stu-id="8e296-105">Represents the delegated permissions that have been granted to an application's service principal.</span></span>

<span data-ttu-id="8e296-106">Предоставленные делегированные разрешения могут быть созданы в результате того, что пользователь отправил запрос на доступ к API или создал его напрямую.</span><span class="sxs-lookup"><span data-stu-id="8e296-106">Delegated permissions grants can be created as a result of a user consenting the an application's request to access an API, or created directly.</span></span>

<span data-ttu-id="8e296-107">Делегированные разрешения иногда называются "областями" OAuth 2,0 "или" Scopes ".</span><span class="sxs-lookup"><span data-stu-id="8e296-107">Delegated permissions are sometimes referred to as "OAuth 2.0 scopes" or "scopes".</span></span>

## <a name="methods"></a><span data-ttu-id="8e296-108">Методы</span><span class="sxs-lookup"><span data-stu-id="8e296-108">Methods</span></span>

| <span data-ttu-id="8e296-109">Метод</span><span class="sxs-lookup"><span data-stu-id="8e296-109">Method</span></span> | <span data-ttu-id="8e296-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="8e296-110">Return Type</span></span> | <span data-ttu-id="8e296-111">Описание</span><span class="sxs-lookup"><span data-stu-id="8e296-111">Description</span></span> |
|:---------------|:--------|:----------|
| [<span data-ttu-id="8e296-112">Список oAuth2PermissionGrants</span><span class="sxs-lookup"><span data-stu-id="8e296-112">List oAuth2PermissionGrants</span></span>](../api/oauth2permissiongrant-list.md) | <span data-ttu-id="8e296-113">Коллекция [oAuth2PermissionGrant](oauth2permissiongrant.md)</span><span class="sxs-lookup"><span data-stu-id="8e296-113">[oAuth2PermissionGrant](oauth2permissiongrant.md) collection</span></span> | <span data-ttu-id="8e296-114">Получение списка предоставленных делегированных разрешений.</span><span class="sxs-lookup"><span data-stu-id="8e296-114">Retrieve a list of delegated permission grants.</span></span> |
| [<span data-ttu-id="8e296-115">Получение oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="8e296-115">Get oAuth2PermissionGrant</span></span>](../api/oauth2permissiongrant-get.md) | [<span data-ttu-id="8e296-116">oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="8e296-116">oAuth2PermissionGrant</span></span>](oauth2permissiongrant.md)  | <span data-ttu-id="8e296-117">Считывание разрешения с одним делегированным делегированием.</span><span class="sxs-lookup"><span data-stu-id="8e296-117">Read a single delegated permission grant.</span></span>|
| [<span data-ttu-id="8e296-118">Создание oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="8e296-118">Create oAuth2PermissionGrant</span></span>](../api/oauth2permissiongrant-post.md) | [<span data-ttu-id="8e296-119">oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="8e296-119">oAuth2PermissionGrant</span></span>](oauth2permissiongrant.md) | <span data-ttu-id="8e296-120">Создайте делегированное предоставление разрешений.</span><span class="sxs-lookup"><span data-stu-id="8e296-120">Create a delegated permission grant.</span></span> |
| [<span data-ttu-id="8e296-121">Обновление oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="8e296-121">Update oAuth2PermissionGrant</span></span>](../api/oauth2permissiongrant-update.md) | <span data-ttu-id="8e296-122">Нет</span><span class="sxs-lookup"><span data-stu-id="8e296-122">None</span></span> | <span data-ttu-id="8e296-123">Обновление объекта oAuth2PermissionGrant.</span><span class="sxs-lookup"><span data-stu-id="8e296-123">Update oAuth2PermissionGrant object.</span></span> |
| [<span data-ttu-id="8e296-124">Удаление oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="8e296-124">Delete oAuth2PermissionGrant</span></span>](../api/oauth2permissiongrant-delete.md) | <span data-ttu-id="8e296-125">Нет</span><span class="sxs-lookup"><span data-stu-id="8e296-125">None</span></span>  | <span data-ttu-id="8e296-126">Удаление делегированного предоставления разрешений.</span><span class="sxs-lookup"><span data-stu-id="8e296-126">Delete a delegated permission grant.</span></span> |
|[<span data-ttu-id="8e296-127">Получение дельты</span><span class="sxs-lookup"><span data-stu-id="8e296-127">Get delta</span></span>](../api/oauth2permissiongrant-delta.md)|[<span data-ttu-id="8e296-128">oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="8e296-128">oAuth2PermissionGrant</span></span>](oauth2permissiongrant.md)|<span data-ttu-id="8e296-129">Получение только что созданных, обновленных или удаленных объектов **oauth2permissiongrant** без выполнения полного считывания всей коллекции ресурсов.</span><span class="sxs-lookup"><span data-stu-id="8e296-129">Get newly created, updated, or deleted **oauth2permissiongrant** objects without performing a full read of the entire resource collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="8e296-130">Свойства</span><span class="sxs-lookup"><span data-stu-id="8e296-130">Properties</span></span>

| <span data-ttu-id="8e296-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="8e296-131">Property</span></span> | <span data-ttu-id="8e296-132">Тип</span><span class="sxs-lookup"><span data-stu-id="8e296-132">Type</span></span> | <span data-ttu-id="8e296-133">Описание</span><span class="sxs-lookup"><span data-stu-id="8e296-133">Description</span></span> |
|:---------------|:--------|:----------|
| <span data-ttu-id="8e296-134">id</span><span class="sxs-lookup"><span data-stu-id="8e296-134">id</span></span> | <span data-ttu-id="8e296-135">String</span><span class="sxs-lookup"><span data-stu-id="8e296-135">String</span></span> | <span data-ttu-id="8e296-136">Уникальный идентификатор для **oAuth2PermissionGrant**.</span><span class="sxs-lookup"><span data-stu-id="8e296-136">Unique identifier for the **oAuth2PermissionGrant**.</span></span> <span data-ttu-id="8e296-137">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8e296-137">Read-only.</span></span>|
| <span data-ttu-id="8e296-138">clientId</span><span class="sxs-lookup"><span data-stu-id="8e296-138">clientId</span></span> | <span data-ttu-id="8e296-139">String</span><span class="sxs-lookup"><span data-stu-id="8e296-139">String</span></span> | <span data-ttu-id="8e296-140">**Идентификатор** [субъекта-службы](serviceprincipal.md) клиента для приложения, которому разрешено работать от имени вошедшего пользователя при доступе к API.</span><span class="sxs-lookup"><span data-stu-id="8e296-140">The **id** of the client [service principal](serviceprincipal.md) for the application which is authorized to act on behalf of a signed-in user when accessing an API.</span></span> <span data-ttu-id="8e296-141">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="8e296-141">Required.</span></span> <span data-ttu-id="8e296-142">Поддерживается `$filter` ( `eq` только).</span><span class="sxs-lookup"><span data-stu-id="8e296-142">Supports `$filter` (`eq` only).</span></span> |
| <span data-ttu-id="8e296-143">консенттипе</span><span class="sxs-lookup"><span data-stu-id="8e296-143">consentType</span></span> | <span data-ttu-id="8e296-144">String</span><span class="sxs-lookup"><span data-stu-id="8e296-144">String</span></span> | <span data-ttu-id="8e296-145">Указывает, предоставляется ли авторизация клиентскому приложению для олицетворения всех пользователей или только определенного пользователя.</span><span class="sxs-lookup"><span data-stu-id="8e296-145">Indicates if authorization is granted for the client application to impersonate all users or only a specific user.</span></span> <span data-ttu-id="8e296-146">*АллпринЦипалс* указывает авторизацию для олицетворения всех пользователей.</span><span class="sxs-lookup"><span data-stu-id="8e296-146">*AllPrincipals* indicates authorization to impersonate all users.</span></span> <span data-ttu-id="8e296-147">*Субъект* указывает на авторизацию для олицетворения определенного пользователя.</span><span class="sxs-lookup"><span data-stu-id="8e296-147">*Principal* indicates authorization to impersonate a specific user.</span></span> <span data-ttu-id="8e296-148">Согласие от имени всех пользователей может быть предоставлено администратором.</span><span class="sxs-lookup"><span data-stu-id="8e296-148">Consent on behalf of all users can be granted by an administrator.</span></span> <span data-ttu-id="8e296-149">Пользователи, не являющиеся администраторами, могут быть авторизованы для разрешения от чужого имени в некоторых случаях для некоторых делегированных разрешений.</span><span class="sxs-lookup"><span data-stu-id="8e296-149">Non-admin users may be authorized to consent on behalf of themselves in some cases, for some delegated permissions.</span></span> <span data-ttu-id="8e296-150">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="8e296-150">Required.</span></span> <span data-ttu-id="8e296-151">Поддерживается `$filter` ( `eq` только).</span><span class="sxs-lookup"><span data-stu-id="8e296-151">Supports `$filter` (`eq` only).</span></span> |
| <span data-ttu-id="8e296-152">principalId</span><span class="sxs-lookup"><span data-stu-id="8e296-152">principalId</span></span> | <span data-ttu-id="8e296-153">String</span><span class="sxs-lookup"><span data-stu-id="8e296-153">String</span></span> | <span data-ttu-id="8e296-154">**Идентификатор** [пользователя](user.md) , от имени которого клиент имеет право доступа к ресурсу, когда **консенттипе** является *субъектом*.</span><span class="sxs-lookup"><span data-stu-id="8e296-154">The **id** of the [user](user.md) on behalf of whom the client is authorized to access the resource, when **consentType** is *Principal*.</span></span> <span data-ttu-id="8e296-155">Если **консенттипе** — *аллпринЦипалс* , это значение равно null.</span><span class="sxs-lookup"><span data-stu-id="8e296-155">If **consentType** is *AllPrincipals* this value is null.</span></span> <span data-ttu-id="8e296-156">Является обязательным, если **консенттипе** является *субъектом*.</span><span class="sxs-lookup"><span data-stu-id="8e296-156">Required when **consentType** is *Principal*.</span></span> |
| <span data-ttu-id="8e296-157">resourceId</span><span class="sxs-lookup"><span data-stu-id="8e296-157">resourceId</span></span> | <span data-ttu-id="8e296-158">String</span><span class="sxs-lookup"><span data-stu-id="8e296-158">String</span></span> | <span data-ttu-id="8e296-159">**Идентификатор** [субъекта службы](serviceprincipal.md) ресурсов, которому разрешен доступ.</span><span class="sxs-lookup"><span data-stu-id="8e296-159">The **id** of the resource [service principal](serviceprincipal.md) to which access is authorized.</span></span> <span data-ttu-id="8e296-160">Этот параметр определяет API, который клиент может пытаться вызвать от имени пользователя, выполнившего вход в систему.</span><span class="sxs-lookup"><span data-stu-id="8e296-160">This identifies the API which the client is authorized to attempt to call on behalf of a signed-in user.</span></span> |
| <span data-ttu-id="8e296-161">scope</span><span class="sxs-lookup"><span data-stu-id="8e296-161">scope</span></span> | <span data-ttu-id="8e296-162">String</span><span class="sxs-lookup"><span data-stu-id="8e296-162">String</span></span> | <span data-ttu-id="8e296-163">Разделенный пробелами список значений утверждений для делегированных разрешений, которые следует включить в маркеры доступа для приложения ресурсов (API).</span><span class="sxs-lookup"><span data-stu-id="8e296-163">A space-separated list of the claim values for delegated permissions which should be included in access tokens for the resource application (the API).</span></span> <span data-ttu-id="8e296-164">Например, `openid User.Read GroupMember.Read.All`.</span><span class="sxs-lookup"><span data-stu-id="8e296-164">For example, `openid User.Read GroupMember.Read.All`.</span></span> <span data-ttu-id="8e296-165">Каждое значение утверждения должно быть согласовано с полем **значение** одного из делегированных разрешений, определенных API, указанным в свойстве **публишедпермиссионскопес** [субъекта-службы](serviceprincipal.md)ресурсов.</span><span class="sxs-lookup"><span data-stu-id="8e296-165">Each claim value should match the **value** field of one of the delegated permissions defined by the API, listed in the **publishedPermissionScopes** property of the resource [service principal](serviceprincipal.md).</span></span> |

## <a name="relationships"></a><span data-ttu-id="8e296-166">Связи</span><span class="sxs-lookup"><span data-stu-id="8e296-166">Relationships</span></span>

<span data-ttu-id="8e296-167">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="8e296-167">None.</span></span>

<span data-ttu-id="8e296-168">Этот ресурс поддерживает отслеживание добавлений, удалений и обновлений с помощью [разностного запроса](/graph/delta-query-overview) с функцией [delta](../api/oauth2permissiongrant-delta.md).</span><span class="sxs-lookup"><span data-stu-id="8e296-168">This resource supports using [delta query](/graph/delta-query-overview) to track incremental additions, deletions, and updates, by providing a [delta](../api/oauth2permissiongrant-delta.md) function.</span></span>

## <a name="json-representation"></a><span data-ttu-id="8e296-169">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8e296-169">JSON representation</span></span>

<span data-ttu-id="8e296-170">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8e296-170">The following is a JSON representation of the resource.</span></span>

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


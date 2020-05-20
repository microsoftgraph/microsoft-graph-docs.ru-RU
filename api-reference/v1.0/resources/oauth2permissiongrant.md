---
title: Тип ресурса oAuth2PermissionGrant
description: Представляет делегированные разрешения (области OAuth 2,0), которые были предоставлены приложению, часто в результате процесса согласия пользователя или администратора.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: edf4ff7ed44e9b084ca2206b24fed0e18b5c581c
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/19/2020
ms.locfileid: "44290169"
---
# <a name="oauth2permissiongrant-resource-type"></a><span data-ttu-id="b4132-103">Тип ресурса oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="b4132-103">oAuth2PermissionGrant resource type</span></span>

<span data-ttu-id="b4132-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b4132-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b4132-105">Представляет делегированные разрешения, которые были предоставлены участнику службы приложения.</span><span class="sxs-lookup"><span data-stu-id="b4132-105">Represents the delegated permissions that have been granted to an application's service principal.</span></span>

<span data-ttu-id="b4132-106">Предоставленные делегированные разрешения могут быть созданы в результате того, что пользователь отправил запрос на доступ к API или создал его напрямую.</span><span class="sxs-lookup"><span data-stu-id="b4132-106">Delegated permissions grants can be created as a result of a user consenting the an application's request to access an API, or created directly.</span></span>

<span data-ttu-id="b4132-107">Делегированные разрешения иногда называются "областями" OAuth 2,0 "или" Scopes ".</span><span class="sxs-lookup"><span data-stu-id="b4132-107">Delegated permissions are sometimes referred to as "OAuth 2.0 scopes" or "scopes".</span></span>

## <a name="methods"></a><span data-ttu-id="b4132-108">Методы</span><span class="sxs-lookup"><span data-stu-id="b4132-108">Methods</span></span>

| <span data-ttu-id="b4132-109">Метод</span><span class="sxs-lookup"><span data-stu-id="b4132-109">Method</span></span> | <span data-ttu-id="b4132-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="b4132-110">Return Type</span></span> | <span data-ttu-id="b4132-111">Описание</span><span class="sxs-lookup"><span data-stu-id="b4132-111">Description</span></span> |
|:---------------|:--------|:----------|
| [<span data-ttu-id="b4132-112">Список oAuth2PermissionGrants</span><span class="sxs-lookup"><span data-stu-id="b4132-112">List oAuth2PermissionGrants</span></span>](../api/oauth2permissiongrant-list.md) | <span data-ttu-id="b4132-113">Коллекция [oAuth2PermissionGrant](oauth2permissiongrant.md)</span><span class="sxs-lookup"><span data-stu-id="b4132-113">[oAuth2PermissionGrant](oauth2permissiongrant.md) collection</span></span> | <span data-ttu-id="b4132-114">Получение списка предоставленных делегированных разрешений.</span><span class="sxs-lookup"><span data-stu-id="b4132-114">Retrieve a list of delegated permission grants.</span></span> |
| [<span data-ttu-id="b4132-115">Получение oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="b4132-115">Get oAuth2PermissionGrant</span></span>](../api/oauth2permissiongrant-get.md) | [<span data-ttu-id="b4132-116">oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="b4132-116">oAuth2PermissionGrant</span></span>](oauth2permissiongrant.md)  | <span data-ttu-id="b4132-117">Считывание разрешения с одним делегированным делегированием.</span><span class="sxs-lookup"><span data-stu-id="b4132-117">Read a single delegated permission grant.</span></span>|
| [<span data-ttu-id="b4132-118">Создание oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="b4132-118">Create oAuth2PermissionGrant</span></span>](../api/oauth2permissiongrant-post.md) | [<span data-ttu-id="b4132-119">oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="b4132-119">oAuth2PermissionGrant</span></span>](oauth2permissiongrant.md) | <span data-ttu-id="b4132-120">Создайте делегированное предоставление разрешений.</span><span class="sxs-lookup"><span data-stu-id="b4132-120">Create a delegated permission grant.</span></span> |
| [<span data-ttu-id="b4132-121">Обновление oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="b4132-121">Update oAuth2PermissionGrant</span></span>](../api/oauth2permissiongrant-update.md) | <span data-ttu-id="b4132-122">Нет</span><span class="sxs-lookup"><span data-stu-id="b4132-122">None</span></span> | <span data-ttu-id="b4132-123">Обновление объекта oAuth2PermissionGrant.</span><span class="sxs-lookup"><span data-stu-id="b4132-123">Update oAuth2PermissionGrant object.</span></span> |
| [<span data-ttu-id="b4132-124">Удаление oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="b4132-124">Delete oAuth2PermissionGrant</span></span>](../api/oauth2permissiongrant-delete.md) | <span data-ttu-id="b4132-125">Нет</span><span class="sxs-lookup"><span data-stu-id="b4132-125">None</span></span>  | <span data-ttu-id="b4132-126">Удаление делегированного предоставления разрешений.</span><span class="sxs-lookup"><span data-stu-id="b4132-126">Delete a delegated permission grant.</span></span> |

## <a name="properties"></a><span data-ttu-id="b4132-127">Свойства</span><span class="sxs-lookup"><span data-stu-id="b4132-127">Properties</span></span>

| <span data-ttu-id="b4132-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="b4132-128">Property</span></span> | <span data-ttu-id="b4132-129">Тип</span><span class="sxs-lookup"><span data-stu-id="b4132-129">Type</span></span> | <span data-ttu-id="b4132-130">Описание</span><span class="sxs-lookup"><span data-stu-id="b4132-130">Description</span></span> |
|:---------------|:--------|:----------|
| <span data-ttu-id="b4132-131">id</span><span class="sxs-lookup"><span data-stu-id="b4132-131">id</span></span> | <span data-ttu-id="b4132-132">Строка</span><span class="sxs-lookup"><span data-stu-id="b4132-132">String</span></span> | <span data-ttu-id="b4132-133">Уникальный идентификатор для **oAuth2PermissionGrant**.</span><span class="sxs-lookup"><span data-stu-id="b4132-133">Unique identifier for the **oAuth2PermissionGrant**.</span></span> <span data-ttu-id="b4132-134">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b4132-134">Read-only.</span></span>|
| <span data-ttu-id="b4132-135">clientId</span><span class="sxs-lookup"><span data-stu-id="b4132-135">clientId</span></span> | <span data-ttu-id="b4132-136">String</span><span class="sxs-lookup"><span data-stu-id="b4132-136">String</span></span> | <span data-ttu-id="b4132-137">**Идентификатор** [субъекта-службы](serviceprincipal.md) клиента для приложения, которому разрешено работать от имени вошедшего пользователя при доступе к API.</span><span class="sxs-lookup"><span data-stu-id="b4132-137">The **id** of the client [service principal](serviceprincipal.md) for the application which is authorized to act on behalf of a signed-in user when accessing an API.</span></span> <span data-ttu-id="b4132-138">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="b4132-138">Required.</span></span> <span data-ttu-id="b4132-139">Поддерживается `$filter` ( `eq` только).</span><span class="sxs-lookup"><span data-stu-id="b4132-139">Supports `$filter` (`eq` only).</span></span> |
| <span data-ttu-id="b4132-140">консенттипе</span><span class="sxs-lookup"><span data-stu-id="b4132-140">consentType</span></span> | <span data-ttu-id="b4132-141">String</span><span class="sxs-lookup"><span data-stu-id="b4132-141">String</span></span> | <span data-ttu-id="b4132-142">Указывает, предоставляется ли авторизация клиентскому приложению для олицетворения всех пользователей или только определенного пользователя.</span><span class="sxs-lookup"><span data-stu-id="b4132-142">Indicates if authorization is granted for the client application to impersonate all users or only a specific user.</span></span> <span data-ttu-id="b4132-143">*АллпринЦипалс* указывает авторизацию для олицетворения всех пользователей.</span><span class="sxs-lookup"><span data-stu-id="b4132-143">*AllPrincipals* indicates authorization to impersonate all users.</span></span> <span data-ttu-id="b4132-144">*Субъект* указывает на авторизацию для олицетворения определенного пользователя.</span><span class="sxs-lookup"><span data-stu-id="b4132-144">*Principal* indicates authorization to impersonate a specific user.</span></span> <span data-ttu-id="b4132-145">Согласие от имени всех пользователей может быть предоставлено администратором.</span><span class="sxs-lookup"><span data-stu-id="b4132-145">Consent on behalf of all users can be granted by an administrator.</span></span> <span data-ttu-id="b4132-146">Пользователи, не являющиеся администраторами, могут быть авторизованы для разрешения от чужого имени в некоторых случаях для некоторых делегированных разрешений.</span><span class="sxs-lookup"><span data-stu-id="b4132-146">Non-admin users may be authorized to consent on behalf of themselves in some cases, for some delegated permissions.</span></span> <span data-ttu-id="b4132-147">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="b4132-147">Required.</span></span> <span data-ttu-id="b4132-148">Поддерживается `$filter` ( `eq` только).</span><span class="sxs-lookup"><span data-stu-id="b4132-148">Supports `$filter` (`eq` only).</span></span> |
| <span data-ttu-id="b4132-149">principalId</span><span class="sxs-lookup"><span data-stu-id="b4132-149">principalId</span></span> | <span data-ttu-id="b4132-150">String</span><span class="sxs-lookup"><span data-stu-id="b4132-150">String</span></span> | <span data-ttu-id="b4132-151">**Идентификатор** [пользователя](user.md) , от имени которого клиент имеет право доступа к ресурсу, когда **консенттипе** является *субъектом*.</span><span class="sxs-lookup"><span data-stu-id="b4132-151">The **id** of the [user](user.md) on behalf of whom the client is authorized to access the resource, when **consentType** is *Principal*.</span></span> <span data-ttu-id="b4132-152">Если **консенттипе** — *аллпринЦипалс* , это значение равно null.</span><span class="sxs-lookup"><span data-stu-id="b4132-152">If **consentType** is *AllPrincipals* this value is null.</span></span> <span data-ttu-id="b4132-153">Является обязательным, если **консенттипе** является *субъектом*.</span><span class="sxs-lookup"><span data-stu-id="b4132-153">Required when **consentType** is *Principal*.</span></span> |
| <span data-ttu-id="b4132-154">resourceId</span><span class="sxs-lookup"><span data-stu-id="b4132-154">resourceId</span></span> | <span data-ttu-id="b4132-155">String</span><span class="sxs-lookup"><span data-stu-id="b4132-155">String</span></span> | <span data-ttu-id="b4132-156">**Идентификатор** [субъекта службы](serviceprincipal.md) ресурсов, которому разрешен доступ.</span><span class="sxs-lookup"><span data-stu-id="b4132-156">The **id** of the resource [service principal](serviceprincipal.md) to which access is authorized.</span></span> <span data-ttu-id="b4132-157">Этот параметр определяет API, который клиент может пытаться вызвать от имени пользователя, выполнившего вход в систему.</span><span class="sxs-lookup"><span data-stu-id="b4132-157">This identifies the API which the client is authorized to attempt to call on behalf of a signed-in user.</span></span> |
| <span data-ttu-id="b4132-158">scope</span><span class="sxs-lookup"><span data-stu-id="b4132-158">scope</span></span> | <span data-ttu-id="b4132-159">String</span><span class="sxs-lookup"><span data-stu-id="b4132-159">String</span></span> | <span data-ttu-id="b4132-160">Разделенный пробелами список значений утверждений для делегированных разрешений, которые следует включить в маркеры доступа для приложения ресурсов (API).</span><span class="sxs-lookup"><span data-stu-id="b4132-160">A space-separated list of the claim values for delegated permissions which should be included in access tokens for the resource application (the API).</span></span> <span data-ttu-id="b4132-161">Например, `openid User.Read GroupMember.Read.All`.</span><span class="sxs-lookup"><span data-stu-id="b4132-161">For example, `openid User.Read GroupMember.Read.All`.</span></span> <span data-ttu-id="b4132-162">Каждое значение утверждения должно быть согласовано с полем **значение** одного из делегированных разрешений, определенных API, указанным в свойстве **публишедпермиссионскопес** [субъекта-службы](serviceprincipal.md)ресурсов.</span><span class="sxs-lookup"><span data-stu-id="b4132-162">Each claim value should match the **value** field of one of the delegated permissions defined by the API, listed in the **publishedPermissionScopes** property of the resource [service principal](serviceprincipal.md).</span></span> |

## <a name="relationships"></a><span data-ttu-id="b4132-163">Отношения</span><span class="sxs-lookup"><span data-stu-id="b4132-163">Relationships</span></span>

<span data-ttu-id="b4132-164">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="b4132-164">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b4132-165">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="b4132-165">JSON representation</span></span>

<span data-ttu-id="b4132-166">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b4132-166">The following is a JSON representation of the resource.</span></span>

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

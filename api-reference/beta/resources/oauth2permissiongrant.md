---
title: Тип ресурса oAuth2PermissionGrant
description: Представляет области OAuth 2,0 (делегированные разрешения), которые были предоставлены приложению (представленному субъектом-службой) в рамках процесса разрешения пользователя или администратора.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: psignoret
ms.openlocfilehash: f00d9aa79e6a18e5dddf6881e251b3cbf00172e6
ms.sourcegitcommit: d14e2abb24d9fbab519458b1c9fec890a5e51d70
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/17/2020
ms.locfileid: "43543417"
---
# <a name="oauth2permissiongrant-resource-type"></a><span data-ttu-id="47342-103">Тип ресурса oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="47342-103">oAuth2PermissionGrant resource type</span></span>

<span data-ttu-id="47342-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="47342-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="47342-105">Представляет области OAuth 2,0 (делегированные разрешения), которые были предоставлены приложению (представленному субъектом-службой) в рамках процесса разрешения пользователя или администратора.</span><span class="sxs-lookup"><span data-stu-id="47342-105">Represents the OAuth 2.0 scopes (delegated permissions) that have been granted to an application (represented by a service principal) as part of the user or admin consent process.</span></span>

<span data-ttu-id="47342-106">Этот ресурс поддерживает отслеживание добавлений, удалений и обновлений с помощью [разностного запроса](/graph/delta-query-overview) с функцией [delta](../api/oauth2permissiongrant-delta.md).</span><span class="sxs-lookup"><span data-stu-id="47342-106">This resource supports using [delta query](/graph/delta-query-overview) to track incremental additions, deletions, and updates, by providing a [delta](../api/oauth2permissiongrant-delta.md) function.</span></span>

## <a name="methods"></a><span data-ttu-id="47342-107">Методы</span><span class="sxs-lookup"><span data-stu-id="47342-107">Methods</span></span>

| <span data-ttu-id="47342-108">Метод</span><span class="sxs-lookup"><span data-stu-id="47342-108">Method</span></span>           | <span data-ttu-id="47342-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="47342-109">Return Type</span></span>    |<span data-ttu-id="47342-110">Описание</span><span class="sxs-lookup"><span data-stu-id="47342-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="47342-111">Список oAuth2PermissionGrants</span><span class="sxs-lookup"><span data-stu-id="47342-111">List oAuth2PermissionGrants</span></span>](../api/oauth2permissiongrant-list.md) | <span data-ttu-id="47342-112">Коллекция [oAuth2PermissionGrant](oauth2permissiongrant.md)</span><span class="sxs-lookup"><span data-stu-id="47342-112">[oAuth2PermissionGrant](oauth2permissiongrant.md) collection</span></span> | <span data-ttu-id="47342-113">Получение списка объектов **oauth2PermissionGrant** .</span><span class="sxs-lookup"><span data-stu-id="47342-113">Retrieve a list of **oauth2PermissionGrant** objects.</span></span> |
|[<span data-ttu-id="47342-114">Получение oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="47342-114">Get oAuth2PermissionGrant</span></span>](../api/oauth2permissiongrant-get.md) | [<span data-ttu-id="47342-115">oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="47342-115">oAuth2PermissionGrant</span></span>](oauth2permissiongrant.md) |<span data-ttu-id="47342-116">Чтение свойств и связей объекта **oAuth2PermissionGrant** .</span><span class="sxs-lookup"><span data-stu-id="47342-116">Read the properties and relationships of an **oAuth2PermissionGrant** object.</span></span>|
|[<span data-ttu-id="47342-117">Обновление oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="47342-117">Update oAuth2PermissionGrant</span></span>](../api/oauth2permissiongrant-update.md) | [<span data-ttu-id="47342-118">oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="47342-118">oAuth2PermissionGrant</span></span>](oauth2permissiongrant.md) |<span data-ttu-id="47342-119">Обновление объекта **oAuth2PermissionGrant** .</span><span class="sxs-lookup"><span data-stu-id="47342-119">Update an  **oAuth2PermissionGrant** object.</span></span> |
|[<span data-ttu-id="47342-120">Удаление oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="47342-120">Delete oAuth2PermissionGrant</span></span>](../api/oauth2permissiongrant-delete.md) | <span data-ttu-id="47342-121">Нет</span><span class="sxs-lookup"><span data-stu-id="47342-121">None</span></span> |<span data-ttu-id="47342-122">Удаление объекта **oAuth2PermissionGrant** .</span><span class="sxs-lookup"><span data-stu-id="47342-122">Delete an **oAuth2PermissionGrant** object.</span></span> |
|[<span data-ttu-id="47342-123">Получение дельты</span><span class="sxs-lookup"><span data-stu-id="47342-123">Get delta</span></span>](../api/oauth2permissiongrant-delta.md)|[<span data-ttu-id="47342-124">oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="47342-124">oAuth2PermissionGrant</span></span>](oauth2permissiongrant.md)|<span data-ttu-id="47342-125">Получение только что созданных, обновленных или удаленных объектов **oauth2permissiongrant** без выполнения полного считывания всей коллекции ресурсов.</span><span class="sxs-lookup"><span data-stu-id="47342-125">Get newly created, updated, or deleted **oauth2permissiongrant** objects without performing a full read of the entire resource collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="47342-126">Свойства</span><span class="sxs-lookup"><span data-stu-id="47342-126">Properties</span></span>
| <span data-ttu-id="47342-127">Свойство</span><span class="sxs-lookup"><span data-stu-id="47342-127">Property</span></span>     | <span data-ttu-id="47342-128">Тип</span><span class="sxs-lookup"><span data-stu-id="47342-128">Type</span></span>   |<span data-ttu-id="47342-129">Описание</span><span class="sxs-lookup"><span data-stu-id="47342-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="47342-130">clientId</span><span class="sxs-lookup"><span data-stu-id="47342-130">clientId</span></span>|<span data-ttu-id="47342-131">String</span><span class="sxs-lookup"><span data-stu-id="47342-131">String</span></span>| <span data-ttu-id="47342-132">Идентификатор субъекта-службы, которому предоставлено согласие на олицетворение пользователя при доступе к ресурсу (представленному свойством resourceId).</span><span class="sxs-lookup"><span data-stu-id="47342-132">The id of the service principal granted consent to impersonate the user when accessing the resource (represented by the resourceId property).</span></span> |
|<span data-ttu-id="47342-133">консенттипе</span><span class="sxs-lookup"><span data-stu-id="47342-133">consentType</span></span>|<span data-ttu-id="47342-134">String</span><span class="sxs-lookup"><span data-stu-id="47342-134">String</span></span>| <span data-ttu-id="47342-135">Указывает, было ли согласие предоставлено администратором (от имени Организации) или отдельным пользователем.</span><span class="sxs-lookup"><span data-stu-id="47342-135">Indicates if consent was provided by the administrator (on behalf of the organization) or by an individual.</span></span> <span data-ttu-id="47342-136">Возможные значения: *аллпринЦипалс* или *Principal*.</span><span class="sxs-lookup"><span data-stu-id="47342-136">The possible values are *AllPrincipals* or *Principal*.</span></span> |
|<span data-ttu-id="47342-137">експиритиме</span><span class="sxs-lookup"><span data-stu-id="47342-137">expiryTime</span></span>|<span data-ttu-id="47342-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="47342-138">DateTimeOffset</span></span>| <span data-ttu-id="47342-139">В настоящее время значение срока действия игнорируется.</span><span class="sxs-lookup"><span data-stu-id="47342-139">Currently, the expiry time value is ignored.</span></span> |
|<span data-ttu-id="47342-140">id</span><span class="sxs-lookup"><span data-stu-id="47342-140">id</span></span>|<span data-ttu-id="47342-141">Строка</span><span class="sxs-lookup"><span data-stu-id="47342-141">String</span></span>| <span data-ttu-id="47342-142">Уникальный идентификатор.</span><span class="sxs-lookup"><span data-stu-id="47342-142">Unique identifier.</span></span> <span data-ttu-id="47342-143">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="47342-143">Read-only.</span></span>|
|<span data-ttu-id="47342-144">principalId</span><span class="sxs-lookup"><span data-stu-id="47342-144">principalId</span></span>|<span data-ttu-id="47342-145">String</span><span class="sxs-lookup"><span data-stu-id="47342-145">String</span></span>| <span data-ttu-id="47342-146">Если Консенттипе — *аллпринЦипалс* , это значение равно null, а согласие применяется ко всем пользователям в Организации.</span><span class="sxs-lookup"><span data-stu-id="47342-146">If consentType is *AllPrincipals* this value is null, and the consent applies to all users in the organization.</span></span> <span data-ttu-id="47342-147">Если Консенттипе является *субъектом*, это свойство указывает идентификатор пользователя, который предоставил согласие и применяется только для этого пользователя.</span><span class="sxs-lookup"><span data-stu-id="47342-147">If consentType is *Principal*, then this property specifies the id of the user that granted consent and applies only for that user.</span></span> |
|<span data-ttu-id="47342-148">resourceId</span><span class="sxs-lookup"><span data-stu-id="47342-148">resourceId</span></span>|<span data-ttu-id="47342-149">String</span><span class="sxs-lookup"><span data-stu-id="47342-149">String</span></span>| <span data-ttu-id="47342-150">Указывает идентификатор субъекта службы ресурсов, которому предоставлен доступ.</span><span class="sxs-lookup"><span data-stu-id="47342-150">Specifies the id of the resource service principal to which access has been granted.</span></span> |
|<span data-ttu-id="47342-151">scope</span><span class="sxs-lookup"><span data-stu-id="47342-151">scope</span></span>|<span data-ttu-id="47342-152">String</span><span class="sxs-lookup"><span data-stu-id="47342-152">String</span></span>| <span data-ttu-id="47342-153">Указывает значение утверждения [области](/graph/permissions-reference) , которое должно ожидать приложение ресурсов в маркере доступа OAuth 2,0.</span><span class="sxs-lookup"><span data-stu-id="47342-153">Specifies the value of the [scope](/graph/permissions-reference) claim that the resource application should expect in the OAuth 2.0 access token.</span></span> <span data-ttu-id="47342-154">Например, *User. Read*</span><span class="sxs-lookup"><span data-stu-id="47342-154">For example, *User.Read*</span></span> |
|<span data-ttu-id="47342-155">startTime</span><span class="sxs-lookup"><span data-stu-id="47342-155">startTime</span></span>|<span data-ttu-id="47342-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="47342-156">DateTimeOffset</span></span>| <span data-ttu-id="47342-157">В настоящее время значение времени начала игнорируется.</span><span class="sxs-lookup"><span data-stu-id="47342-157">Currently, the start time value is ignored.</span></span> |

## <a name="relationships"></a><span data-ttu-id="47342-158">Связи</span><span class="sxs-lookup"><span data-stu-id="47342-158">Relationships</span></span>
<span data-ttu-id="47342-159">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="47342-159">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="47342-160">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="47342-160">JSON representation</span></span>

<span data-ttu-id="47342-161">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="47342-161">The following is a JSON representation of the resource.</span></span>

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
  "expiryTime": "String (timestamp)",
  "id": "string (identifier)",
  "principalId": "string",
  "resourceId": "string",
  "scope": "string",
  "startTime": "String (timestamp)"
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

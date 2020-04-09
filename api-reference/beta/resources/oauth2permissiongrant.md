---
title: Тип ресурса oAuth2PermissionGrant
description: Представляет области OAuth 2,0 (делегированные разрешения), которые были предоставлены приложению (представленному субъектом-службой) в рамках процесса разрешения пользователя или администратора.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: psignoret
ms.openlocfilehash: 9a403ac53d50c31a41a65c47db7423439a5befd0
ms.sourcegitcommit: ee41ba9ec6001716f1a9d575741bbeef577e2473
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/09/2020
ms.locfileid: "43200133"
---
# <a name="oauth2permissiongrant-resource-type"></a><span data-ttu-id="cbb02-103">Тип ресурса oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="cbb02-103">oAuth2PermissionGrant resource type</span></span>

<span data-ttu-id="cbb02-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cbb02-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cbb02-105">Представляет области OAuth 2,0 (делегированные разрешения), которые были предоставлены приложению (представленному субъектом-службой) в рамках процесса разрешения пользователя или администратора.</span><span class="sxs-lookup"><span data-stu-id="cbb02-105">Represents the OAuth 2.0 scopes (delegated permissions) that have been granted to an application (represented by a service principal) as part of the user or admin consent process.</span></span>

## <a name="json-representation"></a><span data-ttu-id="cbb02-106">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="cbb02-106">JSON representation</span></span>

<span data-ttu-id="cbb02-107">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="cbb02-107">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="cbb02-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="cbb02-108">Properties</span></span>
| <span data-ttu-id="cbb02-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="cbb02-109">Property</span></span>     | <span data-ttu-id="cbb02-110">Тип</span><span class="sxs-lookup"><span data-stu-id="cbb02-110">Type</span></span>   |<span data-ttu-id="cbb02-111">Описание</span><span class="sxs-lookup"><span data-stu-id="cbb02-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cbb02-112">clientId</span><span class="sxs-lookup"><span data-stu-id="cbb02-112">clientId</span></span>|<span data-ttu-id="cbb02-113">String</span><span class="sxs-lookup"><span data-stu-id="cbb02-113">String</span></span>| <span data-ttu-id="cbb02-114">Идентификатор субъекта-службы, которому предоставлено согласие на олицетворение пользователя при доступе к ресурсу (представленному свойством resourceId).</span><span class="sxs-lookup"><span data-stu-id="cbb02-114">The id of the service principal granted consent to impersonate the user when accessing the resource (represented by the resourceId property).</span></span> |
|<span data-ttu-id="cbb02-115">консенттипе</span><span class="sxs-lookup"><span data-stu-id="cbb02-115">consentType</span></span>|<span data-ttu-id="cbb02-116">String</span><span class="sxs-lookup"><span data-stu-id="cbb02-116">String</span></span>| <span data-ttu-id="cbb02-117">Указывает, было ли согласие предоставлено администратором (от имени Организации) или отдельным пользователем.</span><span class="sxs-lookup"><span data-stu-id="cbb02-117">Indicates if consent was provided by the administrator (on behalf of the organization) or by an individual.</span></span> <span data-ttu-id="cbb02-118">Возможные значения: *аллпринЦипалс* или *Principal*.</span><span class="sxs-lookup"><span data-stu-id="cbb02-118">The possible values are *AllPrincipals* or *Principal*.</span></span> |
|<span data-ttu-id="cbb02-119">експиритиме</span><span class="sxs-lookup"><span data-stu-id="cbb02-119">expiryTime</span></span>|<span data-ttu-id="cbb02-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cbb02-120">DateTimeOffset</span></span>| <span data-ttu-id="cbb02-121">В настоящее время значение срока действия игнорируется.</span><span class="sxs-lookup"><span data-stu-id="cbb02-121">Currently, the expiry time value is ignored.</span></span> |
|<span data-ttu-id="cbb02-122">id</span><span class="sxs-lookup"><span data-stu-id="cbb02-122">id</span></span>|<span data-ttu-id="cbb02-123">Строка</span><span class="sxs-lookup"><span data-stu-id="cbb02-123">String</span></span>| <span data-ttu-id="cbb02-124">Уникальный идентификатор.</span><span class="sxs-lookup"><span data-stu-id="cbb02-124">Unique identifier.</span></span> <span data-ttu-id="cbb02-125">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="cbb02-125">Read-only.</span></span>|
|<span data-ttu-id="cbb02-126">principalId</span><span class="sxs-lookup"><span data-stu-id="cbb02-126">principalId</span></span>|<span data-ttu-id="cbb02-127">String</span><span class="sxs-lookup"><span data-stu-id="cbb02-127">String</span></span>| <span data-ttu-id="cbb02-128">Если Консенттипе — *аллпринЦипалс* , это значение равно null, а согласие применяется ко всем пользователям в Организации.</span><span class="sxs-lookup"><span data-stu-id="cbb02-128">If consentType is *AllPrincipals* this value is null, and the consent applies to all users in the organization.</span></span> <span data-ttu-id="cbb02-129">Если Консенттипе является *субъектом*, это свойство указывает идентификатор пользователя, который предоставил согласие и применяется только для этого пользователя.</span><span class="sxs-lookup"><span data-stu-id="cbb02-129">If consentType is *Principal*, then this property specifies the id of the user that granted consent and applies only for that user.</span></span> |
|<span data-ttu-id="cbb02-130">resourceId</span><span class="sxs-lookup"><span data-stu-id="cbb02-130">resourceId</span></span>|<span data-ttu-id="cbb02-131">String</span><span class="sxs-lookup"><span data-stu-id="cbb02-131">String</span></span>| <span data-ttu-id="cbb02-132">Указывает идентификатор субъекта службы ресурсов, которому предоставлен доступ.</span><span class="sxs-lookup"><span data-stu-id="cbb02-132">Specifies the id of the resource service principal to which access has been granted.</span></span> |
|<span data-ttu-id="cbb02-133">scope</span><span class="sxs-lookup"><span data-stu-id="cbb02-133">scope</span></span>|<span data-ttu-id="cbb02-134">String</span><span class="sxs-lookup"><span data-stu-id="cbb02-134">String</span></span>| <span data-ttu-id="cbb02-135">Указывает значение утверждения [области](/graph/permissions-reference) , которое должно ожидать приложение ресурсов в маркере доступа OAuth 2,0.</span><span class="sxs-lookup"><span data-stu-id="cbb02-135">Specifies the value of the [scope](/graph/permissions-reference) claim that the resource application should expect in the OAuth 2.0 access token.</span></span> <span data-ttu-id="cbb02-136">Например, *User. Read*</span><span class="sxs-lookup"><span data-stu-id="cbb02-136">For example, *User.Read*</span></span> |
|<span data-ttu-id="cbb02-137">startTime</span><span class="sxs-lookup"><span data-stu-id="cbb02-137">startTime</span></span>|<span data-ttu-id="cbb02-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cbb02-138">DateTimeOffset</span></span>| <span data-ttu-id="cbb02-139">В настоящее время значение времени начала игнорируется.</span><span class="sxs-lookup"><span data-stu-id="cbb02-139">Currently, the start time value is ignored.</span></span> |

## <a name="relationships"></a><span data-ttu-id="cbb02-140">Отношения</span><span class="sxs-lookup"><span data-stu-id="cbb02-140">Relationships</span></span>
<span data-ttu-id="cbb02-141">Нет</span><span class="sxs-lookup"><span data-stu-id="cbb02-141">None</span></span>


## <a name="methods"></a><span data-ttu-id="cbb02-142">Методы</span><span class="sxs-lookup"><span data-stu-id="cbb02-142">Methods</span></span>

| <span data-ttu-id="cbb02-143">Метод</span><span class="sxs-lookup"><span data-stu-id="cbb02-143">Method</span></span>           | <span data-ttu-id="cbb02-144">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="cbb02-144">Return Type</span></span>    |<span data-ttu-id="cbb02-145">Описание</span><span class="sxs-lookup"><span data-stu-id="cbb02-145">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="cbb02-146">Получение oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="cbb02-146">Get oAuth2PermissionGrant</span></span>](../api/oauth2permissiongrant-get.md) | [<span data-ttu-id="cbb02-147">oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="cbb02-147">oAuth2PermissionGrant</span></span>](oauth2permissiongrant.md) |<span data-ttu-id="cbb02-148">Чтение свойств и связей объекта oAuth2PermissionGrant.</span><span class="sxs-lookup"><span data-stu-id="cbb02-148">Read properties and relationships of oAuth2PermissionGrant object.</span></span>|
|[<span data-ttu-id="cbb02-149">Список oAuth2PermissionGrants</span><span class="sxs-lookup"><span data-stu-id="cbb02-149">List oAuth2PermissionGrants</span></span>](../api/oauth2permissiongrant-list.md) | <span data-ttu-id="cbb02-150">Коллекция [oAuth2PermissionGrant](oauth2permissiongrant.md)</span><span class="sxs-lookup"><span data-stu-id="cbb02-150">[oAuth2PermissionGrant](oauth2permissiongrant.md) collection</span></span> | <span data-ttu-id="cbb02-151">Получение списка объектов oauth2PermissionGrant.</span><span class="sxs-lookup"><span data-stu-id="cbb02-151">Retrieve a list of oauth2PermissionGrant objects.</span></span> |
|[<span data-ttu-id="cbb02-152">Обновление oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="cbb02-152">Update oAuth2PermissionGrant</span></span>](../api/oauth2permissiongrant-update.md) | [<span data-ttu-id="cbb02-153">oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="cbb02-153">oAuth2PermissionGrant</span></span>](oauth2permissiongrant.md) |<span data-ttu-id="cbb02-154">Обновление объекта oAuth2PermissionGrant.</span><span class="sxs-lookup"><span data-stu-id="cbb02-154">Update oAuth2PermissionGrant object.</span></span> |
|[<span data-ttu-id="cbb02-155">Удаление oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="cbb02-155">Delete oAuth2PermissionGrant</span></span>](../api/oauth2permissiongrant-delete.md) | <span data-ttu-id="cbb02-156">Нет</span><span class="sxs-lookup"><span data-stu-id="cbb02-156">None</span></span> |<span data-ttu-id="cbb02-157">Удаление объекта oAuth2PermissionGrant.</span><span class="sxs-lookup"><span data-stu-id="cbb02-157">Delete oAuth2PermissionGrant object.</span></span> |

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

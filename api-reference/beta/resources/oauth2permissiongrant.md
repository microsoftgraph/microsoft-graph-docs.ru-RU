---
title: Тип ресурса oAuth2PermissionGrant
description: Представляет области OAuth 2,0 (делегированные разрешения), которые были предоставлены приложению (представленному субъектом-службой) в рамках процесса разрешения пользователя или администратора.
localization_priority: Normal
ms.openlocfilehash: f23d2e7a8b57b324a92a1268ab4cc0393d8906f0
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33342074"
---
# <a name="oauth2permissiongrant-resource-type"></a><span data-ttu-id="c2c86-103">Тип ресурса oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="c2c86-103">oAuth2PermissionGrant resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c2c86-104">Представляет области OAuth 2,0 (делегированные разрешения), которые были предоставлены приложению (представленному субъектом-службой) в рамках процесса разрешения пользователя или администратора.</span><span class="sxs-lookup"><span data-stu-id="c2c86-104">Represents the OAuth 2.0 scopes (delegated permissions) that have been granted to an application (represented by a service principal) as part of the user or admin consent process.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c2c86-105">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c2c86-105">JSON representation</span></span>

<span data-ttu-id="c2c86-106">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="c2c86-106">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="c2c86-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="c2c86-107">Properties</span></span>
| <span data-ttu-id="c2c86-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="c2c86-108">Property</span></span>     | <span data-ttu-id="c2c86-109">Тип</span><span class="sxs-lookup"><span data-stu-id="c2c86-109">Type</span></span>   |<span data-ttu-id="c2c86-110">Описание</span><span class="sxs-lookup"><span data-stu-id="c2c86-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c2c86-111">clientId</span><span class="sxs-lookup"><span data-stu-id="c2c86-111">clientId</span></span>|<span data-ttu-id="c2c86-112">String</span><span class="sxs-lookup"><span data-stu-id="c2c86-112">String</span></span>| <span data-ttu-id="c2c86-113">Идентификатор субъекта-службы, которому предоставлено согласие на олицетворение пользователя при доступе к ресурсу (представленному свойством resourceId).</span><span class="sxs-lookup"><span data-stu-id="c2c86-113">The id of the service principal granted consent to impersonate the user when accessing the resource (represented by the resourceId property).</span></span> |
|<span data-ttu-id="c2c86-114">Консенттипе</span><span class="sxs-lookup"><span data-stu-id="c2c86-114">consentType</span></span>|<span data-ttu-id="c2c86-115">String</span><span class="sxs-lookup"><span data-stu-id="c2c86-115">String</span></span>| <span data-ttu-id="c2c86-116">Указывает, было ли согласие предоставлено администратором (от имени Организации) или отдельным пользователем.</span><span class="sxs-lookup"><span data-stu-id="c2c86-116">Indicates if consent was provided by the administrator (on behalf of the organization) or by an individual.</span></span> <span data-ttu-id="c2c86-117">Возможные значения: *аллпринЦипалс* или *Principal*.</span><span class="sxs-lookup"><span data-stu-id="c2c86-117">The possible values are *AllPrincipals* or *Principal*.</span></span> |
|<span data-ttu-id="c2c86-118">Експиритиме</span><span class="sxs-lookup"><span data-stu-id="c2c86-118">expiryTime</span></span>|<span data-ttu-id="c2c86-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c2c86-119">DateTimeOffset</span></span>| <span data-ttu-id="c2c86-120">В настоящее время значение срока действия игнорируется.</span><span class="sxs-lookup"><span data-stu-id="c2c86-120">Currently, the expiry time value is ignored.</span></span> |
|<span data-ttu-id="c2c86-121">id</span><span class="sxs-lookup"><span data-stu-id="c2c86-121">id</span></span>|<span data-ttu-id="c2c86-122">Строка</span><span class="sxs-lookup"><span data-stu-id="c2c86-122">String</span></span>| <span data-ttu-id="c2c86-123">Уникальный идентификатор.</span><span class="sxs-lookup"><span data-stu-id="c2c86-123">Unique identifier.</span></span> <span data-ttu-id="c2c86-124">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c2c86-124">Read-only.</span></span>|
|<span data-ttu-id="c2c86-125">principalId</span><span class="sxs-lookup"><span data-stu-id="c2c86-125">principalId</span></span>|<span data-ttu-id="c2c86-126">String</span><span class="sxs-lookup"><span data-stu-id="c2c86-126">String</span></span>| <span data-ttu-id="c2c86-127">Если Консенттипе — *аллпринЦипалс* , это значение равно null, а согласие применяется ко всем пользователям в Организации.</span><span class="sxs-lookup"><span data-stu-id="c2c86-127">If consentType is *AllPrincipals* this value is null, and the consent applies to all users in the organization.</span></span> <span data-ttu-id="c2c86-128">Если Консенттипе является *субъектом*, это свойство указывает идентификатор пользователя, который предоставил согласие и применяется только для этого пользователя.</span><span class="sxs-lookup"><span data-stu-id="c2c86-128">If consentType is *Principal*, then this property specifies the id of the user that granted consent and applies only for that user.</span></span> |
|<span data-ttu-id="c2c86-129">resourceId</span><span class="sxs-lookup"><span data-stu-id="c2c86-129">resourceId</span></span>|<span data-ttu-id="c2c86-130">String</span><span class="sxs-lookup"><span data-stu-id="c2c86-130">String</span></span>| <span data-ttu-id="c2c86-131">Указывает идентификатор субъекта службы ресурсов, которому предоставлен доступ.</span><span class="sxs-lookup"><span data-stu-id="c2c86-131">Specifies the id of the resource service principal to which access has been granted.</span></span> |
|<span data-ttu-id="c2c86-132">scope</span><span class="sxs-lookup"><span data-stu-id="c2c86-132">scope</span></span>|<span data-ttu-id="c2c86-133">String</span><span class="sxs-lookup"><span data-stu-id="c2c86-133">String</span></span>| <span data-ttu-id="c2c86-134">Указывает значение утверждения [области](/graph/permissions-reference) , которое должно ожидать приложение ресурсов в маркере доступа OAuth 2,0.</span><span class="sxs-lookup"><span data-stu-id="c2c86-134">Specifies the value of the [scope](/graph/permissions-reference) claim that the resource application should expect in the OAuth 2.0 access token.</span></span> <span data-ttu-id="c2c86-135">Например, *User. Read*</span><span class="sxs-lookup"><span data-stu-id="c2c86-135">For example, *User.Read*</span></span> |
|<span data-ttu-id="c2c86-136">startTime</span><span class="sxs-lookup"><span data-stu-id="c2c86-136">startTime</span></span>|<span data-ttu-id="c2c86-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c2c86-137">DateTimeOffset</span></span>| <span data-ttu-id="c2c86-138">В настоящее время значение времени начала игнорируется.</span><span class="sxs-lookup"><span data-stu-id="c2c86-138">Currently, the start time value is ignored.</span></span> |

## <a name="relationships"></a><span data-ttu-id="c2c86-139">Связи</span><span class="sxs-lookup"><span data-stu-id="c2c86-139">Relationships</span></span>
<span data-ttu-id="c2c86-140">Нет</span><span class="sxs-lookup"><span data-stu-id="c2c86-140">None</span></span>


## <a name="methods"></a><span data-ttu-id="c2c86-141">Методы</span><span class="sxs-lookup"><span data-stu-id="c2c86-141">Methods</span></span>

| <span data-ttu-id="c2c86-142">Метод</span><span class="sxs-lookup"><span data-stu-id="c2c86-142">Method</span></span>           | <span data-ttu-id="c2c86-143">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="c2c86-143">Return Type</span></span>    |<span data-ttu-id="c2c86-144">Описание</span><span class="sxs-lookup"><span data-stu-id="c2c86-144">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c2c86-145">Получение oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="c2c86-145">Get oAuth2PermissionGrant</span></span>](../api/oauth2permissiongrant-get.md) | [<span data-ttu-id="c2c86-146">oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="c2c86-146">oAuth2PermissionGrant</span></span>](oauth2permissiongrant.md) |<span data-ttu-id="c2c86-147">Чтение свойств и связей объекта oAuth2PermissionGrant.</span><span class="sxs-lookup"><span data-stu-id="c2c86-147">Read properties and relationships of oAuth2PermissionGrant object.</span></span>|
|[<span data-ttu-id="c2c86-148">Список oAuth2PermissionGrants</span><span class="sxs-lookup"><span data-stu-id="c2c86-148">List oAuth2PermissionGrants</span></span>](../api/oauth2permissiongrant-list.md) | <span data-ttu-id="c2c86-149">Коллекция [oAuth2PermissionGrant](oauth2permissiongrant.md)</span><span class="sxs-lookup"><span data-stu-id="c2c86-149">[oAuth2PermissionGrant](oauth2permissiongrant.md) collection</span></span> | <span data-ttu-id="c2c86-150">Получение списка объектов oauth2PermissionGrant.</span><span class="sxs-lookup"><span data-stu-id="c2c86-150">Retrieve a list of oauth2PermissionGrant objects.</span></span> |
|[<span data-ttu-id="c2c86-151">Обновление oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="c2c86-151">Update oAuth2PermissionGrant</span></span>](../api/oauth2permissiongrant-update.md) | [<span data-ttu-id="c2c86-152">oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="c2c86-152">oAuth2PermissionGrant</span></span>](oauth2permissiongrant.md) |<span data-ttu-id="c2c86-153">Обновление объекта oAuth2PermissionGrant.</span><span class="sxs-lookup"><span data-stu-id="c2c86-153">Update oAuth2PermissionGrant object.</span></span> |
|[<span data-ttu-id="c2c86-154">Удаление oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="c2c86-154">Delete oAuth2PermissionGrant</span></span>](../api/oauth2permissiongrant-delete.md) | <span data-ttu-id="c2c86-155">Нет</span><span class="sxs-lookup"><span data-stu-id="c2c86-155">None</span></span> |<span data-ttu-id="c2c86-156">Удаление объекта oAuth2PermissionGrant.</span><span class="sxs-lookup"><span data-stu-id="c2c86-156">Delete oAuth2PermissionGrant object.</span></span> |

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

---
title: Тип ресурса oAuth2PermissionGrant
description: Представляет области OAuth 2,0 (делегированные разрешения), которые были предоставлены приложению (представленному субъектом-службой) в рамках процесса разрешения пользователя или администратора.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 25f012baca1a7dfa5aeb62b8885b00b151a657ed
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966617"
---
# <a name="oauth2permissiongrant-resource-type"></a><span data-ttu-id="e0598-103">Тип ресурса oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="e0598-103">oAuth2PermissionGrant resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e0598-104">Представляет области OAuth 2,0 (делегированные разрешения), которые были предоставлены приложению (представленному субъектом-службой) в рамках процесса разрешения пользователя или администратора.</span><span class="sxs-lookup"><span data-stu-id="e0598-104">Represents the OAuth 2.0 scopes (delegated permissions) that have been granted to an application (represented by a service principal) as part of the user or admin consent process.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e0598-105">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e0598-105">JSON representation</span></span>

<span data-ttu-id="e0598-106">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="e0598-106">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="e0598-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="e0598-107">Properties</span></span>
| <span data-ttu-id="e0598-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="e0598-108">Property</span></span>     | <span data-ttu-id="e0598-109">Тип</span><span class="sxs-lookup"><span data-stu-id="e0598-109">Type</span></span>   |<span data-ttu-id="e0598-110">Описание</span><span class="sxs-lookup"><span data-stu-id="e0598-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e0598-111">clientId</span><span class="sxs-lookup"><span data-stu-id="e0598-111">clientId</span></span>|<span data-ttu-id="e0598-112">String</span><span class="sxs-lookup"><span data-stu-id="e0598-112">String</span></span>| <span data-ttu-id="e0598-113">Идентификатор субъекта-службы, которому предоставлено согласие на олицетворение пользователя при доступе к ресурсу (представленному свойством resourceId).</span><span class="sxs-lookup"><span data-stu-id="e0598-113">The id of the service principal granted consent to impersonate the user when accessing the resource (represented by the resourceId property).</span></span> |
|<span data-ttu-id="e0598-114">Консенттипе</span><span class="sxs-lookup"><span data-stu-id="e0598-114">consentType</span></span>|<span data-ttu-id="e0598-115">String</span><span class="sxs-lookup"><span data-stu-id="e0598-115">String</span></span>| <span data-ttu-id="e0598-116">Указывает, было ли согласие предоставлено администратором (от имени Организации) или отдельным пользователем.</span><span class="sxs-lookup"><span data-stu-id="e0598-116">Indicates if consent was provided by the administrator (on behalf of the organization) or by an individual.</span></span> <span data-ttu-id="e0598-117">Возможные значения: *аллпринЦипалс* или *Principal*.</span><span class="sxs-lookup"><span data-stu-id="e0598-117">The possible values are *AllPrincipals* or *Principal*.</span></span> |
|<span data-ttu-id="e0598-118">Експиритиме</span><span class="sxs-lookup"><span data-stu-id="e0598-118">expiryTime</span></span>|<span data-ttu-id="e0598-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e0598-119">DateTimeOffset</span></span>| <span data-ttu-id="e0598-120">В настоящее время значение срока действия игнорируется.</span><span class="sxs-lookup"><span data-stu-id="e0598-120">Currently, the expiry time value is ignored.</span></span> |
|<span data-ttu-id="e0598-121">id</span><span class="sxs-lookup"><span data-stu-id="e0598-121">id</span></span>|<span data-ttu-id="e0598-122">Строка</span><span class="sxs-lookup"><span data-stu-id="e0598-122">String</span></span>| <span data-ttu-id="e0598-123">Уникальный идентификатор.</span><span class="sxs-lookup"><span data-stu-id="e0598-123">Unique identifier.</span></span> <span data-ttu-id="e0598-124">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e0598-124">Read-only.</span></span>|
|<span data-ttu-id="e0598-125">principalId</span><span class="sxs-lookup"><span data-stu-id="e0598-125">principalId</span></span>|<span data-ttu-id="e0598-126">String</span><span class="sxs-lookup"><span data-stu-id="e0598-126">String</span></span>| <span data-ttu-id="e0598-127">Если Консенттипе — *аллпринЦипалс* , это значение равно null, а согласие применяется ко всем пользователям в Организации.</span><span class="sxs-lookup"><span data-stu-id="e0598-127">If consentType is *AllPrincipals* this value is null, and the consent applies to all users in the organization.</span></span> <span data-ttu-id="e0598-128">Если Консенттипе является *субъектом*, это свойство указывает идентификатор пользователя, который предоставил согласие и применяется только для этого пользователя.</span><span class="sxs-lookup"><span data-stu-id="e0598-128">If consentType is *Principal*, then this property specifies the id of the user that granted consent and applies only for that user.</span></span> |
|<span data-ttu-id="e0598-129">resourceId</span><span class="sxs-lookup"><span data-stu-id="e0598-129">resourceId</span></span>|<span data-ttu-id="e0598-130">String</span><span class="sxs-lookup"><span data-stu-id="e0598-130">String</span></span>| <span data-ttu-id="e0598-131">Указывает идентификатор субъекта службы ресурсов, которому предоставлен доступ.</span><span class="sxs-lookup"><span data-stu-id="e0598-131">Specifies the id of the resource service principal to which access has been granted.</span></span> |
|<span data-ttu-id="e0598-132">scope</span><span class="sxs-lookup"><span data-stu-id="e0598-132">scope</span></span>|<span data-ttu-id="e0598-133">String</span><span class="sxs-lookup"><span data-stu-id="e0598-133">String</span></span>| <span data-ttu-id="e0598-134">Указывает значение утверждения [области](/graph/permissions-reference) , которое должно ожидать приложение ресурсов в маркере доступа OAuth 2,0.</span><span class="sxs-lookup"><span data-stu-id="e0598-134">Specifies the value of the [scope](/graph/permissions-reference) claim that the resource application should expect in the OAuth 2.0 access token.</span></span> <span data-ttu-id="e0598-135">Например, *User. Read*</span><span class="sxs-lookup"><span data-stu-id="e0598-135">For example, *User.Read*</span></span> |
|<span data-ttu-id="e0598-136">startTime</span><span class="sxs-lookup"><span data-stu-id="e0598-136">startTime</span></span>|<span data-ttu-id="e0598-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e0598-137">DateTimeOffset</span></span>| <span data-ttu-id="e0598-138">В настоящее время значение времени начала игнорируется.</span><span class="sxs-lookup"><span data-stu-id="e0598-138">Currently, the start time value is ignored.</span></span> |

## <a name="relationships"></a><span data-ttu-id="e0598-139">Отношения</span><span class="sxs-lookup"><span data-stu-id="e0598-139">Relationships</span></span>
<span data-ttu-id="e0598-140">Нет</span><span class="sxs-lookup"><span data-stu-id="e0598-140">None</span></span>


## <a name="methods"></a><span data-ttu-id="e0598-141">Методы</span><span class="sxs-lookup"><span data-stu-id="e0598-141">Methods</span></span>

| <span data-ttu-id="e0598-142">Метод</span><span class="sxs-lookup"><span data-stu-id="e0598-142">Method</span></span>           | <span data-ttu-id="e0598-143">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="e0598-143">Return Type</span></span>    |<span data-ttu-id="e0598-144">Описание</span><span class="sxs-lookup"><span data-stu-id="e0598-144">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e0598-145">Получение oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="e0598-145">Get oAuth2PermissionGrant</span></span>](../api/oauth2permissiongrant-get.md) | [<span data-ttu-id="e0598-146">oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="e0598-146">oAuth2PermissionGrant</span></span>](oauth2permissiongrant.md) |<span data-ttu-id="e0598-147">Чтение свойств и связей объекта oAuth2PermissionGrant.</span><span class="sxs-lookup"><span data-stu-id="e0598-147">Read properties and relationships of oAuth2PermissionGrant object.</span></span>|
|[<span data-ttu-id="e0598-148">Список oAuth2PermissionGrants</span><span class="sxs-lookup"><span data-stu-id="e0598-148">List oAuth2PermissionGrants</span></span>](../api/oauth2permissiongrant-list.md) | <span data-ttu-id="e0598-149">Коллекция [oAuth2PermissionGrant](oauth2permissiongrant.md)</span><span class="sxs-lookup"><span data-stu-id="e0598-149">[oAuth2PermissionGrant](oauth2permissiongrant.md) collection</span></span> | <span data-ttu-id="e0598-150">Получение списка объектов oauth2PermissionGrant.</span><span class="sxs-lookup"><span data-stu-id="e0598-150">Retrieve a list of oauth2PermissionGrant objects.</span></span> |
|[<span data-ttu-id="e0598-151">Обновление oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="e0598-151">Update oAuth2PermissionGrant</span></span>](../api/oauth2permissiongrant-update.md) | [<span data-ttu-id="e0598-152">oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="e0598-152">oAuth2PermissionGrant</span></span>](oauth2permissiongrant.md) |<span data-ttu-id="e0598-153">Обновление объекта oAuth2PermissionGrant.</span><span class="sxs-lookup"><span data-stu-id="e0598-153">Update oAuth2PermissionGrant object.</span></span> |
|[<span data-ttu-id="e0598-154">Удаление oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="e0598-154">Delete oAuth2PermissionGrant</span></span>](../api/oauth2permissiongrant-delete.md) | <span data-ttu-id="e0598-155">Нет</span><span class="sxs-lookup"><span data-stu-id="e0598-155">None</span></span> |<span data-ttu-id="e0598-156">Удаление объекта oAuth2PermissionGrant.</span><span class="sxs-lookup"><span data-stu-id="e0598-156">Delete oAuth2PermissionGrant object.</span></span> |

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

---
title: Тип ресурса oAuth2PermissionGrant
description: Представляет области OAuth 2.0 (делегированы разрешения), которые были присвоены приложения (представленного участников-служб) в ходе процесса согласия пользователь или администратор.
localization_priority: Normal
ms.openlocfilehash: 835e4a2c1a8d19c9c21e706adbf2f10a6a505bb3
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27884450"
---
# <a name="oauth2permissiongrant-resource-type"></a><span data-ttu-id="cb800-103">Тип ресурса oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="cb800-103">oAuth2PermissionGrant resource type</span></span>

> <span data-ttu-id="cb800-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="cb800-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cb800-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cb800-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="cb800-106">Представляет области OAuth 2.0 (делегированы разрешения), которые были присвоены приложения (представленного участников-служб) в ходе процесса согласия пользователь или администратор.</span><span class="sxs-lookup"><span data-stu-id="cb800-106">Represents the OAuth 2.0 scopes (delegated permissions) that have been granted to an application (represented by a service principal) as part of the user or admin consent process.</span></span>

## <a name="json-representation"></a><span data-ttu-id="cb800-107">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="cb800-107">JSON representation</span></span>

<span data-ttu-id="cb800-108">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="cb800-108">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.oAuth2Permissiongrant"
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
## <a name="properties"></a><span data-ttu-id="cb800-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="cb800-109">Properties</span></span>
| <span data-ttu-id="cb800-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="cb800-110">Property</span></span>     | <span data-ttu-id="cb800-111">Тип</span><span class="sxs-lookup"><span data-stu-id="cb800-111">Type</span></span>   |<span data-ttu-id="cb800-112">Описание</span><span class="sxs-lookup"><span data-stu-id="cb800-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cb800-113">clientId</span><span class="sxs-lookup"><span data-stu-id="cb800-113">clientId</span></span>|<span data-ttu-id="cb800-114">Строка</span><span class="sxs-lookup"><span data-stu-id="cb800-114">String</span></span>| <span data-ttu-id="cb800-115">Идентификатор участника службы предоставляются разрешения для олицетворения пользователя при доступе к ресурсу, (представлено свойством Ид_ресурса).</span><span class="sxs-lookup"><span data-stu-id="cb800-115">The id of the service principal granted consent to impersonate the user when accessing the resource (represented by the resourceId property).</span></span> |
|<span data-ttu-id="cb800-116">consentType</span><span class="sxs-lookup"><span data-stu-id="cb800-116">consentType</span></span>|<span data-ttu-id="cb800-117">Строка</span><span class="sxs-lookup"><span data-stu-id="cb800-117">String</span></span>| <span data-ttu-id="cb800-118">Указывает, если согласие предоставленный администратором (от имени организации) или пользователем.</span><span class="sxs-lookup"><span data-stu-id="cb800-118">Indicates if consent was provided by the administrator (on behalf of the organization) or by an individual.</span></span> <span data-ttu-id="cb800-119">Возможные значения: *AllPrincipals* или *участника*.</span><span class="sxs-lookup"><span data-stu-id="cb800-119">The possible values are *AllPrincipals* or *Principal*.</span></span> |
|<span data-ttu-id="cb800-120">expiryTime</span><span class="sxs-lookup"><span data-stu-id="cb800-120">expiryTime</span></span>|<span data-ttu-id="cb800-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cb800-121">DateTimeOffset</span></span>| <span data-ttu-id="cb800-122">На данный момент игнорируется значение времени истечения срока действия.</span><span class="sxs-lookup"><span data-stu-id="cb800-122">Currently, the expiry time value is ignored.</span></span> |
|<span data-ttu-id="cb800-123">id</span><span class="sxs-lookup"><span data-stu-id="cb800-123">id</span></span>|<span data-ttu-id="cb800-124">Строка</span><span class="sxs-lookup"><span data-stu-id="cb800-124">String</span></span>| <span data-ttu-id="cb800-125">Уникальный идентификатор.</span><span class="sxs-lookup"><span data-stu-id="cb800-125">Unique identifier.</span></span> <span data-ttu-id="cb800-126">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="cb800-126">Read-only.</span></span>|
|<span data-ttu-id="cb800-127">principalId</span><span class="sxs-lookup"><span data-stu-id="cb800-127">principalId</span></span>|<span data-ttu-id="cb800-128">Строка</span><span class="sxs-lookup"><span data-stu-id="cb800-128">String</span></span>| <span data-ttu-id="cb800-129">Если consentType является *AllPrincipals* это значение равно null и согласия применяется ко всем пользователям в организации.</span><span class="sxs-lookup"><span data-stu-id="cb800-129">If consentType is *AllPrincipals* this value is null, and the consent applies to all users in the organization.</span></span> <span data-ttu-id="cb800-130">Если consentType является *основной*, это свойство определяет идентификатор пользователя, который предоставлены разрешения и применяется только к этому пользователю.</span><span class="sxs-lookup"><span data-stu-id="cb800-130">If consentType is *Principal*, then this property specifies the id of the user that granted consent and applies only for that user.</span></span> |
|<span data-ttu-id="cb800-131">resourceId</span><span class="sxs-lookup"><span data-stu-id="cb800-131">resourceId</span></span>|<span data-ttu-id="cb800-132">String</span><span class="sxs-lookup"><span data-stu-id="cb800-132">String</span></span>| <span data-ttu-id="cb800-133">Задает идентификатор участника службы ресурсов, к которому был разрешен доступ.</span><span class="sxs-lookup"><span data-stu-id="cb800-133">Specifies the id of the resource service principal to which access has been granted.</span></span> |
|<span data-ttu-id="cb800-134">scope</span><span class="sxs-lookup"><span data-stu-id="cb800-134">scope</span></span>|<span data-ttu-id="cb800-135">Строка</span><span class="sxs-lookup"><span data-stu-id="cb800-135">String</span></span>| <span data-ttu-id="cb800-136">Задает значение утверждения [область](/graph/permissions-reference) , должно привести к приложению ресурсов в маркер доступа OAuth 2.0.</span><span class="sxs-lookup"><span data-stu-id="cb800-136">Specifies the value of the [scope](/graph/permissions-reference) claim that the resource application should expect in the OAuth 2.0 access token.</span></span> <span data-ttu-id="cb800-137">Например, *User.Read*</span><span class="sxs-lookup"><span data-stu-id="cb800-137">For example, *User.Read*</span></span> |
|<span data-ttu-id="cb800-138">startTime</span><span class="sxs-lookup"><span data-stu-id="cb800-138">startTime</span></span>|<span data-ttu-id="cb800-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cb800-139">DateTimeOffset</span></span>| <span data-ttu-id="cb800-140">На данный момент времени начала игнорируется.</span><span class="sxs-lookup"><span data-stu-id="cb800-140">Currently, the start time value is ignored.</span></span> |

## <a name="relationships"></a><span data-ttu-id="cb800-141">Связи</span><span class="sxs-lookup"><span data-stu-id="cb800-141">Relationships</span></span>
<span data-ttu-id="cb800-142">Нет</span><span class="sxs-lookup"><span data-stu-id="cb800-142">None</span></span>


## <a name="methods"></a><span data-ttu-id="cb800-143">Методы</span><span class="sxs-lookup"><span data-stu-id="cb800-143">Methods</span></span>

| <span data-ttu-id="cb800-144">Метод</span><span class="sxs-lookup"><span data-stu-id="cb800-144">Method</span></span>           | <span data-ttu-id="cb800-145">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="cb800-145">Return Type</span></span>    |<span data-ttu-id="cb800-146">Описание</span><span class="sxs-lookup"><span data-stu-id="cb800-146">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="cb800-147">Получение oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="cb800-147">Get oAuth2PermissionGrant</span></span>](../api/oauth2permissiongrant-get.md) | [<span data-ttu-id="cb800-148">oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="cb800-148">oAuth2PermissionGrant</span></span>](oauth2permissiongrant.md) |<span data-ttu-id="cb800-149">Чтение свойства и связи объекта oAuth2PermissionGrant.</span><span class="sxs-lookup"><span data-stu-id="cb800-149">Read properties and relationships of oAuth2PermissionGrant object.</span></span>|
|[<span data-ttu-id="cb800-150">Список oAuth2PermissionGrants</span><span class="sxs-lookup"><span data-stu-id="cb800-150">List oAuth2PermissionGrants</span></span>](../api/oauth2permissiongrant-list.md) | <span data-ttu-id="cb800-151">[oAuth2PermissionGrant](oauth2permissiongrant.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="cb800-151">[oAuth2PermissionGrant](oauth2permissiongrant.md) collection</span></span> | <span data-ttu-id="cb800-152">Получение списка объектов oauth2PermissionGrant.</span><span class="sxs-lookup"><span data-stu-id="cb800-152">Retrieve a list of oauth2PermissionGrant objects.</span></span> |
|[<span data-ttu-id="cb800-153">Обновление oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="cb800-153">Update oAuth2PermissionGrant</span></span>](../api/oauth2permissiongrant-update.md) | [<span data-ttu-id="cb800-154">oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="cb800-154">oAuth2PermissionGrant</span></span>](oauth2permissiongrant.md) |<span data-ttu-id="cb800-155">Обновление объекта oAuth2PermissionGrant.</span><span class="sxs-lookup"><span data-stu-id="cb800-155">Update oAuth2PermissionGrant object.</span></span> |
|[<span data-ttu-id="cb800-156">Удаление oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="cb800-156">Delete oAuth2PermissionGrant</span></span>](../api/oauth2permissiongrant-delete.md) | <span data-ttu-id="cb800-157">Нет</span><span class="sxs-lookup"><span data-stu-id="cb800-157">None</span></span> |<span data-ttu-id="cb800-158">Удалите объект oAuth2PermissionGrant.</span><span class="sxs-lookup"><span data-stu-id="cb800-158">Delete oAuth2PermissionGrant object.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "oAuth2PermissionGrant resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

---
title: Тип ресурса oAuth2PermissionGrant
description: Представляет области OAuth 2.0 (делегированы разрешения), которые были присвоены приложения (представленного участников-служб) в ходе процесса согласия пользователь или администратор.
localization_priority: Normal
ms.openlocfilehash: ea6486aedca4c3fcf73e59a5652ccf517fb01ddc
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29516926"
---
# <a name="oauth2permissiongrant-resource-type"></a><span data-ttu-id="47d06-103">Тип ресурса oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="47d06-103">oAuth2PermissionGrant resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="47d06-104">Представляет области OAuth 2.0 (делегированы разрешения), которые были присвоены приложения (представленного участников-служб) в ходе процесса согласия пользователь или администратор.</span><span class="sxs-lookup"><span data-stu-id="47d06-104">Represents the OAuth 2.0 scopes (delegated permissions) that have been granted to an application (represented by a service principal) as part of the user or admin consent process.</span></span>

## <a name="json-representation"></a><span data-ttu-id="47d06-105">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="47d06-105">JSON representation</span></span>

<span data-ttu-id="47d06-106">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="47d06-106">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="47d06-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="47d06-107">Properties</span></span>
| <span data-ttu-id="47d06-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="47d06-108">Property</span></span>     | <span data-ttu-id="47d06-109">Тип</span><span class="sxs-lookup"><span data-stu-id="47d06-109">Type</span></span>   |<span data-ttu-id="47d06-110">Описание</span><span class="sxs-lookup"><span data-stu-id="47d06-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="47d06-111">clientId</span><span class="sxs-lookup"><span data-stu-id="47d06-111">clientId</span></span>|<span data-ttu-id="47d06-112">String</span><span class="sxs-lookup"><span data-stu-id="47d06-112">String</span></span>| <span data-ttu-id="47d06-113">Идентификатор участника службы предоставляются разрешения для олицетворения пользователя при доступе к ресурсу, (представлено свойством Ид_ресурса).</span><span class="sxs-lookup"><span data-stu-id="47d06-113">The id of the service principal granted consent to impersonate the user when accessing the resource (represented by the resourceId property).</span></span> |
|<span data-ttu-id="47d06-114">consentType</span><span class="sxs-lookup"><span data-stu-id="47d06-114">consentType</span></span>|<span data-ttu-id="47d06-115">String</span><span class="sxs-lookup"><span data-stu-id="47d06-115">String</span></span>| <span data-ttu-id="47d06-116">Указывает, если согласие предоставленный администратором (от имени организации) или пользователем.</span><span class="sxs-lookup"><span data-stu-id="47d06-116">Indicates if consent was provided by the administrator (on behalf of the organization) or by an individual.</span></span> <span data-ttu-id="47d06-117">Возможные значения: AllPrincipals и Principal.</span><span class="sxs-lookup"><span data-stu-id="47d06-117">The possible values are *AllPrincipals* or *Principal*.</span></span> |
|<span data-ttu-id="47d06-118">ExpiryTime</span><span class="sxs-lookup"><span data-stu-id="47d06-118">expiryTime</span></span>|<span data-ttu-id="47d06-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="47d06-119">DateTimeOffset</span></span>| <span data-ttu-id="47d06-120">На данный момент игнорируется значение времени истечения срока действия.</span><span class="sxs-lookup"><span data-stu-id="47d06-120">Currently, the expiry time value is ignored.</span></span> |
|<span data-ttu-id="47d06-121">id</span><span class="sxs-lookup"><span data-stu-id="47d06-121">id</span></span>|<span data-ttu-id="47d06-122">String</span><span class="sxs-lookup"><span data-stu-id="47d06-122">String</span></span>| <span data-ttu-id="47d06-123">Уникальный идентификатор.</span><span class="sxs-lookup"><span data-stu-id="47d06-123">Unique identifier.</span></span> <span data-ttu-id="47d06-124">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="47d06-124">Read-only.</span></span>|
|<span data-ttu-id="47d06-125">principalId</span><span class="sxs-lookup"><span data-stu-id="47d06-125">principalId</span></span>|<span data-ttu-id="47d06-126">String</span><span class="sxs-lookup"><span data-stu-id="47d06-126">String</span></span>| <span data-ttu-id="47d06-127">Если consentType является *AllPrincipals* это значение равно null и согласия применяется ко всем пользователям в организации.</span><span class="sxs-lookup"><span data-stu-id="47d06-127">If consentType is *AllPrincipals* this value is null, and the consent applies to all users in the organization.</span></span> <span data-ttu-id="47d06-128">Если consentType является *основной*, это свойство определяет идентификатор пользователя, который предоставлены разрешения и применяется только к этому пользователю.</span><span class="sxs-lookup"><span data-stu-id="47d06-128">If consentType is *Principal*, then this property specifies the id of the user that granted consent and applies only for that user.</span></span> |
|<span data-ttu-id="47d06-129">resourceId</span><span class="sxs-lookup"><span data-stu-id="47d06-129">resourceId</span></span>|<span data-ttu-id="47d06-130">String</span><span class="sxs-lookup"><span data-stu-id="47d06-130">String</span></span>| <span data-ttu-id="47d06-131">Задает идентификатор участника службы ресурсов, к которому был разрешен доступ.</span><span class="sxs-lookup"><span data-stu-id="47d06-131">Specifies the id of the resource service principal to which access has been granted.</span></span> |
|<span data-ttu-id="47d06-132">scope</span><span class="sxs-lookup"><span data-stu-id="47d06-132">scope</span></span>|<span data-ttu-id="47d06-133">String</span><span class="sxs-lookup"><span data-stu-id="47d06-133">String</span></span>| <span data-ttu-id="47d06-134">Задает значение утверждения [область](/graph/permissions-reference) , должно привести к приложению ресурсов в маркер доступа OAuth 2.0.</span><span class="sxs-lookup"><span data-stu-id="47d06-134">Specifies the value of the [scope](/graph/permissions-reference) claim that the resource application should expect in the OAuth 2.0 access token.</span></span> <span data-ttu-id="47d06-135">Например, *User.Read*</span><span class="sxs-lookup"><span data-stu-id="47d06-135">For example, *User.Read*</span></span> |
|<span data-ttu-id="47d06-136">startTime</span><span class="sxs-lookup"><span data-stu-id="47d06-136">startTime</span></span>|<span data-ttu-id="47d06-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="47d06-137">DateTimeOffset</span></span>| <span data-ttu-id="47d06-138">На данный момент времени начала игнорируется.</span><span class="sxs-lookup"><span data-stu-id="47d06-138">Currently, the start time value is ignored.</span></span> |

## <a name="relationships"></a><span data-ttu-id="47d06-139">Отношения</span><span class="sxs-lookup"><span data-stu-id="47d06-139">Relationships</span></span>
<span data-ttu-id="47d06-140">Нет</span><span class="sxs-lookup"><span data-stu-id="47d06-140">None</span></span>


## <a name="methods"></a><span data-ttu-id="47d06-141">Методы</span><span class="sxs-lookup"><span data-stu-id="47d06-141">Methods</span></span>

| <span data-ttu-id="47d06-142">Метод</span><span class="sxs-lookup"><span data-stu-id="47d06-142">Method</span></span>           | <span data-ttu-id="47d06-143">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="47d06-143">Return Type</span></span>    |<span data-ttu-id="47d06-144">Описание</span><span class="sxs-lookup"><span data-stu-id="47d06-144">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="47d06-145">Получение oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="47d06-145">Get oAuth2PermissionGrant</span></span>](../api/oauth2permissiongrant-get.md) | [<span data-ttu-id="47d06-146">oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="47d06-146">oAuth2PermissionGrant</span></span>](oauth2permissiongrant.md) |<span data-ttu-id="47d06-147">Чтение свойства и связи объекта oAuth2PermissionGrant.</span><span class="sxs-lookup"><span data-stu-id="47d06-147">Read properties and relationships of oAuth2PermissionGrant object.</span></span>|
|[<span data-ttu-id="47d06-148">Список oAuth2PermissionGrants</span><span class="sxs-lookup"><span data-stu-id="47d06-148">List oAuth2PermissionGrants</span></span>](../api/oauth2permissiongrant-list.md) | <span data-ttu-id="47d06-149">[oAuth2PermissionGrant](oauth2permissiongrant.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="47d06-149">[oAuth2PermissionGrant](oauth2permissiongrant.md) collection</span></span> | <span data-ttu-id="47d06-150">Получение списка объектов oauth2PermissionGrant.</span><span class="sxs-lookup"><span data-stu-id="47d06-150">Retrieve a list of oauth2PermissionGrant objects.</span></span> |
|[<span data-ttu-id="47d06-151">Обновление oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="47d06-151">Update oAuth2PermissionGrant</span></span>](../api/oauth2permissiongrant-update.md) | [<span data-ttu-id="47d06-152">oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="47d06-152">oAuth2PermissionGrant</span></span>](oauth2permissiongrant.md) |<span data-ttu-id="47d06-153">Обновление объекта oAuth2PermissionGrant.</span><span class="sxs-lookup"><span data-stu-id="47d06-153">Update oAuth2PermissionGrant object.</span></span> |
|[<span data-ttu-id="47d06-154">Удаление oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="47d06-154">Delete oAuth2PermissionGrant</span></span>](../api/oauth2permissiongrant-delete.md) | <span data-ttu-id="47d06-155">Нет</span><span class="sxs-lookup"><span data-stu-id="47d06-155">None</span></span> |<span data-ttu-id="47d06-156">Удалите объект oAuth2PermissionGrant.</span><span class="sxs-lookup"><span data-stu-id="47d06-156">Delete oAuth2PermissionGrant object.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "oAuth2PermissionGrant resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/oauth2permissiongrant.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

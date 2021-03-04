---
title: тип ресурса connectedOrganization
description: В управлении правами Azure AD подключенная организация является ссылкой на каталог или домен другой организации, пользователи которой могут запрашивать доступ.
author: markwahl-msft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 23deb11dc582228cd398dfc1f88d576b3cb15a86
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50444303"
---
# <a name="connectedorganization-resource-type"></a><span data-ttu-id="e63f2-103">тип ресурса connectedOrganization</span><span class="sxs-lookup"><span data-stu-id="e63f2-103">connectedOrganization resource type</span></span>

<span data-ttu-id="e63f2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e63f2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e63f2-105">В [управлении правами Azure AD](entitlementmanagement-root.md)подключенная организация является ссылкой на каталог или домен другой организации, пользователи которой могут запрашивать доступ.</span><span class="sxs-lookup"><span data-stu-id="e63f2-105">In [Azure AD entitlement management](entitlementmanagement-root.md), a connected organization is a reference to a directory or domain of another organization whose users can request access.</span></span>

## <a name="methods"></a><span data-ttu-id="e63f2-106">Методы</span><span class="sxs-lookup"><span data-stu-id="e63f2-106">Methods</span></span>

|<span data-ttu-id="e63f2-107">Метод</span><span class="sxs-lookup"><span data-stu-id="e63f2-107">Method</span></span>|<span data-ttu-id="e63f2-108">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="e63f2-108">Return type</span></span>|<span data-ttu-id="e63f2-109">Описание</span><span class="sxs-lookup"><span data-stu-id="e63f2-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="e63f2-110">Списки подключенныхОрганизацией</span><span class="sxs-lookup"><span data-stu-id="e63f2-110">List connectedOrganizations</span></span>](../api/connectedorganization-list.md) | <span data-ttu-id="e63f2-111">[connectedOrganization](connectedorganization.md) collection</span><span class="sxs-lookup"><span data-stu-id="e63f2-111">[connectedOrganization](connectedorganization.md) collection</span></span> | <span data-ttu-id="e63f2-112">Извлечение списка объектов connectedOrganization.</span><span class="sxs-lookup"><span data-stu-id="e63f2-112">Retrieve a list of connectedOrganization objects.</span></span> |
|[<span data-ttu-id="e63f2-113">Создание connectedOrganization</span><span class="sxs-lookup"><span data-stu-id="e63f2-113">Create connectedOrganization</span></span>](../api/connectedorganization-post.md) | [<span data-ttu-id="e63f2-114">connectedOrganization</span><span class="sxs-lookup"><span data-stu-id="e63f2-114">connectedOrganization</span></span>](connectedorganization.md) | <span data-ttu-id="e63f2-115">Создание нового объекта connectedOrganization.</span><span class="sxs-lookup"><span data-stu-id="e63f2-115">Create a new connectedOrganization object.</span></span> |
|[<span data-ttu-id="e63f2-116">ПодключениеОрганизация</span><span class="sxs-lookup"><span data-stu-id="e63f2-116">Get connectedOrganization</span></span>](../api/connectedorganization-get.md) | [<span data-ttu-id="e63f2-117">connectedOrganization</span><span class="sxs-lookup"><span data-stu-id="e63f2-117">connectedOrganization</span></span>](connectedorganization.md) | <span data-ttu-id="e63f2-118">Чтение свойств и связей объекта connectedOrganization.</span><span class="sxs-lookup"><span data-stu-id="e63f2-118">Read properties and relationships of a connectedOrganization object.</span></span> |
|[<span data-ttu-id="e63f2-119">Обновление connectedOrganization</span><span class="sxs-lookup"><span data-stu-id="e63f2-119">Update connectedOrganization</span></span>](../api/connectedorganization-update.md) | | <span data-ttu-id="e63f2-120">Обновление подключеннойорганизации.</span><span class="sxs-lookup"><span data-stu-id="e63f2-120">Update a connectedOrganization.</span></span> |
|[<span data-ttu-id="e63f2-121">Удаление connectedOrganization</span><span class="sxs-lookup"><span data-stu-id="e63f2-121">Delete connectedOrganization</span></span>](../api/connectedorganization-delete.md) |<span data-ttu-id="e63f2-122">Нет</span><span class="sxs-lookup"><span data-stu-id="e63f2-122">None</span></span> | <span data-ttu-id="e63f2-123">Удаление подключеннойорганизации.</span><span class="sxs-lookup"><span data-stu-id="e63f2-123">Delete a connectedOrganization.</span></span> |
|[<span data-ttu-id="e63f2-124">Список internalSponsors</span><span class="sxs-lookup"><span data-stu-id="e63f2-124">List internalSponsors</span></span>](../api/connectedorganization-list-internalsponsors.md) | <span data-ttu-id="e63f2-125">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="e63f2-125">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="e63f2-126">Извлечение списка внутренних спонсоров connectedOrganization.</span><span class="sxs-lookup"><span data-stu-id="e63f2-126">Retrieve a list of a connectedOrganization's internal sponsors.</span></span> |
|[<span data-ttu-id="e63f2-127">Список externalSponsors</span><span class="sxs-lookup"><span data-stu-id="e63f2-127">List externalSponsors</span></span>](../api/connectedorganization-list-externalsponsors.md) | <span data-ttu-id="e63f2-128">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="e63f2-128">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="e63f2-129">Извлечение списка внешних спонсоров connectedOrganization.</span><span class="sxs-lookup"><span data-stu-id="e63f2-129">Retrieve a list of a connectedOrganization's external sponsors.</span></span> |
|[<span data-ttu-id="e63f2-130">Добавление internalSponsors</span><span class="sxs-lookup"><span data-stu-id="e63f2-130">Add internalSponsors</span></span>](../api/connectedorganization-post-internalsponsors.md) | <span data-ttu-id="e63f2-131">Нет</span><span class="sxs-lookup"><span data-stu-id="e63f2-131">None</span></span> | <span data-ttu-id="e63f2-132">Добавьте пользователя или группу во внутренние спонсоры connectedOrganization.</span><span class="sxs-lookup"><span data-stu-id="e63f2-132">Add a user or group to a connectedOrganization's internal sponsors.</span></span> |
|[<span data-ttu-id="e63f2-133">Добавление externalSponsors</span><span class="sxs-lookup"><span data-stu-id="e63f2-133">Add externalSponsors</span></span>](../api/connectedorganization-post-externalsponsors.md) | <span data-ttu-id="e63f2-134">Нет</span><span class="sxs-lookup"><span data-stu-id="e63f2-134">None</span></span> | <span data-ttu-id="e63f2-135">Добавьте пользователя или группу к внешним спонсорам connectedOrganization.</span><span class="sxs-lookup"><span data-stu-id="e63f2-135">Add a user or group to a connectedOrganization's external sponsors.</span></span> |
|[<span data-ttu-id="e63f2-136">Удаление internalSponsors</span><span class="sxs-lookup"><span data-stu-id="e63f2-136">Remove internalSponsors</span></span>](../api/connectedorganization-delete-internalsponsors.md) | <span data-ttu-id="e63f2-137">Нет</span><span class="sxs-lookup"><span data-stu-id="e63f2-137">None</span></span> | <span data-ttu-id="e63f2-138">Удалите пользователя или группу из внутренних спонсоров connectedOrganization.</span><span class="sxs-lookup"><span data-stu-id="e63f2-138">Remove a user or group from a connectedOrganization's internal sponsors.</span></span> |
|[<span data-ttu-id="e63f2-139">Удаление externalSponsors</span><span class="sxs-lookup"><span data-stu-id="e63f2-139">Remove externalSponsors</span></span>](../api/connectedorganization-delete-externalsponsors.md) | <span data-ttu-id="e63f2-140">Нет</span><span class="sxs-lookup"><span data-stu-id="e63f2-140">None</span></span> | <span data-ttu-id="e63f2-141">Удалите пользователя или группу из внешних спонсоров connectedOrganization.</span><span class="sxs-lookup"><span data-stu-id="e63f2-141">Remove a user or group from a connectedOrganization's external sponsors.</span></span> |

## <a name="properties"></a><span data-ttu-id="e63f2-142">Свойства</span><span class="sxs-lookup"><span data-stu-id="e63f2-142">Properties</span></span>

|<span data-ttu-id="e63f2-143">Свойство</span><span class="sxs-lookup"><span data-stu-id="e63f2-143">Property</span></span>|<span data-ttu-id="e63f2-144">Тип</span><span class="sxs-lookup"><span data-stu-id="e63f2-144">Type</span></span>|<span data-ttu-id="e63f2-145">Описание</span><span class="sxs-lookup"><span data-stu-id="e63f2-145">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e63f2-146">createdBy</span><span class="sxs-lookup"><span data-stu-id="e63f2-146">createdBy</span></span>|<span data-ttu-id="e63f2-147">String</span><span class="sxs-lookup"><span data-stu-id="e63f2-147">String</span></span>|<span data-ttu-id="e63f2-148">UPN пользователя, создавшего этот ресурс.</span><span class="sxs-lookup"><span data-stu-id="e63f2-148">UPN of the user who created this resource.</span></span> <span data-ttu-id="e63f2-149">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e63f2-149">Read-only.</span></span>|
|<span data-ttu-id="e63f2-150">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e63f2-150">createdDateTime</span></span>|<span data-ttu-id="e63f2-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e63f2-151">DateTimeOffset</span></span>|<span data-ttu-id="e63f2-152">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="e63f2-152">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="e63f2-153">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="e63f2-153">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="e63f2-154">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e63f2-154">Read-only.</span></span>|
|<span data-ttu-id="e63f2-155">description</span><span class="sxs-lookup"><span data-stu-id="e63f2-155">description</span></span>|<span data-ttu-id="e63f2-156">String</span><span class="sxs-lookup"><span data-stu-id="e63f2-156">String</span></span>|<span data-ttu-id="e63f2-157">Описание связанной организации.</span><span class="sxs-lookup"><span data-stu-id="e63f2-157">The description of the connected organization.</span></span>|
|<span data-ttu-id="e63f2-158">displayName</span><span class="sxs-lookup"><span data-stu-id="e63f2-158">displayName</span></span>|<span data-ttu-id="e63f2-159">String</span><span class="sxs-lookup"><span data-stu-id="e63f2-159">String</span></span>|<span data-ttu-id="e63f2-160">Отображает имя подключенной организации.</span><span class="sxs-lookup"><span data-stu-id="e63f2-160">The display name of the connected organization.</span></span>|
|<span data-ttu-id="e63f2-161">id</span><span class="sxs-lookup"><span data-stu-id="e63f2-161">id</span></span>|<span data-ttu-id="e63f2-162">String</span><span class="sxs-lookup"><span data-stu-id="e63f2-162">String</span></span>| <span data-ttu-id="e63f2-163">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e63f2-163">Read-only.</span></span>|
|<span data-ttu-id="e63f2-164">modifiedBy</span><span class="sxs-lookup"><span data-stu-id="e63f2-164">modifiedBy</span></span>|<span data-ttu-id="e63f2-165">String</span><span class="sxs-lookup"><span data-stu-id="e63f2-165">String</span></span>|<span data-ttu-id="e63f2-166">UPN пользователя, который в последний раз изменил этот ресурс.</span><span class="sxs-lookup"><span data-stu-id="e63f2-166">UPN of the user who last modified this resource.</span></span> <span data-ttu-id="e63f2-167">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e63f2-167">Read-only.</span></span>|
|<span data-ttu-id="e63f2-168">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e63f2-168">modifiedDateTime</span></span>|<span data-ttu-id="e63f2-169">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e63f2-169">DateTimeOffset</span></span>|<span data-ttu-id="e63f2-170">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="e63f2-170">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="e63f2-171">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="e63f2-171">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="e63f2-172">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e63f2-172">Read-only.</span></span>|
|<span data-ttu-id="e63f2-173">state</span><span class="sxs-lookup"><span data-stu-id="e63f2-173">state</span></span>|<span data-ttu-id="e63f2-174">connectedOrganizationState</span><span class="sxs-lookup"><span data-stu-id="e63f2-174">connectedOrganizationState</span></span>|<span data-ttu-id="e63f2-175">Состояние связанной организации определяет, применимы ли политики назначения с типом области `AllConfiguredConnectedOrganizationSubjects` запроса.</span><span class="sxs-lookup"><span data-stu-id="e63f2-175">The state of a connected organization defines whether assignment policies with requestor scope type `AllConfiguredConnectedOrganizationSubjects` are applicable or not.</span></span> <span data-ttu-id="e63f2-176">Возможные значения: `configured`, `proposed`.</span><span class="sxs-lookup"><span data-stu-id="e63f2-176">Possible values are: `configured`, `proposed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e63f2-177">Связи</span><span class="sxs-lookup"><span data-stu-id="e63f2-177">Relationships</span></span>

|<span data-ttu-id="e63f2-178">Связь</span><span class="sxs-lookup"><span data-stu-id="e63f2-178">Relationship</span></span>|<span data-ttu-id="e63f2-179">Тип</span><span class="sxs-lookup"><span data-stu-id="e63f2-179">Type</span></span>|<span data-ttu-id="e63f2-180">Описание</span><span class="sxs-lookup"><span data-stu-id="e63f2-180">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e63f2-181">identitySources</span><span class="sxs-lookup"><span data-stu-id="e63f2-181">identitySources</span></span>|<span data-ttu-id="e63f2-182">[коллекция identitySource](identitySource.md)</span><span class="sxs-lookup"><span data-stu-id="e63f2-182">[identitySource](identitySource.md) collection</span></span>| <span data-ttu-id="e63f2-183">Источники удостоверений в этой связанной организации, один из [azureActiveDirectoryTenant,](azureactivedirectorytenant.md) [domainIdentitySource](domainidentitysource.md) или [externalDomainFederation.](externaldomainfederation.md)</span><span class="sxs-lookup"><span data-stu-id="e63f2-183">The identity sources in this connected organization, one of [azureActiveDirectoryTenant](azureactivedirectorytenant.md), [domainIdentitySource](domainidentitysource.md) or [externalDomainFederation](externaldomainfederation.md).</span></span> <span data-ttu-id="e63f2-184">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e63f2-184">Read-only.</span></span> <span data-ttu-id="e63f2-185">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="e63f2-185">Nullable.</span></span>|
|<span data-ttu-id="e63f2-186">internalSponsors</span><span class="sxs-lookup"><span data-stu-id="e63f2-186">internalSponsors</span></span>| <span data-ttu-id="e63f2-187">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="e63f2-187">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="e63f2-188">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="e63f2-188">Nullable.</span></span>|
|<span data-ttu-id="e63f2-189">externalSponsors</span><span class="sxs-lookup"><span data-stu-id="e63f2-189">externalSponsors</span></span>| <span data-ttu-id="e63f2-190">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="e63f2-190">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="e63f2-191">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="e63f2-191">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e63f2-192">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e63f2-192">JSON representation</span></span>

<span data-ttu-id="e63f2-193">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e63f2-193">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.connectedOrganization",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->

```json
{
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "createdBy": "String",
  "createdDateTime": "String (timestamp)",
  "modifiedBy": "String",
  "modifiedDateTime": "String (timestamp)",
  "identitySources": [
    {
      "@odata.type": "microsoft.graph.azureActiveDirectoryTenant",
      "tenantId": "String (identifier)",
      "displayName": "String"
    }
  ],
  "state": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "connectedOrganization resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->



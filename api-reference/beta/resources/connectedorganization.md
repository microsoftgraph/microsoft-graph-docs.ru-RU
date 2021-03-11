---
title: тип ресурса connectedOrganization
description: В управлении правами Azure AD подключенная организация является ссылкой на каталог или домен другой организации, пользователи которой могут запрашивать доступ.
author: markwahl-msft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 01837683481008fa79c2213970404413bdd6efe2
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50721686"
---
# <a name="connectedorganization-resource-type"></a><span data-ttu-id="3f4cb-103">тип ресурса connectedOrganization</span><span class="sxs-lookup"><span data-stu-id="3f4cb-103">connectedOrganization resource type</span></span>

<span data-ttu-id="3f4cb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3f4cb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3f4cb-105">В [управлении правами Azure AD](entitlementmanagement-root.md)подключенная организация является ссылкой на каталог или домен другой организации, пользователи которой могут запрашивать доступ.</span><span class="sxs-lookup"><span data-stu-id="3f4cb-105">In [Azure AD entitlement management](entitlementmanagement-root.md), a connected organization is a reference to a directory or domain of another organization whose users can request access.</span></span>

## <a name="methods"></a><span data-ttu-id="3f4cb-106">Методы</span><span class="sxs-lookup"><span data-stu-id="3f4cb-106">Methods</span></span>

|<span data-ttu-id="3f4cb-107">Метод</span><span class="sxs-lookup"><span data-stu-id="3f4cb-107">Method</span></span>|<span data-ttu-id="3f4cb-108">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="3f4cb-108">Return type</span></span>|<span data-ttu-id="3f4cb-109">Описание</span><span class="sxs-lookup"><span data-stu-id="3f4cb-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="3f4cb-110">Списки подключенныхОрганизацией</span><span class="sxs-lookup"><span data-stu-id="3f4cb-110">List connectedOrganizations</span></span>](../api/connectedorganization-list.md) | <span data-ttu-id="3f4cb-111">[connectedOrganization](connectedorganization.md) collection</span><span class="sxs-lookup"><span data-stu-id="3f4cb-111">[connectedOrganization](connectedorganization.md) collection</span></span> | <span data-ttu-id="3f4cb-112">Извлечение списка объектов connectedOrganization.</span><span class="sxs-lookup"><span data-stu-id="3f4cb-112">Retrieve a list of connectedOrganization objects.</span></span> |
|[<span data-ttu-id="3f4cb-113">Создание connectedOrganization</span><span class="sxs-lookup"><span data-stu-id="3f4cb-113">Create connectedOrganization</span></span>](../api/connectedorganization-post.md) | [<span data-ttu-id="3f4cb-114">connectedOrganization</span><span class="sxs-lookup"><span data-stu-id="3f4cb-114">connectedOrganization</span></span>](connectedorganization.md) | <span data-ttu-id="3f4cb-115">Создание нового объекта connectedOrganization.</span><span class="sxs-lookup"><span data-stu-id="3f4cb-115">Create a new connectedOrganization object.</span></span> |
|[<span data-ttu-id="3f4cb-116">ПодключениеОрганизация</span><span class="sxs-lookup"><span data-stu-id="3f4cb-116">Get connectedOrganization</span></span>](../api/connectedorganization-get.md) | [<span data-ttu-id="3f4cb-117">connectedOrganization</span><span class="sxs-lookup"><span data-stu-id="3f4cb-117">connectedOrganization</span></span>](connectedorganization.md) | <span data-ttu-id="3f4cb-118">Чтение свойств и связей объекта connectedOrganization.</span><span class="sxs-lookup"><span data-stu-id="3f4cb-118">Read properties and relationships of a connectedOrganization object.</span></span> |
|[<span data-ttu-id="3f4cb-119">Обновление connectedOrganization</span><span class="sxs-lookup"><span data-stu-id="3f4cb-119">Update connectedOrganization</span></span>](../api/connectedorganization-update.md) | | <span data-ttu-id="3f4cb-120">Обновление подключеннойорганизации.</span><span class="sxs-lookup"><span data-stu-id="3f4cb-120">Update a connectedOrganization.</span></span> |
|[<span data-ttu-id="3f4cb-121">Удаление connectedOrganization</span><span class="sxs-lookup"><span data-stu-id="3f4cb-121">Delete connectedOrganization</span></span>](../api/connectedorganization-delete.md) |<span data-ttu-id="3f4cb-122">Нет</span><span class="sxs-lookup"><span data-stu-id="3f4cb-122">None</span></span> | <span data-ttu-id="3f4cb-123">Удаление подключеннойорганизации.</span><span class="sxs-lookup"><span data-stu-id="3f4cb-123">Delete a connectedOrganization.</span></span> |
|[<span data-ttu-id="3f4cb-124">Список internalSponsors</span><span class="sxs-lookup"><span data-stu-id="3f4cb-124">List internalSponsors</span></span>](../api/connectedorganization-list-internalsponsors.md) | <span data-ttu-id="3f4cb-125">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="3f4cb-125">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="3f4cb-126">Извлечение списка внутренних спонсоров connectedOrganization.</span><span class="sxs-lookup"><span data-stu-id="3f4cb-126">Retrieve a list of a connectedOrganization's internal sponsors.</span></span> |
|[<span data-ttu-id="3f4cb-127">Список externalSponsors</span><span class="sxs-lookup"><span data-stu-id="3f4cb-127">List externalSponsors</span></span>](../api/connectedorganization-list-externalsponsors.md) | <span data-ttu-id="3f4cb-128">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="3f4cb-128">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="3f4cb-129">Извлечение списка внешних спонсоров connectedOrganization.</span><span class="sxs-lookup"><span data-stu-id="3f4cb-129">Retrieve a list of a connectedOrganization's external sponsors.</span></span> |
|[<span data-ttu-id="3f4cb-130">Добавление internalSponsors</span><span class="sxs-lookup"><span data-stu-id="3f4cb-130">Add internalSponsors</span></span>](../api/connectedorganization-post-internalsponsors.md) | <span data-ttu-id="3f4cb-131">Нет</span><span class="sxs-lookup"><span data-stu-id="3f4cb-131">None</span></span> | <span data-ttu-id="3f4cb-132">Добавьте пользователя или группу во внутренние спонсоры connectedOrganization.</span><span class="sxs-lookup"><span data-stu-id="3f4cb-132">Add a user or group to a connectedOrganization's internal sponsors.</span></span> |
|[<span data-ttu-id="3f4cb-133">Добавление externalSponsors</span><span class="sxs-lookup"><span data-stu-id="3f4cb-133">Add externalSponsors</span></span>](../api/connectedorganization-post-externalsponsors.md) | <span data-ttu-id="3f4cb-134">Нет</span><span class="sxs-lookup"><span data-stu-id="3f4cb-134">None</span></span> | <span data-ttu-id="3f4cb-135">Добавьте пользователя или группу к внешним спонсорам connectedOrganization.</span><span class="sxs-lookup"><span data-stu-id="3f4cb-135">Add a user or group to a connectedOrganization's external sponsors.</span></span> |
|[<span data-ttu-id="3f4cb-136">Удаление internalSponsors</span><span class="sxs-lookup"><span data-stu-id="3f4cb-136">Remove internalSponsors</span></span>](../api/connectedorganization-delete-internalsponsors.md) | <span data-ttu-id="3f4cb-137">Нет</span><span class="sxs-lookup"><span data-stu-id="3f4cb-137">None</span></span> | <span data-ttu-id="3f4cb-138">Удалите пользователя или группу из внутренних спонсоров connectedOrganization.</span><span class="sxs-lookup"><span data-stu-id="3f4cb-138">Remove a user or group from a connectedOrganization's internal sponsors.</span></span> |
|[<span data-ttu-id="3f4cb-139">Удаление externalSponsors</span><span class="sxs-lookup"><span data-stu-id="3f4cb-139">Remove externalSponsors</span></span>](../api/connectedorganization-delete-externalsponsors.md) | <span data-ttu-id="3f4cb-140">Нет</span><span class="sxs-lookup"><span data-stu-id="3f4cb-140">None</span></span> | <span data-ttu-id="3f4cb-141">Удалите пользователя или группу из внешних спонсоров connectedOrganization.</span><span class="sxs-lookup"><span data-stu-id="3f4cb-141">Remove a user or group from a connectedOrganization's external sponsors.</span></span> |

## <a name="properties"></a><span data-ttu-id="3f4cb-142">Свойства</span><span class="sxs-lookup"><span data-stu-id="3f4cb-142">Properties</span></span>

|<span data-ttu-id="3f4cb-143">Свойство</span><span class="sxs-lookup"><span data-stu-id="3f4cb-143">Property</span></span>|<span data-ttu-id="3f4cb-144">Тип</span><span class="sxs-lookup"><span data-stu-id="3f4cb-144">Type</span></span>|<span data-ttu-id="3f4cb-145">Описание</span><span class="sxs-lookup"><span data-stu-id="3f4cb-145">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3f4cb-146">createdBy</span><span class="sxs-lookup"><span data-stu-id="3f4cb-146">createdBy</span></span>|<span data-ttu-id="3f4cb-147">String</span><span class="sxs-lookup"><span data-stu-id="3f4cb-147">String</span></span>|<span data-ttu-id="3f4cb-148">UPN пользователя, создавшего этот ресурс.</span><span class="sxs-lookup"><span data-stu-id="3f4cb-148">UPN of the user who created this resource.</span></span> <span data-ttu-id="3f4cb-149">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3f4cb-149">Read-only.</span></span>|
|<span data-ttu-id="3f4cb-150">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3f4cb-150">createdDateTime</span></span>|<span data-ttu-id="3f4cb-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3f4cb-151">DateTimeOffset</span></span>|<span data-ttu-id="3f4cb-152">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="3f4cb-152">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="3f4cb-153">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="3f4cb-153">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="3f4cb-154">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3f4cb-154">Read-only.</span></span>|
|<span data-ttu-id="3f4cb-155">description</span><span class="sxs-lookup"><span data-stu-id="3f4cb-155">description</span></span>|<span data-ttu-id="3f4cb-156">String</span><span class="sxs-lookup"><span data-stu-id="3f4cb-156">String</span></span>|<span data-ttu-id="3f4cb-157">Описание связанной организации.</span><span class="sxs-lookup"><span data-stu-id="3f4cb-157">The description of the connected organization.</span></span>|
|<span data-ttu-id="3f4cb-158">displayName</span><span class="sxs-lookup"><span data-stu-id="3f4cb-158">displayName</span></span>|<span data-ttu-id="3f4cb-159">String</span><span class="sxs-lookup"><span data-stu-id="3f4cb-159">String</span></span>|<span data-ttu-id="3f4cb-160">Отображает имя подключенной организации.</span><span class="sxs-lookup"><span data-stu-id="3f4cb-160">The display name of the connected organization.</span></span>|
|<span data-ttu-id="3f4cb-161">id</span><span class="sxs-lookup"><span data-stu-id="3f4cb-161">id</span></span>|<span data-ttu-id="3f4cb-162">String</span><span class="sxs-lookup"><span data-stu-id="3f4cb-162">String</span></span>| <span data-ttu-id="3f4cb-163">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3f4cb-163">Read-only.</span></span>|
|<span data-ttu-id="3f4cb-164">modifiedBy</span><span class="sxs-lookup"><span data-stu-id="3f4cb-164">modifiedBy</span></span>|<span data-ttu-id="3f4cb-165">String</span><span class="sxs-lookup"><span data-stu-id="3f4cb-165">String</span></span>|<span data-ttu-id="3f4cb-166">UPN пользователя, который в последний раз изменил этот ресурс.</span><span class="sxs-lookup"><span data-stu-id="3f4cb-166">UPN of the user who last modified this resource.</span></span> <span data-ttu-id="3f4cb-167">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3f4cb-167">Read-only.</span></span>|
|<span data-ttu-id="3f4cb-168">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3f4cb-168">modifiedDateTime</span></span>|<span data-ttu-id="3f4cb-169">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3f4cb-169">DateTimeOffset</span></span>|<span data-ttu-id="3f4cb-170">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="3f4cb-170">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="3f4cb-171">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="3f4cb-171">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="3f4cb-172">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3f4cb-172">Read-only.</span></span>|
|<span data-ttu-id="3f4cb-173">state</span><span class="sxs-lookup"><span data-stu-id="3f4cb-173">state</span></span>|<span data-ttu-id="3f4cb-174">connectedOrganizationState</span><span class="sxs-lookup"><span data-stu-id="3f4cb-174">connectedOrganizationState</span></span>|<span data-ttu-id="3f4cb-175">Состояние связанной организации определяет, применимы ли политики назначения с типом области `AllConfiguredConnectedOrganizationSubjects` запроса.</span><span class="sxs-lookup"><span data-stu-id="3f4cb-175">The state of a connected organization defines whether assignment policies with requestor scope type `AllConfiguredConnectedOrganizationSubjects` are applicable or not.</span></span> <span data-ttu-id="3f4cb-176">Возможные значения: `configured`, `proposed`.</span><span class="sxs-lookup"><span data-stu-id="3f4cb-176">Possible values are: `configured`, `proposed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3f4cb-177">Связи</span><span class="sxs-lookup"><span data-stu-id="3f4cb-177">Relationships</span></span>

|<span data-ttu-id="3f4cb-178">Связь</span><span class="sxs-lookup"><span data-stu-id="3f4cb-178">Relationship</span></span>|<span data-ttu-id="3f4cb-179">Тип</span><span class="sxs-lookup"><span data-stu-id="3f4cb-179">Type</span></span>|<span data-ttu-id="3f4cb-180">Описание</span><span class="sxs-lookup"><span data-stu-id="3f4cb-180">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3f4cb-181">identitySources</span><span class="sxs-lookup"><span data-stu-id="3f4cb-181">identitySources</span></span>|<span data-ttu-id="3f4cb-182">[коллекция identitySource](identitySource.md)</span><span class="sxs-lookup"><span data-stu-id="3f4cb-182">[identitySource](identitySource.md) collection</span></span>| <span data-ttu-id="3f4cb-183">Источники удостоверений в этой связанной организации, один из [azureActiveDirectoryTenant,](azureactivedirectorytenant.md) [domainIdentitySource](domainidentitysource.md) или [externalDomainFederation.](externaldomainfederation.md)</span><span class="sxs-lookup"><span data-stu-id="3f4cb-183">The identity sources in this connected organization, one of [azureActiveDirectoryTenant](azureactivedirectorytenant.md), [domainIdentitySource](domainidentitysource.md) or [externalDomainFederation](externaldomainfederation.md).</span></span> <span data-ttu-id="3f4cb-184">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3f4cb-184">Read-only.</span></span> <span data-ttu-id="3f4cb-185">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="3f4cb-185">Nullable.</span></span>|
|<span data-ttu-id="3f4cb-186">internalSponsors</span><span class="sxs-lookup"><span data-stu-id="3f4cb-186">internalSponsors</span></span>| <span data-ttu-id="3f4cb-187">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="3f4cb-187">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="3f4cb-188">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="3f4cb-188">Nullable.</span></span>|
|<span data-ttu-id="3f4cb-189">externalSponsors</span><span class="sxs-lookup"><span data-stu-id="3f4cb-189">externalSponsors</span></span>| <span data-ttu-id="3f4cb-190">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="3f4cb-190">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="3f4cb-191">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="3f4cb-191">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3f4cb-192">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3f4cb-192">JSON representation</span></span>

<span data-ttu-id="3f4cb-193">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3f4cb-193">The following is a JSON representation of the resource.</span></span>

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



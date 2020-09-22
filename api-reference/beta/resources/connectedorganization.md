---
title: Тип ресурса Коннектедорганизатион
description: В управлении службой управления правами Azure AD подключенная организация является ссылкой на каталог или домен другой организации, чьи пользователи могут запрашивать доступ.
author: markwahl-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 95cce32d4336c34a61d6845b74e6e428d1774d21
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48027213"
---
# <a name="connectedorganization-resource-type"></a><span data-ttu-id="42d76-103">Тип ресурса Коннектедорганизатион</span><span class="sxs-lookup"><span data-stu-id="42d76-103">connectedOrganization resource type</span></span>

<span data-ttu-id="42d76-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="42d76-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="42d76-105">В [управлении службой управления правами Azure AD](entitlementmanagement-root.md)подключенная организация является ссылкой на каталог или домен другой организации, чьи пользователи могут запрашивать доступ.</span><span class="sxs-lookup"><span data-stu-id="42d76-105">In [Azure AD entitlement management](entitlementmanagement-root.md), a connected organization is a reference to a directory or domain of another organization whose users can request access.</span></span>

## <a name="methods"></a><span data-ttu-id="42d76-106">Методы</span><span class="sxs-lookup"><span data-stu-id="42d76-106">Methods</span></span>

|<span data-ttu-id="42d76-107">Метод</span><span class="sxs-lookup"><span data-stu-id="42d76-107">Method</span></span>|<span data-ttu-id="42d76-108">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="42d76-108">Return type</span></span>|<span data-ttu-id="42d76-109">Описание</span><span class="sxs-lookup"><span data-stu-id="42d76-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="42d76-110">Список Коннектедорганизатионс</span><span class="sxs-lookup"><span data-stu-id="42d76-110">List connectedOrganizations</span></span>](../api/connectedorganization-list.md) | <span data-ttu-id="42d76-111">Коллекция [коннектедорганизатион](connectedorganization.md)</span><span class="sxs-lookup"><span data-stu-id="42d76-111">[connectedOrganization](connectedorganization.md) collection</span></span> | <span data-ttu-id="42d76-112">Получение списка объектов Коннектедорганизатион.</span><span class="sxs-lookup"><span data-stu-id="42d76-112">Retrieve a list of connectedOrganization objects.</span></span> |
|[<span data-ttu-id="42d76-113">Создание Коннектедорганизатион</span><span class="sxs-lookup"><span data-stu-id="42d76-113">Create connectedOrganization</span></span>](../api/connectedorganization-post.md) | [<span data-ttu-id="42d76-114">коннектедорганизатион</span><span class="sxs-lookup"><span data-stu-id="42d76-114">connectedOrganization</span></span>](connectedorganization.md) | <span data-ttu-id="42d76-115">Создание нового объекта Коннектедорганизатион.</span><span class="sxs-lookup"><span data-stu-id="42d76-115">Create a new connectedOrganization object.</span></span> |
|[<span data-ttu-id="42d76-116">Получение Коннектедорганизатион</span><span class="sxs-lookup"><span data-stu-id="42d76-116">Get connectedOrganization</span></span>](../api/connectedorganization-get.md) | [<span data-ttu-id="42d76-117">коннектедорганизатион</span><span class="sxs-lookup"><span data-stu-id="42d76-117">connectedOrganization</span></span>](connectedorganization.md) | <span data-ttu-id="42d76-118">Чтение свойств и связей объекта Коннектедорганизатион.</span><span class="sxs-lookup"><span data-stu-id="42d76-118">Read properties and relationships of a connectedOrganization object.</span></span> |
|[<span data-ttu-id="42d76-119">Обновление Коннектедорганизатион</span><span class="sxs-lookup"><span data-stu-id="42d76-119">Update connectedOrganization</span></span>](../api/connectedorganization-update.md) | | <span data-ttu-id="42d76-120">Обновление Коннектедорганизатион.</span><span class="sxs-lookup"><span data-stu-id="42d76-120">Update a connectedOrganization.</span></span> |
|[<span data-ttu-id="42d76-121">Удаление Коннектедорганизатион</span><span class="sxs-lookup"><span data-stu-id="42d76-121">Delete connectedOrganization</span></span>](../api/connectedorganization-delete.md) |<span data-ttu-id="42d76-122">Нет</span><span class="sxs-lookup"><span data-stu-id="42d76-122">None</span></span> | <span data-ttu-id="42d76-123">Удаление объекта Коннектедорганизатион.</span><span class="sxs-lookup"><span data-stu-id="42d76-123">Delete a connectedOrganization.</span></span> |
|[<span data-ttu-id="42d76-124">Список Интерналспонсорс</span><span class="sxs-lookup"><span data-stu-id="42d76-124">List internalSponsors</span></span>](../api/connectedorganization-list-internalsponsors.md) | <span data-ttu-id="42d76-125">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="42d76-125">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="42d76-126">Получение списка внутренних спонсоров Коннектедорганизатион.</span><span class="sxs-lookup"><span data-stu-id="42d76-126">Retrieve a list of a connectedOrganization's internal sponsors.</span></span> |
|[<span data-ttu-id="42d76-127">Список Екстерналспонсорс</span><span class="sxs-lookup"><span data-stu-id="42d76-127">List externalSponsors</span></span>](../api/connectedorganization-list-externalsponsors.md) | <span data-ttu-id="42d76-128">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="42d76-128">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="42d76-129">Получение списка внешних спонсоров Коннектедорганизатион.</span><span class="sxs-lookup"><span data-stu-id="42d76-129">Retrieve a list of a connectedOrganization's external sponsors.</span></span> |
|[<span data-ttu-id="42d76-130">Добавление Интерналспонсорс</span><span class="sxs-lookup"><span data-stu-id="42d76-130">Add internalSponsors</span></span>](../api/connectedorganization-post-internalsponsors.md) | <span data-ttu-id="42d76-131">Нет</span><span class="sxs-lookup"><span data-stu-id="42d76-131">None</span></span> | <span data-ttu-id="42d76-132">Добавление пользователя или группы в внутренние спонсоры Коннектедорганизатион.</span><span class="sxs-lookup"><span data-stu-id="42d76-132">Add a user or group to a connectedOrganization's internal sponsors.</span></span> |
|[<span data-ttu-id="42d76-133">Добавление Екстерналспонсорс</span><span class="sxs-lookup"><span data-stu-id="42d76-133">Add externalSponsors</span></span>](../api/connectedorganization-post-externalsponsors.md) | <span data-ttu-id="42d76-134">Нет</span><span class="sxs-lookup"><span data-stu-id="42d76-134">None</span></span> | <span data-ttu-id="42d76-135">Добавление пользователя или группы во внешние спонсоры Коннектедорганизатион.</span><span class="sxs-lookup"><span data-stu-id="42d76-135">Add a user or group to a connectedOrganization's external sponsors.</span></span> |
|[<span data-ttu-id="42d76-136">Удаление Интерналспонсорс</span><span class="sxs-lookup"><span data-stu-id="42d76-136">Remove internalSponsors</span></span>](../api/connectedorganization-delete-internalsponsors.md) | <span data-ttu-id="42d76-137">Нет</span><span class="sxs-lookup"><span data-stu-id="42d76-137">None</span></span> | <span data-ttu-id="42d76-138">Удаление пользователя или группы из внутренних спонсоров Коннектедорганизатион.</span><span class="sxs-lookup"><span data-stu-id="42d76-138">Remove a user or group from a connectedOrganization's internal sponsors.</span></span> |
|[<span data-ttu-id="42d76-139">Удаление Екстерналспонсорс</span><span class="sxs-lookup"><span data-stu-id="42d76-139">Remove externalSponsors</span></span>](../api/connectedorganization-delete-externalsponsors.md) | <span data-ttu-id="42d76-140">Нет</span><span class="sxs-lookup"><span data-stu-id="42d76-140">None</span></span> | <span data-ttu-id="42d76-141">Удаление пользователя или группы из внешних спонсоров Коннектедорганизатион.</span><span class="sxs-lookup"><span data-stu-id="42d76-141">Remove a user or group from a connectedOrganization's external sponsors.</span></span> |

## <a name="properties"></a><span data-ttu-id="42d76-142">Свойства</span><span class="sxs-lookup"><span data-stu-id="42d76-142">Properties</span></span>

|<span data-ttu-id="42d76-143">Свойство</span><span class="sxs-lookup"><span data-stu-id="42d76-143">Property</span></span>|<span data-ttu-id="42d76-144">Тип</span><span class="sxs-lookup"><span data-stu-id="42d76-144">Type</span></span>|<span data-ttu-id="42d76-145">Описание</span><span class="sxs-lookup"><span data-stu-id="42d76-145">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="42d76-146">createdBy</span><span class="sxs-lookup"><span data-stu-id="42d76-146">createdBy</span></span>|<span data-ttu-id="42d76-147">String</span><span class="sxs-lookup"><span data-stu-id="42d76-147">String</span></span>|<span data-ttu-id="42d76-148">Имя участника-пользователя, создавшего этот ресурс.</span><span class="sxs-lookup"><span data-stu-id="42d76-148">UPN of the user who created this resource.</span></span> <span data-ttu-id="42d76-149">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="42d76-149">Read-only.</span></span>|
|<span data-ttu-id="42d76-150">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="42d76-150">createdDateTime</span></span>|<span data-ttu-id="42d76-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="42d76-151">DateTimeOffset</span></span>|<span data-ttu-id="42d76-152">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="42d76-152">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="42d76-153">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="42d76-153">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="42d76-154">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="42d76-154">Read-only.</span></span>|
|<span data-ttu-id="42d76-155">description</span><span class="sxs-lookup"><span data-stu-id="42d76-155">description</span></span>|<span data-ttu-id="42d76-156">String</span><span class="sxs-lookup"><span data-stu-id="42d76-156">String</span></span>|<span data-ttu-id="42d76-157">Описание подключенной Организации.</span><span class="sxs-lookup"><span data-stu-id="42d76-157">The description of the connected organization.</span></span>|
|<span data-ttu-id="42d76-158">displayName</span><span class="sxs-lookup"><span data-stu-id="42d76-158">displayName</span></span>|<span data-ttu-id="42d76-159">String</span><span class="sxs-lookup"><span data-stu-id="42d76-159">String</span></span>|<span data-ttu-id="42d76-160">Отображаемое имя подключенной Организации.</span><span class="sxs-lookup"><span data-stu-id="42d76-160">The display name of the connected organization.</span></span>|
|<span data-ttu-id="42d76-161">id</span><span class="sxs-lookup"><span data-stu-id="42d76-161">id</span></span>|<span data-ttu-id="42d76-162">String</span><span class="sxs-lookup"><span data-stu-id="42d76-162">String</span></span>| <span data-ttu-id="42d76-163">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="42d76-163">Read-only.</span></span>|
|<span data-ttu-id="42d76-164">модифиедби</span><span class="sxs-lookup"><span data-stu-id="42d76-164">modifiedBy</span></span>|<span data-ttu-id="42d76-165">String</span><span class="sxs-lookup"><span data-stu-id="42d76-165">String</span></span>|<span data-ttu-id="42d76-166">Имя участника-пользователя, который последним изменил этот ресурс.</span><span class="sxs-lookup"><span data-stu-id="42d76-166">UPN of the user who last modified this resource.</span></span> <span data-ttu-id="42d76-167">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="42d76-167">Read-only.</span></span>|
|<span data-ttu-id="42d76-168">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="42d76-168">modifiedDateTime</span></span>|<span data-ttu-id="42d76-169">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="42d76-169">DateTimeOffset</span></span>|<span data-ttu-id="42d76-170">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="42d76-170">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="42d76-171">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="42d76-171">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="42d76-172">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="42d76-172">Read-only.</span></span>|
|<span data-ttu-id="42d76-173">state</span><span class="sxs-lookup"><span data-stu-id="42d76-173">state</span></span>|<span data-ttu-id="42d76-174">коннектедорганизатионстате</span><span class="sxs-lookup"><span data-stu-id="42d76-174">connectedOrganizationState</span></span>|<span data-ttu-id="42d76-175">Состояние подключенной Организации определяет, применимы ли политики назначения с типом области запрашивающего `AllConfiguredConnectedOrganizationSubjects` .</span><span class="sxs-lookup"><span data-stu-id="42d76-175">The state of a connected organization defines whether assignment policies with requestor scope type `AllConfiguredConnectedOrganizationSubjects` are applicable or not.</span></span> <span data-ttu-id="42d76-176">Возможные значения: `configured`, `proposed`.</span><span class="sxs-lookup"><span data-stu-id="42d76-176">Possible values are: `configured`, `proposed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="42d76-177">Отношения</span><span class="sxs-lookup"><span data-stu-id="42d76-177">Relationships</span></span>

|<span data-ttu-id="42d76-178">Связь</span><span class="sxs-lookup"><span data-stu-id="42d76-178">Relationship</span></span>|<span data-ttu-id="42d76-179">Тип</span><span class="sxs-lookup"><span data-stu-id="42d76-179">Type</span></span>|<span data-ttu-id="42d76-180">Описание</span><span class="sxs-lookup"><span data-stu-id="42d76-180">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="42d76-181">идентитисаурцес</span><span class="sxs-lookup"><span data-stu-id="42d76-181">identitySources</span></span>|<span data-ttu-id="42d76-182">Коллекция [идентитисаурце](identitySource.md)</span><span class="sxs-lookup"><span data-stu-id="42d76-182">[identitySource](identitySource.md) collection</span></span>| <span data-ttu-id="42d76-183">Источники удостоверений в этой подключенной Организации, один из [азуреактиведиректоритенант](azureactivedirectorytenant.md), [домаинидентитисаурце](domainidentitysource.md) или [екстерналдомаинфедератион](externaldomainfederation.md).</span><span class="sxs-lookup"><span data-stu-id="42d76-183">The identity sources in this connected organization, one of [azureActiveDirectoryTenant](azureactivedirectorytenant.md), [domainIdentitySource](domainidentitysource.md) or [externalDomainFederation](externaldomainfederation.md).</span></span> <span data-ttu-id="42d76-184">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="42d76-184">Read-only.</span></span> <span data-ttu-id="42d76-185">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="42d76-185">Nullable.</span></span>|
|<span data-ttu-id="42d76-186">интерналспонсорс</span><span class="sxs-lookup"><span data-stu-id="42d76-186">internalSponsors</span></span>| <span data-ttu-id="42d76-187">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="42d76-187">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="42d76-188">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="42d76-188">Nullable.</span></span>|
|<span data-ttu-id="42d76-189">екстерналспонсорс</span><span class="sxs-lookup"><span data-stu-id="42d76-189">externalSponsors</span></span>| <span data-ttu-id="42d76-190">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="42d76-190">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="42d76-191">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="42d76-191">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="42d76-192">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="42d76-192">JSON representation</span></span>

<span data-ttu-id="42d76-193">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="42d76-193">The following is a JSON representation of the resource.</span></span>

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



---
title: Тип ресурса Коннектедорганизатион
description: В управлении службой управления правами Azure AD подключенная организация является ссылкой на каталог или домен другой организации, чьи пользователи могут запрашивать доступ.
author: markwahl-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: f5d53e3a24ad8e99c22d61bc6a4d519888c4aafd
ms.sourcegitcommit: ae2e4b8963edcdcc8ce572c06a531db4769d7779
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/29/2020
ms.locfileid: "47311292"
---
# <a name="connectedorganization-resource-type"></a><span data-ttu-id="5a04e-103">Тип ресурса Коннектедорганизатион</span><span class="sxs-lookup"><span data-stu-id="5a04e-103">connectedOrganization resource type</span></span>

<span data-ttu-id="5a04e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5a04e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5a04e-105">В [управлении службой управления правами Azure AD](entitlementmanagement-root.md)подключенная организация является ссылкой на каталог или домен другой организации, чьи пользователи могут запрашивать доступ.</span><span class="sxs-lookup"><span data-stu-id="5a04e-105">In [Azure AD entitlement management](entitlementmanagement-root.md), a connected organization is a reference to a directory or domain of another organization whose users can request access.</span></span>

## <a name="methods"></a><span data-ttu-id="5a04e-106">Методы</span><span class="sxs-lookup"><span data-stu-id="5a04e-106">Methods</span></span>

|<span data-ttu-id="5a04e-107">Метод</span><span class="sxs-lookup"><span data-stu-id="5a04e-107">Method</span></span>|<span data-ttu-id="5a04e-108">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="5a04e-108">Return type</span></span>|<span data-ttu-id="5a04e-109">Описание</span><span class="sxs-lookup"><span data-stu-id="5a04e-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="5a04e-110">Список Коннектедорганизатионс</span><span class="sxs-lookup"><span data-stu-id="5a04e-110">List connectedOrganizations</span></span>](../api/connectedorganization-list.md) | <span data-ttu-id="5a04e-111">Коллекция [коннектедорганизатион](connectedorganization.md)</span><span class="sxs-lookup"><span data-stu-id="5a04e-111">[connectedOrganization](connectedorganization.md) collection</span></span> | <span data-ttu-id="5a04e-112">Получение списка объектов Коннектедорганизатион.</span><span class="sxs-lookup"><span data-stu-id="5a04e-112">Retrieve a list of connectedOrganization objects.</span></span> |
|[<span data-ttu-id="5a04e-113">Создание Коннектедорганизатион</span><span class="sxs-lookup"><span data-stu-id="5a04e-113">Create connectedOrganization</span></span>](../api/connectedorganization-post.md) | [<span data-ttu-id="5a04e-114">коннектедорганизатион</span><span class="sxs-lookup"><span data-stu-id="5a04e-114">connectedOrganization</span></span>](connectedorganization.md) | <span data-ttu-id="5a04e-115">Создание нового объекта Коннектедорганизатион.</span><span class="sxs-lookup"><span data-stu-id="5a04e-115">Create a new connectedOrganization object.</span></span> |
|[<span data-ttu-id="5a04e-116">Получение Коннектедорганизатион</span><span class="sxs-lookup"><span data-stu-id="5a04e-116">Get connectedOrganization</span></span>](../api/connectedorganization-get.md) | [<span data-ttu-id="5a04e-117">коннектедорганизатион</span><span class="sxs-lookup"><span data-stu-id="5a04e-117">connectedOrganization</span></span>](connectedorganization.md) | <span data-ttu-id="5a04e-118">Чтение свойств и связей объекта Коннектедорганизатион.</span><span class="sxs-lookup"><span data-stu-id="5a04e-118">Read properties and relationships of a connectedOrganization object.</span></span> |
|[<span data-ttu-id="5a04e-119">Обновление Коннектедорганизатион</span><span class="sxs-lookup"><span data-stu-id="5a04e-119">Update connectedOrganization</span></span>](../api/connectedorganization-update.md) | | <span data-ttu-id="5a04e-120">Обновление Коннектедорганизатион.</span><span class="sxs-lookup"><span data-stu-id="5a04e-120">Update a connectedOrganization.</span></span> |
|[<span data-ttu-id="5a04e-121">Удаление Коннектедорганизатион</span><span class="sxs-lookup"><span data-stu-id="5a04e-121">Delete connectedOrganization</span></span>](../api/connectedorganization-delete.md) |<span data-ttu-id="5a04e-122">Нет</span><span class="sxs-lookup"><span data-stu-id="5a04e-122">None</span></span> | <span data-ttu-id="5a04e-123">Удаление объекта Коннектедорганизатион.</span><span class="sxs-lookup"><span data-stu-id="5a04e-123">Delete a connectedOrganization.</span></span> |
|[<span data-ttu-id="5a04e-124">Список Интерналспонсорс</span><span class="sxs-lookup"><span data-stu-id="5a04e-124">List internalSponsors</span></span>](../api/connectedorganization-list-internalsponsors.md) | <span data-ttu-id="5a04e-125">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="5a04e-125">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="5a04e-126">Получение списка внутренних спонсоров Коннектедорганизатион.</span><span class="sxs-lookup"><span data-stu-id="5a04e-126">Retrieve a list of a connectedOrganization's internal sponsors.</span></span> |
|[<span data-ttu-id="5a04e-127">Список Екстерналспонсорс</span><span class="sxs-lookup"><span data-stu-id="5a04e-127">List externalSponsors</span></span>](../api/connectedorganization-list-externalsponsors.md) | <span data-ttu-id="5a04e-128">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="5a04e-128">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="5a04e-129">Получение списка внешних спонсоров Коннектедорганизатион.</span><span class="sxs-lookup"><span data-stu-id="5a04e-129">Retrieve a list of a connectedOrganization's external sponsors.</span></span> |
|[<span data-ttu-id="5a04e-130">Добавление Интерналспонсорс</span><span class="sxs-lookup"><span data-stu-id="5a04e-130">Add internalSponsors</span></span>](../api/connectedorganization-post-internalsponsors.md) | <span data-ttu-id="5a04e-131">Нет</span><span class="sxs-lookup"><span data-stu-id="5a04e-131">None</span></span> | <span data-ttu-id="5a04e-132">Добавление пользователя или группы в внутренние спонсоры Коннектедорганизатион.</span><span class="sxs-lookup"><span data-stu-id="5a04e-132">Add a user or group to a connectedOrganization's internal sponsors.</span></span> |
|[<span data-ttu-id="5a04e-133">Добавление Екстерналспонсорс</span><span class="sxs-lookup"><span data-stu-id="5a04e-133">Add externalSponsors</span></span>](../api/connectedorganization-post-externalsponsors.md) | <span data-ttu-id="5a04e-134">Нет</span><span class="sxs-lookup"><span data-stu-id="5a04e-134">None</span></span> | <span data-ttu-id="5a04e-135">Добавление пользователя или группы во внешние спонсоры Коннектедорганизатион.</span><span class="sxs-lookup"><span data-stu-id="5a04e-135">Add a user or group to a connectedOrganization's external sponsors.</span></span> |
|[<span data-ttu-id="5a04e-136">Удаление Интерналспонсорс</span><span class="sxs-lookup"><span data-stu-id="5a04e-136">Remove internalSponsors</span></span>](../api/connectedorganization-delete-internalsponsors.md) | <span data-ttu-id="5a04e-137">Нет</span><span class="sxs-lookup"><span data-stu-id="5a04e-137">None</span></span> | <span data-ttu-id="5a04e-138">Удаление пользователя или группы из внутренних спонсоров Коннектедорганизатион.</span><span class="sxs-lookup"><span data-stu-id="5a04e-138">Remove a user or group from a connectedOrganization's internal sponsors.</span></span> |
|[<span data-ttu-id="5a04e-139">Удаление Екстерналспонсорс</span><span class="sxs-lookup"><span data-stu-id="5a04e-139">Remove externalSponsors</span></span>](../api/connectedorganization-delete-externalsponsors.md) | <span data-ttu-id="5a04e-140">Нет</span><span class="sxs-lookup"><span data-stu-id="5a04e-140">None</span></span> | <span data-ttu-id="5a04e-141">Удаление пользователя или группы из внешних спонсоров Коннектедорганизатион.</span><span class="sxs-lookup"><span data-stu-id="5a04e-141">Remove a user or group from a connectedOrganization's external sponsors.</span></span> |

## <a name="properties"></a><span data-ttu-id="5a04e-142">Свойства</span><span class="sxs-lookup"><span data-stu-id="5a04e-142">Properties</span></span>

|<span data-ttu-id="5a04e-143">Свойство</span><span class="sxs-lookup"><span data-stu-id="5a04e-143">Property</span></span>|<span data-ttu-id="5a04e-144">Тип</span><span class="sxs-lookup"><span data-stu-id="5a04e-144">Type</span></span>|<span data-ttu-id="5a04e-145">Описание</span><span class="sxs-lookup"><span data-stu-id="5a04e-145">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5a04e-146">createdBy</span><span class="sxs-lookup"><span data-stu-id="5a04e-146">createdBy</span></span>|<span data-ttu-id="5a04e-147">String</span><span class="sxs-lookup"><span data-stu-id="5a04e-147">String</span></span>|<span data-ttu-id="5a04e-148">Имя участника-пользователя, создавшего этот ресурс.</span><span class="sxs-lookup"><span data-stu-id="5a04e-148">UPN of the user who created this resource.</span></span> <span data-ttu-id="5a04e-149">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5a04e-149">Read-only.</span></span>|
|<span data-ttu-id="5a04e-150">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5a04e-150">createdDateTime</span></span>|<span data-ttu-id="5a04e-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5a04e-151">DateTimeOffset</span></span>|<span data-ttu-id="5a04e-152">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="5a04e-152">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="5a04e-153">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="5a04e-153">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="5a04e-154">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5a04e-154">Read-only.</span></span>|
|<span data-ttu-id="5a04e-155">description</span><span class="sxs-lookup"><span data-stu-id="5a04e-155">description</span></span>|<span data-ttu-id="5a04e-156">String</span><span class="sxs-lookup"><span data-stu-id="5a04e-156">String</span></span>|<span data-ttu-id="5a04e-157">Описание подключенной Организации.</span><span class="sxs-lookup"><span data-stu-id="5a04e-157">The description of the connected organization.</span></span>|
|<span data-ttu-id="5a04e-158">displayName</span><span class="sxs-lookup"><span data-stu-id="5a04e-158">displayName</span></span>|<span data-ttu-id="5a04e-159">String</span><span class="sxs-lookup"><span data-stu-id="5a04e-159">String</span></span>|<span data-ttu-id="5a04e-160">Отображаемое имя подключенной Организации.</span><span class="sxs-lookup"><span data-stu-id="5a04e-160">The display name of the connected organization.</span></span>|
|<span data-ttu-id="5a04e-161">id</span><span class="sxs-lookup"><span data-stu-id="5a04e-161">id</span></span>|<span data-ttu-id="5a04e-162">String</span><span class="sxs-lookup"><span data-stu-id="5a04e-162">String</span></span>| <span data-ttu-id="5a04e-163">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5a04e-163">Read-only.</span></span>|
|<span data-ttu-id="5a04e-164">модифиедби</span><span class="sxs-lookup"><span data-stu-id="5a04e-164">modifiedBy</span></span>|<span data-ttu-id="5a04e-165">String</span><span class="sxs-lookup"><span data-stu-id="5a04e-165">String</span></span>|<span data-ttu-id="5a04e-166">Имя участника-пользователя, который последним изменил этот ресурс.</span><span class="sxs-lookup"><span data-stu-id="5a04e-166">UPN of the user who last modified this resource.</span></span> <span data-ttu-id="5a04e-167">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5a04e-167">Read-only.</span></span>|
|<span data-ttu-id="5a04e-168">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5a04e-168">modifiedDateTime</span></span>|<span data-ttu-id="5a04e-169">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5a04e-169">DateTimeOffset</span></span>|<span data-ttu-id="5a04e-170">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="5a04e-170">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="5a04e-171">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="5a04e-171">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="5a04e-172">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5a04e-172">Read-only.</span></span>|
|<span data-ttu-id="5a04e-173">state</span><span class="sxs-lookup"><span data-stu-id="5a04e-173">state</span></span>|<span data-ttu-id="5a04e-174">коннектедорганизатионстате</span><span class="sxs-lookup"><span data-stu-id="5a04e-174">connectedOrganizationState</span></span>|<span data-ttu-id="5a04e-175">Состояние подключенной Организации определяет, применимы ли политики назначения с типом области запрашивающего `AllConfiguredConnectedOrganizationSubjects` .</span><span class="sxs-lookup"><span data-stu-id="5a04e-175">The state of a connected organization defines whether assignment policies with requestor scope type `AllConfiguredConnectedOrganizationSubjects` are applicable or not.</span></span> <span data-ttu-id="5a04e-176">Возможные значения: `configured`, `proposed`.</span><span class="sxs-lookup"><span data-stu-id="5a04e-176">Possible values are: `configured`, `proposed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5a04e-177">Отношения</span><span class="sxs-lookup"><span data-stu-id="5a04e-177">Relationships</span></span>

|<span data-ttu-id="5a04e-178">Связь</span><span class="sxs-lookup"><span data-stu-id="5a04e-178">Relationship</span></span>|<span data-ttu-id="5a04e-179">Тип</span><span class="sxs-lookup"><span data-stu-id="5a04e-179">Type</span></span>|<span data-ttu-id="5a04e-180">Описание</span><span class="sxs-lookup"><span data-stu-id="5a04e-180">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5a04e-181">идентитисаурцес</span><span class="sxs-lookup"><span data-stu-id="5a04e-181">identitySources</span></span>|<span data-ttu-id="5a04e-182">Коллекция [идентитисаурце](identitySource.md)</span><span class="sxs-lookup"><span data-stu-id="5a04e-182">[identitySource](identitySource.md) collection</span></span>| <span data-ttu-id="5a04e-183">Источники удостоверений в этой подключенной Организации, один из [азуреактиведиректоритенант](azureactivedirectorytenant.md), [домаинидентитисаурце](domainidentitysource.md) или [екстерналдомаинфедератион](externaldomainfederation.md).</span><span class="sxs-lookup"><span data-stu-id="5a04e-183">The identity sources in this connected organization, one of [azureActiveDirectoryTenant](azureactivedirectorytenant.md), [domainIdentitySource](domainidentitysource.md) or [externalDomainFederation](externaldomainfederation.md).</span></span> <span data-ttu-id="5a04e-184">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5a04e-184">Read-only.</span></span> <span data-ttu-id="5a04e-185">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="5a04e-185">Nullable.</span></span>|
|<span data-ttu-id="5a04e-186">интерналспонсорс</span><span class="sxs-lookup"><span data-stu-id="5a04e-186">internalSponsors</span></span>| <span data-ttu-id="5a04e-187">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="5a04e-187">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="5a04e-188">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="5a04e-188">Nullable.</span></span>|
|<span data-ttu-id="5a04e-189">екстерналспонсорс</span><span class="sxs-lookup"><span data-stu-id="5a04e-189">externalSponsors</span></span>| <span data-ttu-id="5a04e-190">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="5a04e-190">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="5a04e-191">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="5a04e-191">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5a04e-192">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5a04e-192">JSON representation</span></span>

<span data-ttu-id="5a04e-193">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5a04e-193">The following is a JSON representation of the resource.</span></span>

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

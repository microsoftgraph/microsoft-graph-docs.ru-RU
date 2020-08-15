---
title: Тип ресурса Коннектедорганизатион
description: В управлении службой управления правами Azure AD подключенная организация является ссылкой на каталог или домен другой организации, чьи пользователи могут запрашивать доступ.
author: markwahl-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 5356a48aae90f22fdd54a54ed5fe7132598b9d42
ms.sourcegitcommit: da4f3d03e98ee5fa13f8c7a263d931e68a20a12c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/15/2020
ms.locfileid: "46757295"
---
# <a name="connectedorganization-resource-type"></a><span data-ttu-id="232da-103">Тип ресурса Коннектедорганизатион</span><span class="sxs-lookup"><span data-stu-id="232da-103">connectedOrganization resource type</span></span>

<span data-ttu-id="232da-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="232da-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="232da-105">В [управлении службой управления правами Azure AD](entitlementmanagement-root.md)подключенная организация является ссылкой на каталог или домен другой организации, чьи пользователи могут запрашивать доступ.</span><span class="sxs-lookup"><span data-stu-id="232da-105">In [Azure AD entitlement management](entitlementmanagement-root.md), a connected organization is a reference to a directory or domain of another organization whose users can request access.</span></span>

## <a name="methods"></a><span data-ttu-id="232da-106">Методы</span><span class="sxs-lookup"><span data-stu-id="232da-106">Methods</span></span>

|<span data-ttu-id="232da-107">Метод</span><span class="sxs-lookup"><span data-stu-id="232da-107">Method</span></span>|<span data-ttu-id="232da-108">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="232da-108">Return type</span></span>|<span data-ttu-id="232da-109">Описание</span><span class="sxs-lookup"><span data-stu-id="232da-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="232da-110">Список Коннектедорганизатионс</span><span class="sxs-lookup"><span data-stu-id="232da-110">List connectedOrganizations</span></span>](../api/connectedorganization-list.md) | <span data-ttu-id="232da-111">Коллекция [коннектедорганизатион](connectedorganization.md)</span><span class="sxs-lookup"><span data-stu-id="232da-111">[connectedOrganization](connectedorganization.md) collection</span></span> | <span data-ttu-id="232da-112">Получение списка объектов Коннектедорганизатион.</span><span class="sxs-lookup"><span data-stu-id="232da-112">Retrieve a list of connectedOrganization objects.</span></span> |
|[<span data-ttu-id="232da-113">Создание Коннектедорганизатион</span><span class="sxs-lookup"><span data-stu-id="232da-113">Create connectedOrganization</span></span>](../api/connectedorganization-post.md) | [<span data-ttu-id="232da-114">коннектедорганизатион</span><span class="sxs-lookup"><span data-stu-id="232da-114">connectedOrganization</span></span>](connectedorganization.md) | <span data-ttu-id="232da-115">Создание нового объекта Коннектедорганизатион.</span><span class="sxs-lookup"><span data-stu-id="232da-115">Create a new connectedOrganization object.</span></span> |
|[<span data-ttu-id="232da-116">Получение Коннектедорганизатион</span><span class="sxs-lookup"><span data-stu-id="232da-116">Get connectedOrganization</span></span>](../api/connectedorganization-get.md) | [<span data-ttu-id="232da-117">коннектедорганизатион</span><span class="sxs-lookup"><span data-stu-id="232da-117">connectedOrganization</span></span>](connectedorganization.md) | <span data-ttu-id="232da-118">Чтение свойств и связей объекта Коннектедорганизатион.</span><span class="sxs-lookup"><span data-stu-id="232da-118">Read properties and relationships of a connectedOrganization object.</span></span> |
|[<span data-ttu-id="232da-119">Обновление Коннектедорганизатион</span><span class="sxs-lookup"><span data-stu-id="232da-119">Update connectedOrganization</span></span>](../api/connectedorganization-update.md) | | <span data-ttu-id="232da-120">Обновление Коннектедорганизатион.</span><span class="sxs-lookup"><span data-stu-id="232da-120">Update a connectedOrganization.</span></span> |
|[<span data-ttu-id="232da-121">Удаление Коннектедорганизатион</span><span class="sxs-lookup"><span data-stu-id="232da-121">Delete connectedOrganization</span></span>](../api/connectedorganization-delete.md) |<span data-ttu-id="232da-122">Нет</span><span class="sxs-lookup"><span data-stu-id="232da-122">None</span></span> | <span data-ttu-id="232da-123">Удаление объекта Коннектедорганизатион.</span><span class="sxs-lookup"><span data-stu-id="232da-123">Delete a connectedOrganization.</span></span> |
|[<span data-ttu-id="232da-124">Список Интерналспонсорс</span><span class="sxs-lookup"><span data-stu-id="232da-124">List internalSponsors</span></span>](../api/connectedorganization-list-internalsponsors.md) | <span data-ttu-id="232da-125">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="232da-125">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="232da-126">Получение списка внутренних спонсоров Коннектедорганизатион.</span><span class="sxs-lookup"><span data-stu-id="232da-126">Retrieve a list of a connectedOrganization's internal sponsors.</span></span> |
|[<span data-ttu-id="232da-127">Список Екстерналспонсорс</span><span class="sxs-lookup"><span data-stu-id="232da-127">List externalSponsors</span></span>](../api/connectedorganization-list-externalsponsors.md) | <span data-ttu-id="232da-128">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="232da-128">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="232da-129">Получение списка внешних спонсоров Коннектедорганизатион.</span><span class="sxs-lookup"><span data-stu-id="232da-129">Retrieve a list of a connectedOrganization's external sponsors.</span></span> |
|[<span data-ttu-id="232da-130">Добавление Интерналспонсорс</span><span class="sxs-lookup"><span data-stu-id="232da-130">Add internalSponsors</span></span>](../api/connectedorganization-post-internalsponsors.md) | <span data-ttu-id="232da-131">Нет</span><span class="sxs-lookup"><span data-stu-id="232da-131">None</span></span> | <span data-ttu-id="232da-132">Добавление пользователя или группы в внутренние спонсоры Коннектедорганизатион.</span><span class="sxs-lookup"><span data-stu-id="232da-132">Add a user or group to a connectedOrganization's internal sponsors.</span></span> |
|[<span data-ttu-id="232da-133">Добавление Екстерналспонсорс</span><span class="sxs-lookup"><span data-stu-id="232da-133">Add externalSponsors</span></span>](../api/connectedorganization-post-externalsponsors.md) | <span data-ttu-id="232da-134">Нет</span><span class="sxs-lookup"><span data-stu-id="232da-134">None</span></span> | <span data-ttu-id="232da-135">Добавление пользователя или группы во внешние спонсоры Коннектедорганизатион.</span><span class="sxs-lookup"><span data-stu-id="232da-135">Add a user or group to a connectedOrganization's external sponsors.</span></span> |
|[<span data-ttu-id="232da-136">Удаление Интерналспонсорс</span><span class="sxs-lookup"><span data-stu-id="232da-136">Remove internalSponsors</span></span>](../api/connectedorganization-delete-internalsponsors.md) | <span data-ttu-id="232da-137">Нет</span><span class="sxs-lookup"><span data-stu-id="232da-137">None</span></span> | <span data-ttu-id="232da-138">Удаление пользователя или группы из внутренних спонсоров Коннектедорганизатион.</span><span class="sxs-lookup"><span data-stu-id="232da-138">Remove a user or group from a connectedOrganization's internal sponsors.</span></span> |
|[<span data-ttu-id="232da-139">Удаление Екстерналспонсорс</span><span class="sxs-lookup"><span data-stu-id="232da-139">Remove externalSponsors</span></span>](../api/connectedorganization-delete-externalsponsors.md) | <span data-ttu-id="232da-140">Нет</span><span class="sxs-lookup"><span data-stu-id="232da-140">None</span></span> | <span data-ttu-id="232da-141">Удаление пользователя или группы из внешних спонсоров Коннектедорганизатион.</span><span class="sxs-lookup"><span data-stu-id="232da-141">Remove a user or group from a connectedOrganization's external sponsors.</span></span> |

## <a name="properties"></a><span data-ttu-id="232da-142">Свойства</span><span class="sxs-lookup"><span data-stu-id="232da-142">Properties</span></span>

|<span data-ttu-id="232da-143">Свойство</span><span class="sxs-lookup"><span data-stu-id="232da-143">Property</span></span>|<span data-ttu-id="232da-144">Тип</span><span class="sxs-lookup"><span data-stu-id="232da-144">Type</span></span>|<span data-ttu-id="232da-145">Описание</span><span class="sxs-lookup"><span data-stu-id="232da-145">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="232da-146">createdBy</span><span class="sxs-lookup"><span data-stu-id="232da-146">createdBy</span></span>|<span data-ttu-id="232da-147">Строка</span><span class="sxs-lookup"><span data-stu-id="232da-147">String</span></span>|<span data-ttu-id="232da-148">Имя участника-пользователя, создавшего этот ресурс.</span><span class="sxs-lookup"><span data-stu-id="232da-148">UPN of the user who created this resource.</span></span> <span data-ttu-id="232da-149">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="232da-149">Read-only.</span></span>|
|<span data-ttu-id="232da-150">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="232da-150">createdDateTime</span></span>|<span data-ttu-id="232da-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="232da-151">DateTimeOffset</span></span>|<span data-ttu-id="232da-152">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="232da-152">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="232da-153">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="232da-153">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="232da-154">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="232da-154">Read-only.</span></span>|
|<span data-ttu-id="232da-155">description</span><span class="sxs-lookup"><span data-stu-id="232da-155">description</span></span>|<span data-ttu-id="232da-156">String</span><span class="sxs-lookup"><span data-stu-id="232da-156">String</span></span>|<span data-ttu-id="232da-157">Описание подключенной Организации.</span><span class="sxs-lookup"><span data-stu-id="232da-157">The description of the connected organization.</span></span>|
|<span data-ttu-id="232da-158">displayName</span><span class="sxs-lookup"><span data-stu-id="232da-158">displayName</span></span>|<span data-ttu-id="232da-159">Строка</span><span class="sxs-lookup"><span data-stu-id="232da-159">String</span></span>|<span data-ttu-id="232da-160">Отображаемое имя подключенной Организации.</span><span class="sxs-lookup"><span data-stu-id="232da-160">The display name of the connected organization.</span></span>|
|<span data-ttu-id="232da-161">id</span><span class="sxs-lookup"><span data-stu-id="232da-161">id</span></span>|<span data-ttu-id="232da-162">String</span><span class="sxs-lookup"><span data-stu-id="232da-162">String</span></span>| <span data-ttu-id="232da-163">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="232da-163">Read-only.</span></span>|
|<span data-ttu-id="232da-164">модифиедби</span><span class="sxs-lookup"><span data-stu-id="232da-164">modifiedBy</span></span>|<span data-ttu-id="232da-165">Строка</span><span class="sxs-lookup"><span data-stu-id="232da-165">String</span></span>|<span data-ttu-id="232da-166">Имя участника-пользователя, который последним изменил этот ресурс.</span><span class="sxs-lookup"><span data-stu-id="232da-166">UPN of the user who last modified this resource.</span></span> <span data-ttu-id="232da-167">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="232da-167">Read-only.</span></span>|
|<span data-ttu-id="232da-168">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="232da-168">modifiedDateTime</span></span>|<span data-ttu-id="232da-169">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="232da-169">DateTimeOffset</span></span>|<span data-ttu-id="232da-170">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="232da-170">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="232da-171">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="232da-171">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="232da-172">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="232da-172">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="232da-173">Отношения</span><span class="sxs-lookup"><span data-stu-id="232da-173">Relationships</span></span>

|<span data-ttu-id="232da-174">Связь</span><span class="sxs-lookup"><span data-stu-id="232da-174">Relationship</span></span>|<span data-ttu-id="232da-175">Тип</span><span class="sxs-lookup"><span data-stu-id="232da-175">Type</span></span>|<span data-ttu-id="232da-176">Описание</span><span class="sxs-lookup"><span data-stu-id="232da-176">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="232da-177">идентитисаурцес</span><span class="sxs-lookup"><span data-stu-id="232da-177">identitySources</span></span>|<span data-ttu-id="232da-178">Коллекция [идентитисаурце](identitySource.md)</span><span class="sxs-lookup"><span data-stu-id="232da-178">[identitySource](identitySource.md) collection</span></span>| <span data-ttu-id="232da-179">Источники удостоверений в этой подключенной Организации, один из [азуреактиведиректоритенант](azureactivedirectorytenant.md), [домаинидентитисаурце](domainidentitysource.md) или [екстерналдомаинфедератион](externaldomainfederation.md).</span><span class="sxs-lookup"><span data-stu-id="232da-179">The identity sources in this connected organization, one of [azureActiveDirectoryTenant](azureactivedirectorytenant.md), [domainIdentitySource](domainidentitysource.md) or [externalDomainFederation](externaldomainfederation.md).</span></span> <span data-ttu-id="232da-180">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="232da-180">Read-only.</span></span> <span data-ttu-id="232da-181">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="232da-181">Nullable.</span></span>|
|<span data-ttu-id="232da-182">интерналспонсорс</span><span class="sxs-lookup"><span data-stu-id="232da-182">internalSponsors</span></span>| <span data-ttu-id="232da-183">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="232da-183">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="232da-184">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="232da-184">Nullable.</span></span>|
|<span data-ttu-id="232da-185">екстерналспонсорс</span><span class="sxs-lookup"><span data-stu-id="232da-185">externalSponsors</span></span>| <span data-ttu-id="232da-186">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="232da-186">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="232da-187">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="232da-187">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="232da-188">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="232da-188">JSON representation</span></span>

<span data-ttu-id="232da-189">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="232da-189">The following is a JSON representation of the resource.</span></span>

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
  ]
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

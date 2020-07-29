---
title: Тип ресурса Коннектедорганизатион
description: В управлении службой управления правами Azure AD подключенная организация является ссылкой на каталог или домен другой организации, чьи пользователи могут запрашивать доступ.
author: markwahl-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: cb82ac88f1f81bf7d2f3238657818d0782ed6b60
ms.sourcegitcommit: 9faca60f0cc4ee9d6dce33fd25c72e14b5487d34
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/29/2020
ms.locfileid: "46510364"
---
# <a name="connectedorganization-resource-type"></a><span data-ttu-id="3c140-103">Тип ресурса Коннектедорганизатион</span><span class="sxs-lookup"><span data-stu-id="3c140-103">connectedOrganization resource type</span></span>

<span data-ttu-id="3c140-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3c140-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3c140-105">В [управлении службой управления правами Azure AD](entitlementmanagement-root.md)подключенная организация является ссылкой на каталог или домен другой организации, чьи пользователи могут запрашивать доступ.</span><span class="sxs-lookup"><span data-stu-id="3c140-105">In [Azure AD entitlement management](entitlementmanagement-root.md), a connected organization is a reference to a directory or domain of another organization whose users can request access.</span></span>

## <a name="methods"></a><span data-ttu-id="3c140-106">Методы</span><span class="sxs-lookup"><span data-stu-id="3c140-106">Methods</span></span>

|<span data-ttu-id="3c140-107">Метод</span><span class="sxs-lookup"><span data-stu-id="3c140-107">Method</span></span>|<span data-ttu-id="3c140-108">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="3c140-108">Return type</span></span>|<span data-ttu-id="3c140-109">Описание</span><span class="sxs-lookup"><span data-stu-id="3c140-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="3c140-110">Список Коннектедорганизатионс</span><span class="sxs-lookup"><span data-stu-id="3c140-110">List connectedOrganizations</span></span>](../api/connectedorganization-list.md) | <span data-ttu-id="3c140-111">Коллекция [коннектедорганизатион](connectedorganization.md)</span><span class="sxs-lookup"><span data-stu-id="3c140-111">[connectedOrganization](connectedorganization.md) collection</span></span> | <span data-ttu-id="3c140-112">Получение списка объектов Коннектедорганизатион.</span><span class="sxs-lookup"><span data-stu-id="3c140-112">Retrieve a list of connectedOrganization objects.</span></span> |
|[<span data-ttu-id="3c140-113">Создание Коннектедорганизатион</span><span class="sxs-lookup"><span data-stu-id="3c140-113">Create connectedOrganization</span></span>](../api/connectedorganization-post.md) | [<span data-ttu-id="3c140-114">коннектедорганизатион</span><span class="sxs-lookup"><span data-stu-id="3c140-114">connectedOrganization</span></span>](connectedorganization.md) | <span data-ttu-id="3c140-115">Создание нового объекта Коннектедорганизатион.</span><span class="sxs-lookup"><span data-stu-id="3c140-115">Create a new connectedOrganization object.</span></span> |
|[<span data-ttu-id="3c140-116">Получение Коннектедорганизатион</span><span class="sxs-lookup"><span data-stu-id="3c140-116">Get connectedOrganization</span></span>](../api/connectedorganization-get.md) | [<span data-ttu-id="3c140-117">коннектедорганизатион</span><span class="sxs-lookup"><span data-stu-id="3c140-117">connectedOrganization</span></span>](connectedorganization.md) | <span data-ttu-id="3c140-118">Чтение свойств и связей объекта Коннектедорганизатион.</span><span class="sxs-lookup"><span data-stu-id="3c140-118">Read properties and relationships of a connectedOrganization object.</span></span> |
|[<span data-ttu-id="3c140-119">Обновление Коннектедорганизатион</span><span class="sxs-lookup"><span data-stu-id="3c140-119">Update connectedOrganization</span></span>](../api/connectedorganization-update.md) | | <span data-ttu-id="3c140-120">Обновление Коннектедорганизатион.</span><span class="sxs-lookup"><span data-stu-id="3c140-120">Update a connectedOrganization.</span></span> |
|[<span data-ttu-id="3c140-121">Удаление Коннектедорганизатион</span><span class="sxs-lookup"><span data-stu-id="3c140-121">Delete connectedOrganization</span></span>](../api/connectedorganization-delete.md) |<span data-ttu-id="3c140-122">Нет</span><span class="sxs-lookup"><span data-stu-id="3c140-122">None</span></span> | <span data-ttu-id="3c140-123">Удаление объекта Коннектедорганизатион.</span><span class="sxs-lookup"><span data-stu-id="3c140-123">Delete a connectedOrganization.</span></span> |

## <a name="properties"></a><span data-ttu-id="3c140-124">Свойства</span><span class="sxs-lookup"><span data-stu-id="3c140-124">Properties</span></span>

|<span data-ttu-id="3c140-125">Свойство</span><span class="sxs-lookup"><span data-stu-id="3c140-125">Property</span></span>|<span data-ttu-id="3c140-126">Тип</span><span class="sxs-lookup"><span data-stu-id="3c140-126">Type</span></span>|<span data-ttu-id="3c140-127">Описание</span><span class="sxs-lookup"><span data-stu-id="3c140-127">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3c140-128">createdBy</span><span class="sxs-lookup"><span data-stu-id="3c140-128">createdBy</span></span>|<span data-ttu-id="3c140-129">Строка</span><span class="sxs-lookup"><span data-stu-id="3c140-129">String</span></span>|<span data-ttu-id="3c140-130">Имя участника-пользователя, создавшего этот ресурс.</span><span class="sxs-lookup"><span data-stu-id="3c140-130">UPN of the user who created this resource.</span></span> <span data-ttu-id="3c140-131">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3c140-131">Read-only.</span></span>|
|<span data-ttu-id="3c140-132">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3c140-132">createdDateTime</span></span>|<span data-ttu-id="3c140-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3c140-133">DateTimeOffset</span></span>|<span data-ttu-id="3c140-134">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="3c140-134">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="3c140-135">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="3c140-135">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="3c140-136">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3c140-136">Read-only.</span></span>|
|<span data-ttu-id="3c140-137">description</span><span class="sxs-lookup"><span data-stu-id="3c140-137">description</span></span>|<span data-ttu-id="3c140-138">String</span><span class="sxs-lookup"><span data-stu-id="3c140-138">String</span></span>|<span data-ttu-id="3c140-139">Описание подключенной Организации.</span><span class="sxs-lookup"><span data-stu-id="3c140-139">The description of the connected organization.</span></span>|
|<span data-ttu-id="3c140-140">displayName</span><span class="sxs-lookup"><span data-stu-id="3c140-140">displayName</span></span>|<span data-ttu-id="3c140-141">Строка</span><span class="sxs-lookup"><span data-stu-id="3c140-141">String</span></span>|<span data-ttu-id="3c140-142">Отображаемое имя подключенной Организации.</span><span class="sxs-lookup"><span data-stu-id="3c140-142">The display name of the connected organization.</span></span>|
|<span data-ttu-id="3c140-143">id</span><span class="sxs-lookup"><span data-stu-id="3c140-143">id</span></span>|<span data-ttu-id="3c140-144">String</span><span class="sxs-lookup"><span data-stu-id="3c140-144">String</span></span>| <span data-ttu-id="3c140-145">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3c140-145">Read-only.</span></span>|
|<span data-ttu-id="3c140-146">модифиедби</span><span class="sxs-lookup"><span data-stu-id="3c140-146">modifiedBy</span></span>|<span data-ttu-id="3c140-147">Строка</span><span class="sxs-lookup"><span data-stu-id="3c140-147">String</span></span>|<span data-ttu-id="3c140-148">Имя участника-пользователя, который последним изменил этот ресурс.</span><span class="sxs-lookup"><span data-stu-id="3c140-148">UPN of the user who last modified this resource.</span></span> <span data-ttu-id="3c140-149">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3c140-149">Read-only.</span></span>|
|<span data-ttu-id="3c140-150">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3c140-150">modifiedDateTime</span></span>|<span data-ttu-id="3c140-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3c140-151">DateTimeOffset</span></span>|<span data-ttu-id="3c140-152">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="3c140-152">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="3c140-153">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="3c140-153">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="3c140-154">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3c140-154">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3c140-155">Отношения</span><span class="sxs-lookup"><span data-stu-id="3c140-155">Relationships</span></span>

|<span data-ttu-id="3c140-156">Связь</span><span class="sxs-lookup"><span data-stu-id="3c140-156">Relationship</span></span>|<span data-ttu-id="3c140-157">Тип</span><span class="sxs-lookup"><span data-stu-id="3c140-157">Type</span></span>|<span data-ttu-id="3c140-158">Описание</span><span class="sxs-lookup"><span data-stu-id="3c140-158">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3c140-159">идентитисаурцес</span><span class="sxs-lookup"><span data-stu-id="3c140-159">identitySources</span></span>|<span data-ttu-id="3c140-160">Коллекция [идентитисаурце](identitySource.md)</span><span class="sxs-lookup"><span data-stu-id="3c140-160">[identitySource](identitySource.md) collection</span></span>| <span data-ttu-id="3c140-161">Источники удостоверений в этой подключенной Организации, один из [азуреактиведиректоритенант](azureactivedirectorytenant.md), [домаинидентитисаурце](domainidentitysource.md) или [екстерналдомаинфедератион](externaldomainfederation.md).</span><span class="sxs-lookup"><span data-stu-id="3c140-161">The identity sources in this connected organization, one of [azureActiveDirectoryTenant](azureactivedirectorytenant.md), [domainIdentitySource](domainidentitysource.md) or [externalDomainFederation](externaldomainfederation.md).</span></span> <span data-ttu-id="3c140-162">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3c140-162">Read-only.</span></span> <span data-ttu-id="3c140-163">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="3c140-163">Nullable.</span></span>|
|<span data-ttu-id="3c140-164">интерналспонсорс</span><span class="sxs-lookup"><span data-stu-id="3c140-164">internalSponsors</span></span>| <span data-ttu-id="3c140-165">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="3c140-165">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="3c140-166">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="3c140-166">Nullable.</span></span>|
|<span data-ttu-id="3c140-167">екстерналспонсорс</span><span class="sxs-lookup"><span data-stu-id="3c140-167">externalSponsors</span></span>| <span data-ttu-id="3c140-168">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="3c140-168">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="3c140-169">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="3c140-169">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3c140-170">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3c140-170">JSON representation</span></span>

<span data-ttu-id="3c140-171">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3c140-171">The following is a JSON representation of the resource.</span></span>

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

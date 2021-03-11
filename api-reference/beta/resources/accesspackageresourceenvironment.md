---
title: тип ресурса accessPackageResourceEnvironment
description: Среда ресурсов пакета доступа является ссылкой на среду геолокации, в которой находится ресурс.
author: hanki-microsoft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 09bd318036874bb52bfab0ed522a2948cbe83233
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50722202"
---
# <a name="accesspackageresourceenvironment-resource-type"></a><span data-ttu-id="3c368-103">тип ресурса accessPackageResourceEnvironment</span><span class="sxs-lookup"><span data-stu-id="3c368-103">accessPackageResourceEnvironment resource type</span></span>

<span data-ttu-id="3c368-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3c368-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3c368-105">В [Azure AD Entitlement Management](entitlementmanagement-root.md)среда ресурсов пакета доступа является ссылкой на среду геолокации, в которой находится ресурс.</span><span class="sxs-lookup"><span data-stu-id="3c368-105">In [Azure AD Entitlement Management](entitlementmanagement-root.md), an access package resource environment is a reference to the geolocation environment in which a resource is located.</span></span> <span data-ttu-id="3c368-106">Эта среда автоматически предоставляется в рамках управления правами Azure AD.</span><span class="sxs-lookup"><span data-stu-id="3c368-106">This environment is automatically provided as part of Azure AD Entitlement Management.</span></span> <span data-ttu-id="3c368-107">API применим только к сайтам Multi-Geo SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="3c368-107">The API is only applicable to Multi-Geo SharePoint Online sites.</span></span>

## <a name="methods"></a><span data-ttu-id="3c368-108">Методы</span><span class="sxs-lookup"><span data-stu-id="3c368-108">Methods</span></span>
|<span data-ttu-id="3c368-109">Метод</span><span class="sxs-lookup"><span data-stu-id="3c368-109">Method</span></span>|<span data-ttu-id="3c368-110">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="3c368-110">Return type</span></span>|<span data-ttu-id="3c368-111">Описание</span><span class="sxs-lookup"><span data-stu-id="3c368-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="3c368-112">Список accessPackageResourceEnvironments</span><span class="sxs-lookup"><span data-stu-id="3c368-112">List accessPackageResourceEnvironments</span></span>](../api/accesspackageresourceenvironment-list.md)|<span data-ttu-id="3c368-113">[accessPackageResourceEnvironment](../resources/accesspackageresourceenvironment.md) collection</span><span class="sxs-lookup"><span data-stu-id="3c368-113">[accessPackageResourceEnvironment](../resources/accesspackageresourceenvironment.md) collection</span></span>|<span data-ttu-id="3c368-114">Извлечение списка [объектов accessPackageResourceEnvironment.](../resources/accesspackageresourceenvironment.md)</span><span class="sxs-lookup"><span data-stu-id="3c368-114">Retrieve a list of [accessPackageResourceEnvironment](../resources/accesspackageresourceenvironment.md) objects.</span></span>|
|[<span data-ttu-id="3c368-115">Получите accessPackageResourceEnvironment</span><span class="sxs-lookup"><span data-stu-id="3c368-115">Get accessPackageResourceEnvironment</span></span>](../api/accesspackageresourceenvironment-get.md)|[<span data-ttu-id="3c368-116">accessPackageResourceEnvironment</span><span class="sxs-lookup"><span data-stu-id="3c368-116">accessPackageResourceEnvironment</span></span>](../resources/accesspackageresourceenvironment.md)|<span data-ttu-id="3c368-117">Ознакомьтесь с свойствами и отношениями объекта [accessPackageResourceEnvironment.](../resources/accesspackageresourceenvironment.md)</span><span class="sxs-lookup"><span data-stu-id="3c368-117">Read the properties and relationships of an [accessPackageResourceEnvironment](../resources/accesspackageresourceenvironment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="3c368-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="3c368-118">Properties</span></span>
|<span data-ttu-id="3c368-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="3c368-119">Property</span></span>|<span data-ttu-id="3c368-120">Тип</span><span class="sxs-lookup"><span data-stu-id="3c368-120">Type</span></span>|<span data-ttu-id="3c368-121">Описание</span><span class="sxs-lookup"><span data-stu-id="3c368-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3c368-122">connectionInfo</span><span class="sxs-lookup"><span data-stu-id="3c368-122">connectionInfo</span></span>|[<span data-ttu-id="3c368-123">connectionInfo</span><span class="sxs-lookup"><span data-stu-id="3c368-123">connectionInfo</span></span>](../resources/connectioninfo.md)|<span data-ttu-id="3c368-124">Сведения о подключении среды, используемой для подключения к ресурсу.</span><span class="sxs-lookup"><span data-stu-id="3c368-124">Connection information of an environment used to connect to a resource.</span></span> |
|<span data-ttu-id="3c368-125">createdBy</span><span class="sxs-lookup"><span data-stu-id="3c368-125">createdBy</span></span>|<span data-ttu-id="3c368-126">String</span><span class="sxs-lookup"><span data-stu-id="3c368-126">String</span></span>|<span data-ttu-id="3c368-127">Отображает имя пользователя, создав этот объект.</span><span class="sxs-lookup"><span data-stu-id="3c368-127">The display name of the user that created this object.</span></span>|
|<span data-ttu-id="3c368-128">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3c368-128">createdDateTime</span></span>|<span data-ttu-id="3c368-129">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3c368-129">DateTimeOffset</span></span>|<span data-ttu-id="3c368-130">Дата и время создания этого объекта.</span><span class="sxs-lookup"><span data-stu-id="3c368-130">The date and time that this object was created.</span></span> <br><span data-ttu-id="3c368-131">Тип DateTimeOffset представляет сведения о дате и времени с использованием формата ISO 8601 и всегда указывает время в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="3c368-131">The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="3c368-132">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="3c368-132">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span>|
|<span data-ttu-id="3c368-133">description</span><span class="sxs-lookup"><span data-stu-id="3c368-133">description</span></span>|<span data-ttu-id="3c368-134">String</span><span class="sxs-lookup"><span data-stu-id="3c368-134">String</span></span>|<span data-ttu-id="3c368-135">Описание этого *объекта accessPackageResourceEnvironment.*</span><span class="sxs-lookup"><span data-stu-id="3c368-135">The description of this *accessPackageResourceEnvironment* object.</span></span>|
|<span data-ttu-id="3c368-136">displayName</span><span class="sxs-lookup"><span data-stu-id="3c368-136">displayName</span></span>|<span data-ttu-id="3c368-137">String</span><span class="sxs-lookup"><span data-stu-id="3c368-137">String</span></span>|<span data-ttu-id="3c368-138">Отображает имя этого объекта.</span><span class="sxs-lookup"><span data-stu-id="3c368-138">The display name of this object.</span></span>|
|<span data-ttu-id="3c368-139">id</span><span class="sxs-lookup"><span data-stu-id="3c368-139">id</span></span>|<span data-ttu-id="3c368-140">String</span><span class="sxs-lookup"><span data-stu-id="3c368-140">String</span></span>|<span data-ttu-id="3c368-141">Уникальный идентификатор объекта, назначенного системой.</span><span class="sxs-lookup"><span data-stu-id="3c368-141">The system-assigned unique identifier of the object.</span></span>|
|<span data-ttu-id="3c368-142">isDefaultEnvironment</span><span class="sxs-lookup"><span data-stu-id="3c368-142">isDefaultEnvironment</span></span>|<span data-ttu-id="3c368-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="3c368-143">Boolean</span></span>|<span data-ttu-id="3c368-144">Определяет, является ли это среда по умолчанию или нет.</span><span class="sxs-lookup"><span data-stu-id="3c368-144">Determines whether this is default environment or not.</span></span> <span data-ttu-id="3c368-145">Он установлен для `true` всех систем статического происхождения, таких как группы Azure AD и Приложения Azure AD.</span><span class="sxs-lookup"><span data-stu-id="3c368-145">It is set to `true` for all static origin systems, such as Azure AD groups and Azure AD Applications.</span></span>|
|<span data-ttu-id="3c368-146">modifiedBy</span><span class="sxs-lookup"><span data-stu-id="3c368-146">modifiedBy</span></span>|<span data-ttu-id="3c368-147">String</span><span class="sxs-lookup"><span data-stu-id="3c368-147">String</span></span>|<span data-ttu-id="3c368-148">Отображает имя сущности, которая в последний раз меняла этот объект.</span><span class="sxs-lookup"><span data-stu-id="3c368-148">The display name of the entity that last modified this object.</span></span>|
|<span data-ttu-id="3c368-149">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3c368-149">modifiedDateTime</span></span>|<span data-ttu-id="3c368-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3c368-150">DateTimeOffset</span></span>|<span data-ttu-id="3c368-151">Дата и время последнего изменения этого объекта.</span><span class="sxs-lookup"><span data-stu-id="3c368-151">The date and time that this object was last modified.</span></span> <br><span data-ttu-id="3c368-152">Тип DateTimeOffset представляет сведения о дате и времени с использованием формата ISO 8601 и всегда указывает время в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="3c368-152">The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="3c368-153">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="3c368-153">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> |
|<span data-ttu-id="3c368-154">OriginId</span><span class="sxs-lookup"><span data-stu-id="3c368-154">originId</span></span>|<span data-ttu-id="3c368-155">String</span><span class="sxs-lookup"><span data-stu-id="3c368-155">String</span></span>|<span data-ttu-id="3c368-156">Уникальный идентификатор этой среды в системе происхождения.</span><span class="sxs-lookup"><span data-stu-id="3c368-156">The unique identifier of this environment in the origin system.</span></span>|
|<span data-ttu-id="3c368-157">originSystem</span><span class="sxs-lookup"><span data-stu-id="3c368-157">originSystem</span></span>|<span data-ttu-id="3c368-158">String</span><span class="sxs-lookup"><span data-stu-id="3c368-158">String</span></span>|<span data-ttu-id="3c368-159">Тип ресурса в системе происхождения, например `SharePointOnline` .</span><span class="sxs-lookup"><span data-stu-id="3c368-159">The type of the resource in the origin system such as `SharePointOnline`.</span></span> <span data-ttu-id="3c368-160">Поддерживает `$filter`.</span><span class="sxs-lookup"><span data-stu-id="3c368-160">Supports `$filter`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3c368-161">Связи</span><span class="sxs-lookup"><span data-stu-id="3c368-161">Relationships</span></span>
|<span data-ttu-id="3c368-162">Связь</span><span class="sxs-lookup"><span data-stu-id="3c368-162">Relationship</span></span>|<span data-ttu-id="3c368-163">Тип</span><span class="sxs-lookup"><span data-stu-id="3c368-163">Type</span></span>|<span data-ttu-id="3c368-164">Описание</span><span class="sxs-lookup"><span data-stu-id="3c368-164">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3c368-165">accessPackageResources</span><span class="sxs-lookup"><span data-stu-id="3c368-165">accessPackageResources</span></span>|<span data-ttu-id="3c368-166">[коллекция accessPackageResource](../resources/accesspackageresource.md)</span><span class="sxs-lookup"><span data-stu-id="3c368-166">[accessPackageResource](../resources/accesspackageresource.md) collection</span></span>|<span data-ttu-id="3c368-167">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3c368-167">Read-only.</span></span> <span data-ttu-id="3c368-168">Обязательный атрибут.</span><span class="sxs-lookup"><span data-stu-id="3c368-168">Required.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3c368-169">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3c368-169">JSON representation</span></span>
<span data-ttu-id="3c368-170">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3c368-170">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.accessPackageResourceEnvironment",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessPackageResourceEnvironment",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "originSystem": "String",
  "originId": "String",
  "isDefaultEnvironment": "Boolean",
  "connectionInfo": {
    "@odata.type": "microsoft.graph.connectionInfo"
  },
  "createdBy": "String",
  "createdDateTime": "String (timestamp)",
  "modifiedBy": "String",
  "modifiedDateTime": "String (timestamp)"
}
```

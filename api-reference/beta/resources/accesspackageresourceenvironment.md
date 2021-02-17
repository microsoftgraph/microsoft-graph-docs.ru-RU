---
title: Тип ресурса accessPackageResourceEnvironment
description: Среда ресурсов пакета доступа — это ссылка на среду географического местонахождения, в которой расположен ресурс.
author: hanki-microsoft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 2f03e2c754ea09cdc797b71d4ef59372ac47ff9b
ms.sourcegitcommit: 42fdb068616222eb6b0813e93b33e830fc7eedc0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/17/2021
ms.locfileid: "50272529"
---
# <a name="accesspackageresourceenvironment-resource-type"></a><span data-ttu-id="fb353-103">Тип ресурса accessPackageResourceEnvironment</span><span class="sxs-lookup"><span data-stu-id="fb353-103">accessPackageResourceEnvironment resource type</span></span>

<span data-ttu-id="fb353-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fb353-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fb353-105">В [azure AD Entitlement Management](entitlementmanagement-root.md)среда ресурсов пакета доступа является ссылкой на среду географического местонахождения, в которой расположен ресурс.</span><span class="sxs-lookup"><span data-stu-id="fb353-105">In [Azure AD Entitlement Management](entitlementmanagement-root.md), an access package resource environment is a reference to the geolocation environment in which a resource is located.</span></span> <span data-ttu-id="fb353-106">Эта среда автоматически предоставляется в рамках управления правами Azure AD.</span><span class="sxs-lookup"><span data-stu-id="fb353-106">This environment is automatically provided as part of Azure AD Entitlement Management.</span></span> <span data-ttu-id="fb353-107">API применим только к сайтам SharePoint Online с несколькими географическими режимами.</span><span class="sxs-lookup"><span data-stu-id="fb353-107">The API is only applicable to Multi-Geo SharePoint Online sites.</span></span>

## <a name="methods"></a><span data-ttu-id="fb353-108">Методы</span><span class="sxs-lookup"><span data-stu-id="fb353-108">Methods</span></span>
|<span data-ttu-id="fb353-109">Метод</span><span class="sxs-lookup"><span data-stu-id="fb353-109">Method</span></span>|<span data-ttu-id="fb353-110">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="fb353-110">Return type</span></span>|<span data-ttu-id="fb353-111">Описание</span><span class="sxs-lookup"><span data-stu-id="fb353-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="fb353-112">Список accessPackageResourceEnvironments</span><span class="sxs-lookup"><span data-stu-id="fb353-112">List accessPackageResourceEnvironments</span></span>](../api/accesspackageresourceenvironment-list.md)|<span data-ttu-id="fb353-113">[Коллекция accessPackageResourceEnvironment](../resources/accesspackageresourceenvironment.md)</span><span class="sxs-lookup"><span data-stu-id="fb353-113">[accessPackageResourceEnvironment](../resources/accesspackageresourceenvironment.md) collection</span></span>|<span data-ttu-id="fb353-114">Получить список объектов [accessPackageResourceEnvironment.](../resources/accesspackageresourceenvironment.md)</span><span class="sxs-lookup"><span data-stu-id="fb353-114">Retrieve a list of [accessPackageResourceEnvironment](../resources/accesspackageresourceenvironment.md) objects.</span></span>|
|[<span data-ttu-id="fb353-115">Get accessPackageResourceEnvironment</span><span class="sxs-lookup"><span data-stu-id="fb353-115">Get accessPackageResourceEnvironment</span></span>](../api/accesspackageresourceenvironment-get.md)|[<span data-ttu-id="fb353-116">accessPackageResourceEnvironment</span><span class="sxs-lookup"><span data-stu-id="fb353-116">accessPackageResourceEnvironment</span></span>](../resources/accesspackageresourceenvironment.md)|<span data-ttu-id="fb353-117">Чтение свойств и связей объекта [accessPackageResourceEnvironment.](../resources/accesspackageresourceenvironment.md)</span><span class="sxs-lookup"><span data-stu-id="fb353-117">Read the properties and relationships of an [accessPackageResourceEnvironment](../resources/accesspackageresourceenvironment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="fb353-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="fb353-118">Properties</span></span>
|<span data-ttu-id="fb353-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="fb353-119">Property</span></span>|<span data-ttu-id="fb353-120">Тип</span><span class="sxs-lookup"><span data-stu-id="fb353-120">Type</span></span>|<span data-ttu-id="fb353-121">Описание</span><span class="sxs-lookup"><span data-stu-id="fb353-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fb353-122">connectionInfo</span><span class="sxs-lookup"><span data-stu-id="fb353-122">connectionInfo</span></span>|[<span data-ttu-id="fb353-123">connectionInfo</span><span class="sxs-lookup"><span data-stu-id="fb353-123">connectionInfo</span></span>](../resources/connectioninfo.md)|<span data-ttu-id="fb353-124">Сведения о подключении среды, используемой для подключения к ресурсу.</span><span class="sxs-lookup"><span data-stu-id="fb353-124">Connection information of an environment used to connect to a resource.</span></span> |
|<span data-ttu-id="fb353-125">createdBy</span><span class="sxs-lookup"><span data-stu-id="fb353-125">createdBy</span></span>|<span data-ttu-id="fb353-126">String</span><span class="sxs-lookup"><span data-stu-id="fb353-126">String</span></span>|<span data-ttu-id="fb353-127">Отображаемого имени пользователя, создав этот объект.</span><span class="sxs-lookup"><span data-stu-id="fb353-127">The display name of the user that created this object.</span></span>|
|<span data-ttu-id="fb353-128">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="fb353-128">createdDateTime</span></span>|<span data-ttu-id="fb353-129">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fb353-129">DateTimeOffset</span></span>|<span data-ttu-id="fb353-130">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="fb353-130">The date and time that this object was created.</span></span> <br><span data-ttu-id="fb353-131">Тип DateTimeOffset представляет сведения о дате и времени с использованием формата ISO 8601 и всегда указывает время в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="fb353-131">The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="fb353-132">Например, полуночи 1 января 2014 г. в UTC — `'2014-01-01T00:00:00Z'` это .</span><span class="sxs-lookup"><span data-stu-id="fb353-132">For example, midnight UTC on Jan 1, 2014 is `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="fb353-133">description</span><span class="sxs-lookup"><span data-stu-id="fb353-133">description</span></span>|<span data-ttu-id="fb353-134">String</span><span class="sxs-lookup"><span data-stu-id="fb353-134">String</span></span>|<span data-ttu-id="fb353-135">Описание этого объекта *accessPackageResourceEnvironment.*</span><span class="sxs-lookup"><span data-stu-id="fb353-135">The description of this *accessPackageResourceEnvironment* object.</span></span>|
|<span data-ttu-id="fb353-136">displayName</span><span class="sxs-lookup"><span data-stu-id="fb353-136">displayName</span></span>|<span data-ttu-id="fb353-137">String</span><span class="sxs-lookup"><span data-stu-id="fb353-137">String</span></span>|<span data-ttu-id="fb353-138">Отображаемого имени этого объекта.</span><span class="sxs-lookup"><span data-stu-id="fb353-138">The display name of this object.</span></span>|
|<span data-ttu-id="fb353-139">id</span><span class="sxs-lookup"><span data-stu-id="fb353-139">id</span></span>|<span data-ttu-id="fb353-140">String</span><span class="sxs-lookup"><span data-stu-id="fb353-140">String</span></span>|<span data-ttu-id="fb353-141">Уникальный идентификатор объекта, присвоенный системе.</span><span class="sxs-lookup"><span data-stu-id="fb353-141">The system-assigned unique identifier of the object.</span></span>|
|<span data-ttu-id="fb353-142">isDefaultEnvironment</span><span class="sxs-lookup"><span data-stu-id="fb353-142">isDefaultEnvironment</span></span>|<span data-ttu-id="fb353-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="fb353-143">Boolean</span></span>|<span data-ttu-id="fb353-144">Определяет, является ли эта среда средой по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="fb353-144">Determines whether this is default environment or not.</span></span> <span data-ttu-id="fb353-145">Он установлен для всех систем статического источника, таких как группы `true` Azure AD и приложения Azure AD.</span><span class="sxs-lookup"><span data-stu-id="fb353-145">It is set to `true` for all static origin systems, such as Azure AD groups and Azure AD Applications.</span></span>|
|<span data-ttu-id="fb353-146">modifiedBy</span><span class="sxs-lookup"><span data-stu-id="fb353-146">modifiedBy</span></span>|<span data-ttu-id="fb353-147">String</span><span class="sxs-lookup"><span data-stu-id="fb353-147">String</span></span>|<span data-ttu-id="fb353-148">Отображаемого имени объекта, который последним изменил этот объект.</span><span class="sxs-lookup"><span data-stu-id="fb353-148">The display name of the entity that last modified this object.</span></span>|
|<span data-ttu-id="fb353-149">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fb353-149">modifiedDateTime</span></span>|<span data-ttu-id="fb353-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fb353-150">DateTimeOffset</span></span>|<span data-ttu-id="fb353-151">Дата и время последнего изменения этого объекта.</span><span class="sxs-lookup"><span data-stu-id="fb353-151">The date and time that this object was last modified.</span></span> <br><span data-ttu-id="fb353-152">Тип DateTimeOffset представляет сведения о дате и времени с использованием формата ISO 8601 и всегда указывает время в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="fb353-152">The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="fb353-153">Например, полуночи 1 января 2014 г. в UTC — `'2014-01-01T00:00:00Z'` это .</span><span class="sxs-lookup"><span data-stu-id="fb353-153">For example, midnight UTC on Jan 1, 2014 is `'2014-01-01T00:00:00Z'`.</span></span> |
|<span data-ttu-id="fb353-154">originId</span><span class="sxs-lookup"><span data-stu-id="fb353-154">originId</span></span>|<span data-ttu-id="fb353-155">String</span><span class="sxs-lookup"><span data-stu-id="fb353-155">String</span></span>|<span data-ttu-id="fb353-156">Уникальный идентификатор этой среды в системе источника.</span><span class="sxs-lookup"><span data-stu-id="fb353-156">The unique identifier of this environment in the origin system.</span></span>|
|<span data-ttu-id="fb353-157">originSystem</span><span class="sxs-lookup"><span data-stu-id="fb353-157">originSystem</span></span>|<span data-ttu-id="fb353-158">String</span><span class="sxs-lookup"><span data-stu-id="fb353-158">String</span></span>|<span data-ttu-id="fb353-159">Тип ресурса в системе источника, например `SharePointOnline` .</span><span class="sxs-lookup"><span data-stu-id="fb353-159">The type of the resource in the origin system such as `SharePointOnline`.</span></span> <span data-ttu-id="fb353-160">Поддерживает `$filter`.</span><span class="sxs-lookup"><span data-stu-id="fb353-160">Supports `$filter`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fb353-161">Связи</span><span class="sxs-lookup"><span data-stu-id="fb353-161">Relationships</span></span>
|<span data-ttu-id="fb353-162">Связь</span><span class="sxs-lookup"><span data-stu-id="fb353-162">Relationship</span></span>|<span data-ttu-id="fb353-163">Тип</span><span class="sxs-lookup"><span data-stu-id="fb353-163">Type</span></span>|<span data-ttu-id="fb353-164">Описание</span><span class="sxs-lookup"><span data-stu-id="fb353-164">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fb353-165">accessPackageResources</span><span class="sxs-lookup"><span data-stu-id="fb353-165">accessPackageResources</span></span>|<span data-ttu-id="fb353-166">[Коллекция accessPackageResource](../resources/accesspackageresource.md)</span><span class="sxs-lookup"><span data-stu-id="fb353-166">[accessPackageResource](../resources/accesspackageresource.md) collection</span></span>|<span data-ttu-id="fb353-167">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fb353-167">Read-only.</span></span> <span data-ttu-id="fb353-168">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fb353-168">Required.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fb353-169">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="fb353-169">JSON representation</span></span>
<span data-ttu-id="fb353-170">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fb353-170">The following is a JSON representation of the resource.</span></span>
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

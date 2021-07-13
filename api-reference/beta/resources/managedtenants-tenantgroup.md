---
title: Тип ресурса tenantGroup
description: Представляет логическую группу управляемых клиентов.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: 2ab0d97afff68dca7d76b1ad6c4e461ad6af6233
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402693"
---
# <a name="tenantgroup-resource-type"></a><span data-ttu-id="556e0-103">Тип ресурса tenantGroup</span><span class="sxs-lookup"><span data-stu-id="556e0-103">tenantGroup resource type</span></span>

<span data-ttu-id="556e0-104">Пространство имен: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="556e0-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="556e0-105">Представляет логическую группу управляемых клиентов.</span><span class="sxs-lookup"><span data-stu-id="556e0-105">Represents a logical group of managed tenants.</span></span>

## <a name="methods"></a><span data-ttu-id="556e0-106">Методы</span><span class="sxs-lookup"><span data-stu-id="556e0-106">Methods</span></span>
|<span data-ttu-id="556e0-107">Метод</span><span class="sxs-lookup"><span data-stu-id="556e0-107">Method</span></span>|<span data-ttu-id="556e0-108">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="556e0-108">Return type</span></span>|<span data-ttu-id="556e0-109">Описание</span><span class="sxs-lookup"><span data-stu-id="556e0-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="556e0-110">Список tenantGroups</span><span class="sxs-lookup"><span data-stu-id="556e0-110">List tenantGroups</span></span>](../api/managedtenants-managedtenant-list-tenantgroups.md)|<span data-ttu-id="556e0-111">[коллекция microsoft.graph.managedTenants.tenantGroup](../resources/managedtenants-tenantgroup.md)</span><span class="sxs-lookup"><span data-stu-id="556e0-111">[microsoft.graph.managedTenants.tenantGroup](../resources/managedtenants-tenantgroup.md) collection</span></span>|<span data-ttu-id="556e0-112">Получите список объектов [tenantGroup](../resources/managedtenants-tenantgroup.md) и их свойств.</span><span class="sxs-lookup"><span data-stu-id="556e0-112">Get a list of the [tenantGroup](../resources/managedtenants-tenantgroup.md) objects and their properties.</span></span>|
|[<span data-ttu-id="556e0-113">Get tenantGroup</span><span class="sxs-lookup"><span data-stu-id="556e0-113">Get tenantGroup</span></span>](../api/managedtenants-tenantgroup-get.md)|[<span data-ttu-id="556e0-114">microsoft.graph.managedTenants.tenantGroup</span><span class="sxs-lookup"><span data-stu-id="556e0-114">microsoft.graph.managedTenants.tenantGroup</span></span>](../resources/managedtenants-tenantgroup.md)|<span data-ttu-id="556e0-115">Ознакомьтесь с свойствами и отношениями объекта [tenantGroup.](../resources/managedtenants-tenantgroup.md)</span><span class="sxs-lookup"><span data-stu-id="556e0-115">Read the properties and relationships of a [tenantGroup](../resources/managedtenants-tenantgroup.md) object.</span></span>|
|[<span data-ttu-id="556e0-116">tenantSearch</span><span class="sxs-lookup"><span data-stu-id="556e0-116">tenantSearch</span></span>](../api/managedtenants-tenantgroup-tenantsearch.md)|<span data-ttu-id="556e0-117">[коллекция microsoft.graph.managedTenants.tenantGroup](../resources/managedtenants-tenantgroup.md)</span><span class="sxs-lookup"><span data-stu-id="556e0-117">[microsoft.graph.managedTenants.tenantGroup](../resources/managedtenants-tenantgroup.md) collection</span></span>|<span data-ttu-id="556e0-118">Поиск определенного управляемого клиента в группах клиентов.</span><span class="sxs-lookup"><span data-stu-id="556e0-118">Searches for the specific managed tenant across tenant groups.</span></span>|

## <a name="properties"></a><span data-ttu-id="556e0-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="556e0-119">Properties</span></span>
|<span data-ttu-id="556e0-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="556e0-120">Property</span></span>|<span data-ttu-id="556e0-121">Тип</span><span class="sxs-lookup"><span data-stu-id="556e0-121">Type</span></span>|<span data-ttu-id="556e0-122">Описание</span><span class="sxs-lookup"><span data-stu-id="556e0-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="556e0-123">allTenantsIncluded</span><span class="sxs-lookup"><span data-stu-id="556e0-123">allTenantsIncluded</span></span>|<span data-ttu-id="556e0-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="556e0-124">Boolean</span></span>|<span data-ttu-id="556e0-125">Флаг, указывающий, включены ли все управляемые клиенты в группу клиента.</span><span class="sxs-lookup"><span data-stu-id="556e0-125">A flag indicating whether all managed tenant are included in the tenant group.</span></span> <span data-ttu-id="556e0-126">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="556e0-126">Required.</span></span> <span data-ttu-id="556e0-127">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="556e0-127">Read-only.</span></span>|
|<span data-ttu-id="556e0-128">displayName</span><span class="sxs-lookup"><span data-stu-id="556e0-128">displayName</span></span>|<span data-ttu-id="556e0-129">String</span><span class="sxs-lookup"><span data-stu-id="556e0-129">String</span></span>|<span data-ttu-id="556e0-130">Имя отображения для группы клиента.</span><span class="sxs-lookup"><span data-stu-id="556e0-130">The display name for the tenant group.</span></span> <span data-ttu-id="556e0-131">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="556e0-131">Optional.</span></span> <span data-ttu-id="556e0-132">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="556e0-132">Read-only.</span></span>|
|<span data-ttu-id="556e0-133">id</span><span class="sxs-lookup"><span data-stu-id="556e0-133">id</span></span>|<span data-ttu-id="556e0-134">String</span><span class="sxs-lookup"><span data-stu-id="556e0-134">String</span></span>|<span data-ttu-id="556e0-135">Уникальный идентификатор для группы клиентов.</span><span class="sxs-lookup"><span data-stu-id="556e0-135">The unique identifier for the tenant group.</span></span> <span data-ttu-id="556e0-136">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="556e0-136">Required.</span></span> <span data-ttu-id="556e0-137">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="556e0-137">Read-only.</span></span>|
|<span data-ttu-id="556e0-138">managementActions</span><span class="sxs-lookup"><span data-stu-id="556e0-138">managementActions</span></span>|<span data-ttu-id="556e0-139">[коллекция microsoft.graph.managedTenants.managementActionInfo](../resources/managedtenants-managementactioninfo.md)</span><span class="sxs-lookup"><span data-stu-id="556e0-139">[microsoft.graph.managedTenants.managementActionInfo](../resources/managedtenants-managementactioninfo.md) collection</span></span>|<span data-ttu-id="556e0-140">Коллекция действий управления, связанных с группой клиентов.</span><span class="sxs-lookup"><span data-stu-id="556e0-140">The collection of management action associated with the tenant group.</span></span> <span data-ttu-id="556e0-141">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="556e0-141">Optional.</span></span> <span data-ttu-id="556e0-142">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="556e0-142">Read-only.</span></span>|
|<span data-ttu-id="556e0-143">managementIntents</span><span class="sxs-lookup"><span data-stu-id="556e0-143">managementIntents</span></span>|<span data-ttu-id="556e0-144">[коллекция microsoft.graph.managedTenants.managementIntentInfo](../resources/managedtenants-managementintentinfo.md)</span><span class="sxs-lookup"><span data-stu-id="556e0-144">[microsoft.graph.managedTenants.managementIntentInfo](../resources/managedtenants-managementintentinfo.md) collection</span></span>|<span data-ttu-id="556e0-145">Коллекция намерений управления, связанных с группой клиента.</span><span class="sxs-lookup"><span data-stu-id="556e0-145">The collection of management intents associated with the tenant group.</span></span> <span data-ttu-id="556e0-146">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="556e0-146">Optional.</span></span> <span data-ttu-id="556e0-147">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="556e0-147">Read-only.</span></span>|
|<span data-ttu-id="556e0-148">tenantIds</span><span class="sxs-lookup"><span data-stu-id="556e0-148">tenantIds</span></span>|<span data-ttu-id="556e0-149">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="556e0-149">String collection</span></span>|<span data-ttu-id="556e0-150">Коллекция управляемых идентификаторов клиента включается в группу клиентов.</span><span class="sxs-lookup"><span data-stu-id="556e0-150">The collection of managed tenant identifiers include in the tenant group.</span></span> <span data-ttu-id="556e0-151">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="556e0-151">Optional.</span></span> <span data-ttu-id="556e0-152">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="556e0-152">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="556e0-153">Связи</span><span class="sxs-lookup"><span data-stu-id="556e0-153">Relationships</span></span>
<span data-ttu-id="556e0-154">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="556e0-154">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="556e0-155">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="556e0-155">JSON representation</span></span>
<span data-ttu-id="556e0-156">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="556e0-156">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedTenants.tenantGroup",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.tenantGroup",
  "id": "String (identifier)",
  "displayName": "String",
  "allTenantsIncluded": "Boolean",
  "tenantIds": [
    "String"
  ],
  "managementIntents": [
    {
      "@odata.type": "microsoft.graph.managedTenants.managementIntentInfo"
    }
  ],
  "managementActions": [
    {
      "@odata.type": "microsoft.graph.managedTenants.managementActionInfo"
    }
  ]
}
```

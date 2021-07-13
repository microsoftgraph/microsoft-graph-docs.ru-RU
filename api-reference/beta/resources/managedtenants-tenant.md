---
title: тип ресурса клиента
description: Представляет клиента, связанного с управляющей сущностью.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: ee4bd57aa4e7fa2ea15c86376389d3b6e12198ea
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/13/2021
ms.locfileid: "53403161"
---
# <a name="tenant-resource-type"></a><span data-ttu-id="caa93-103">тип ресурса клиента</span><span class="sxs-lookup"><span data-stu-id="caa93-103">tenant resource type</span></span>

<span data-ttu-id="caa93-104">Пространство имен: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="caa93-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="caa93-105">Представляет клиента, связанного с управляющей сущностью.</span><span class="sxs-lookup"><span data-stu-id="caa93-105">Represents a tenant associated with the managing entity.</span></span>

## <a name="methods"></a><span data-ttu-id="caa93-106">Методы</span><span class="sxs-lookup"><span data-stu-id="caa93-106">Methods</span></span>
|<span data-ttu-id="caa93-107">Метод</span><span class="sxs-lookup"><span data-stu-id="caa93-107">Method</span></span>|<span data-ttu-id="caa93-108">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="caa93-108">Return type</span></span>|<span data-ttu-id="caa93-109">Описание</span><span class="sxs-lookup"><span data-stu-id="caa93-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="caa93-110">Список клиентов</span><span class="sxs-lookup"><span data-stu-id="caa93-110">List tenants</span></span>](../api/managedtenants-managedtenant-list-tenants.md)|<span data-ttu-id="caa93-111">[коллекция microsoft.graph.managedTenants.tenant](../resources/managedtenants-tenant.md)</span><span class="sxs-lookup"><span data-stu-id="caa93-111">[microsoft.graph.managedTenants.tenant](../resources/managedtenants-tenant.md) collection</span></span>|<span data-ttu-id="caa93-112">Получите список объектов [клиента](../resources/managedtenants-tenant.md) и их свойств.</span><span class="sxs-lookup"><span data-stu-id="caa93-112">Get a list of the [tenant](../resources/managedtenants-tenant.md) objects and their properties.</span></span>|
|[<span data-ttu-id="caa93-113">Получить клиента</span><span class="sxs-lookup"><span data-stu-id="caa93-113">Get tenant</span></span>](../api/managedtenants-tenant-get.md)|[<span data-ttu-id="caa93-114">microsoft.graph.managedTenants.tenant</span><span class="sxs-lookup"><span data-stu-id="caa93-114">microsoft.graph.managedTenants.tenant</span></span>](../resources/managedtenants-tenant.md)|<span data-ttu-id="caa93-115">Ознакомьтесь с свойствами и отношениями [объекта-клиента.](../resources/managedtenants-tenant.md)</span><span class="sxs-lookup"><span data-stu-id="caa93-115">Read the properties and relationships of a [tenant](../resources/managedtenants-tenant.md) object.</span></span>|
|[<span data-ttu-id="caa93-116">offboardTenant</span><span class="sxs-lookup"><span data-stu-id="caa93-116">offboardTenant</span></span>](../api/managedtenants-tenant-offboardtenant.md)|[<span data-ttu-id="caa93-117">microsoft.graph.managedTenants.tenant</span><span class="sxs-lookup"><span data-stu-id="caa93-117">microsoft.graph.managedTenants.tenant</span></span>](../resources/managedtenants-tenant.md)|<span data-ttu-id="caa93-118">Off boards a tenant from the multi-tenant management platform.</span><span class="sxs-lookup"><span data-stu-id="caa93-118">Off boards a tenant from the multi-tenant management platform.</span></span>|
|[<span data-ttu-id="caa93-119">resetTenantOnboardingStatus</span><span class="sxs-lookup"><span data-stu-id="caa93-119">resetTenantOnboardingStatus</span></span>](../api/managedtenants-tenant-resettenantonboardingstatus.md)|[<span data-ttu-id="caa93-120">microsoft.graph.managedTenants.tenant</span><span class="sxs-lookup"><span data-stu-id="caa93-120">microsoft.graph.managedTenants.tenant</span></span>](../resources/managedtenants-tenant.md)|<span data-ttu-id="caa93-121">Сбрасывает состояние onboarding клиента с помощью платформы управления с несколькими клиентами.</span><span class="sxs-lookup"><span data-stu-id="caa93-121">Resets the tenant onboarding status with the multi-tenant management platform.</span></span>|

## <a name="properties"></a><span data-ttu-id="caa93-122">Свойства</span><span class="sxs-lookup"><span data-stu-id="caa93-122">Properties</span></span>
|<span data-ttu-id="caa93-123">Свойство</span><span class="sxs-lookup"><span data-stu-id="caa93-123">Property</span></span>|<span data-ttu-id="caa93-124">Тип</span><span class="sxs-lookup"><span data-stu-id="caa93-124">Type</span></span>|<span data-ttu-id="caa93-125">Описание</span><span class="sxs-lookup"><span data-stu-id="caa93-125">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="caa93-126">contract</span><span class="sxs-lookup"><span data-stu-id="caa93-126">contract</span></span>|[<span data-ttu-id="caa93-127">microsoft.graph.managedTenants.tenantContract</span><span class="sxs-lookup"><span data-stu-id="caa93-127">microsoft.graph.managedTenants.tenantContract</span></span>](../resources/managedtenants-tenantcontract.md)|<span data-ttu-id="caa93-128">Сведения об отношениях клиента с управляющей сущностью.</span><span class="sxs-lookup"><span data-stu-id="caa93-128">The relationship details for the tenant with the managing entity.</span></span>|
|<span data-ttu-id="caa93-129">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="caa93-129">createdDateTime</span></span>|<span data-ttu-id="caa93-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="caa93-130">DateTimeOffset</span></span>|<span data-ttu-id="caa93-131">Дата и время создания клиента на платформе управления с несколькими арендаторами.</span><span class="sxs-lookup"><span data-stu-id="caa93-131">The date and time the tenant was created in the multi-tenant management platform.</span></span> <span data-ttu-id="caa93-132">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="caa93-132">Optional.</span></span> <span data-ttu-id="caa93-133">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="caa93-133">Read-only.</span></span>|
|<span data-ttu-id="caa93-134">displayName</span><span class="sxs-lookup"><span data-stu-id="caa93-134">displayName</span></span>|<span data-ttu-id="caa93-135">String</span><span class="sxs-lookup"><span data-stu-id="caa93-135">String</span></span>|<span data-ttu-id="caa93-136">Отображаемое имя для клиента.</span><span class="sxs-lookup"><span data-stu-id="caa93-136">The display name for the tenant.</span></span> <span data-ttu-id="caa93-137">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="caa93-137">Required.</span></span> <span data-ttu-id="caa93-138">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="caa93-138">Read-only.</span></span>|
|<span data-ttu-id="caa93-139">id</span><span class="sxs-lookup"><span data-stu-id="caa93-139">id</span></span>|<span data-ttu-id="caa93-140">String</span><span class="sxs-lookup"><span data-stu-id="caa93-140">String</span></span>|<span data-ttu-id="caa93-141">Идентификатор Azure Active Directory клиента для клиента.</span><span class="sxs-lookup"><span data-stu-id="caa93-141">The Azure Active Directory tenant identifier for the tenant.</span></span> <span data-ttu-id="caa93-142">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="caa93-142">Required.</span></span> <span data-ttu-id="caa93-143">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="caa93-143">Read-only.</span></span>|
|<span data-ttu-id="caa93-144">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="caa93-144">lastUpdatedDateTime</span></span>|<span data-ttu-id="caa93-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="caa93-145">DateTimeOffset</span></span>|<span data-ttu-id="caa93-146">Дата и время последнего обновления клиента в платформе управления с несколькими клиентами.</span><span class="sxs-lookup"><span data-stu-id="caa93-146">The date and time the tenant was last updated within the multi-tenant management platform.</span></span> <span data-ttu-id="caa93-147">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="caa93-147">Optional.</span></span> <span data-ttu-id="caa93-148">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="caa93-148">Read-only.</span></span>|
|<span data-ttu-id="caa93-149">tenantId</span><span class="sxs-lookup"><span data-stu-id="caa93-149">tenantId</span></span>|<span data-ttu-id="caa93-150">String</span><span class="sxs-lookup"><span data-stu-id="caa93-150">String</span></span>|<span data-ttu-id="caa93-151">Идентификатор Azure Active Directory клиента для [управляемого клиента.](../resources/managedtenants-tenant.md)</span><span class="sxs-lookup"><span data-stu-id="caa93-151">The Azure Active Directory tenant identifier for the [managed tenant](../resources/managedtenants-tenant.md).</span></span> <span data-ttu-id="caa93-152">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="caa93-152">Optional.</span></span> <span data-ttu-id="caa93-153">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="caa93-153">Read-only.</span></span>|
|<span data-ttu-id="caa93-154">tenantStatusInformation</span><span class="sxs-lookup"><span data-stu-id="caa93-154">tenantStatusInformation</span></span>|[<span data-ttu-id="caa93-155">microsoft.graph.managedTenants.tenantStatusInformation</span><span class="sxs-lookup"><span data-stu-id="caa93-155">microsoft.graph.managedTenants.tenantStatusInformation</span></span>](../resources/managedtenants-tenantstatusinformation.md)|<span data-ttu-id="caa93-156">Сведения о состоянии на борту для клиента.</span><span class="sxs-lookup"><span data-stu-id="caa93-156">The onboarding status information for the tenant.</span></span> <span data-ttu-id="caa93-157">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="caa93-157">Optional.</span></span> <span data-ttu-id="caa93-158">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="caa93-158">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="caa93-159">Связи</span><span class="sxs-lookup"><span data-stu-id="caa93-159">Relationships</span></span>
<span data-ttu-id="caa93-160">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="caa93-160">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="caa93-161">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="caa93-161">JSON representation</span></span>
<span data-ttu-id="caa93-162">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="caa93-162">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedTenants.tenant",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.tenant",
  "id": "String (identifier)",
  "tenantId": "String",
  "displayName": "String",
  "contract": {
    "@odata.type": "microsoft.graph.managedTenants.tenantContract"
  },
  "tenantStatusInformation": {
    "@odata.type": "microsoft.graph.managedTenants.tenantStatusInformation"
  },
  "lastUpdatedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)"
}
```

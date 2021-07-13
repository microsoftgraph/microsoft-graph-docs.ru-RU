---
title: тип ресурса aggregatedPolicyCompliance
description: Представляет сводное представление соответствия требованиям устройств для управляемого клиента.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: 8b2c6ce85c0ec6df361ddfeb13a851740efb2acb
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402555"
---
# <a name="aggregatedpolicycompliance-resource-type"></a><span data-ttu-id="2232d-103">тип ресурса aggregatedPolicyCompliance</span><span class="sxs-lookup"><span data-stu-id="2232d-103">aggregatedPolicyCompliance resource type</span></span>

<span data-ttu-id="2232d-104">Пространство имен: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="2232d-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2232d-105">Представляет сводное представление соответствия требованиям устройств для управляемого клиента.</span><span class="sxs-lookup"><span data-stu-id="2232d-105">Represents an aggregate view of device compliance for a managed tenant.</span></span>

## <a name="methods"></a><span data-ttu-id="2232d-106">Методы</span><span class="sxs-lookup"><span data-stu-id="2232d-106">Methods</span></span>
|<span data-ttu-id="2232d-107">Метод</span><span class="sxs-lookup"><span data-stu-id="2232d-107">Method</span></span>|<span data-ttu-id="2232d-108">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="2232d-108">Return type</span></span>|<span data-ttu-id="2232d-109">Описание</span><span class="sxs-lookup"><span data-stu-id="2232d-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="2232d-110">Список агрегированныхPolicyCompliances</span><span class="sxs-lookup"><span data-stu-id="2232d-110">List aggregatedPolicyCompliances</span></span>](../api/managedtenants-managedtenant-list-aggregatedpolicycompliances.md)|<span data-ttu-id="2232d-111">[коллекция microsoft.graph.managedTenants.aggregatedPolicyCompliance](../resources/managedtenants-aggregatedpolicycompliance.md)</span><span class="sxs-lookup"><span data-stu-id="2232d-111">[microsoft.graph.managedTenants.aggregatedPolicyCompliance](../resources/managedtenants-aggregatedpolicycompliance.md) collection</span></span>|<span data-ttu-id="2232d-112">Получите список объектов [aggregatedPolicyCompliance](../resources/managedtenants-aggregatedpolicycompliance.md) и их свойств.</span><span class="sxs-lookup"><span data-stu-id="2232d-112">Get a list of the [aggregatedPolicyCompliance](../resources/managedtenants-aggregatedpolicycompliance.md) objects and their properties.</span></span>|

## <a name="properties"></a><span data-ttu-id="2232d-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="2232d-113">Properties</span></span>
|<span data-ttu-id="2232d-114">Свойство</span><span class="sxs-lookup"><span data-stu-id="2232d-114">Property</span></span>|<span data-ttu-id="2232d-115">Тип</span><span class="sxs-lookup"><span data-stu-id="2232d-115">Type</span></span>|<span data-ttu-id="2232d-116">Описание</span><span class="sxs-lookup"><span data-stu-id="2232d-116">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2232d-117">compliancePolicyId</span><span class="sxs-lookup"><span data-stu-id="2232d-117">compliancePolicyId</span></span>|<span data-ttu-id="2232d-118">String</span><span class="sxs-lookup"><span data-stu-id="2232d-118">String</span></span>|<span data-ttu-id="2232d-119">Идентификатор для политики соответствия требованиям к устройству.</span><span class="sxs-lookup"><span data-stu-id="2232d-119">Identifier for the device compliance policy.</span></span> <span data-ttu-id="2232d-120">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="2232d-120">Optional.</span></span> <span data-ttu-id="2232d-121">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2232d-121">Read-only.</span></span>|
|<span data-ttu-id="2232d-122">compliancePolicyName</span><span class="sxs-lookup"><span data-stu-id="2232d-122">compliancePolicyName</span></span>|<span data-ttu-id="2232d-123">String</span><span class="sxs-lookup"><span data-stu-id="2232d-123">String</span></span>|<span data-ttu-id="2232d-124">Имя политики соответствия требованиям к устройству.</span><span class="sxs-lookup"><span data-stu-id="2232d-124">Name of the device compliance policy.</span></span> <span data-ttu-id="2232d-125">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="2232d-125">Optional.</span></span> <span data-ttu-id="2232d-126">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2232d-126">Read-only.</span></span>|
|<span data-ttu-id="2232d-127">compliancePolicyPlatform</span><span class="sxs-lookup"><span data-stu-id="2232d-127">compliancePolicyPlatform</span></span>|<span data-ttu-id="2232d-128">String</span><span class="sxs-lookup"><span data-stu-id="2232d-128">String</span></span>|<span data-ttu-id="2232d-129">Платформа для политики соответствия требованиям к устройствам.</span><span class="sxs-lookup"><span data-stu-id="2232d-129">Platform for the device compliance policy.</span></span> <span data-ttu-id="2232d-130">Возможные значения: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `androidAOSP`, `all`.</span><span class="sxs-lookup"><span data-stu-id="2232d-130">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `androidAOSP`, `all`.</span></span> <span data-ttu-id="2232d-131">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="2232d-131">Optional.</span></span> <span data-ttu-id="2232d-132">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2232d-132">Read-only.</span></span>|
|<span data-ttu-id="2232d-133">compliancePolicyType</span><span class="sxs-lookup"><span data-stu-id="2232d-133">compliancePolicyType</span></span>|<span data-ttu-id="2232d-134">String</span><span class="sxs-lookup"><span data-stu-id="2232d-134">String</span></span>|<span data-ttu-id="2232d-135">Тип политики соответствия требованиям.</span><span class="sxs-lookup"><span data-stu-id="2232d-135">The type of compliance policy.</span></span> <span data-ttu-id="2232d-136">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="2232d-136">Optional.</span></span> <span data-ttu-id="2232d-137">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2232d-137">Read-only.</span></span>|
|<span data-ttu-id="2232d-138">id</span><span class="sxs-lookup"><span data-stu-id="2232d-138">id</span></span>|<span data-ttu-id="2232d-139">String</span><span class="sxs-lookup"><span data-stu-id="2232d-139">String</span></span>|<span data-ttu-id="2232d-140">Уникальный идентификатор для общей политики соответствия требованиям к устройствам.</span><span class="sxs-lookup"><span data-stu-id="2232d-140">Unique identifier for the aggregate device compliance policy.</span></span> <span data-ttu-id="2232d-141">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2232d-141">Required.</span></span> <span data-ttu-id="2232d-142">Только для чтения</span><span class="sxs-lookup"><span data-stu-id="2232d-142">Read-only</span></span>|
|<span data-ttu-id="2232d-143">lastRefreshedDateTime</span><span class="sxs-lookup"><span data-stu-id="2232d-143">lastRefreshedDateTime</span></span>|<span data-ttu-id="2232d-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2232d-144">DateTimeOffset</span></span>|<span data-ttu-id="2232d-145">Дата и время последнего обновления объекта на платформе управления с несколькими клиентами.</span><span class="sxs-lookup"><span data-stu-id="2232d-145">Date and time the entity was last updated in the multi-tenant management platform.</span></span> <span data-ttu-id="2232d-146">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="2232d-146">Optional.</span></span> <span data-ttu-id="2232d-147">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2232d-147">Read-only.</span></span>|
|<span data-ttu-id="2232d-148">numberOfCompliantDevices</span><span class="sxs-lookup"><span data-stu-id="2232d-148">numberOfCompliantDevices</span></span>|<span data-ttu-id="2232d-149">Int64</span><span class="sxs-lookup"><span data-stu-id="2232d-149">Int64</span></span>|<span data-ttu-id="2232d-150">Количество устройств, которые находятся в состоянии совместимых.</span><span class="sxs-lookup"><span data-stu-id="2232d-150">The number of devices that are in a compliant status.</span></span> <span data-ttu-id="2232d-151">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="2232d-151">Optional.</span></span> <span data-ttu-id="2232d-152">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2232d-152">Read-only.</span></span>|
|<span data-ttu-id="2232d-153">numberOfErrorDevices</span><span class="sxs-lookup"><span data-stu-id="2232d-153">numberOfErrorDevices</span></span>|<span data-ttu-id="2232d-154">Int64</span><span class="sxs-lookup"><span data-stu-id="2232d-154">Int64</span></span>|<span data-ttu-id="2232d-155">Количество устройств, которые находятся в состоянии ошибки.</span><span class="sxs-lookup"><span data-stu-id="2232d-155">The number of devices that are in an error status.</span></span> <span data-ttu-id="2232d-156">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="2232d-156">Optional.</span></span> <span data-ttu-id="2232d-157">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2232d-157">Read-only.</span></span>|
|<span data-ttu-id="2232d-158">numberOfNonCompliantDevices</span><span class="sxs-lookup"><span data-stu-id="2232d-158">numberOfNonCompliantDevices</span></span>|<span data-ttu-id="2232d-159">Int64</span><span class="sxs-lookup"><span data-stu-id="2232d-159">Int64</span></span>|<span data-ttu-id="2232d-160">Количество устройств, которые находятся в состоянии, не удовлетворяемом требованиям.</span><span class="sxs-lookup"><span data-stu-id="2232d-160">The number of device that are in a non-compliant status.</span></span> <span data-ttu-id="2232d-161">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="2232d-161">Optional.</span></span> <span data-ttu-id="2232d-162">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2232d-162">Read-only.</span></span>|
|<span data-ttu-id="2232d-163">policyModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2232d-163">policyModifiedDateTime</span></span>|<span data-ttu-id="2232d-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2232d-164">DateTimeOffset</span></span>|<span data-ttu-id="2232d-165">Дата и время последнего изменения политики устройства.</span><span class="sxs-lookup"><span data-stu-id="2232d-165">The date and time the device policy was last modified.</span></span> <span data-ttu-id="2232d-166">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="2232d-166">Optional.</span></span> <span data-ttu-id="2232d-167">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2232d-167">Read-only.</span></span>|
|<span data-ttu-id="2232d-168">tenantDisplayName</span><span class="sxs-lookup"><span data-stu-id="2232d-168">tenantDisplayName</span></span>|<span data-ttu-id="2232d-169">String</span><span class="sxs-lookup"><span data-stu-id="2232d-169">String</span></span>|<span data-ttu-id="2232d-170">Имя отображения управляемого клиента.</span><span class="sxs-lookup"><span data-stu-id="2232d-170">The display name for the managed tenant.</span></span> <span data-ttu-id="2232d-171">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="2232d-171">Optional.</span></span> <span data-ttu-id="2232d-172">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2232d-172">Read-only.</span></span>|
|<span data-ttu-id="2232d-173">tenantId</span><span class="sxs-lookup"><span data-stu-id="2232d-173">tenantId</span></span>|<span data-ttu-id="2232d-174">String</span><span class="sxs-lookup"><span data-stu-id="2232d-174">String</span></span>|<span data-ttu-id="2232d-175">Идентификатор Azure Active Directory клиента для [управляемого клиента.](../resources/managedtenants-tenant.md)</span><span class="sxs-lookup"><span data-stu-id="2232d-175">The Azure Active Directory tenant identifier for the [managed tenant](../resources/managedtenants-tenant.md).</span></span> <span data-ttu-id="2232d-176">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="2232d-176">Optional.</span></span> <span data-ttu-id="2232d-177">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2232d-177">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2232d-178">Связи</span><span class="sxs-lookup"><span data-stu-id="2232d-178">Relationships</span></span>
<span data-ttu-id="2232d-179">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="2232d-179">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="2232d-180">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="2232d-180">JSON representation</span></span>
<span data-ttu-id="2232d-181">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2232d-181">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedTenants.aggregatedPolicyCompliance",
  "baseType": "microsoft.graph.entity",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.aggregatedPolicyCompliance",
  "id": "String (identifier)",
  "tenantId": "String",
  "tenantDisplayName": "String",
  "compliancePolicyId": "String",
  "compliancePolicyName": "String",
  "compliancePolicyType": "String",
  "compliancePolicyPlatform": "String",
  "numberOfCompliantDevices": "Integer",
  "numberOfNonCompliantDevices": "Integer",
  "numberOfErrorDevices": "Integer",
  "policyModifiedDateTime": "String (timestamp)",
  "lastRefreshedDateTime": "String (timestamp)"
}
```

---
title: тип ресурса managedDeviceComplianceTrend
description: Представляет тенденцию совместимых и не совместимых устройств для данного управляемого клиента.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: 70c3c84c5da6ffb2660a6289bc55c6ab3eef64be
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402531"
---
# <a name="manageddevicecompliancetrend-resource-type"></a><span data-ttu-id="6622a-103">тип ресурса managedDeviceComplianceTrend</span><span class="sxs-lookup"><span data-stu-id="6622a-103">managedDeviceComplianceTrend resource type</span></span>

<span data-ttu-id="6622a-104">Пространство имен: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="6622a-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6622a-105">Представляет тенденцию совместимых и не совместимых устройств для данного управляемого клиента.</span><span class="sxs-lookup"><span data-stu-id="6622a-105">Represents a trend of compliant and non-compliant devices for a given managed tenant.</span></span>

## <a name="methods"></a><span data-ttu-id="6622a-106">Методы</span><span class="sxs-lookup"><span data-stu-id="6622a-106">Methods</span></span>
|<span data-ttu-id="6622a-107">Метод</span><span class="sxs-lookup"><span data-stu-id="6622a-107">Method</span></span>|<span data-ttu-id="6622a-108">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="6622a-108">Return type</span></span>|<span data-ttu-id="6622a-109">Описание</span><span class="sxs-lookup"><span data-stu-id="6622a-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="6622a-110">Список управляемыхDeviceComplianceTrends</span><span class="sxs-lookup"><span data-stu-id="6622a-110">List managedDeviceComplianceTrends</span></span>](../api/managedtenants-managedtenant-list-manageddevicecompliancetrends.md)|<span data-ttu-id="6622a-111">[коллекция microsoft.graph.managedTenants.managedDeviceComplianceTrend](../resources/managedtenants-manageddevicecompliancetrend.md)</span><span class="sxs-lookup"><span data-stu-id="6622a-111">[microsoft.graph.managedTenants.managedDeviceComplianceTrend](../resources/managedtenants-manageddevicecompliancetrend.md) collection</span></span>|<span data-ttu-id="6622a-112">Получите список объектов [managedDeviceComplianceTrend](../resources/managedtenants-manageddevicecompliancetrend.md) и их свойств.</span><span class="sxs-lookup"><span data-stu-id="6622a-112">Get a list of the [managedDeviceComplianceTrend](../resources/managedtenants-manageddevicecompliancetrend.md) objects and their properties.</span></span>|
|[<span data-ttu-id="6622a-113">Get managedDeviceComplianceTrend</span><span class="sxs-lookup"><span data-stu-id="6622a-113">Get managedDeviceComplianceTrend</span></span>](../api/managedtenants-manageddevicecompliancetrend-get.md)|[<span data-ttu-id="6622a-114">microsoft.graph.managedTenants.managedDeviceComplianceTrend</span><span class="sxs-lookup"><span data-stu-id="6622a-114">microsoft.graph.managedTenants.managedDeviceComplianceTrend</span></span>](../resources/managedtenants-manageddevicecompliancetrend.md)|<span data-ttu-id="6622a-115">Ознакомьтесь с свойствами и отношениями объекта [managedDeviceComplianceTrend.](../resources/managedtenants-manageddevicecompliancetrend.md)</span><span class="sxs-lookup"><span data-stu-id="6622a-115">Read the properties and relationships of a [managedDeviceComplianceTrend](../resources/managedtenants-manageddevicecompliancetrend.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="6622a-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="6622a-116">Properties</span></span>
|<span data-ttu-id="6622a-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="6622a-117">Property</span></span>|<span data-ttu-id="6622a-118">Тип</span><span class="sxs-lookup"><span data-stu-id="6622a-118">Type</span></span>|<span data-ttu-id="6622a-119">Описание</span><span class="sxs-lookup"><span data-stu-id="6622a-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6622a-120">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="6622a-120">compliantDeviceCount</span></span>|<span data-ttu-id="6622a-121">Int32</span><span class="sxs-lookup"><span data-stu-id="6622a-121">Int32</span></span>|<span data-ttu-id="6622a-122">Количество устройств с соответствующим состоянием.</span><span class="sxs-lookup"><span data-stu-id="6622a-122">The number of devices with a compliant status.</span></span> <span data-ttu-id="6622a-123">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6622a-123">Required.</span></span> <span data-ttu-id="6622a-124">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6622a-124">Read-only.</span></span>|
|<span data-ttu-id="6622a-125">configManagerDeviceCount</span><span class="sxs-lookup"><span data-stu-id="6622a-125">configManagerDeviceCount</span></span>|<span data-ttu-id="6622a-126">Int32</span><span class="sxs-lookup"><span data-stu-id="6622a-126">Int32</span></span>|<span data-ttu-id="6622a-127">Количество устройств, вмеяное диспетчером конфигурации.</span><span class="sxs-lookup"><span data-stu-id="6622a-127">The number of devices manged by Configuration Manager.</span></span> <span data-ttu-id="6622a-128">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6622a-128">Required.</span></span> <span data-ttu-id="6622a-129">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6622a-129">Read-only.</span></span>|
|<span data-ttu-id="6622a-130">countDateTime</span><span class="sxs-lookup"><span data-stu-id="6622a-130">countDateTime</span></span>|<span data-ttu-id="6622a-131">String</span><span class="sxs-lookup"><span data-stu-id="6622a-131">String</span></span>|<span data-ttu-id="6622a-132">Был выполнен снимок соответствия требованиям даты и времени.</span><span class="sxs-lookup"><span data-stu-id="6622a-132">The date and time compliance snapshot was performed.</span></span> <span data-ttu-id="6622a-133">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6622a-133">Required.</span></span> <span data-ttu-id="6622a-134">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6622a-134">Read-only.</span></span>|
|<span data-ttu-id="6622a-135">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="6622a-135">errorDeviceCount</span></span>|<span data-ttu-id="6622a-136">Int32</span><span class="sxs-lookup"><span data-stu-id="6622a-136">Int32</span></span>|<span data-ttu-id="6622a-137">Количество устройств с состоянием ошибки.</span><span class="sxs-lookup"><span data-stu-id="6622a-137">The number of devices with an error status.</span></span> <span data-ttu-id="6622a-138">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6622a-138">Required.</span></span> <span data-ttu-id="6622a-139">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6622a-139">Read-only.</span></span>|
|<span data-ttu-id="6622a-140">id</span><span class="sxs-lookup"><span data-stu-id="6622a-140">id</span></span>|<span data-ttu-id="6622a-141">String</span><span class="sxs-lookup"><span data-stu-id="6622a-141">String</span></span>|<span data-ttu-id="6622a-142">Уникальный идентификатор для этого объекта.</span><span class="sxs-lookup"><span data-stu-id="6622a-142">The unique identifier for this entity.</span></span> <span data-ttu-id="6622a-143">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6622a-143">Required.</span></span> <span data-ttu-id="6622a-144">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6622a-144">Read-only.</span></span>|
|<span data-ttu-id="6622a-145">inGracePeriodDeviceCount</span><span class="sxs-lookup"><span data-stu-id="6622a-145">inGracePeriodDeviceCount</span></span>|<span data-ttu-id="6622a-146">Int32</span><span class="sxs-lookup"><span data-stu-id="6622a-146">Int32</span></span>|<span data-ttu-id="6622a-147">Количество устройств, которые находятся в состоянии льготного периода.</span><span class="sxs-lookup"><span data-stu-id="6622a-147">The number of devices that are in a grace period status.</span></span> <span data-ttu-id="6622a-148">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6622a-148">Required.</span></span> <span data-ttu-id="6622a-149">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6622a-149">Read-only.</span></span>|
|<span data-ttu-id="6622a-150">noncompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="6622a-150">noncompliantDeviceCount</span></span>|<span data-ttu-id="6622a-151">Int32</span><span class="sxs-lookup"><span data-stu-id="6622a-151">Int32</span></span>|<span data-ttu-id="6622a-152">Количество устройств, которые находятся в состоянии, не удовлетворяемом требованиям.</span><span class="sxs-lookup"><span data-stu-id="6622a-152">The number of devices that are in a non-compliant status.</span></span> <span data-ttu-id="6622a-153">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6622a-153">Required.</span></span> <span data-ttu-id="6622a-154">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6622a-154">Read-only.</span></span>|
|<span data-ttu-id="6622a-155">tenantDisplayName</span><span class="sxs-lookup"><span data-stu-id="6622a-155">tenantDisplayName</span></span>|<span data-ttu-id="6622a-156">String</span><span class="sxs-lookup"><span data-stu-id="6622a-156">String</span></span>|<span data-ttu-id="6622a-157">Имя отображения управляемого клиента.</span><span class="sxs-lookup"><span data-stu-id="6622a-157">The display name for the managed tenant.</span></span> <span data-ttu-id="6622a-158">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="6622a-158">Optional.</span></span> <span data-ttu-id="6622a-159">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6622a-159">Read-only.</span></span>|
|<span data-ttu-id="6622a-160">tenantId</span><span class="sxs-lookup"><span data-stu-id="6622a-160">tenantId</span></span>|<span data-ttu-id="6622a-161">String</span><span class="sxs-lookup"><span data-stu-id="6622a-161">String</span></span>|<span data-ttu-id="6622a-162">Идентификатор Azure Active Directory клиента для [управляемого клиента.](../resources/managedtenants-tenant.md)</span><span class="sxs-lookup"><span data-stu-id="6622a-162">The Azure Active Directory tenant identifier for the [managed tenant](../resources/managedtenants-tenant.md).</span></span> <span data-ttu-id="6622a-163">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="6622a-163">Optional.</span></span> <span data-ttu-id="6622a-164">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6622a-164">Read-only.</span></span>|
|<span data-ttu-id="6622a-165">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="6622a-165">unknownDeviceCount</span></span>|<span data-ttu-id="6622a-166">Int32</span><span class="sxs-lookup"><span data-stu-id="6622a-166">Int32</span></span>|<span data-ttu-id="6622a-167">Количество устройств в неизвестном состоянии.</span><span class="sxs-lookup"><span data-stu-id="6622a-167">The number of devices in an unknown status.</span></span> <span data-ttu-id="6622a-168">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6622a-168">Required.</span></span> <span data-ttu-id="6622a-169">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6622a-169">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6622a-170">Связи</span><span class="sxs-lookup"><span data-stu-id="6622a-170">Relationships</span></span>
<span data-ttu-id="6622a-171">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="6622a-171">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="6622a-172">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="6622a-172">JSON representation</span></span>
<span data-ttu-id="6622a-173">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6622a-173">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedTenants.managedDeviceComplianceTrend",
  "baseType": "microsoft.graph.entity",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.managedDeviceComplianceTrend",
  "id": "String (identifier)",
  "tenantId": "String",
  "tenantDisplayName": "String",
  "unknownDeviceCount": "Integer",
  "compliantDeviceCount": "Integer",
  "noncompliantDeviceCount": "Integer",
  "errorDeviceCount": "Integer",
  "inGracePeriodDeviceCount": "Integer",
  "configManagerDeviceCount": "Integer",
  "countDateTime": "String"
}
```

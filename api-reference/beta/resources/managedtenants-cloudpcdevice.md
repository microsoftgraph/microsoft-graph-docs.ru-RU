---
title: тип ресурса cloudPcDevice
description: Представляет облачное компьютерное устройство, принадлежающее заданным управляемым клиентом.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: 57eabb6720987a8a9bfca4c18e283057848b65cf
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402549"
---
# <a name="cloudpcdevice-resource-type"></a><span data-ttu-id="c159b-103">тип ресурса cloudPcDevice</span><span class="sxs-lookup"><span data-stu-id="c159b-103">cloudPcDevice resource type</span></span>

<span data-ttu-id="c159b-104">Пространство имен: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="c159b-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c159b-105">Представляет облачное компьютерное устройство, принадлежающее заданным управляемым клиентом.</span><span class="sxs-lookup"><span data-stu-id="c159b-105">Represents a cloud PC device that belongs to a given managed tenant.</span></span>

## <a name="methods"></a><span data-ttu-id="c159b-106">Методы</span><span class="sxs-lookup"><span data-stu-id="c159b-106">Methods</span></span>
|<span data-ttu-id="c159b-107">Метод</span><span class="sxs-lookup"><span data-stu-id="c159b-107">Method</span></span>|<span data-ttu-id="c159b-108">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="c159b-108">Return type</span></span>|<span data-ttu-id="c159b-109">Описание</span><span class="sxs-lookup"><span data-stu-id="c159b-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="c159b-110">Список cloudPcDevices</span><span class="sxs-lookup"><span data-stu-id="c159b-110">List cloudPcDevices</span></span>](../api/managedtenants-managedtenant-list-cloudpcdevices.md)|<span data-ttu-id="c159b-111">[коллекция microsoft.graph.managedTenants.cloudPcDevice](../resources/managedtenants-cloudpcdevice.md)</span><span class="sxs-lookup"><span data-stu-id="c159b-111">[microsoft.graph.managedTenants.cloudPcDevice](../resources/managedtenants-cloudpcdevice.md) collection</span></span>|<span data-ttu-id="c159b-112">Получите список объектов [cloudPcDevice](../resources/managedtenants-cloudpcdevice.md) и их свойств.</span><span class="sxs-lookup"><span data-stu-id="c159b-112">Get a list of the [cloudPcDevice](../resources/managedtenants-cloudpcdevice.md) objects and their properties.</span></span>|
|[<span data-ttu-id="c159b-113">Get cloudPcDevice</span><span class="sxs-lookup"><span data-stu-id="c159b-113">Get cloudPcDevice</span></span>](../api/managedtenants-cloudpcdevice-get.md)|[<span data-ttu-id="c159b-114">microsoft.graph.managedTenants.cloudPcDevice</span><span class="sxs-lookup"><span data-stu-id="c159b-114">microsoft.graph.managedTenants.cloudPcDevice</span></span>](../resources/managedtenants-cloudpcdevice.md)|<span data-ttu-id="c159b-115">Ознакомьтесь с свойствами и отношениями объекта [cloudPcDevice.](../resources/managedtenants-cloudpcdevice.md)</span><span class="sxs-lookup"><span data-stu-id="c159b-115">Read the properties and relationships of a [cloudPcDevice](../resources/managedtenants-cloudpcdevice.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="c159b-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="c159b-116">Properties</span></span>
|<span data-ttu-id="c159b-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="c159b-117">Property</span></span>|<span data-ttu-id="c159b-118">Тип</span><span class="sxs-lookup"><span data-stu-id="c159b-118">Type</span></span>|<span data-ttu-id="c159b-119">Описание</span><span class="sxs-lookup"><span data-stu-id="c159b-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c159b-120">cloudPcStatus</span><span class="sxs-lookup"><span data-stu-id="c159b-120">cloudPcStatus</span></span>|<span data-ttu-id="c159b-121">String</span><span class="sxs-lookup"><span data-stu-id="c159b-121">String</span></span>|<span data-ttu-id="c159b-122">Состояние облачного КОМПЬЮТЕРА.</span><span class="sxs-lookup"><span data-stu-id="c159b-122">The status of the cloud PC.</span></span> <span data-ttu-id="c159b-123">Возможные значения: `notProvisioned`, `provisioning`, `provisioned`, `upgrading`, `inGracePeriod`, `deprovisioning`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="c159b-123">Possible values are: `notProvisioned`, `provisioning`, `provisioned`, `upgrading`, `inGracePeriod`, `deprovisioning`, `failed`.</span></span> <span data-ttu-id="c159b-124">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c159b-124">Required.</span></span> <span data-ttu-id="c159b-125">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c159b-125">Read-only.</span></span>|
|<span data-ttu-id="c159b-126">displayName</span><span class="sxs-lookup"><span data-stu-id="c159b-126">displayName</span></span>|<span data-ttu-id="c159b-127">String</span><span class="sxs-lookup"><span data-stu-id="c159b-127">String</span></span>|<span data-ttu-id="c159b-128">Имя отображения облачного компьютера.</span><span class="sxs-lookup"><span data-stu-id="c159b-128">The display name for the cloud PC.</span></span> <span data-ttu-id="c159b-129">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c159b-129">Required.</span></span> <span data-ttu-id="c159b-130">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c159b-130">Read-only.</span></span>|
|<span data-ttu-id="c159b-131">id</span><span class="sxs-lookup"><span data-stu-id="c159b-131">id</span></span>|<span data-ttu-id="c159b-132">String</span><span class="sxs-lookup"><span data-stu-id="c159b-132">String</span></span>|<span data-ttu-id="c159b-133">Уникальный идентификатор облачного компьютера.</span><span class="sxs-lookup"><span data-stu-id="c159b-133">The unique identifier for the cloud PC.</span></span> <span data-ttu-id="c159b-134">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c159b-134">Required.</span></span> <span data-ttu-id="c159b-135">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c159b-135">Read-only.</span></span>|
|<span data-ttu-id="c159b-136">lastRefreshedDateTime</span><span class="sxs-lookup"><span data-stu-id="c159b-136">lastRefreshedDateTime</span></span>|<span data-ttu-id="c159b-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c159b-137">DateTimeOffset</span></span>|<span data-ttu-id="c159b-138">Дата и время последнего обновления объекта на платформе управления с несколькими клиентами.</span><span class="sxs-lookup"><span data-stu-id="c159b-138">Date and time the entity was last updated in the multi-tenant management platform.</span></span> <span data-ttu-id="c159b-139">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c159b-139">Required.</span></span> <span data-ttu-id="c159b-140">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c159b-140">Read-only.</span></span>|
|<span data-ttu-id="c159b-141">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="c159b-141">managedDeviceId</span></span>|<span data-ttu-id="c159b-142">String</span><span class="sxs-lookup"><span data-stu-id="c159b-142">String</span></span>|<span data-ttu-id="c159b-143">Идентификатор управляемого устройства для облачного КОМПЬЮТЕРА.</span><span class="sxs-lookup"><span data-stu-id="c159b-143">The managed device identifier for the cloud PC.</span></span> <span data-ttu-id="c159b-144">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="c159b-144">Optional.</span></span> <span data-ttu-id="c159b-145">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c159b-145">Read-only.</span></span>|
|<span data-ttu-id="c159b-146">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="c159b-146">managedDeviceName</span></span>|<span data-ttu-id="c159b-147">String</span><span class="sxs-lookup"><span data-stu-id="c159b-147">String</span></span>|<span data-ttu-id="c159b-148">Имя отображения управляемого устройства для облачного компьютера.</span><span class="sxs-lookup"><span data-stu-id="c159b-148">The managed device display name for the cloud PC.</span></span> <span data-ttu-id="c159b-149">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="c159b-149">Optional.</span></span> <span data-ttu-id="c159b-150">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c159b-150">Read-only.</span></span>|
|<span data-ttu-id="c159b-151">provisioningPolicyId</span><span class="sxs-lookup"><span data-stu-id="c159b-151">provisioningPolicyId</span></span>|<span data-ttu-id="c159b-152">String</span><span class="sxs-lookup"><span data-stu-id="c159b-152">String</span></span>|<span data-ttu-id="c159b-153">Идентификатор политики обеспечения для облачного компьютера.</span><span class="sxs-lookup"><span data-stu-id="c159b-153">The provisioning policy identifier for the cloud PC.</span></span> <span data-ttu-id="c159b-154">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c159b-154">Required.</span></span> <span data-ttu-id="c159b-155">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c159b-155">Read-only.</span></span>|
|<span data-ttu-id="c159b-156">servicePlanName</span><span class="sxs-lookup"><span data-stu-id="c159b-156">servicePlanName</span></span>|<span data-ttu-id="c159b-157">String</span><span class="sxs-lookup"><span data-stu-id="c159b-157">String</span></span>|<span data-ttu-id="c159b-158">Имя плана службы для облачного компьютера.</span><span class="sxs-lookup"><span data-stu-id="c159b-158">The service plan name for the cloud PC.</span></span> <span data-ttu-id="c159b-159">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c159b-159">Required.</span></span> <span data-ttu-id="c159b-160">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c159b-160">Read-only.</span></span>|
|<span data-ttu-id="c159b-161">tenantDisplayName</span><span class="sxs-lookup"><span data-stu-id="c159b-161">tenantDisplayName</span></span>|<span data-ttu-id="c159b-162">String</span><span class="sxs-lookup"><span data-stu-id="c159b-162">String</span></span>|<span data-ttu-id="c159b-163">Имя отображения управляемого клиента.</span><span class="sxs-lookup"><span data-stu-id="c159b-163">The display name for the managed tenant.</span></span> <span data-ttu-id="c159b-164">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c159b-164">Required.</span></span> <span data-ttu-id="c159b-165">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c159b-165">Read-only.</span></span>|
|<span data-ttu-id="c159b-166">tenantId</span><span class="sxs-lookup"><span data-stu-id="c159b-166">tenantId</span></span>|<span data-ttu-id="c159b-167">String</span><span class="sxs-lookup"><span data-stu-id="c159b-167">String</span></span>|<span data-ttu-id="c159b-168">Идентификатор Azure Active Directory клиента для [управляемого клиента.](../resources/managedtenants-tenant.md)</span><span class="sxs-lookup"><span data-stu-id="c159b-168">The Azure Active Directory tenant identifier for the [managed tenant](../resources/managedtenants-tenant.md).</span></span> <span data-ttu-id="c159b-169">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c159b-169">Required.</span></span> <span data-ttu-id="c159b-170">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c159b-170">Read-only.</span></span>|
|<span data-ttu-id="c159b-171">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="c159b-171">userPrincipalName</span></span>|<span data-ttu-id="c159b-172">String</span><span class="sxs-lookup"><span data-stu-id="c159b-172">String</span></span>|<span data-ttu-id="c159b-173">Основное имя пользователя (UPN) пользователя, назначенного на облачный КОМПЬЮТЕР.</span><span class="sxs-lookup"><span data-stu-id="c159b-173">The user principal name (UPN) of the user assigned to the cloud PC.</span></span> <span data-ttu-id="c159b-174">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c159b-174">Required.</span></span> <span data-ttu-id="c159b-175">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c159b-175">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c159b-176">Связи</span><span class="sxs-lookup"><span data-stu-id="c159b-176">Relationships</span></span>
<span data-ttu-id="c159b-177">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="c159b-177">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c159b-178">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="c159b-178">JSON representation</span></span>
<span data-ttu-id="c159b-179">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c159b-179">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedTenants.cloudPcDevice",
  "baseType": "microsoft.graph.entity",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.cloudPcDevice",
  "id": "String (identifier)",
  "displayName": "String",
  "tenantId": "String",
  "tenantDisplayName": "String",
  "managedDeviceId": "String",
  "managedDeviceName": "String",
  "userPrincipalName": "String",
  "servicePlanName": "String",
  "cloudPcStatus": "String",
  "provisioningPolicyId": "String",
  "lastRefreshedDateTime": "String (timestamp)"
}
```

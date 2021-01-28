---
title: Тип ресурса cloudPC
description: Виртуальные рабочие столы, управляемые облаком.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: 1b026bccd18af0dcbc9c0a5128595399a0997474
ms.sourcegitcommit: 9a03b719d1316729dd022bf4d268894e91515475
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/28/2021
ms.locfileid: "50033920"
---
# <a name="cloudpc-resource-type"></a><span data-ttu-id="2dfd4-103">Тип ресурса cloudPC</span><span class="sxs-lookup"><span data-stu-id="2dfd4-103">cloudPC resource type</span></span>

<span data-ttu-id="2dfd4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2dfd4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2dfd4-105">Представляет управляемый облаком виртуальный рабочий стол.</span><span class="sxs-lookup"><span data-stu-id="2dfd4-105">Represents a cloud-managed virtual desktop.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="methods"></a><span data-ttu-id="2dfd4-106">Методы</span><span class="sxs-lookup"><span data-stu-id="2dfd4-106">Methods</span></span>

|<span data-ttu-id="2dfd4-107">Метод</span><span class="sxs-lookup"><span data-stu-id="2dfd4-107">Method</span></span>|<span data-ttu-id="2dfd4-108">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="2dfd4-108">Return type</span></span>|<span data-ttu-id="2dfd4-109">Описание</span><span class="sxs-lookup"><span data-stu-id="2dfd4-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="2dfd4-110">Список cloudPCs</span><span class="sxs-lookup"><span data-stu-id="2dfd4-110">List cloudPCs</span></span>](../api/virtualendpoint-list-cloudpcs.md)|<span data-ttu-id="2dfd4-111">[Коллекция cloudPC](../resources/cloudpc.md)</span><span class="sxs-lookup"><span data-stu-id="2dfd4-111">[cloudPC](../resources/cloudpc.md) collection</span></span>|<span data-ttu-id="2dfd4-112">Список свойств и связей объектов [cloudPC.](../resources/cloudpc.md)</span><span class="sxs-lookup"><span data-stu-id="2dfd4-112">List properties and relationships of the [cloudPC](../resources/cloudpc.md) objects.</span></span>|
|[<span data-ttu-id="2dfd4-113">Get cloudPC</span><span class="sxs-lookup"><span data-stu-id="2dfd4-113">Get cloudPC</span></span>](../api/cloudpc-get.md)|[<span data-ttu-id="2dfd4-114">cloudPC</span><span class="sxs-lookup"><span data-stu-id="2dfd4-114">cloudPC</span></span>](../resources/cloudpc.md)|<span data-ttu-id="2dfd4-115">Чтение свойств и связей объекта [cloudPC.](../resources/cloudpc.md)</span><span class="sxs-lookup"><span data-stu-id="2dfd4-115">Read the properties and relationships of a [cloudPC](../resources/cloudpc.md) object.</span></span>|
|[<span data-ttu-id="2dfd4-116">Reprovision</span><span class="sxs-lookup"><span data-stu-id="2dfd4-116">Reprovision</span></span>](../api/cloudpc-reprovision.md)|<span data-ttu-id="2dfd4-117">Нет</span><span class="sxs-lookup"><span data-stu-id="2dfd4-117">None</span></span>|<span data-ttu-id="2dfd4-118">Повторное создание объекта [cloudPC.](../resources/cloudpc.md)</span><span class="sxs-lookup"><span data-stu-id="2dfd4-118">Reprovision a [cloudPC](../resources/cloudpc.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="2dfd4-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="2dfd4-119">Properties</span></span>

|<span data-ttu-id="2dfd4-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="2dfd4-120">Property</span></span>|<span data-ttu-id="2dfd4-121">Тип</span><span class="sxs-lookup"><span data-stu-id="2dfd4-121">Type</span></span>|<span data-ttu-id="2dfd4-122">Описание</span><span class="sxs-lookup"><span data-stu-id="2dfd4-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2dfd4-123">id</span><span class="sxs-lookup"><span data-stu-id="2dfd4-123">id</span></span>|<span data-ttu-id="2dfd4-124">String</span><span class="sxs-lookup"><span data-stu-id="2dfd4-124">String</span></span>|<span data-ttu-id="2dfd4-125">Уникальный идентификатор для облачного ПК.</span><span class="sxs-lookup"><span data-stu-id="2dfd4-125">Unique identifier for the cloud PC.</span></span> <span data-ttu-id="2dfd4-126">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2dfd4-126">Read-only.</span></span>|
|<span data-ttu-id="2dfd4-127">displayName</span><span class="sxs-lookup"><span data-stu-id="2dfd4-127">displayName</span></span>|<span data-ttu-id="2dfd4-128">String</span><span class="sxs-lookup"><span data-stu-id="2dfd4-128">String</span></span>|<span data-ttu-id="2dfd4-129">Отображаемая версия облачного компьютера.</span><span class="sxs-lookup"><span data-stu-id="2dfd4-129">The cloud PC display name.</span></span>|
|<span data-ttu-id="2dfd4-130">imageDisplayName</span><span class="sxs-lookup"><span data-stu-id="2dfd4-130">imageDisplayName</span></span>|<span data-ttu-id="2dfd4-131">String</span><span class="sxs-lookup"><span data-stu-id="2dfd4-131">String</span></span>|<span data-ttu-id="2dfd4-132">Имя образа ОС на облачном компьютере.</span><span class="sxs-lookup"><span data-stu-id="2dfd4-132">Name of the OS image that's on the cloud PC.</span></span>|
|<span data-ttu-id="2dfd4-133">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="2dfd4-133">managedDeviceId</span></span>|<span data-ttu-id="2dfd4-134">String</span><span class="sxs-lookup"><span data-stu-id="2dfd4-134">String</span></span>|<span data-ttu-id="2dfd4-135">ИД устройства Intune на облачном компьютере.</span><span class="sxs-lookup"><span data-stu-id="2dfd4-135">The cloud PC’s Intune device ID.</span></span>|
|<span data-ttu-id="2dfd4-136">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="2dfd4-136">managedDeviceName</span></span>|<span data-ttu-id="2dfd4-137">String</span><span class="sxs-lookup"><span data-stu-id="2dfd4-137">String</span></span>|<span data-ttu-id="2dfd4-138">Имя устройства Intune облачного ПК.</span><span class="sxs-lookup"><span data-stu-id="2dfd4-138">The cloud PC’s Intune device name.</span></span>|
|<span data-ttu-id="2dfd4-139">provisioningPolicyId</span><span class="sxs-lookup"><span data-stu-id="2dfd4-139">provisioningPolicyId</span></span>|<span data-ttu-id="2dfd4-140">String</span><span class="sxs-lookup"><span data-stu-id="2dfd4-140">String</span></span>|<span data-ttu-id="2dfd4-141">ИД политики предоставления на облачном компьютере.</span><span class="sxs-lookup"><span data-stu-id="2dfd4-141">The cloud PC's provisioning policy ID.</span></span>|
|<span data-ttu-id="2dfd4-142">servicePlanId</span><span class="sxs-lookup"><span data-stu-id="2dfd4-142">servicePlanId</span></span>|<span data-ttu-id="2dfd4-143">String</span><span class="sxs-lookup"><span data-stu-id="2dfd4-143">String</span></span>|<span data-ttu-id="2dfd4-144">ИД плана обслуживания облачного ПК.</span><span class="sxs-lookup"><span data-stu-id="2dfd4-144">The cloud PC's service plan ID.</span></span>|
|<span data-ttu-id="2dfd4-145">servicePlanName</span><span class="sxs-lookup"><span data-stu-id="2dfd4-145">servicePlanName</span></span>|<span data-ttu-id="2dfd4-146">String</span><span class="sxs-lookup"><span data-stu-id="2dfd4-146">String</span></span>|<span data-ttu-id="2dfd4-147">Имя плана обслуживания облачного ПК.</span><span class="sxs-lookup"><span data-stu-id="2dfd4-147">The cloud PC's service plan name.</span></span>|
|<span data-ttu-id="2dfd4-148">status</span><span class="sxs-lookup"><span data-stu-id="2dfd4-148">status</span></span>|[<span data-ttu-id="2dfd4-149">cloudPcStatus</span><span class="sxs-lookup"><span data-stu-id="2dfd4-149">cloudPcStatus</span></span>](#cloudpcstatus-values)|<span data-ttu-id="2dfd4-150">Состояние облачного ПК.</span><span class="sxs-lookup"><span data-stu-id="2dfd4-150">Status of the cloud PC.</span></span> <span data-ttu-id="2dfd4-151">Возможные значения: `notProvisioned`, `provisioning`, `provisioned`, `upgrading`, `inGracePeriod`, `deprovisioning`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="2dfd4-151">Possible values are: `notProvisioned`, `provisioning`, `provisioned`, `upgrading`, `inGracePeriod`, `deprovisioning`, `failed`.</span></span>|
|<span data-ttu-id="2dfd4-152">statusDetails</span><span class="sxs-lookup"><span data-stu-id="2dfd4-152">statusDetails</span></span>|[<span data-ttu-id="2dfd4-153">cloudPcStatusDetails</span><span class="sxs-lookup"><span data-stu-id="2dfd4-153">cloudPcStatusDetails</span></span>](../resources/cloudpcstatusdetails.md)|<span data-ttu-id="2dfd4-154">Сведения о состоянии облачного ПК.</span><span class="sxs-lookup"><span data-stu-id="2dfd4-154">The details of the cloud PC status.</span></span>|
|<span data-ttu-id="2dfd4-155">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="2dfd4-155">userPrincipalName</span></span>|<span data-ttu-id="2dfd4-156">String</span><span class="sxs-lookup"><span data-stu-id="2dfd4-156">String</span></span>|<span data-ttu-id="2dfd4-157">Имя основного пользователя (UPN) пользователя, назначенного облачному компьютеру.</span><span class="sxs-lookup"><span data-stu-id="2dfd4-157">The user principal name (UPN) of the user assigned to the cloud PC.</span></span>|
|<span data-ttu-id="2dfd4-158">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2dfd4-158">lastModifiedDateTime</span></span>|<span data-ttu-id="2dfd4-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2dfd4-159">DateTimeOffset</span></span>|<span data-ttu-id="2dfd4-160">Дата и время последнего изменения облачного ПК.</span><span class="sxs-lookup"><span data-stu-id="2dfd4-160">The cloud PC's last modified date and time.</span></span> <span data-ttu-id="2dfd4-161">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="2dfd4-161">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="2dfd4-162">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: "2014-01-01T00:00:00Z".</span><span class="sxs-lookup"><span data-stu-id="2dfd4-162">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span>|

### <a name="cloudpcstatus-values"></a><span data-ttu-id="2dfd4-163">Значения cloudPcStatus</span><span class="sxs-lookup"><span data-stu-id="2dfd4-163">cloudPcStatus values</span></span>

|<span data-ttu-id="2dfd4-164">Member</span><span class="sxs-lookup"><span data-stu-id="2dfd4-164">Member</span></span>|<span data-ttu-id="2dfd4-165">Описание</span><span class="sxs-lookup"><span data-stu-id="2dfd4-165">Description</span></span>|
|:---|:---|
|<span data-ttu-id="2dfd4-166">notProvisioned</span><span class="sxs-lookup"><span data-stu-id="2dfd4-166">notProvisioned</span></span>|<span data-ttu-id="2dfd4-167">Облачный КОМПЬЮТЕР не был предусмотрен.</span><span class="sxs-lookup"><span data-stu-id="2dfd4-167">The Cloud PC hasn’t been provisioned.</span></span>|
|<span data-ttu-id="2dfd4-168">подготовка</span><span class="sxs-lookup"><span data-stu-id="2dfd4-168">provisioning</span></span>|<span data-ttu-id="2dfd4-169">Подготовка облачных компьютеров идет.</span><span class="sxs-lookup"><span data-stu-id="2dfd4-169">Cloud PC provisioning is in progress.</span></span>|
|<span data-ttu-id="2dfd4-170">provisioned</span><span class="sxs-lookup"><span data-stu-id="2dfd4-170">provisioned</span></span>|<span data-ttu-id="2dfd4-171">Облачный компьютер уже предусмотрен и к нему могут получить доступ конечные пользователи.</span><span class="sxs-lookup"><span data-stu-id="2dfd4-171">The Cloud PC is provisioned and can be accessed by end users.</span></span>|
|<span data-ttu-id="2dfd4-172">обновление</span><span class="sxs-lookup"><span data-stu-id="2dfd4-172">upgrading</span></span>|<span data-ttu-id="2dfd4-173">В настоящее время идет процесс добиться их добиться.</span><span class="sxs-lookup"><span data-stu-id="2dfd4-173">Cloud PC resize is in progress.</span></span>|
|<span data-ttu-id="2dfd4-174">inGracePeriod</span><span class="sxs-lookup"><span data-stu-id="2dfd4-174">inGracePeriod</span></span>|<span data-ttu-id="2dfd4-175">Облачный пк находится в течение одной недели льготного периода, прежде чем он будет отсюжен.</span><span class="sxs-lookup"><span data-stu-id="2dfd4-175">The Cloud PC is in the one week grace period before it’s deprovisioned.</span></span>|
|<span data-ttu-id="2dfd4-176">deprovisioning</span><span class="sxs-lookup"><span data-stu-id="2dfd4-176">deprovisioning</span></span>|<span data-ttu-id="2dfd4-177">Облачный КОМПЬЮТЕР не подает продукты.</span><span class="sxs-lookup"><span data-stu-id="2dfd4-177">The Cloud PC is deprovisioning.</span></span>|
|<span data-ttu-id="2dfd4-178">failed</span><span class="sxs-lookup"><span data-stu-id="2dfd4-178">failed</span></span>|<span data-ttu-id="2dfd4-179">Сбой операции на облачном компьютере.</span><span class="sxs-lookup"><span data-stu-id="2dfd4-179">The operation on Cloud PC has failed.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2dfd4-180">Связи</span><span class="sxs-lookup"><span data-stu-id="2dfd4-180">Relationships</span></span>

<span data-ttu-id="2dfd4-181">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="2dfd4-181">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="2dfd4-182">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="2dfd4-182">JSON representation</span></span>

<span data-ttu-id="2dfd4-183">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2dfd4-183">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.cloudPC",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.cloudPC",
  "id": "String (identifier)",
  "displayName": "String",
  "imageDisplayName": "String",
  "managedDeviceId": "String",
  "managedDeviceName": "String",
  "provisioningPolicyId": "String",
  "servicePlanId": "String",
  "servicePlanName": "String",
  "status": "String",
  "userPrincipalName": "String",
  "lastModifiedDateTime": "String (timestamp)"
}
```

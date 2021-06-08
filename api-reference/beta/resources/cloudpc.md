---
title: Тип ресурса cloudPC
description: Облачные управляемые виртуальные настольные компьютеры.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: 232ad6a8de6634f028ec59080114110c902ce184
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/06/2021
ms.locfileid: "52787501"
---
# <a name="cloudpc-resource-type"></a><span data-ttu-id="b3138-103">Тип ресурса cloudPC</span><span class="sxs-lookup"><span data-stu-id="b3138-103">cloudPC resource type</span></span>

<span data-ttu-id="b3138-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b3138-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b3138-105">Представляет виртуальный рабочий стол с облачным управлением.</span><span class="sxs-lookup"><span data-stu-id="b3138-105">Represents a cloud-managed virtual desktop.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="methods"></a><span data-ttu-id="b3138-106">Методы</span><span class="sxs-lookup"><span data-stu-id="b3138-106">Methods</span></span>

|<span data-ttu-id="b3138-107">Метод</span><span class="sxs-lookup"><span data-stu-id="b3138-107">Method</span></span>|<span data-ttu-id="b3138-108">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="b3138-108">Return type</span></span>|<span data-ttu-id="b3138-109">Описание</span><span class="sxs-lookup"><span data-stu-id="b3138-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="b3138-110">CloudPCs списка</span><span class="sxs-lookup"><span data-stu-id="b3138-110">List cloudPCs</span></span>](../api/virtualendpoint-list-cloudpcs.md)|<span data-ttu-id="b3138-111">[коллекция cloudPC](../resources/cloudpc.md)</span><span class="sxs-lookup"><span data-stu-id="b3138-111">[cloudPC](../resources/cloudpc.md) collection</span></span>|<span data-ttu-id="b3138-112">Список свойств и связей объектов [cloudPC.](../resources/cloudpc.md)</span><span class="sxs-lookup"><span data-stu-id="b3138-112">List properties and relationships of the [cloudPC](../resources/cloudpc.md) objects.</span></span>|
|[<span data-ttu-id="b3138-113">Get cloudPC</span><span class="sxs-lookup"><span data-stu-id="b3138-113">Get cloudPC</span></span>](../api/cloudpc-get.md)|[<span data-ttu-id="b3138-114">cloudPC</span><span class="sxs-lookup"><span data-stu-id="b3138-114">cloudPC</span></span>](../resources/cloudpc.md)|<span data-ttu-id="b3138-115">Ознакомьтесь с свойствами и отношениями объекта [cloudPC.](../resources/cloudpc.md)</span><span class="sxs-lookup"><span data-stu-id="b3138-115">Read the properties and relationships of a [cloudPC](../resources/cloudpc.md) object.</span></span>|
|[<span data-ttu-id="b3138-116">Reprovision</span><span class="sxs-lookup"><span data-stu-id="b3138-116">Reprovision</span></span>](../api/cloudpc-reprovision.md)|<span data-ttu-id="b3138-117">Нет</span><span class="sxs-lookup"><span data-stu-id="b3138-117">None</span></span>|<span data-ttu-id="b3138-118">Reprovision a [cloudPC](../resources/cloudpc.md) object.</span><span class="sxs-lookup"><span data-stu-id="b3138-118">Reprovision a [cloudPC](../resources/cloudpc.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="b3138-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="b3138-119">Properties</span></span>

|<span data-ttu-id="b3138-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="b3138-120">Property</span></span>|<span data-ttu-id="b3138-121">Тип</span><span class="sxs-lookup"><span data-stu-id="b3138-121">Type</span></span>|<span data-ttu-id="b3138-122">Описание</span><span class="sxs-lookup"><span data-stu-id="b3138-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b3138-123">id</span><span class="sxs-lookup"><span data-stu-id="b3138-123">id</span></span>|<span data-ttu-id="b3138-124">String</span><span class="sxs-lookup"><span data-stu-id="b3138-124">String</span></span>|<span data-ttu-id="b3138-125">Уникальный идентификатор для облачного КОМПЬЮТЕРА.</span><span class="sxs-lookup"><span data-stu-id="b3138-125">Unique identifier for the cloud PC.</span></span> <span data-ttu-id="b3138-126">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b3138-126">Read-only.</span></span>|
|<span data-ttu-id="b3138-127">displayName</span><span class="sxs-lookup"><span data-stu-id="b3138-127">displayName</span></span>|<span data-ttu-id="b3138-128">String</span><span class="sxs-lookup"><span data-stu-id="b3138-128">String</span></span>|<span data-ttu-id="b3138-129">Имя отображения облачного КОМПЬЮТЕРА.</span><span class="sxs-lookup"><span data-stu-id="b3138-129">The cloud PC display name.</span></span>|
|<span data-ttu-id="b3138-130">imageDisplayName</span><span class="sxs-lookup"><span data-stu-id="b3138-130">imageDisplayName</span></span>|<span data-ttu-id="b3138-131">String</span><span class="sxs-lookup"><span data-stu-id="b3138-131">String</span></span>|<span data-ttu-id="b3138-132">Имя изображения ОС на облачном компьютере.</span><span class="sxs-lookup"><span data-stu-id="b3138-132">Name of the OS image that's on the cloud PC.</span></span>|
|<span data-ttu-id="b3138-133">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="b3138-133">managedDeviceId</span></span>|<span data-ttu-id="b3138-134">String</span><span class="sxs-lookup"><span data-stu-id="b3138-134">String</span></span>|<span data-ttu-id="b3138-135">ID устройства Intune облачного компьютера.</span><span class="sxs-lookup"><span data-stu-id="b3138-135">The cloud PC’s Intune device ID.</span></span>|
|<span data-ttu-id="b3138-136">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="b3138-136">managedDeviceName</span></span>|<span data-ttu-id="b3138-137">String</span><span class="sxs-lookup"><span data-stu-id="b3138-137">String</span></span>|<span data-ttu-id="b3138-138">Имя устройства Intune облачного КОМПЬЮТЕРА.</span><span class="sxs-lookup"><span data-stu-id="b3138-138">The cloud PC’s Intune device name.</span></span>|
|<span data-ttu-id="b3138-139">provisioningPolicyId</span><span class="sxs-lookup"><span data-stu-id="b3138-139">provisioningPolicyId</span></span>|<span data-ttu-id="b3138-140">String</span><span class="sxs-lookup"><span data-stu-id="b3138-140">String</span></span>|<span data-ttu-id="b3138-141">ID политики обеспечения облачного компьютера.</span><span class="sxs-lookup"><span data-stu-id="b3138-141">The cloud PC's provisioning policy ID.</span></span>|
|<span data-ttu-id="b3138-142">provisioningPolicyName</span><span class="sxs-lookup"><span data-stu-id="b3138-142">provisioningPolicyName</span></span>|<span data-ttu-id="b3138-143">String</span><span class="sxs-lookup"><span data-stu-id="b3138-143">String</span></span>|<span data-ttu-id="b3138-144">Политика обеспечения, применяемая при обеспечении облачных компьютеров.</span><span class="sxs-lookup"><span data-stu-id="b3138-144">The provisioning policy that is applied during provisioning of cloud PCs.</span></span>|
|<span data-ttu-id="b3138-145">onPremisesConnectionName</span><span class="sxs-lookup"><span data-stu-id="b3138-145">onPremisesConnectionName</span></span>|<span data-ttu-id="b3138-146">String</span><span class="sxs-lookup"><span data-stu-id="b3138-146">String</span></span>|<span data-ttu-id="b3138-147">Локальное подключение, применяемого при обеспечении облачных компьютеров.</span><span class="sxs-lookup"><span data-stu-id="b3138-147">The on-premises connection that is applied during provisioning of cloud PCs.</span></span>|
|<span data-ttu-id="b3138-148">servicePlanId</span><span class="sxs-lookup"><span data-stu-id="b3138-148">servicePlanId</span></span>|<span data-ttu-id="b3138-149">String</span><span class="sxs-lookup"><span data-stu-id="b3138-149">String</span></span>|<span data-ttu-id="b3138-150">ID плана службы облачного КОМПЬЮТЕРА.</span><span class="sxs-lookup"><span data-stu-id="b3138-150">The cloud PC's service plan ID.</span></span>|
|<span data-ttu-id="b3138-151">servicePlanName</span><span class="sxs-lookup"><span data-stu-id="b3138-151">servicePlanName</span></span>|<span data-ttu-id="b3138-152">String</span><span class="sxs-lookup"><span data-stu-id="b3138-152">String</span></span>|<span data-ttu-id="b3138-153">Имя плана службы облачного КОМПЬЮТЕРА.</span><span class="sxs-lookup"><span data-stu-id="b3138-153">The cloud PC's service plan name.</span></span>|
|<span data-ttu-id="b3138-154">status</span><span class="sxs-lookup"><span data-stu-id="b3138-154">status</span></span>|[<span data-ttu-id="b3138-155">cloudPcStatus</span><span class="sxs-lookup"><span data-stu-id="b3138-155">cloudPcStatus</span></span>](#cloudpcstatus-values)|<span data-ttu-id="b3138-156">Состояние облачного КОМПЬЮТЕРА.</span><span class="sxs-lookup"><span data-stu-id="b3138-156">Status of the cloud PC.</span></span> <span data-ttu-id="b3138-157">Возможные значения: `notProvisioned`, `provisioning`, `provisioned`, `upgrading`, `inGracePeriod`, `deprovisioning`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="b3138-157">Possible values are: `notProvisioned`, `provisioning`, `provisioned`, `upgrading`, `inGracePeriod`, `deprovisioning`, `failed`.</span></span>|
|<span data-ttu-id="b3138-158">statusDetails</span><span class="sxs-lookup"><span data-stu-id="b3138-158">statusDetails</span></span>|[<span data-ttu-id="b3138-159">cloudPcStatusDetails</span><span class="sxs-lookup"><span data-stu-id="b3138-159">cloudPcStatusDetails</span></span>](../resources/cloudpcstatusdetails.md)|<span data-ttu-id="b3138-160">Сведения о состоянии облачного КОМПЬЮТЕРА.</span><span class="sxs-lookup"><span data-stu-id="b3138-160">The details of the cloud PC status.</span></span>|
|<span data-ttu-id="b3138-161">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="b3138-161">userPrincipalName</span></span>|<span data-ttu-id="b3138-162">String</span><span class="sxs-lookup"><span data-stu-id="b3138-162">String</span></span>|<span data-ttu-id="b3138-163">Основное имя пользователя (UPN) пользователя, назначенного на облачный КОМПЬЮТЕР.</span><span class="sxs-lookup"><span data-stu-id="b3138-163">The user principal name (UPN) of the user assigned to the cloud PC.</span></span>|
|<span data-ttu-id="b3138-164">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b3138-164">lastModifiedDateTime</span></span>|<span data-ttu-id="b3138-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b3138-165">DateTimeOffset</span></span>|<span data-ttu-id="b3138-166">Последняя измененная дата и время облачного компьютера.</span><span class="sxs-lookup"><span data-stu-id="b3138-166">The cloud PC's last modified date and time.</span></span> <span data-ttu-id="b3138-167">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="b3138-167">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="b3138-168">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="b3138-168">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span>|
|<span data-ttu-id="b3138-169">gracePeriodEndDateTime</span><span class="sxs-lookup"><span data-stu-id="b3138-169">gracePeriodEndDateTime</span></span>|<span data-ttu-id="b3138-170">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b3138-170">DateTimeOffset</span></span>|<span data-ttu-id="b3138-171">Дата и время окончания льготного периода и переделки/депрограммивинга.</span><span class="sxs-lookup"><span data-stu-id="b3138-171">The date and time when the grace period ends and reprovisioning/deprovisioning happens.</span></span> <span data-ttu-id="b3138-172">Требуется только в том случае, если состояние `inGracePeriod` .</span><span class="sxs-lookup"><span data-stu-id="b3138-172">Required only if status is `inGracePeriod`.</span></span> <span data-ttu-id="b3138-173">Timestamp отображается в формате ISO 8601 и Скоординированное универсальное время (UTC).</span><span class="sxs-lookup"><span data-stu-id="b3138-173">The timestamp is shown in ISO 8601 format and Coordinated Universal Time (UTC).</span></span> <span data-ttu-id="b3138-174">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="b3138-174">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span>|

### <a name="cloudpcstatus-values"></a><span data-ttu-id="b3138-175">значения cloudPcStatus</span><span class="sxs-lookup"><span data-stu-id="b3138-175">cloudPcStatus values</span></span>

|<span data-ttu-id="b3138-176">Member</span><span class="sxs-lookup"><span data-stu-id="b3138-176">Member</span></span>|<span data-ttu-id="b3138-177">Описание</span><span class="sxs-lookup"><span data-stu-id="b3138-177">Description</span></span>|
|:---|:---|
|<span data-ttu-id="b3138-178">notProvisioned</span><span class="sxs-lookup"><span data-stu-id="b3138-178">notProvisioned</span></span>|<span data-ttu-id="b3138-179">Этот Cloud PC не был предварительно.</span><span class="sxs-lookup"><span data-stu-id="b3138-179">The Cloud PC hasn’t been provisioned.</span></span>|
|<span data-ttu-id="b3138-180">подготовка</span><span class="sxs-lookup"><span data-stu-id="b3138-180">provisioning</span></span>|<span data-ttu-id="b3138-181">Cloud PC подготовка продолжается.</span><span class="sxs-lookup"><span data-stu-id="b3138-181">Cloud PC provisioning is in progress.</span></span>|
|<span data-ttu-id="b3138-182">provisioned</span><span class="sxs-lookup"><span data-stu-id="b3138-182">provisioned</span></span>|<span data-ttu-id="b3138-183">Подготовка Cloud PC и доступ к нему могут получить конечные пользователи.</span><span class="sxs-lookup"><span data-stu-id="b3138-183">The Cloud PC is provisioned and can be accessed by end users.</span></span>|
|<span data-ttu-id="b3138-184">обновление</span><span class="sxs-lookup"><span data-stu-id="b3138-184">upgrading</span></span>|<span data-ttu-id="b3138-185">Cloud PC продолжается.</span><span class="sxs-lookup"><span data-stu-id="b3138-185">Cloud PC resize is in progress.</span></span>|
|<span data-ttu-id="b3138-186">inGracePeriod</span><span class="sxs-lookup"><span data-stu-id="b3138-186">inGracePeriod</span></span>|<span data-ttu-id="b3138-187">Срок Cloud PC находится в периоде отсрочки за одну неделю до его деразвения.</span><span class="sxs-lookup"><span data-stu-id="b3138-187">The Cloud PC is in the one week grace period before it’s deprovisioned.</span></span>|
|<span data-ttu-id="b3138-188">deprovisioning</span><span class="sxs-lookup"><span data-stu-id="b3138-188">deprovisioning</span></span>|<span data-ttu-id="b3138-189">The Cloud PC deprovisioning.</span><span class="sxs-lookup"><span data-stu-id="b3138-189">The Cloud PC is deprovisioning.</span></span>|
|<span data-ttu-id="b3138-190">не удалось</span><span class="sxs-lookup"><span data-stu-id="b3138-190">failed</span></span>|<span data-ttu-id="b3138-191">Операция на Cloud PC не удалась.</span><span class="sxs-lookup"><span data-stu-id="b3138-191">The operation on Cloud PC has failed.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b3138-192">Связи</span><span class="sxs-lookup"><span data-stu-id="b3138-192">Relationships</span></span>

<span data-ttu-id="b3138-193">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="b3138-193">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b3138-194">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="b3138-194">JSON representation</span></span>

<span data-ttu-id="b3138-195">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b3138-195">The following is a JSON representation of the resource.</span></span>
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
  "provisioningPolicyName": "String",
  "onPremisesConnectionName": "String",
  "servicePlanId": "String",
  "servicePlanName": "String",
  "status": "String",
  "userPrincipalName": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "gracePeriodEndDateTime": "String (timestamp)"
}
```

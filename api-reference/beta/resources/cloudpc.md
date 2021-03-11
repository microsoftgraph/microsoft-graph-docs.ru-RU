---
title: Тип ресурса cloudPC
description: Облачные управляемые виртуальные настольные компьютеры.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: c5fc858e29abf7d649b32991d9e30ce64cc0b632
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50721616"
---
# <a name="cloudpc-resource-type"></a><span data-ttu-id="c2aea-103">Тип ресурса cloudPC</span><span class="sxs-lookup"><span data-stu-id="c2aea-103">cloudPC resource type</span></span>

<span data-ttu-id="c2aea-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c2aea-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c2aea-105">Представляет виртуальный рабочий стол с облачным управлением.</span><span class="sxs-lookup"><span data-stu-id="c2aea-105">Represents a cloud-managed virtual desktop.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="methods"></a><span data-ttu-id="c2aea-106">Методы</span><span class="sxs-lookup"><span data-stu-id="c2aea-106">Methods</span></span>

|<span data-ttu-id="c2aea-107">Метод</span><span class="sxs-lookup"><span data-stu-id="c2aea-107">Method</span></span>|<span data-ttu-id="c2aea-108">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="c2aea-108">Return type</span></span>|<span data-ttu-id="c2aea-109">Описание</span><span class="sxs-lookup"><span data-stu-id="c2aea-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="c2aea-110">CloudPCs списка</span><span class="sxs-lookup"><span data-stu-id="c2aea-110">List cloudPCs</span></span>](../api/virtualendpoint-list-cloudpcs.md)|<span data-ttu-id="c2aea-111">[коллекция cloudPC](../resources/cloudpc.md)</span><span class="sxs-lookup"><span data-stu-id="c2aea-111">[cloudPC](../resources/cloudpc.md) collection</span></span>|<span data-ttu-id="c2aea-112">Список свойств и связей объектов [cloudPC.](../resources/cloudpc.md)</span><span class="sxs-lookup"><span data-stu-id="c2aea-112">List properties and relationships of the [cloudPC](../resources/cloudpc.md) objects.</span></span>|
|[<span data-ttu-id="c2aea-113">Get cloudPC</span><span class="sxs-lookup"><span data-stu-id="c2aea-113">Get cloudPC</span></span>](../api/cloudpc-get.md)|[<span data-ttu-id="c2aea-114">cloudPC</span><span class="sxs-lookup"><span data-stu-id="c2aea-114">cloudPC</span></span>](../resources/cloudpc.md)|<span data-ttu-id="c2aea-115">Ознакомьтесь с свойствами и отношениями объекта [cloudPC.](../resources/cloudpc.md)</span><span class="sxs-lookup"><span data-stu-id="c2aea-115">Read the properties and relationships of a [cloudPC](../resources/cloudpc.md) object.</span></span>|
|[<span data-ttu-id="c2aea-116">Reprovision</span><span class="sxs-lookup"><span data-stu-id="c2aea-116">Reprovision</span></span>](../api/cloudpc-reprovision.md)|<span data-ttu-id="c2aea-117">Нет</span><span class="sxs-lookup"><span data-stu-id="c2aea-117">None</span></span>|<span data-ttu-id="c2aea-118">Reprovision a [cloudPC](../resources/cloudpc.md) object.</span><span class="sxs-lookup"><span data-stu-id="c2aea-118">Reprovision a [cloudPC](../resources/cloudpc.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="c2aea-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="c2aea-119">Properties</span></span>

|<span data-ttu-id="c2aea-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="c2aea-120">Property</span></span>|<span data-ttu-id="c2aea-121">Тип</span><span class="sxs-lookup"><span data-stu-id="c2aea-121">Type</span></span>|<span data-ttu-id="c2aea-122">Описание</span><span class="sxs-lookup"><span data-stu-id="c2aea-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c2aea-123">id</span><span class="sxs-lookup"><span data-stu-id="c2aea-123">id</span></span>|<span data-ttu-id="c2aea-124">String</span><span class="sxs-lookup"><span data-stu-id="c2aea-124">String</span></span>|<span data-ttu-id="c2aea-125">Уникальный идентификатор для облачного КОМПЬЮТЕРА.</span><span class="sxs-lookup"><span data-stu-id="c2aea-125">Unique identifier for the cloud PC.</span></span> <span data-ttu-id="c2aea-126">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c2aea-126">Read-only.</span></span>|
|<span data-ttu-id="c2aea-127">displayName</span><span class="sxs-lookup"><span data-stu-id="c2aea-127">displayName</span></span>|<span data-ttu-id="c2aea-128">String</span><span class="sxs-lookup"><span data-stu-id="c2aea-128">String</span></span>|<span data-ttu-id="c2aea-129">Имя отображения облачного КОМПЬЮТЕРА.</span><span class="sxs-lookup"><span data-stu-id="c2aea-129">The cloud PC display name.</span></span>|
|<span data-ttu-id="c2aea-130">imageDisplayName</span><span class="sxs-lookup"><span data-stu-id="c2aea-130">imageDisplayName</span></span>|<span data-ttu-id="c2aea-131">String</span><span class="sxs-lookup"><span data-stu-id="c2aea-131">String</span></span>|<span data-ttu-id="c2aea-132">Имя изображения ОС на облачном компьютере.</span><span class="sxs-lookup"><span data-stu-id="c2aea-132">Name of the OS image that's on the cloud PC.</span></span>|
|<span data-ttu-id="c2aea-133">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="c2aea-133">managedDeviceId</span></span>|<span data-ttu-id="c2aea-134">String</span><span class="sxs-lookup"><span data-stu-id="c2aea-134">String</span></span>|<span data-ttu-id="c2aea-135">ID устройства Intune облачного компьютера.</span><span class="sxs-lookup"><span data-stu-id="c2aea-135">The cloud PC’s Intune device ID.</span></span>|
|<span data-ttu-id="c2aea-136">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="c2aea-136">managedDeviceName</span></span>|<span data-ttu-id="c2aea-137">String</span><span class="sxs-lookup"><span data-stu-id="c2aea-137">String</span></span>|<span data-ttu-id="c2aea-138">Имя устройства Intune облачного КОМПЬЮТЕРА.</span><span class="sxs-lookup"><span data-stu-id="c2aea-138">The cloud PC’s Intune device name.</span></span>|
|<span data-ttu-id="c2aea-139">provisioningPolicyId</span><span class="sxs-lookup"><span data-stu-id="c2aea-139">provisioningPolicyId</span></span>|<span data-ttu-id="c2aea-140">String</span><span class="sxs-lookup"><span data-stu-id="c2aea-140">String</span></span>|<span data-ttu-id="c2aea-141">ID политики обеспечения облачного компьютера.</span><span class="sxs-lookup"><span data-stu-id="c2aea-141">The cloud PC's provisioning policy ID.</span></span>|
|<span data-ttu-id="c2aea-142">servicePlanId</span><span class="sxs-lookup"><span data-stu-id="c2aea-142">servicePlanId</span></span>|<span data-ttu-id="c2aea-143">String</span><span class="sxs-lookup"><span data-stu-id="c2aea-143">String</span></span>|<span data-ttu-id="c2aea-144">ID плана службы облачного КОМПЬЮТЕРА.</span><span class="sxs-lookup"><span data-stu-id="c2aea-144">The cloud PC's service plan ID.</span></span>|
|<span data-ttu-id="c2aea-145">servicePlanName</span><span class="sxs-lookup"><span data-stu-id="c2aea-145">servicePlanName</span></span>|<span data-ttu-id="c2aea-146">String</span><span class="sxs-lookup"><span data-stu-id="c2aea-146">String</span></span>|<span data-ttu-id="c2aea-147">Имя плана службы облачного КОМПЬЮТЕРА.</span><span class="sxs-lookup"><span data-stu-id="c2aea-147">The cloud PC's service plan name.</span></span>|
|<span data-ttu-id="c2aea-148">status</span><span class="sxs-lookup"><span data-stu-id="c2aea-148">status</span></span>|[<span data-ttu-id="c2aea-149">cloudPcStatus</span><span class="sxs-lookup"><span data-stu-id="c2aea-149">cloudPcStatus</span></span>](#cloudpcstatus-values)|<span data-ttu-id="c2aea-150">Состояние облачного КОМПЬЮТЕРА.</span><span class="sxs-lookup"><span data-stu-id="c2aea-150">Status of the cloud PC.</span></span> <span data-ttu-id="c2aea-151">Возможные значения: `notProvisioned`, `provisioning`, `provisioned`, `upgrading`, `inGracePeriod`, `deprovisioning`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="c2aea-151">Possible values are: `notProvisioned`, `provisioning`, `provisioned`, `upgrading`, `inGracePeriod`, `deprovisioning`, `failed`.</span></span>|
|<span data-ttu-id="c2aea-152">statusDetails</span><span class="sxs-lookup"><span data-stu-id="c2aea-152">statusDetails</span></span>|[<span data-ttu-id="c2aea-153">cloudPcStatusDetails</span><span class="sxs-lookup"><span data-stu-id="c2aea-153">cloudPcStatusDetails</span></span>](../resources/cloudpcstatusdetails.md)|<span data-ttu-id="c2aea-154">Сведения о состоянии облачного КОМПЬЮТЕРА.</span><span class="sxs-lookup"><span data-stu-id="c2aea-154">The details of the cloud PC status.</span></span>|
|<span data-ttu-id="c2aea-155">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="c2aea-155">userPrincipalName</span></span>|<span data-ttu-id="c2aea-156">String</span><span class="sxs-lookup"><span data-stu-id="c2aea-156">String</span></span>|<span data-ttu-id="c2aea-157">Основное имя пользователя (UPN) пользователя, назначенного на облачный КОМПЬЮТЕР.</span><span class="sxs-lookup"><span data-stu-id="c2aea-157">The user principal name (UPN) of the user assigned to the cloud PC.</span></span>|
|<span data-ttu-id="c2aea-158">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c2aea-158">lastModifiedDateTime</span></span>|<span data-ttu-id="c2aea-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c2aea-159">DateTimeOffset</span></span>|<span data-ttu-id="c2aea-160">Последняя измененная дата и время облачного компьютера.</span><span class="sxs-lookup"><span data-stu-id="c2aea-160">The cloud PC's last modified date and time.</span></span> <span data-ttu-id="c2aea-161">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="c2aea-161">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="c2aea-162">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="c2aea-162">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span>|

### <a name="cloudpcstatus-values"></a><span data-ttu-id="c2aea-163">значения cloudPcStatus</span><span class="sxs-lookup"><span data-stu-id="c2aea-163">cloudPcStatus values</span></span>

|<span data-ttu-id="c2aea-164">Member</span><span class="sxs-lookup"><span data-stu-id="c2aea-164">Member</span></span>|<span data-ttu-id="c2aea-165">Описание</span><span class="sxs-lookup"><span data-stu-id="c2aea-165">Description</span></span>|
|:---|:---|
|<span data-ttu-id="c2aea-166">notProvisioned</span><span class="sxs-lookup"><span data-stu-id="c2aea-166">notProvisioned</span></span>|<span data-ttu-id="c2aea-167">Облачный КОМПЬЮТЕР не был предусмотрен.</span><span class="sxs-lookup"><span data-stu-id="c2aea-167">The Cloud PC hasn’t been provisioned.</span></span>|
|<span data-ttu-id="c2aea-168">подготовка</span><span class="sxs-lookup"><span data-stu-id="c2aea-168">provisioning</span></span>|<span data-ttu-id="c2aea-169">Подготовка облачного компьютера продолжается.</span><span class="sxs-lookup"><span data-stu-id="c2aea-169">Cloud PC provisioning is in progress.</span></span>|
|<span data-ttu-id="c2aea-170">provisioned</span><span class="sxs-lookup"><span data-stu-id="c2aea-170">provisioned</span></span>|<span data-ttu-id="c2aea-171">Облачный компьютер является предварительным и может быть доступ к конечным пользователям.</span><span class="sxs-lookup"><span data-stu-id="c2aea-171">The Cloud PC is provisioned and can be accessed by end users.</span></span>|
|<span data-ttu-id="c2aea-172">обновление</span><span class="sxs-lookup"><span data-stu-id="c2aea-172">upgrading</span></span>|<span data-ttu-id="c2aea-173">В настоящее время идет процесс повторного окантовки облачного компьютера.</span><span class="sxs-lookup"><span data-stu-id="c2aea-173">Cloud PC resize is in progress.</span></span>|
|<span data-ttu-id="c2aea-174">inGracePeriod</span><span class="sxs-lookup"><span data-stu-id="c2aea-174">inGracePeriod</span></span>|<span data-ttu-id="c2aea-175">Облачный компьютер находится в периоде отсрочки на одну неделю до его деразвения.</span><span class="sxs-lookup"><span data-stu-id="c2aea-175">The Cloud PC is in the one week grace period before it’s deprovisioned.</span></span>|
|<span data-ttu-id="c2aea-176">deprovisioning</span><span class="sxs-lookup"><span data-stu-id="c2aea-176">deprovisioning</span></span>|<span data-ttu-id="c2aea-177">Облачный КОМПЬЮТЕР развяжен.</span><span class="sxs-lookup"><span data-stu-id="c2aea-177">The Cloud PC is deprovisioning.</span></span>|
|<span data-ttu-id="c2aea-178">не удалось</span><span class="sxs-lookup"><span data-stu-id="c2aea-178">failed</span></span>|<span data-ttu-id="c2aea-179">Операция на облачном компьютере не удалась.</span><span class="sxs-lookup"><span data-stu-id="c2aea-179">The operation on Cloud PC has failed.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c2aea-180">Связи</span><span class="sxs-lookup"><span data-stu-id="c2aea-180">Relationships</span></span>

<span data-ttu-id="c2aea-181">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="c2aea-181">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c2aea-182">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="c2aea-182">JSON representation</span></span>

<span data-ttu-id="c2aea-183">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c2aea-183">The following is a JSON representation of the resource.</span></span>
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

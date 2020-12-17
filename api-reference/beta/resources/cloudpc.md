---
title: Тип ресурса cloudPC
description: Виртуальные рабочие столы, управляемые облаком.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: 481bcae691632685cafab00a4b7e44addb1ad0cd
ms.sourcegitcommit: ee9e594ad64bef5bc839cf813c0854d083c00aef
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/17/2020
ms.locfileid: "49706089"
---
# <a name="cloudpc-resource-type"></a><span data-ttu-id="38b59-103">Тип ресурса cloudPC</span><span class="sxs-lookup"><span data-stu-id="38b59-103">cloudPC resource type</span></span>

<span data-ttu-id="38b59-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="38b59-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="38b59-105">Представляет управляемый облаком виртуальный рабочий стол.</span><span class="sxs-lookup"><span data-stu-id="38b59-105">Represents a cloud-managed virtual desktop.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="methods"></a><span data-ttu-id="38b59-106">Методы</span><span class="sxs-lookup"><span data-stu-id="38b59-106">Methods</span></span>

|<span data-ttu-id="38b59-107">Метод</span><span class="sxs-lookup"><span data-stu-id="38b59-107">Method</span></span>|<span data-ttu-id="38b59-108">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="38b59-108">Return type</span></span>|<span data-ttu-id="38b59-109">Описание</span><span class="sxs-lookup"><span data-stu-id="38b59-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="38b59-110">Список cloudPCs</span><span class="sxs-lookup"><span data-stu-id="38b59-110">List cloudPCs</span></span>](../api/virtualendpoint-list-cloudpcs.md)|<span data-ttu-id="38b59-111">[Коллекция cloudPC](../resources/cloudpc.md)</span><span class="sxs-lookup"><span data-stu-id="38b59-111">[cloudPC](../resources/cloudpc.md) collection</span></span>|<span data-ttu-id="38b59-112">Список свойств и связей объектов [cloudPC.](../resources/cloudpc.md)</span><span class="sxs-lookup"><span data-stu-id="38b59-112">List properties and relationships of the [cloudPC](../resources/cloudpc.md) objects.</span></span>|
|[<span data-ttu-id="38b59-113">Get cloudPC</span><span class="sxs-lookup"><span data-stu-id="38b59-113">Get cloudPC</span></span>](../api/cloudpc-get.md)|[<span data-ttu-id="38b59-114">cloudPC</span><span class="sxs-lookup"><span data-stu-id="38b59-114">cloudPC</span></span>](../resources/cloudpc.md)|<span data-ttu-id="38b59-115">Чтение свойств и связей объекта [cloudPC.](../resources/cloudpc.md)</span><span class="sxs-lookup"><span data-stu-id="38b59-115">Read the properties and relationships of a [cloudPC](../resources/cloudpc.md) object.</span></span>|
|[<span data-ttu-id="38b59-116">Reprovision</span><span class="sxs-lookup"><span data-stu-id="38b59-116">Reprovision</span></span>](../api/cloudpc-reprovision.md)|<span data-ttu-id="38b59-117">Нет</span><span class="sxs-lookup"><span data-stu-id="38b59-117">None</span></span>|<span data-ttu-id="38b59-118">Повторное создание объекта [cloudPC.](../resources/cloudpc.md)</span><span class="sxs-lookup"><span data-stu-id="38b59-118">Reprovision a [cloudPC](../resources/cloudpc.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="38b59-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="38b59-119">Properties</span></span>

|<span data-ttu-id="38b59-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="38b59-120">Property</span></span>|<span data-ttu-id="38b59-121">Тип</span><span class="sxs-lookup"><span data-stu-id="38b59-121">Type</span></span>|<span data-ttu-id="38b59-122">Описание</span><span class="sxs-lookup"><span data-stu-id="38b59-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="38b59-123">id</span><span class="sxs-lookup"><span data-stu-id="38b59-123">id</span></span>|<span data-ttu-id="38b59-124">String</span><span class="sxs-lookup"><span data-stu-id="38b59-124">String</span></span>|<span data-ttu-id="38b59-125">Уникальный идентификатор для облачного ПК.</span><span class="sxs-lookup"><span data-stu-id="38b59-125">Unique identifier for the cloud PC.</span></span> <span data-ttu-id="38b59-126">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="38b59-126">Read-only.</span></span>|
|<span data-ttu-id="38b59-127">displayName</span><span class="sxs-lookup"><span data-stu-id="38b59-127">displayName</span></span>|<span data-ttu-id="38b59-128">String</span><span class="sxs-lookup"><span data-stu-id="38b59-128">String</span></span>|<span data-ttu-id="38b59-129">Отображаемая версия облачного компьютера.</span><span class="sxs-lookup"><span data-stu-id="38b59-129">The cloud PC display name.</span></span>|
|<span data-ttu-id="38b59-130">imageDisplayName</span><span class="sxs-lookup"><span data-stu-id="38b59-130">imageDisplayName</span></span>|<span data-ttu-id="38b59-131">String</span><span class="sxs-lookup"><span data-stu-id="38b59-131">String</span></span>|<span data-ttu-id="38b59-132">Имя образа ОС на облачном компьютере.</span><span class="sxs-lookup"><span data-stu-id="38b59-132">Name of the OS image that's on the cloud PC.</span></span>|
|<span data-ttu-id="38b59-133">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="38b59-133">managedDeviceId</span></span>|<span data-ttu-id="38b59-134">String</span><span class="sxs-lookup"><span data-stu-id="38b59-134">String</span></span>|<span data-ttu-id="38b59-135">ИД устройства Intune на облачном компьютере.</span><span class="sxs-lookup"><span data-stu-id="38b59-135">The cloud PC’s Intune device ID.</span></span>|
|<span data-ttu-id="38b59-136">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="38b59-136">managedDeviceName</span></span>|<span data-ttu-id="38b59-137">String</span><span class="sxs-lookup"><span data-stu-id="38b59-137">String</span></span>|<span data-ttu-id="38b59-138">Имя устройства Intune облачного ПК.</span><span class="sxs-lookup"><span data-stu-id="38b59-138">The cloud PC’s Intune device name.</span></span>|
|<span data-ttu-id="38b59-139">provisioningPolicyId</span><span class="sxs-lookup"><span data-stu-id="38b59-139">provisioningPolicyId</span></span>|<span data-ttu-id="38b59-140">String</span><span class="sxs-lookup"><span data-stu-id="38b59-140">String</span></span>|<span data-ttu-id="38b59-141">ИД политики предоставления на облачном компьютере.</span><span class="sxs-lookup"><span data-stu-id="38b59-141">The cloud PC's provisioning policy ID.</span></span>|
|<span data-ttu-id="38b59-142">servicePlanId</span><span class="sxs-lookup"><span data-stu-id="38b59-142">servicePlanId</span></span>|<span data-ttu-id="38b59-143">String</span><span class="sxs-lookup"><span data-stu-id="38b59-143">String</span></span>|<span data-ttu-id="38b59-144">ИД плана обслуживания облачного КОМПЬЮТЕРА.</span><span class="sxs-lookup"><span data-stu-id="38b59-144">The cloud PC's service plan ID.</span></span>|
|<span data-ttu-id="38b59-145">servicePlanName</span><span class="sxs-lookup"><span data-stu-id="38b59-145">servicePlanName</span></span>|<span data-ttu-id="38b59-146">String</span><span class="sxs-lookup"><span data-stu-id="38b59-146">String</span></span>|<span data-ttu-id="38b59-147">Имя плана обслуживания облачного ПК.</span><span class="sxs-lookup"><span data-stu-id="38b59-147">The cloud PC's service plan name.</span></span>|
|<span data-ttu-id="38b59-148">status</span><span class="sxs-lookup"><span data-stu-id="38b59-148">status</span></span>|<span data-ttu-id="38b59-149">cloudPcStatus</span><span class="sxs-lookup"><span data-stu-id="38b59-149">cloudPcStatus</span></span>|<span data-ttu-id="38b59-150">Состояние облачного ПК.</span><span class="sxs-lookup"><span data-stu-id="38b59-150">Status of the cloud PC.</span></span> <span data-ttu-id="38b59-151">Возможные значения: `notProvisioned`, `provisioning`, `provisioned`, `upgrading`, `inGracePeriod`, `deprovisioning`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="38b59-151">Possible values are: `notProvisioned`, `provisioning`, `provisioned`, `upgrading`, `inGracePeriod`, `deprovisioning`, `failed`.</span></span>|
|<span data-ttu-id="38b59-152">statusDetails</span><span class="sxs-lookup"><span data-stu-id="38b59-152">statusDetails</span></span>|[<span data-ttu-id="38b59-153">cloudPcStatusDetails</span><span class="sxs-lookup"><span data-stu-id="38b59-153">cloudPcStatusDetails</span></span>](../resources/cloudpcstatusdetails.md)|<span data-ttu-id="38b59-154">Сведения о состоянии облачного ПК.</span><span class="sxs-lookup"><span data-stu-id="38b59-154">The details of the cloud PC status.</span></span>|
|<span data-ttu-id="38b59-155">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="38b59-155">userPrincipalName</span></span>|<span data-ttu-id="38b59-156">String</span><span class="sxs-lookup"><span data-stu-id="38b59-156">String</span></span>|<span data-ttu-id="38b59-157">Имя основного пользователя (UPN) пользователя, назначенного облачному компьютеру.</span><span class="sxs-lookup"><span data-stu-id="38b59-157">The user principal name (UPN) of the user assigned to the cloud PC.</span></span>|
|<span data-ttu-id="38b59-158">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="38b59-158">lastModifiedDateTime</span></span>|<span data-ttu-id="38b59-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="38b59-159">DateTimeOffset</span></span>|<span data-ttu-id="38b59-160">Дата и время последнего изменения облачного ПК.</span><span class="sxs-lookup"><span data-stu-id="38b59-160">The cloud PC's last modified date and time.</span></span> <span data-ttu-id="38b59-161">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="38b59-161">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="38b59-162">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: "2014-01-01T00:00:00Z".</span><span class="sxs-lookup"><span data-stu-id="38b59-162">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span>|

## <a name="relationships"></a><span data-ttu-id="38b59-163">Связи</span><span class="sxs-lookup"><span data-stu-id="38b59-163">Relationships</span></span>

<span data-ttu-id="38b59-164">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="38b59-164">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="38b59-165">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="38b59-165">JSON representation</span></span>

<span data-ttu-id="38b59-166">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="38b59-166">The following is a JSON representation of the resource.</span></span>
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

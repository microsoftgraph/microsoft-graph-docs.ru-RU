---
title: Тип ресурса Клаудпк
description: Облачные управляемые виртуальные рабочие столы.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: d1109ceb81f741cefa9b26662bc1c8c5de8a8329
ms.sourcegitcommit: 958b540f118ef3ce64d4d4e96b29264e2b56d703
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/03/2020
ms.locfileid: "49563840"
---
# <a name="cloudpc-resource-type"></a><span data-ttu-id="10629-103">Тип ресурса Клаудпк</span><span class="sxs-lookup"><span data-stu-id="10629-103">cloudPC resource type</span></span>

<span data-ttu-id="10629-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="10629-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="10629-105">Представляет виртуальный рабочий стол, управляемый облаком.</span><span class="sxs-lookup"><span data-stu-id="10629-105">Represents a cloud-managed virtual desktop.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="methods"></a><span data-ttu-id="10629-106">Методы</span><span class="sxs-lookup"><span data-stu-id="10629-106">Methods</span></span>

|<span data-ttu-id="10629-107">Метод</span><span class="sxs-lookup"><span data-stu-id="10629-107">Method</span></span>|<span data-ttu-id="10629-108">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="10629-108">Return type</span></span>|<span data-ttu-id="10629-109">Описание</span><span class="sxs-lookup"><span data-stu-id="10629-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="10629-110">Список Клаудпкс</span><span class="sxs-lookup"><span data-stu-id="10629-110">List cloudPCs</span></span>](../api/virtualendpoint-list-cloudpcs.md)|<span data-ttu-id="10629-111">Коллекция [клаудпк](../resources/cloudpc.md)</span><span class="sxs-lookup"><span data-stu-id="10629-111">[cloudPC](../resources/cloudpc.md) collection</span></span>|<span data-ttu-id="10629-112">Список свойств и связей объектов [клаудпк](../resources/cloudpc.md) .</span><span class="sxs-lookup"><span data-stu-id="10629-112">List properties and relationships of the [cloudPC](../resources/cloudpc.md) objects.</span></span>|
|[<span data-ttu-id="10629-113">Получение Клаудпк</span><span class="sxs-lookup"><span data-stu-id="10629-113">Get cloudPC</span></span>](../api/cloudpc-get.md)|[<span data-ttu-id="10629-114">клаудпк</span><span class="sxs-lookup"><span data-stu-id="10629-114">cloudPC</span></span>](../resources/cloudpc.md)|<span data-ttu-id="10629-115">Чтение свойств и связей объекта [клаудпк](../resources/cloudpc.md) .</span><span class="sxs-lookup"><span data-stu-id="10629-115">Read the properties and relationships of a [cloudPC](../resources/cloudpc.md) object.</span></span>|
|[<span data-ttu-id="10629-116">Повторная подготовка</span><span class="sxs-lookup"><span data-stu-id="10629-116">Reprovision</span></span>](../api/cloudpc-reprovision.md)|<span data-ttu-id="10629-117">Нет</span><span class="sxs-lookup"><span data-stu-id="10629-117">None</span></span>|<span data-ttu-id="10629-118">Повторное наполнение объекта [клаудпк](../resources/cloudpc.md) .</span><span class="sxs-lookup"><span data-stu-id="10629-118">Reprovision a [cloudPC](../resources/cloudpc.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="10629-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="10629-119">Properties</span></span>

|<span data-ttu-id="10629-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="10629-120">Property</span></span>|<span data-ttu-id="10629-121">Тип</span><span class="sxs-lookup"><span data-stu-id="10629-121">Type</span></span>|<span data-ttu-id="10629-122">Описание</span><span class="sxs-lookup"><span data-stu-id="10629-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="10629-123">id</span><span class="sxs-lookup"><span data-stu-id="10629-123">id</span></span>|<span data-ttu-id="10629-124">String</span><span class="sxs-lookup"><span data-stu-id="10629-124">String</span></span>|<span data-ttu-id="10629-125">Уникальный идентификатор для облачного компьютера.</span><span class="sxs-lookup"><span data-stu-id="10629-125">Unique identifier for the cloud PC.</span></span> <span data-ttu-id="10629-126">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="10629-126">Read-only.</span></span>|
|<span data-ttu-id="10629-127">displayName</span><span class="sxs-lookup"><span data-stu-id="10629-127">displayName</span></span>|<span data-ttu-id="10629-128">String</span><span class="sxs-lookup"><span data-stu-id="10629-128">String</span></span>|<span data-ttu-id="10629-129">Отображаемое имя Cloud PC.</span><span class="sxs-lookup"><span data-stu-id="10629-129">The cloud PC display name.</span></span>|
|<span data-ttu-id="10629-130">имажедисплайнаме</span><span class="sxs-lookup"><span data-stu-id="10629-130">imageDisplayName</span></span>|<span data-ttu-id="10629-131">String</span><span class="sxs-lookup"><span data-stu-id="10629-131">String</span></span>|<span data-ttu-id="10629-132">Имя образа операционной системы, который находится на облачном компьютере.</span><span class="sxs-lookup"><span data-stu-id="10629-132">Name of the OS image that's on the cloud PC.</span></span>|
|<span data-ttu-id="10629-133">манажеддевицеид</span><span class="sxs-lookup"><span data-stu-id="10629-133">managedDeviceId</span></span>|<span data-ttu-id="10629-134">String</span><span class="sxs-lookup"><span data-stu-id="10629-134">String</span></span>|<span data-ttu-id="10629-135">ИДЕНТИФИКАТОР устройства Intune облачного компьютера.</span><span class="sxs-lookup"><span data-stu-id="10629-135">The cloud PC’s Intune device ID.</span></span>|
|<span data-ttu-id="10629-136">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="10629-136">managedDeviceName</span></span>|<span data-ttu-id="10629-137">String</span><span class="sxs-lookup"><span data-stu-id="10629-137">String</span></span>|<span data-ttu-id="10629-138">Имя устройства в Intune на облачном компьютере.</span><span class="sxs-lookup"><span data-stu-id="10629-138">The cloud PC’s Intune device name.</span></span>|
|<span data-ttu-id="10629-139">провисионингполициид</span><span class="sxs-lookup"><span data-stu-id="10629-139">provisioningPolicyId</span></span>|<span data-ttu-id="10629-140">String</span><span class="sxs-lookup"><span data-stu-id="10629-140">String</span></span>|<span data-ttu-id="10629-141">Идентификатор политики подготовки для облачного компьютера.</span><span class="sxs-lookup"><span data-stu-id="10629-141">The cloud PC's provisioning policy ID.</span></span>|
|<span data-ttu-id="10629-142">сервицепланид</span><span class="sxs-lookup"><span data-stu-id="10629-142">servicePlanId</span></span>|<span data-ttu-id="10629-143">String</span><span class="sxs-lookup"><span data-stu-id="10629-143">String</span></span>|<span data-ttu-id="10629-144">ИДЕНТИФИКАТОР плана обслуживания Cloud PC.</span><span class="sxs-lookup"><span data-stu-id="10629-144">The cloud PC's service plan ID.</span></span>|
|<span data-ttu-id="10629-145">сервицепланнаме</span><span class="sxs-lookup"><span data-stu-id="10629-145">servicePlanName</span></span>|<span data-ttu-id="10629-146">String</span><span class="sxs-lookup"><span data-stu-id="10629-146">String</span></span>|<span data-ttu-id="10629-147">Имя плана обслуживания для облачного компьютера.</span><span class="sxs-lookup"><span data-stu-id="10629-147">The cloud PC's service plan name.</span></span>|
|<span data-ttu-id="10629-148">status</span><span class="sxs-lookup"><span data-stu-id="10629-148">status</span></span>|<span data-ttu-id="10629-149">клаудпкстатус</span><span class="sxs-lookup"><span data-stu-id="10629-149">cloudPcStatus</span></span>|<span data-ttu-id="10629-150">Состояние облачного компьютера.</span><span class="sxs-lookup"><span data-stu-id="10629-150">Status of the cloud PC.</span></span> <span data-ttu-id="10629-151">Возможные значения: `notProvisioned`, `provisioning`, `provisioned`, `upgrading`, `inGracePeriod`, `deprovisioning`, `upgradeFailed`, `provisionFailed`, `deprovisionFailed`, `reprovisionFailed`.</span><span class="sxs-lookup"><span data-stu-id="10629-151">Possible values are: `notProvisioned`, `provisioning`, `provisioned`, `upgrading`, `inGracePeriod`, `deprovisioning`, `upgradeFailed`, `provisionFailed`, `deprovisionFailed`, `reprovisionFailed`.</span></span>|
|<span data-ttu-id="10629-152">статусдетаилс</span><span class="sxs-lookup"><span data-stu-id="10629-152">statusDetails</span></span>|[<span data-ttu-id="10629-153">клаудпкстатусдетаилс</span><span class="sxs-lookup"><span data-stu-id="10629-153">cloudPcStatusDetails</span></span>](../resources/cloudpcstatusdetails.md)|<span data-ttu-id="10629-154">Сведения о состоянии облачного компьютера.</span><span class="sxs-lookup"><span data-stu-id="10629-154">The details of the cloud PC status.</span></span>|
|<span data-ttu-id="10629-155">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="10629-155">userPrincipalName</span></span>|<span data-ttu-id="10629-156">String</span><span class="sxs-lookup"><span data-stu-id="10629-156">String</span></span>|<span data-ttu-id="10629-157">Имя участника-пользователя (UPN) пользователя, назначенное облачному компьютеру.</span><span class="sxs-lookup"><span data-stu-id="10629-157">The user principal name (UPN) of the user assigned to the cloud PC.</span></span>|
|<span data-ttu-id="10629-158">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="10629-158">lastModifiedDateTime</span></span>|<span data-ttu-id="10629-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="10629-159">DateTimeOffset</span></span>|<span data-ttu-id="10629-160">Дата и время последнего изменения в облачном ПК.</span><span class="sxs-lookup"><span data-stu-id="10629-160">The cloud PC's last modified date and time.</span></span> <span data-ttu-id="10629-161">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="10629-161">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="10629-162">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: "2014-01-01T00:00:00Z".</span><span class="sxs-lookup"><span data-stu-id="10629-162">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span>|

## <a name="relationships"></a><span data-ttu-id="10629-163">Связи</span><span class="sxs-lookup"><span data-stu-id="10629-163">Relationships</span></span>

<span data-ttu-id="10629-164">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="10629-164">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="10629-165">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="10629-165">JSON representation</span></span>

<span data-ttu-id="10629-166">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="10629-166">The following is a JSON representation of the resource.</span></span>
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

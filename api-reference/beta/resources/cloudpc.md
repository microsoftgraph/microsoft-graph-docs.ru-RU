---
title: Тип ресурса Клаудпк
description: Облачные управляемые виртуальные рабочие столы.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 95758299f87ac463bac6fdc30f7d70fb59eb6c92
ms.sourcegitcommit: 3644a6cee51ab2bd19fa94e698d064073323d1dd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/21/2020
ms.locfileid: "49378608"
---
# <a name="cloudpc-resource-type"></a><span data-ttu-id="19d97-103">Тип ресурса Клаудпк</span><span class="sxs-lookup"><span data-stu-id="19d97-103">cloudPC resource type</span></span>

<span data-ttu-id="19d97-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="19d97-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="19d97-105">Представляет виртуальный рабочий стол, управляемый облаком.</span><span class="sxs-lookup"><span data-stu-id="19d97-105">Represents a cloud-managed virtual desktop.</span></span>

## <a name="methods"></a><span data-ttu-id="19d97-106">Методы</span><span class="sxs-lookup"><span data-stu-id="19d97-106">Methods</span></span>

|<span data-ttu-id="19d97-107">Метод</span><span class="sxs-lookup"><span data-stu-id="19d97-107">Method</span></span>|<span data-ttu-id="19d97-108">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="19d97-108">Return type</span></span>|<span data-ttu-id="19d97-109">Описание</span><span class="sxs-lookup"><span data-stu-id="19d97-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="19d97-110">Список Клаудпкс</span><span class="sxs-lookup"><span data-stu-id="19d97-110">List cloudPCs</span></span>](../api/virtualendpoint-list-cloudpcs.md)|<span data-ttu-id="19d97-111">Коллекция [клаудпк](../resources/cloudpc.md)</span><span class="sxs-lookup"><span data-stu-id="19d97-111">[cloudPC](../resources/cloudpc.md) collection</span></span>|<span data-ttu-id="19d97-112">Список свойств и связей объектов [клаудпк](../resources/cloudpc.md) .</span><span class="sxs-lookup"><span data-stu-id="19d97-112">List properties and relationships of the [cloudPC](../resources/cloudpc.md) objects.</span></span>|
|[<span data-ttu-id="19d97-113">Получение Клаудпк</span><span class="sxs-lookup"><span data-stu-id="19d97-113">Get cloudPC</span></span>](../api/cloudpc-get.md)|[<span data-ttu-id="19d97-114">клаудпк</span><span class="sxs-lookup"><span data-stu-id="19d97-114">cloudPC</span></span>](../resources/cloudpc.md)|<span data-ttu-id="19d97-115">Чтение свойств и связей объекта [клаудпк](../resources/cloudpc.md) .</span><span class="sxs-lookup"><span data-stu-id="19d97-115">Read the properties and relationships of a [cloudPC](../resources/cloudpc.md) object.</span></span>|
|[<span data-ttu-id="19d97-116">Повторная подготовка</span><span class="sxs-lookup"><span data-stu-id="19d97-116">Reprovision</span></span>](../api/cloudpc-reprovision.md)|<span data-ttu-id="19d97-117">Нет</span><span class="sxs-lookup"><span data-stu-id="19d97-117">None</span></span>|<span data-ttu-id="19d97-118">Повторное наполнение объекта [клаудпк](../resources/cloudpc.md) .</span><span class="sxs-lookup"><span data-stu-id="19d97-118">Reprovision a [cloudPC](../resources/cloudpc.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="19d97-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="19d97-119">Properties</span></span>

|<span data-ttu-id="19d97-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="19d97-120">Property</span></span>|<span data-ttu-id="19d97-121">Тип</span><span class="sxs-lookup"><span data-stu-id="19d97-121">Type</span></span>|<span data-ttu-id="19d97-122">Описание</span><span class="sxs-lookup"><span data-stu-id="19d97-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="19d97-123">id</span><span class="sxs-lookup"><span data-stu-id="19d97-123">id</span></span>|<span data-ttu-id="19d97-124">Строка</span><span class="sxs-lookup"><span data-stu-id="19d97-124">String</span></span>|<span data-ttu-id="19d97-125">Уникальный идентификатор для облачного компьютера.</span><span class="sxs-lookup"><span data-stu-id="19d97-125">Unique identifier for the cloud PC.</span></span> <span data-ttu-id="19d97-126">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="19d97-126">Read-only.</span></span>|
|<span data-ttu-id="19d97-127">displayName</span><span class="sxs-lookup"><span data-stu-id="19d97-127">displayName</span></span>|<span data-ttu-id="19d97-128">Строка</span><span class="sxs-lookup"><span data-stu-id="19d97-128">String</span></span>|<span data-ttu-id="19d97-129">Отображаемое имя Cloud PC.</span><span class="sxs-lookup"><span data-stu-id="19d97-129">The cloud PC display name.</span></span>|
|<span data-ttu-id="19d97-130">имажедисплайнаме</span><span class="sxs-lookup"><span data-stu-id="19d97-130">imageDisplayName</span></span>|<span data-ttu-id="19d97-131">Строка</span><span class="sxs-lookup"><span data-stu-id="19d97-131">String</span></span>|<span data-ttu-id="19d97-132">Имя образа операционной системы, который находится на облачном компьютере.</span><span class="sxs-lookup"><span data-stu-id="19d97-132">Name of the OS image that's on the cloud PC.</span></span>|
|<span data-ttu-id="19d97-133">манажеддевицеид</span><span class="sxs-lookup"><span data-stu-id="19d97-133">managedDeviceId</span></span>|<span data-ttu-id="19d97-134">Строка</span><span class="sxs-lookup"><span data-stu-id="19d97-134">String</span></span>|<span data-ttu-id="19d97-135">ИДЕНТИФИКАТОР устройства Intune облачного компьютера.</span><span class="sxs-lookup"><span data-stu-id="19d97-135">The cloud PC’s Intune device ID.</span></span>|
|<span data-ttu-id="19d97-136">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="19d97-136">managedDeviceName</span></span>|<span data-ttu-id="19d97-137">String</span><span class="sxs-lookup"><span data-stu-id="19d97-137">String</span></span>|<span data-ttu-id="19d97-138">Имя устройства в Intune на облачном компьютере.</span><span class="sxs-lookup"><span data-stu-id="19d97-138">The cloud PC’s Intune device name.</span></span>|
|<span data-ttu-id="19d97-139">провисионингполициид</span><span class="sxs-lookup"><span data-stu-id="19d97-139">provisioningPolicyId</span></span>|<span data-ttu-id="19d97-140">Строка</span><span class="sxs-lookup"><span data-stu-id="19d97-140">String</span></span>|<span data-ttu-id="19d97-141">Идентификатор политики подготовки для облачного компьютера.</span><span class="sxs-lookup"><span data-stu-id="19d97-141">The cloud PC's provisioning policy ID.</span></span>|
|<span data-ttu-id="19d97-142">сервицепланид</span><span class="sxs-lookup"><span data-stu-id="19d97-142">servicePlanId</span></span>|<span data-ttu-id="19d97-143">Строка</span><span class="sxs-lookup"><span data-stu-id="19d97-143">String</span></span>|<span data-ttu-id="19d97-144">ИДЕНТИФИКАТОР плана обслуживания Cloud PC.</span><span class="sxs-lookup"><span data-stu-id="19d97-144">The cloud PC's service plan ID.</span></span>|
|<span data-ttu-id="19d97-145">сервицепланнаме</span><span class="sxs-lookup"><span data-stu-id="19d97-145">servicePlanName</span></span>|<span data-ttu-id="19d97-146">String</span><span class="sxs-lookup"><span data-stu-id="19d97-146">String</span></span>|<span data-ttu-id="19d97-147">Имя плана обслуживания для облачного компьютера.</span><span class="sxs-lookup"><span data-stu-id="19d97-147">The cloud PC's service plan name.</span></span>|
|<span data-ttu-id="19d97-148">status</span><span class="sxs-lookup"><span data-stu-id="19d97-148">status</span></span>|<span data-ttu-id="19d97-149">клаудпкстатус</span><span class="sxs-lookup"><span data-stu-id="19d97-149">cloudPcStatus</span></span>|<span data-ttu-id="19d97-150">Состояние облачного компьютера.</span><span class="sxs-lookup"><span data-stu-id="19d97-150">Status of the cloud PC.</span></span> <span data-ttu-id="19d97-151">Возможные значения: `notProvisioned`, `provisioning`, `provisioned`, `upgrading`, `inGracePeriod`, `deprovisioning`, `upgradeFailed`, `provisionFailed`, `deprovisionFailed`, `reprovisionFailed`.</span><span class="sxs-lookup"><span data-stu-id="19d97-151">Possible values are: `notProvisioned`, `provisioning`, `provisioned`, `upgrading`, `inGracePeriod`, `deprovisioning`, `upgradeFailed`, `provisionFailed`, `deprovisionFailed`, `reprovisionFailed`.</span></span>|
|<span data-ttu-id="19d97-152">статусдетаилс</span><span class="sxs-lookup"><span data-stu-id="19d97-152">statusDetails</span></span>|[<span data-ttu-id="19d97-153">клаудпкстатусдетаилс</span><span class="sxs-lookup"><span data-stu-id="19d97-153">cloudPcStatusDetails</span></span>](../resources/cloudpcstatusdetails.md)|<span data-ttu-id="19d97-154">Сведения о состоянии облачного компьютера.</span><span class="sxs-lookup"><span data-stu-id="19d97-154">The details of the cloud PC status.</span></span>|
|<span data-ttu-id="19d97-155">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="19d97-155">userPrincipalName</span></span>|<span data-ttu-id="19d97-156">String</span><span class="sxs-lookup"><span data-stu-id="19d97-156">String</span></span>|<span data-ttu-id="19d97-157">Имя участника-пользователя (UPN) пользователя, назначенное облачному компьютеру.</span><span class="sxs-lookup"><span data-stu-id="19d97-157">The user principal name (UPN) of the user assigned to the cloud PC.</span></span>|
|<span data-ttu-id="19d97-158">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="19d97-158">lastModifiedDateTime</span></span>|<span data-ttu-id="19d97-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="19d97-159">DateTimeOffset</span></span>|<span data-ttu-id="19d97-160">Дата и время последнего изменения в облачном ПК.</span><span class="sxs-lookup"><span data-stu-id="19d97-160">The cloud PC's last modified date and time.</span></span> <span data-ttu-id="19d97-161">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="19d97-161">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="19d97-162">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: "2014-01-01T00:00:00Z".</span><span class="sxs-lookup"><span data-stu-id="19d97-162">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span>|

## <a name="relationships"></a><span data-ttu-id="19d97-163">Связи</span><span class="sxs-lookup"><span data-stu-id="19d97-163">Relationships</span></span>

<span data-ttu-id="19d97-164">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="19d97-164">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="19d97-165">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="19d97-165">JSON representation</span></span>

<span data-ttu-id="19d97-166">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="19d97-166">The following is a JSON representation of the resource.</span></span>
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

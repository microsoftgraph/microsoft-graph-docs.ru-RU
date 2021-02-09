---
title: Тип ресурса virtualEndpoint
description: Ресурс virtualEndpoint представляет контейнер для функций управления облачными КОМПЬЮТЕРами.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: ea76f9267bc9be33c88a4d6a615f2fe881a3b193
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50156681"
---
# <a name="virtualendpoint-resource-type"></a><span data-ttu-id="480c6-103">Тип ресурса virtualEndpoint</span><span class="sxs-lookup"><span data-stu-id="480c6-103">virtualEndpoint resource type</span></span>

<span data-ttu-id="480c6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="480c6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="480c6-105">Ресурс virtualEndpoint представляет контейнер для API для управления облачным компьютером.</span><span class="sxs-lookup"><span data-stu-id="480c6-105">The virtualEndpoint resource represents a container for APIs to manage cloud PC.</span></span>

<span data-ttu-id="480c6-106">Используйте API облачных КОМПЬЮТЕРов для предоставления и управления виртуальными рабочими столами для сотрудников организации.</span><span class="sxs-lookup"><span data-stu-id="480c6-106">Use the cloud PC API to provision and manage virtual desktops for employees in an organization.</span></span> <span data-ttu-id="480c6-107">Используйте его вместе с [API Intune](../resources/intune-graph-overview.md) для управления физическими и виртуальными конечными точками.</span><span class="sxs-lookup"><span data-stu-id="480c6-107">Use it in conjunction with the [Intune API](../resources/intune-graph-overview.md) to manage physical and virtual endpoints.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]
## <a name="methods"></a><span data-ttu-id="480c6-108">Методы</span><span class="sxs-lookup"><span data-stu-id="480c6-108">Methods</span></span>

|<span data-ttu-id="480c6-109">Метод</span><span class="sxs-lookup"><span data-stu-id="480c6-109">Method</span></span>|<span data-ttu-id="480c6-110">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="480c6-110">Return type</span></span>|<span data-ttu-id="480c6-111">Описание</span><span class="sxs-lookup"><span data-stu-id="480c6-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="480c6-112">Получите эффективные разрешения</span><span class="sxs-lookup"><span data-stu-id="480c6-112">Get effective permissions</span></span>](../api/virtualendpoint-geteffectivepermissions.md)|<span data-ttu-id="480c6-113">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="480c6-113">String collection</span></span>|<span data-ttu-id="480c6-114">Просмотр эффективных разрешений для пользователя, который в настоящее время проходит проверку подлинности.</span><span class="sxs-lookup"><span data-stu-id="480c6-114">View the effective permissions of the currently authenticated user.</span></span>|
|[<span data-ttu-id="480c6-115">Список cloudPCs</span><span class="sxs-lookup"><span data-stu-id="480c6-115">List cloudPCs</span></span>](../api/virtualendpoint-list-cloudpcs.md)|<span data-ttu-id="480c6-116">[Коллекция cloudPC](../resources/cloudpc.md)</span><span class="sxs-lookup"><span data-stu-id="480c6-116">[cloudPC](../resources/cloudpc.md) collection</span></span>|<span data-ttu-id="480c6-117">Список свойств и связей объектов [cloudPC.](../resources/cloudpc.md)</span><span class="sxs-lookup"><span data-stu-id="480c6-117">List properties and relationships of the [cloudPC](../resources/cloudpc.md) objects.</span></span>|
|[<span data-ttu-id="480c6-118">Список deviceImages</span><span class="sxs-lookup"><span data-stu-id="480c6-118">List deviceImages</span></span>](../api/virtualendpoint-list-deviceimages.md)|<span data-ttu-id="480c6-119">[Коллекция cloudPcDeviceImage](../resources/cloudpcdeviceimage.md)</span><span class="sxs-lookup"><span data-stu-id="480c6-119">[cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) collection</span></span>|<span data-ttu-id="480c6-120">Список свойств и связей объектов [cloudPcDeviceImage.](../resources/cloudpcdeviceimage.md)</span><span class="sxs-lookup"><span data-stu-id="480c6-120">List the properties and relationships of [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) objects.</span></span>|
|[<span data-ttu-id="480c6-121">Создание cloudPcDeviceImage</span><span class="sxs-lookup"><span data-stu-id="480c6-121">Create cloudPcDeviceImage</span></span>](../api/virtualendpoint-post-deviceimages.md)|[<span data-ttu-id="480c6-122">cloudPcDeviceImage</span><span class="sxs-lookup"><span data-stu-id="480c6-122">cloudPcDeviceImage</span></span>](../resources/cloudpcdeviceimage.md)|<span data-ttu-id="480c6-123">Создание объекта [cloudPcDeviceImage.](../resources/cloudpcdeviceimage.md)</span><span class="sxs-lookup"><span data-stu-id="480c6-123">Create a new [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) object.</span></span>|
|[<span data-ttu-id="480c6-124">Список onPremisesConnections</span><span class="sxs-lookup"><span data-stu-id="480c6-124">List onPremisesConnections</span></span>](../api/virtualendpoint-list-onpremisesconnections.md)|<span data-ttu-id="480c6-125">[Коллекция cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md)</span><span class="sxs-lookup"><span data-stu-id="480c6-125">[cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) collection</span></span>|<span data-ttu-id="480c6-126">Список свойств и связей объектов [cloudPcOnPremisesConnection.](../resources/cloudpconpremisesconnection.md)</span><span class="sxs-lookup"><span data-stu-id="480c6-126">List properties and relationships of the [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) objects.</span></span>|
|[<span data-ttu-id="480c6-127">Создание cloudPcOnPremisesConnection</span><span class="sxs-lookup"><span data-stu-id="480c6-127">Create cloudPcOnPremisesConnection</span></span>](../api/virtualendpoint-post-onpremisesconnections.md)|[<span data-ttu-id="480c6-128">cloudPcOnPremisesConnection</span><span class="sxs-lookup"><span data-stu-id="480c6-128">cloudPcOnPremisesConnection</span></span>](../resources/cloudpconpremisesconnection.md)|<span data-ttu-id="480c6-129">Создание объекта [cloudPcOnPremisesConnection.](../resources/cloudpconpremisesconnection.md)</span><span class="sxs-lookup"><span data-stu-id="480c6-129">Create a new [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) object.</span></span>|
|[<span data-ttu-id="480c6-130">Список provisioningPolicies</span><span class="sxs-lookup"><span data-stu-id="480c6-130">List provisioningPolicies</span></span>](../api/virtualendpoint-list-provisioningpolicies.md)|<span data-ttu-id="480c6-131">[Коллекция cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="480c6-131">[cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) collection</span></span>|<span data-ttu-id="480c6-132">Список свойств и связей объектов [cloudPcProvisioningPolicy.](../resources/cloudpcprovisioningpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="480c6-132">List properties and relationships of the [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) objects.</span></span>|
|[<span data-ttu-id="480c6-133">Создание cloudPcProvisioningPolicy</span><span class="sxs-lookup"><span data-stu-id="480c6-133">Create cloudPcProvisioningPolicy</span></span>](../api/virtualendpoint-post-provisioningpolicies.md)|[<span data-ttu-id="480c6-134">cloudPcProvisioningPolicy</span><span class="sxs-lookup"><span data-stu-id="480c6-134">cloudPcProvisioningPolicy</span></span>](../resources/cloudpcprovisioningpolicy.md)|<span data-ttu-id="480c6-135">Создание объекта [cloudPcProvisioningPolicy.](../resources/cloudpcprovisioningpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="480c6-135">Create a new [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="480c6-136">Свойства</span><span class="sxs-lookup"><span data-stu-id="480c6-136">Properties</span></span>

|<span data-ttu-id="480c6-137">Свойство</span><span class="sxs-lookup"><span data-stu-id="480c6-137">Property</span></span>|<span data-ttu-id="480c6-138">Тип</span><span class="sxs-lookup"><span data-stu-id="480c6-138">Type</span></span>|<span data-ttu-id="480c6-139">Описание</span><span class="sxs-lookup"><span data-stu-id="480c6-139">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="480c6-140">id</span><span class="sxs-lookup"><span data-stu-id="480c6-140">id</span></span>|<span data-ttu-id="480c6-141">String</span><span class="sxs-lookup"><span data-stu-id="480c6-141">String</span></span>|<span data-ttu-id="480c6-142">Уникальный идентификатор для идентификатора виртуальной конечной точки. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="480c6-142">The unique identifier for the virtual endpoint id. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="480c6-143">Связи</span><span class="sxs-lookup"><span data-stu-id="480c6-143">Relationships</span></span>

|<span data-ttu-id="480c6-144">Связь</span><span class="sxs-lookup"><span data-stu-id="480c6-144">Relationship</span></span>|<span data-ttu-id="480c6-145">Тип</span><span class="sxs-lookup"><span data-stu-id="480c6-145">Type</span></span>|<span data-ttu-id="480c6-146">Описание</span><span class="sxs-lookup"><span data-stu-id="480c6-146">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="480c6-147">cloudPCs</span><span class="sxs-lookup"><span data-stu-id="480c6-147">cloudPCs</span></span>|<span data-ttu-id="480c6-148">[Коллекция cloudPC](../resources/cloudpc.md)</span><span class="sxs-lookup"><span data-stu-id="480c6-148">[cloudPC](../resources/cloudpc.md) collection</span></span>|<span data-ttu-id="480c6-149">Виртуальные рабочие столы, управляемые облаком.</span><span class="sxs-lookup"><span data-stu-id="480c6-149">Cloud managed virtual desktops.</span></span>|
|<span data-ttu-id="480c6-150">deviceImages</span><span class="sxs-lookup"><span data-stu-id="480c6-150">deviceImages</span></span>|<span data-ttu-id="480c6-151">[Коллекция cloudPcDeviceImage](../resources/cloudpcdeviceimage.md)</span><span class="sxs-lookup"><span data-stu-id="480c6-151">[cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) collection</span></span>|<span data-ttu-id="480c6-152">Ресурс изображения на облачном компьютере.</span><span class="sxs-lookup"><span data-stu-id="480c6-152">The image resource on cloud PC.</span></span>|
|<span data-ttu-id="480c6-153">onPremisesConnections</span><span class="sxs-lookup"><span data-stu-id="480c6-153">onPremisesConnections</span></span>|<span data-ttu-id="480c6-154">[Коллекция cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md)</span><span class="sxs-lookup"><span data-stu-id="480c6-154">[cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) collection</span></span>|<span data-ttu-id="480c6-155">Заданная коллекция сведений о ресурсах Azure, которую можно использовать для подключения к локальной сети для облачных компьютеров.</span><span class="sxs-lookup"><span data-stu-id="480c6-155">A defined collection of Azure resource information that can be used to establish on-premises network connectivity for cloud PCs.</span></span>|
|<span data-ttu-id="480c6-156">provisioningPolicies</span><span class="sxs-lookup"><span data-stu-id="480c6-156">provisioningPolicies</span></span>|<span data-ttu-id="480c6-157">[Коллекция cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="480c6-157">[cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) collection</span></span>|<span data-ttu-id="480c6-158">политика предоставления облачных компьютеров;</span><span class="sxs-lookup"><span data-stu-id="480c6-158">cloud PC provisioning policy.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="480c6-159">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="480c6-159">JSON representation</span></span>

<span data-ttu-id="480c6-160">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="480c6-160">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.virtualEndpoint",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.virtualEndpoint",
  "id": "string"
}
```

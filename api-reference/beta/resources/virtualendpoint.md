---
title: Тип ресурса Виртуалендпоинт
description: Ресурс Виртуалендпоинт представляет контейнер для функций управления Cloud PC.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: 7e29e59658914e0f07af7635979e1b8938b99491
ms.sourcegitcommit: 958b540f118ef3ce64d4d4e96b29264e2b56d703
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/03/2020
ms.locfileid: "49563949"
---
# <a name="virtualendpoint-resource-type"></a><span data-ttu-id="35b8d-103">Тип ресурса Виртуалендпоинт</span><span class="sxs-lookup"><span data-stu-id="35b8d-103">virtualEndpoint resource type</span></span>

<span data-ttu-id="35b8d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="35b8d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="35b8d-105">Ресурс Виртуалендпоинт представляет контейнер для API для управления облачным компьютером.</span><span class="sxs-lookup"><span data-stu-id="35b8d-105">The virtualEndpoint resource represents a container for APIs to manage cloud PC.</span></span>

<span data-ttu-id="35b8d-106">Использование API Cloud PC для подготовки виртуальных рабочих столов для сотрудников Организации и управления ими.</span><span class="sxs-lookup"><span data-stu-id="35b8d-106">Use the cloud PC API to provision and manage virtual desktops for employees in an organization.</span></span> <span data-ttu-id="35b8d-107">Используйте его совместно с [API Intune](../resources/intune-graph-overview.md) для управления физическими и виртуальными конечными точками.</span><span class="sxs-lookup"><span data-stu-id="35b8d-107">Use it in conjunction with the [Intune API](../resources/intune-graph-overview.md) to manage physical and virtual endpoints.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]
## <a name="methods"></a><span data-ttu-id="35b8d-108">Методы</span><span class="sxs-lookup"><span data-stu-id="35b8d-108">Methods</span></span>

|<span data-ttu-id="35b8d-109">Метод</span><span class="sxs-lookup"><span data-stu-id="35b8d-109">Method</span></span>|<span data-ttu-id="35b8d-110">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="35b8d-110">Return type</span></span>|<span data-ttu-id="35b8d-111">Описание</span><span class="sxs-lookup"><span data-stu-id="35b8d-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="35b8d-112">Получение действующих разрешений</span><span class="sxs-lookup"><span data-stu-id="35b8d-112">Get effective permissions</span></span>](../api/virtualendpoint-geteffectivepermissions.md)|<span data-ttu-id="35b8d-113">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="35b8d-113">String collection</span></span>|<span data-ttu-id="35b8d-114">Просмотр действующих разрешений текущего пользователя, прошедшего проверку подлинности.</span><span class="sxs-lookup"><span data-stu-id="35b8d-114">View the effective permissions of the currently authenticated user.</span></span>|
|[<span data-ttu-id="35b8d-115">Список Клаудпкс</span><span class="sxs-lookup"><span data-stu-id="35b8d-115">List cloudPCs</span></span>](../api/virtualendpoint-list-cloudpcs.md)|<span data-ttu-id="35b8d-116">Коллекция [клаудпк](../resources/cloudpc.md)</span><span class="sxs-lookup"><span data-stu-id="35b8d-116">[cloudPC](../resources/cloudpc.md) collection</span></span>|<span data-ttu-id="35b8d-117">Список свойств и связей объектов [клаудпк](../resources/cloudpc.md) .</span><span class="sxs-lookup"><span data-stu-id="35b8d-117">List properties and relationships of the [cloudPC](../resources/cloudpc.md) objects.</span></span>|
|[<span data-ttu-id="35b8d-118">Список Девицеимажес</span><span class="sxs-lookup"><span data-stu-id="35b8d-118">List deviceImages</span></span>](../api/virtualendpoint-list-deviceimages.md)|<span data-ttu-id="35b8d-119">Коллекция [клаудпкдевицеимаже](../resources/cloudpcdeviceimage.md)</span><span class="sxs-lookup"><span data-stu-id="35b8d-119">[cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) collection</span></span>|<span data-ttu-id="35b8d-120">Перечисление свойств и связей объектов [клаудпкдевицеимаже](../resources/cloudpcdeviceimage.md) .</span><span class="sxs-lookup"><span data-stu-id="35b8d-120">List the properties and relationships of [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) objects.</span></span>|
|[<span data-ttu-id="35b8d-121">Создание Клаудпкдевицеимаже</span><span class="sxs-lookup"><span data-stu-id="35b8d-121">Create cloudPcDeviceImage</span></span>](../api/virtualendpoint-post-deviceimages.md)|[<span data-ttu-id="35b8d-122">клаудпкдевицеимаже</span><span class="sxs-lookup"><span data-stu-id="35b8d-122">cloudPcDeviceImage</span></span>](../resources/cloudpcdeviceimage.md)|<span data-ttu-id="35b8d-123">Создание нового объекта [клаудпкдевицеимаже](../resources/cloudpcdeviceimage.md) .</span><span class="sxs-lookup"><span data-stu-id="35b8d-123">Create a new [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) object.</span></span>|
|[<span data-ttu-id="35b8d-124">Список Онпремисесконнектионс</span><span class="sxs-lookup"><span data-stu-id="35b8d-124">List onPremisesConnections</span></span>](../api/virtualendpoint-list-onpremisesconnections.md)|<span data-ttu-id="35b8d-125">Коллекция [клаудпконпремисесконнектион](../resources/cloudpconpremisesconnection.md)</span><span class="sxs-lookup"><span data-stu-id="35b8d-125">[cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) collection</span></span>|<span data-ttu-id="35b8d-126">Список свойств и связей объектов [клаудпконпремисесконнектион](../resources/cloudpconpremisesconnection.md) .</span><span class="sxs-lookup"><span data-stu-id="35b8d-126">List properties and relationships of the [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) objects.</span></span>|
|[<span data-ttu-id="35b8d-127">Создание Клаудпконпремисесконнектион</span><span class="sxs-lookup"><span data-stu-id="35b8d-127">Create cloudPcOnPremisesConnection</span></span>](../api/virtualendpoint-post-onpremisesconnections.md)|[<span data-ttu-id="35b8d-128">клаудпконпремисесконнектион</span><span class="sxs-lookup"><span data-stu-id="35b8d-128">cloudPcOnPremisesConnection</span></span>](../resources/cloudpconpremisesconnection.md)|<span data-ttu-id="35b8d-129">Создание нового объекта [клаудпконпремисесконнектион](../resources/cloudpconpremisesconnection.md) .</span><span class="sxs-lookup"><span data-stu-id="35b8d-129">Create a new [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) object.</span></span>|
|[<span data-ttu-id="35b8d-130">Список ПровисионингполиЦиес</span><span class="sxs-lookup"><span data-stu-id="35b8d-130">List provisioningPolicies</span></span>](../api/virtualendpoint-list-provisioningpolicies.md)|<span data-ttu-id="35b8d-131">Коллекция [клаудпкпровисионингполици](../resources/cloudpcprovisioningpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="35b8d-131">[cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) collection</span></span>|<span data-ttu-id="35b8d-132">Список свойств и связей объектов [клаудпкпровисионингполици](../resources/cloudpcprovisioningpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="35b8d-132">List properties and relationships of the [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) objects.</span></span>|
|[<span data-ttu-id="35b8d-133">Создание Клаудпкпровисионингполици</span><span class="sxs-lookup"><span data-stu-id="35b8d-133">Create cloudPcProvisioningPolicy</span></span>](../api/virtualendpoint-post-provisioningpolicies.md)|[<span data-ttu-id="35b8d-134">клаудпкпровисионингполици</span><span class="sxs-lookup"><span data-stu-id="35b8d-134">cloudPcProvisioningPolicy</span></span>](../resources/cloudpcprovisioningpolicy.md)|<span data-ttu-id="35b8d-135">Создание нового объекта [клаудпкпровисионингполици](../resources/cloudpcprovisioningpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="35b8d-135">Create a new [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="35b8d-136">Свойства</span><span class="sxs-lookup"><span data-stu-id="35b8d-136">Properties</span></span>

|<span data-ttu-id="35b8d-137">Свойство</span><span class="sxs-lookup"><span data-stu-id="35b8d-137">Property</span></span>|<span data-ttu-id="35b8d-138">Тип</span><span class="sxs-lookup"><span data-stu-id="35b8d-138">Type</span></span>|<span data-ttu-id="35b8d-139">Описание</span><span class="sxs-lookup"><span data-stu-id="35b8d-139">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="35b8d-140">id</span><span class="sxs-lookup"><span data-stu-id="35b8d-140">id</span></span>|<span data-ttu-id="35b8d-141">String</span><span class="sxs-lookup"><span data-stu-id="35b8d-141">String</span></span>|<span data-ttu-id="35b8d-142">Уникальный идентификатор идентификатора виртуальной конечной точки. только для чтения.</span><span class="sxs-lookup"><span data-stu-id="35b8d-142">The unique identifier for the virtual endpoint id. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="35b8d-143">Связи</span><span class="sxs-lookup"><span data-stu-id="35b8d-143">Relationships</span></span>

|<span data-ttu-id="35b8d-144">Связь</span><span class="sxs-lookup"><span data-stu-id="35b8d-144">Relationship</span></span>|<span data-ttu-id="35b8d-145">Тип</span><span class="sxs-lookup"><span data-stu-id="35b8d-145">Type</span></span>|<span data-ttu-id="35b8d-146">Описание</span><span class="sxs-lookup"><span data-stu-id="35b8d-146">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="35b8d-147">клаудпкс</span><span class="sxs-lookup"><span data-stu-id="35b8d-147">cloudPCs</span></span>|<span data-ttu-id="35b8d-148">Коллекция [клаудпк](../resources/cloudpc.md)</span><span class="sxs-lookup"><span data-stu-id="35b8d-148">[cloudPC](../resources/cloudpc.md) collection</span></span>|<span data-ttu-id="35b8d-149">Облачные управляемые виртуальные рабочие столы.</span><span class="sxs-lookup"><span data-stu-id="35b8d-149">Cloud managed virtual desktops.</span></span>|
|<span data-ttu-id="35b8d-150">девицеимажес</span><span class="sxs-lookup"><span data-stu-id="35b8d-150">deviceImages</span></span>|<span data-ttu-id="35b8d-151">Коллекция [клаудпкдевицеимаже](../resources/cloudpcdeviceimage.md)</span><span class="sxs-lookup"><span data-stu-id="35b8d-151">[cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) collection</span></span>|<span data-ttu-id="35b8d-152">Ресурс Image (изображение) на облачном компьютере.</span><span class="sxs-lookup"><span data-stu-id="35b8d-152">The image resource on cloud PC.</span></span>|
|<span data-ttu-id="35b8d-153">онпремисесконнектионс</span><span class="sxs-lookup"><span data-stu-id="35b8d-153">onPremisesConnections</span></span>|<span data-ttu-id="35b8d-154">Коллекция [клаудпконпремисесконнектион](../resources/cloudpconpremisesconnection.md)</span><span class="sxs-lookup"><span data-stu-id="35b8d-154">[cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) collection</span></span>|<span data-ttu-id="35b8d-155">Определенная коллекция сведений о ресурсах Azure, которую можно использовать для установки локальной сети для облачных компьютеров.</span><span class="sxs-lookup"><span data-stu-id="35b8d-155">A defined collection of Azure resource information that can be used to establish on-premises network connectivity for cloud PCs.</span></span>|
|<span data-ttu-id="35b8d-156">провисионингполиЦиес</span><span class="sxs-lookup"><span data-stu-id="35b8d-156">provisioningPolicies</span></span>|<span data-ttu-id="35b8d-157">Коллекция [клаудпкпровисионингполици](../resources/cloudpcprovisioningpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="35b8d-157">[cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) collection</span></span>|<span data-ttu-id="35b8d-158">политика подготовки облачных ПК.</span><span class="sxs-lookup"><span data-stu-id="35b8d-158">cloud PC provisioning policy.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="35b8d-159">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="35b8d-159">JSON representation</span></span>

<span data-ttu-id="35b8d-160">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="35b8d-160">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.virtualEndpoint",
  "baseType": "",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.virtualEndpoint",
  "id": "string"
}
```

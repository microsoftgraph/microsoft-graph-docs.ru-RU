---
title: Тип ресурса unmanagedDevice
description: Неугодное устройство, обнаруженное в сети.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 0163fb0f3704bee86622574428954b3c3c9f805a
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50160643"
---
# <a name="unmanageddevice-resource-type"></a><span data-ttu-id="4fac2-103">Тип ресурса unmanagedDevice</span><span class="sxs-lookup"><span data-stu-id="4fac2-103">unmanagedDevice resource type</span></span>

<span data-ttu-id="4fac2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4fac2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4fac2-105">**Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4fac2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4fac2-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4fac2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4fac2-107">Неугодное устройство, обнаруженное в сети.</span><span class="sxs-lookup"><span data-stu-id="4fac2-107">Unmanaged device discovered in the network.</span></span>

## <a name="properties"></a><span data-ttu-id="4fac2-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="4fac2-108">Properties</span></span>
|<span data-ttu-id="4fac2-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="4fac2-109">Property</span></span>|<span data-ttu-id="4fac2-110">Тип</span><span class="sxs-lookup"><span data-stu-id="4fac2-110">Type</span></span>|<span data-ttu-id="4fac2-111">Описание</span><span class="sxs-lookup"><span data-stu-id="4fac2-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4fac2-112">os</span><span class="sxs-lookup"><span data-stu-id="4fac2-112">os</span></span>|<span data-ttu-id="4fac2-113">String</span><span class="sxs-lookup"><span data-stu-id="4fac2-113">String</span></span>|<span data-ttu-id="4fac2-114">Операционная система.</span><span class="sxs-lookup"><span data-stu-id="4fac2-114">Operating system.</span></span>|
|<span data-ttu-id="4fac2-115">osVersion</span><span class="sxs-lookup"><span data-stu-id="4fac2-115">osVersion</span></span>|<span data-ttu-id="4fac2-116">String</span><span class="sxs-lookup"><span data-stu-id="4fac2-116">String</span></span>|<span data-ttu-id="4fac2-117">Версия операционной системы.</span><span class="sxs-lookup"><span data-stu-id="4fac2-117">Operating system version.</span></span>|
|<span data-ttu-id="4fac2-118">ipAddress</span><span class="sxs-lookup"><span data-stu-id="4fac2-118">ipAddress</span></span>|<span data-ttu-id="4fac2-119">String</span><span class="sxs-lookup"><span data-stu-id="4fac2-119">String</span></span>|<span data-ttu-id="4fac2-120">IP-адрес.</span><span class="sxs-lookup"><span data-stu-id="4fac2-120">IP address.</span></span>|
|<span data-ttu-id="4fac2-121">deviceName</span><span class="sxs-lookup"><span data-stu-id="4fac2-121">deviceName</span></span>|<span data-ttu-id="4fac2-122">String</span><span class="sxs-lookup"><span data-stu-id="4fac2-122">String</span></span>|<span data-ttu-id="4fac2-123">Имя устройства.</span><span class="sxs-lookup"><span data-stu-id="4fac2-123">Device name.</span></span>|
|<span data-ttu-id="4fac2-124">macAddress</span><span class="sxs-lookup"><span data-stu-id="4fac2-124">macAddress</span></span>|<span data-ttu-id="4fac2-125">String</span><span class="sxs-lookup"><span data-stu-id="4fac2-125">String</span></span>|<span data-ttu-id="4fac2-126">MAC-адрес.</span><span class="sxs-lookup"><span data-stu-id="4fac2-126">MAC address.</span></span>|
|<span data-ttu-id="4fac2-127">domain</span><span class="sxs-lookup"><span data-stu-id="4fac2-127">domain</span></span>|<span data-ttu-id="4fac2-128">String</span><span class="sxs-lookup"><span data-stu-id="4fac2-128">String</span></span>|<span data-ttu-id="4fac2-129">Домен.</span><span class="sxs-lookup"><span data-stu-id="4fac2-129">Domain.</span></span>|
|<span data-ttu-id="4fac2-130">manufacturer</span><span class="sxs-lookup"><span data-stu-id="4fac2-130">manufacturer</span></span>|<span data-ttu-id="4fac2-131">String</span><span class="sxs-lookup"><span data-stu-id="4fac2-131">String</span></span>|<span data-ttu-id="4fac2-132">Изготовитель.</span><span class="sxs-lookup"><span data-stu-id="4fac2-132">Manufacturer.</span></span>|
|<span data-ttu-id="4fac2-133">model</span><span class="sxs-lookup"><span data-stu-id="4fac2-133">model</span></span>|<span data-ttu-id="4fac2-134">String</span><span class="sxs-lookup"><span data-stu-id="4fac2-134">String</span></span>|<span data-ttu-id="4fac2-135">Модель.</span><span class="sxs-lookup"><span data-stu-id="4fac2-135">Model.</span></span>|
|<span data-ttu-id="4fac2-136">расположение;</span><span class="sxs-lookup"><span data-stu-id="4fac2-136">location</span></span>|<span data-ttu-id="4fac2-137">String</span><span class="sxs-lookup"><span data-stu-id="4fac2-137">String</span></span>|<span data-ttu-id="4fac2-138">Расположение.</span><span class="sxs-lookup"><span data-stu-id="4fac2-138">Location.</span></span>|
|<span data-ttu-id="4fac2-139">lastLoggedOnUser</span><span class="sxs-lookup"><span data-stu-id="4fac2-139">lastLoggedOnUser</span></span>|<span data-ttu-id="4fac2-140">String</span><span class="sxs-lookup"><span data-stu-id="4fac2-140">String</span></span>|<span data-ttu-id="4fac2-141">Последний вход пользователя.</span><span class="sxs-lookup"><span data-stu-id="4fac2-141">Last logged on user.</span></span>|
|<span data-ttu-id="4fac2-142">lastSeenDateTime</span><span class="sxs-lookup"><span data-stu-id="4fac2-142">lastSeenDateTime</span></span>|<span data-ttu-id="4fac2-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4fac2-143">DateTimeOffset</span></span>|<span data-ttu-id="4fac2-144">Дата и время последнего просмотров.</span><span class="sxs-lookup"><span data-stu-id="4fac2-144">Last seen date and time.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4fac2-145">Связи</span><span class="sxs-lookup"><span data-stu-id="4fac2-145">Relationships</span></span>
<span data-ttu-id="4fac2-146">Нет</span><span class="sxs-lookup"><span data-stu-id="4fac2-146">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4fac2-147">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4fac2-147">JSON Representation</span></span>
<span data-ttu-id="4fac2-148">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4fac2-148">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.unmanagedDevice"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.unmanagedDevice",
  "os": "String",
  "osVersion": "String",
  "ipAddress": "String",
  "deviceName": "String",
  "macAddress": "String",
  "domain": "String",
  "manufacturer": "String",
  "model": "String",
  "location": "String",
  "lastLoggedOnUser": "String",
  "lastSeenDateTime": "String (timestamp)"
}
```





---
title: Тип ресурса Команажеддевицессуммари
description: Сводные данные для совместно управляемых устройств
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 42a92fd725c9f0b99037825c240dd017bf6c9c82
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48060778"
---
# <a name="comanageddevicessummary-resource-type"></a><span data-ttu-id="d41e4-103">Тип ресурса Команажеддевицессуммари</span><span class="sxs-lookup"><span data-stu-id="d41e4-103">comanagedDevicesSummary resource type</span></span>

<span data-ttu-id="d41e4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d41e4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d41e4-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d41e4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d41e4-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d41e4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d41e4-107">Сводные данные для совместно управляемых устройств</span><span class="sxs-lookup"><span data-stu-id="d41e4-107">Summary data for co managed devices</span></span>

## <a name="properties"></a><span data-ttu-id="d41e4-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="d41e4-108">Properties</span></span>
|<span data-ttu-id="d41e4-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="d41e4-109">Property</span></span>|<span data-ttu-id="d41e4-110">Тип</span><span class="sxs-lookup"><span data-stu-id="d41e4-110">Type</span></span>|<span data-ttu-id="d41e4-111">Описание</span><span class="sxs-lookup"><span data-stu-id="d41e4-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d41e4-112">инвенторикаунт</span><span class="sxs-lookup"><span data-stu-id="d41e4-112">inventoryCount</span></span>|<span data-ttu-id="d41e4-113">Int32</span><span class="sxs-lookup"><span data-stu-id="d41e4-113">Int32</span></span>|<span data-ttu-id="d41e4-114">Количество устройств с свунгом инвентаризации.</span><span class="sxs-lookup"><span data-stu-id="d41e4-114">Number of devices with Inventory swung-over.</span></span> <span data-ttu-id="d41e4-115">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d41e4-115">This property is read-only.</span></span>|
|<span data-ttu-id="d41e4-116">комплианцеполицикаунт</span><span class="sxs-lookup"><span data-stu-id="d41e4-116">compliancePolicyCount</span></span>|<span data-ttu-id="d41e4-117">Int32</span><span class="sxs-lookup"><span data-stu-id="d41e4-117">Int32</span></span>|<span data-ttu-id="d41e4-118">Количество устройств с Комплианцеполици свунг.</span><span class="sxs-lookup"><span data-stu-id="d41e4-118">Number of devices with CompliancePolicy swung-over.</span></span> <span data-ttu-id="d41e4-119">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d41e4-119">This property is read-only.</span></span>|
|<span data-ttu-id="d41e4-120">ресаурцеакцесскаунт</span><span class="sxs-lookup"><span data-stu-id="d41e4-120">resourceAccessCount</span></span>|<span data-ttu-id="d41e4-121">Int32</span><span class="sxs-lookup"><span data-stu-id="d41e4-121">Int32</span></span>|<span data-ttu-id="d41e4-122">Количество устройств с Ресаурцеакцесс свунг.</span><span class="sxs-lookup"><span data-stu-id="d41e4-122">Number of devices with ResourceAccess swung-over.</span></span> <span data-ttu-id="d41e4-123">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d41e4-123">This property is read-only.</span></span>|
|<span data-ttu-id="d41e4-124">конфигуратионсеттингскаунт</span><span class="sxs-lookup"><span data-stu-id="d41e4-124">configurationSettingsCount</span></span>|<span data-ttu-id="d41e4-125">Int32</span><span class="sxs-lookup"><span data-stu-id="d41e4-125">Int32</span></span>|<span data-ttu-id="d41e4-126">Количество устройств с Конфигуратионсеттингс свунг.</span><span class="sxs-lookup"><span data-stu-id="d41e4-126">Number of devices with ConfigurationSettings swung-over.</span></span> <span data-ttu-id="d41e4-127">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d41e4-127">This property is read-only.</span></span>|
|<span data-ttu-id="d41e4-128">виндовсупдатефорбусинесскаунт</span><span class="sxs-lookup"><span data-stu-id="d41e4-128">windowsUpdateForBusinessCount</span></span>|<span data-ttu-id="d41e4-129">Int32</span><span class="sxs-lookup"><span data-stu-id="d41e4-129">Int32</span></span>|<span data-ttu-id="d41e4-130">Количество устройств с Виндовсупдатефорбусинесс свунг.</span><span class="sxs-lookup"><span data-stu-id="d41e4-130">Number of devices with WindowsUpdateForBusiness swung-over.</span></span> <span data-ttu-id="d41e4-131">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d41e4-131">This property is read-only.</span></span>|
|<span data-ttu-id="d41e4-132">ендпоинтпротектионкаунт</span><span class="sxs-lookup"><span data-stu-id="d41e4-132">endpointProtectionCount</span></span>|<span data-ttu-id="d41e4-133">Int32</span><span class="sxs-lookup"><span data-stu-id="d41e4-133">Int32</span></span>|<span data-ttu-id="d41e4-134">Количество устройств с Ендпоинтпротектион свунг.</span><span class="sxs-lookup"><span data-stu-id="d41e4-134">Number of devices with EndpointProtection swung-over.</span></span> <span data-ttu-id="d41e4-135">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d41e4-135">This property is read-only.</span></span>|
|<span data-ttu-id="d41e4-136">модернаппскаунт</span><span class="sxs-lookup"><span data-stu-id="d41e4-136">modernAppsCount</span></span>|<span data-ttu-id="d41e4-137">Int32</span><span class="sxs-lookup"><span data-stu-id="d41e4-137">Int32</span></span>|<span data-ttu-id="d41e4-138">Количество устройств с Модернаппс свунг.</span><span class="sxs-lookup"><span data-stu-id="d41e4-138">Number of devices with ModernApps swung-over.</span></span> <span data-ttu-id="d41e4-139">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d41e4-139">This property is read-only.</span></span>|
|<span data-ttu-id="d41e4-140">оффицеаппскаунт</span><span class="sxs-lookup"><span data-stu-id="d41e4-140">officeAppsCount</span></span>|<span data-ttu-id="d41e4-141">Int32</span><span class="sxs-lookup"><span data-stu-id="d41e4-141">Int32</span></span>|<span data-ttu-id="d41e4-142">Количество устройств с Оффицеаппс свунг.</span><span class="sxs-lookup"><span data-stu-id="d41e4-142">Number of devices with OfficeApps swung-over.</span></span> <span data-ttu-id="d41e4-143">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d41e4-143">This property is read-only.</span></span>|
|<span data-ttu-id="d41e4-144">тоталкоманажедкаунт</span><span class="sxs-lookup"><span data-stu-id="d41e4-144">totalComanagedCount</span></span>|<span data-ttu-id="d41e4-145">Int32</span><span class="sxs-lookup"><span data-stu-id="d41e4-145">Int32</span></span>|<span data-ttu-id="d41e4-146">Количество совместно управляемых устройств.</span><span class="sxs-lookup"><span data-stu-id="d41e4-146">Number of Co-Managed Devices.</span></span> <span data-ttu-id="d41e4-147">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d41e4-147">This property is read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d41e4-148">Связи</span><span class="sxs-lookup"><span data-stu-id="d41e4-148">Relationships</span></span>
<span data-ttu-id="d41e4-149">Нет</span><span class="sxs-lookup"><span data-stu-id="d41e4-149">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d41e4-150">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d41e4-150">JSON Representation</span></span>
<span data-ttu-id="d41e4-151">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d41e4-151">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.comanagedDevicesSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.comanagedDevicesSummary",
  "inventoryCount": 1024,
  "compliancePolicyCount": 1024,
  "resourceAccessCount": 1024,
  "configurationSettingsCount": 1024,
  "windowsUpdateForBusinessCount": 1024,
  "endpointProtectionCount": 1024,
  "modernAppsCount": 1024,
  "officeAppsCount": 1024,
  "totalComanagedCount": 1024
}
```







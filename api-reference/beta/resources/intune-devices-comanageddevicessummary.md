---
title: Тип ресурса Команажеддевицессуммари
description: Сводные данные для совместно управляемых устройств
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b25820e4356fadaa4f991c103500a8ef8f5c0122
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49214850"
---
# <a name="comanageddevicessummary-resource-type"></a><span data-ttu-id="f5f3e-103">Тип ресурса Команажеддевицессуммари</span><span class="sxs-lookup"><span data-stu-id="f5f3e-103">comanagedDevicesSummary resource type</span></span>

<span data-ttu-id="f5f3e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f5f3e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f5f3e-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f5f3e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f5f3e-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f5f3e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f5f3e-107">Сводные данные для совместно управляемых устройств</span><span class="sxs-lookup"><span data-stu-id="f5f3e-107">Summary data for co managed devices</span></span>

## <a name="properties"></a><span data-ttu-id="f5f3e-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="f5f3e-108">Properties</span></span>
|<span data-ttu-id="f5f3e-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="f5f3e-109">Property</span></span>|<span data-ttu-id="f5f3e-110">Тип</span><span class="sxs-lookup"><span data-stu-id="f5f3e-110">Type</span></span>|<span data-ttu-id="f5f3e-111">Описание</span><span class="sxs-lookup"><span data-stu-id="f5f3e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f5f3e-112">инвенторикаунт</span><span class="sxs-lookup"><span data-stu-id="f5f3e-112">inventoryCount</span></span>|<span data-ttu-id="f5f3e-113">Int32</span><span class="sxs-lookup"><span data-stu-id="f5f3e-113">Int32</span></span>|<span data-ttu-id="f5f3e-114">Количество устройств с свунгом инвентаризации.</span><span class="sxs-lookup"><span data-stu-id="f5f3e-114">Number of devices with Inventory swung-over.</span></span> <span data-ttu-id="f5f3e-115">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f5f3e-115">This property is read-only.</span></span>|
|<span data-ttu-id="f5f3e-116">комплианцеполицикаунт</span><span class="sxs-lookup"><span data-stu-id="f5f3e-116">compliancePolicyCount</span></span>|<span data-ttu-id="f5f3e-117">Int32</span><span class="sxs-lookup"><span data-stu-id="f5f3e-117">Int32</span></span>|<span data-ttu-id="f5f3e-118">Количество устройств с Комплианцеполици свунг.</span><span class="sxs-lookup"><span data-stu-id="f5f3e-118">Number of devices with CompliancePolicy swung-over.</span></span> <span data-ttu-id="f5f3e-119">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f5f3e-119">This property is read-only.</span></span>|
|<span data-ttu-id="f5f3e-120">ресаурцеакцесскаунт</span><span class="sxs-lookup"><span data-stu-id="f5f3e-120">resourceAccessCount</span></span>|<span data-ttu-id="f5f3e-121">Int32</span><span class="sxs-lookup"><span data-stu-id="f5f3e-121">Int32</span></span>|<span data-ttu-id="f5f3e-122">Количество устройств с Ресаурцеакцесс свунг.</span><span class="sxs-lookup"><span data-stu-id="f5f3e-122">Number of devices with ResourceAccess swung-over.</span></span> <span data-ttu-id="f5f3e-123">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f5f3e-123">This property is read-only.</span></span>|
|<span data-ttu-id="f5f3e-124">конфигуратионсеттингскаунт</span><span class="sxs-lookup"><span data-stu-id="f5f3e-124">configurationSettingsCount</span></span>|<span data-ttu-id="f5f3e-125">Int32</span><span class="sxs-lookup"><span data-stu-id="f5f3e-125">Int32</span></span>|<span data-ttu-id="f5f3e-126">Количество устройств с Конфигуратионсеттингс свунг.</span><span class="sxs-lookup"><span data-stu-id="f5f3e-126">Number of devices with ConfigurationSettings swung-over.</span></span> <span data-ttu-id="f5f3e-127">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f5f3e-127">This property is read-only.</span></span>|
|<span data-ttu-id="f5f3e-128">виндовсупдатефорбусинесскаунт</span><span class="sxs-lookup"><span data-stu-id="f5f3e-128">windowsUpdateForBusinessCount</span></span>|<span data-ttu-id="f5f3e-129">Int32</span><span class="sxs-lookup"><span data-stu-id="f5f3e-129">Int32</span></span>|<span data-ttu-id="f5f3e-130">Количество устройств с Виндовсупдатефорбусинесс свунг.</span><span class="sxs-lookup"><span data-stu-id="f5f3e-130">Number of devices with WindowsUpdateForBusiness swung-over.</span></span> <span data-ttu-id="f5f3e-131">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f5f3e-131">This property is read-only.</span></span>|
|<span data-ttu-id="f5f3e-132">ендпоинтпротектионкаунт</span><span class="sxs-lookup"><span data-stu-id="f5f3e-132">endpointProtectionCount</span></span>|<span data-ttu-id="f5f3e-133">Int32</span><span class="sxs-lookup"><span data-stu-id="f5f3e-133">Int32</span></span>|<span data-ttu-id="f5f3e-134">Количество устройств с Ендпоинтпротектион свунг.</span><span class="sxs-lookup"><span data-stu-id="f5f3e-134">Number of devices with EndpointProtection swung-over.</span></span> <span data-ttu-id="f5f3e-135">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f5f3e-135">This property is read-only.</span></span>|
|<span data-ttu-id="f5f3e-136">модернаппскаунт</span><span class="sxs-lookup"><span data-stu-id="f5f3e-136">modernAppsCount</span></span>|<span data-ttu-id="f5f3e-137">Int32</span><span class="sxs-lookup"><span data-stu-id="f5f3e-137">Int32</span></span>|<span data-ttu-id="f5f3e-138">Количество устройств с Модернаппс свунг.</span><span class="sxs-lookup"><span data-stu-id="f5f3e-138">Number of devices with ModernApps swung-over.</span></span> <span data-ttu-id="f5f3e-139">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f5f3e-139">This property is read-only.</span></span>|
|<span data-ttu-id="f5f3e-140">оффицеаппскаунт</span><span class="sxs-lookup"><span data-stu-id="f5f3e-140">officeAppsCount</span></span>|<span data-ttu-id="f5f3e-141">Int32</span><span class="sxs-lookup"><span data-stu-id="f5f3e-141">Int32</span></span>|<span data-ttu-id="f5f3e-142">Количество устройств с Оффицеаппс свунг.</span><span class="sxs-lookup"><span data-stu-id="f5f3e-142">Number of devices with OfficeApps swung-over.</span></span> <span data-ttu-id="f5f3e-143">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f5f3e-143">This property is read-only.</span></span>|
|<span data-ttu-id="f5f3e-144">тоталкоманажедкаунт</span><span class="sxs-lookup"><span data-stu-id="f5f3e-144">totalComanagedCount</span></span>|<span data-ttu-id="f5f3e-145">Int32</span><span class="sxs-lookup"><span data-stu-id="f5f3e-145">Int32</span></span>|<span data-ttu-id="f5f3e-146">Количество устройств Co-Managed.</span><span class="sxs-lookup"><span data-stu-id="f5f3e-146">Number of Co-Managed Devices.</span></span> <span data-ttu-id="f5f3e-147">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f5f3e-147">This property is read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f5f3e-148">Связи</span><span class="sxs-lookup"><span data-stu-id="f5f3e-148">Relationships</span></span>
<span data-ttu-id="f5f3e-149">Нет</span><span class="sxs-lookup"><span data-stu-id="f5f3e-149">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f5f3e-150">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f5f3e-150">JSON Representation</span></span>
<span data-ttu-id="f5f3e-151">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f5f3e-151">Here is a JSON representation of the resource.</span></span>
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





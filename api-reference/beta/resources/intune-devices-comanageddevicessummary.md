---
title: Тип ресурса Команажеддевицессуммари
description: Сводные данные для совместно управляемых устройств
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 0e12a946db3e568faa171fa53299e6ec3546d455
ms.sourcegitcommit: dc3bade0c096d5ce716d4bc07cd9c7cabb52477b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/18/2020
ms.locfileid: "46791794"
---
# <a name="comanageddevicessummary-resource-type"></a><span data-ttu-id="17706-103">Тип ресурса Команажеддевицессуммари</span><span class="sxs-lookup"><span data-stu-id="17706-103">comanagedDevicesSummary resource type</span></span>

<span data-ttu-id="17706-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="17706-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="17706-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="17706-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="17706-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="17706-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="17706-107">Сводные данные для совместно управляемых устройств</span><span class="sxs-lookup"><span data-stu-id="17706-107">Summary data for co managed devices</span></span>

## <a name="properties"></a><span data-ttu-id="17706-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="17706-108">Properties</span></span>
|<span data-ttu-id="17706-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="17706-109">Property</span></span>|<span data-ttu-id="17706-110">Тип</span><span class="sxs-lookup"><span data-stu-id="17706-110">Type</span></span>|<span data-ttu-id="17706-111">Описание</span><span class="sxs-lookup"><span data-stu-id="17706-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="17706-112">инвенторикаунт</span><span class="sxs-lookup"><span data-stu-id="17706-112">inventoryCount</span></span>|<span data-ttu-id="17706-113">Int32</span><span class="sxs-lookup"><span data-stu-id="17706-113">Int32</span></span>|<span data-ttu-id="17706-114">Количество устройств с свунгом инвентаризации.</span><span class="sxs-lookup"><span data-stu-id="17706-114">Number of devices with Inventory swung-over.</span></span> <span data-ttu-id="17706-115">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="17706-115">This property is read-only.</span></span>|
|<span data-ttu-id="17706-116">комплианцеполицикаунт</span><span class="sxs-lookup"><span data-stu-id="17706-116">compliancePolicyCount</span></span>|<span data-ttu-id="17706-117">Int32</span><span class="sxs-lookup"><span data-stu-id="17706-117">Int32</span></span>|<span data-ttu-id="17706-118">Количество устройств с Комплианцеполици свунг.</span><span class="sxs-lookup"><span data-stu-id="17706-118">Number of devices with CompliancePolicy swung-over.</span></span> <span data-ttu-id="17706-119">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="17706-119">This property is read-only.</span></span>|
|<span data-ttu-id="17706-120">ресаурцеакцесскаунт</span><span class="sxs-lookup"><span data-stu-id="17706-120">resourceAccessCount</span></span>|<span data-ttu-id="17706-121">Int32</span><span class="sxs-lookup"><span data-stu-id="17706-121">Int32</span></span>|<span data-ttu-id="17706-122">Количество устройств с Ресаурцеакцесс свунг.</span><span class="sxs-lookup"><span data-stu-id="17706-122">Number of devices with ResourceAccess swung-over.</span></span> <span data-ttu-id="17706-123">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="17706-123">This property is read-only.</span></span>|
|<span data-ttu-id="17706-124">конфигуратионсеттингскаунт</span><span class="sxs-lookup"><span data-stu-id="17706-124">configurationSettingsCount</span></span>|<span data-ttu-id="17706-125">Int32</span><span class="sxs-lookup"><span data-stu-id="17706-125">Int32</span></span>|<span data-ttu-id="17706-126">Количество устройств с Конфигуратионсеттингс свунг.</span><span class="sxs-lookup"><span data-stu-id="17706-126">Number of devices with ConfigurationSettings swung-over.</span></span> <span data-ttu-id="17706-127">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="17706-127">This property is read-only.</span></span>|
|<span data-ttu-id="17706-128">виндовсупдатефорбусинесскаунт</span><span class="sxs-lookup"><span data-stu-id="17706-128">windowsUpdateForBusinessCount</span></span>|<span data-ttu-id="17706-129">Int32</span><span class="sxs-lookup"><span data-stu-id="17706-129">Int32</span></span>|<span data-ttu-id="17706-130">Количество устройств с Виндовсупдатефорбусинесс свунг.</span><span class="sxs-lookup"><span data-stu-id="17706-130">Number of devices with WindowsUpdateForBusiness swung-over.</span></span> <span data-ttu-id="17706-131">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="17706-131">This property is read-only.</span></span>|
|<span data-ttu-id="17706-132">ендпоинтпротектионкаунт</span><span class="sxs-lookup"><span data-stu-id="17706-132">endpointProtectionCount</span></span>|<span data-ttu-id="17706-133">Int32</span><span class="sxs-lookup"><span data-stu-id="17706-133">Int32</span></span>|<span data-ttu-id="17706-134">Количество устройств с Ендпоинтпротектион свунг.</span><span class="sxs-lookup"><span data-stu-id="17706-134">Number of devices with EndpointProtection swung-over.</span></span> <span data-ttu-id="17706-135">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="17706-135">This property is read-only.</span></span>|
|<span data-ttu-id="17706-136">модернаппскаунт</span><span class="sxs-lookup"><span data-stu-id="17706-136">modernAppsCount</span></span>|<span data-ttu-id="17706-137">Int32</span><span class="sxs-lookup"><span data-stu-id="17706-137">Int32</span></span>|<span data-ttu-id="17706-138">Количество устройств с Модернаппс свунг.</span><span class="sxs-lookup"><span data-stu-id="17706-138">Number of devices with ModernApps swung-over.</span></span> <span data-ttu-id="17706-139">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="17706-139">This property is read-only.</span></span>|
|<span data-ttu-id="17706-140">оффицеаппскаунт</span><span class="sxs-lookup"><span data-stu-id="17706-140">officeAppsCount</span></span>|<span data-ttu-id="17706-141">Int32</span><span class="sxs-lookup"><span data-stu-id="17706-141">Int32</span></span>|<span data-ttu-id="17706-142">Количество устройств с Оффицеаппс свунг.</span><span class="sxs-lookup"><span data-stu-id="17706-142">Number of devices with OfficeApps swung-over.</span></span> <span data-ttu-id="17706-143">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="17706-143">This property is read-only.</span></span>|
|<span data-ttu-id="17706-144">тоталкоманажедкаунт</span><span class="sxs-lookup"><span data-stu-id="17706-144">totalComanagedCount</span></span>|<span data-ttu-id="17706-145">Int32</span><span class="sxs-lookup"><span data-stu-id="17706-145">Int32</span></span>|<span data-ttu-id="17706-146">Количество совместно управляемых устройств.</span><span class="sxs-lookup"><span data-stu-id="17706-146">Number of Co-Managed Devices.</span></span> <span data-ttu-id="17706-147">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="17706-147">This property is read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="17706-148">Связи</span><span class="sxs-lookup"><span data-stu-id="17706-148">Relationships</span></span>
<span data-ttu-id="17706-149">Нет</span><span class="sxs-lookup"><span data-stu-id="17706-149">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="17706-150">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="17706-150">JSON Representation</span></span>
<span data-ttu-id="17706-151">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="17706-151">Here is a JSON representation of the resource.</span></span>
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




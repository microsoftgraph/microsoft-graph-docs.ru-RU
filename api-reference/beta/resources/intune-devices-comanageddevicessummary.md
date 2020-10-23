---
title: Тип ресурса Команажеддевицессуммари
description: Сводные данные для совместно управляемых устройств
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f1e0266151c2b32baa0c5d66ea1341eee6da28b5
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48725507"
---
# <a name="comanageddevicessummary-resource-type"></a><span data-ttu-id="21708-103">Тип ресурса Команажеддевицессуммари</span><span class="sxs-lookup"><span data-stu-id="21708-103">comanagedDevicesSummary resource type</span></span>

<span data-ttu-id="21708-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="21708-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="21708-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="21708-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="21708-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="21708-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="21708-107">Сводные данные для совместно управляемых устройств</span><span class="sxs-lookup"><span data-stu-id="21708-107">Summary data for co managed devices</span></span>

## <a name="properties"></a><span data-ttu-id="21708-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="21708-108">Properties</span></span>
|<span data-ttu-id="21708-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="21708-109">Property</span></span>|<span data-ttu-id="21708-110">Тип</span><span class="sxs-lookup"><span data-stu-id="21708-110">Type</span></span>|<span data-ttu-id="21708-111">Описание</span><span class="sxs-lookup"><span data-stu-id="21708-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="21708-112">инвенторикаунт</span><span class="sxs-lookup"><span data-stu-id="21708-112">inventoryCount</span></span>|<span data-ttu-id="21708-113">Int32</span><span class="sxs-lookup"><span data-stu-id="21708-113">Int32</span></span>|<span data-ttu-id="21708-114">Количество устройств с свунгом инвентаризации.</span><span class="sxs-lookup"><span data-stu-id="21708-114">Number of devices with Inventory swung-over.</span></span> <span data-ttu-id="21708-115">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="21708-115">This property is read-only.</span></span>|
|<span data-ttu-id="21708-116">комплианцеполицикаунт</span><span class="sxs-lookup"><span data-stu-id="21708-116">compliancePolicyCount</span></span>|<span data-ttu-id="21708-117">Int32</span><span class="sxs-lookup"><span data-stu-id="21708-117">Int32</span></span>|<span data-ttu-id="21708-118">Количество устройств с Комплианцеполици свунг.</span><span class="sxs-lookup"><span data-stu-id="21708-118">Number of devices with CompliancePolicy swung-over.</span></span> <span data-ttu-id="21708-119">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="21708-119">This property is read-only.</span></span>|
|<span data-ttu-id="21708-120">ресаурцеакцесскаунт</span><span class="sxs-lookup"><span data-stu-id="21708-120">resourceAccessCount</span></span>|<span data-ttu-id="21708-121">Int32</span><span class="sxs-lookup"><span data-stu-id="21708-121">Int32</span></span>|<span data-ttu-id="21708-122">Количество устройств с Ресаурцеакцесс свунг.</span><span class="sxs-lookup"><span data-stu-id="21708-122">Number of devices with ResourceAccess swung-over.</span></span> <span data-ttu-id="21708-123">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="21708-123">This property is read-only.</span></span>|
|<span data-ttu-id="21708-124">конфигуратионсеттингскаунт</span><span class="sxs-lookup"><span data-stu-id="21708-124">configurationSettingsCount</span></span>|<span data-ttu-id="21708-125">Int32</span><span class="sxs-lookup"><span data-stu-id="21708-125">Int32</span></span>|<span data-ttu-id="21708-126">Количество устройств с Конфигуратионсеттингс свунг.</span><span class="sxs-lookup"><span data-stu-id="21708-126">Number of devices with ConfigurationSettings swung-over.</span></span> <span data-ttu-id="21708-127">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="21708-127">This property is read-only.</span></span>|
|<span data-ttu-id="21708-128">виндовсупдатефорбусинесскаунт</span><span class="sxs-lookup"><span data-stu-id="21708-128">windowsUpdateForBusinessCount</span></span>|<span data-ttu-id="21708-129">Int32</span><span class="sxs-lookup"><span data-stu-id="21708-129">Int32</span></span>|<span data-ttu-id="21708-130">Количество устройств с Виндовсупдатефорбусинесс свунг.</span><span class="sxs-lookup"><span data-stu-id="21708-130">Number of devices with WindowsUpdateForBusiness swung-over.</span></span> <span data-ttu-id="21708-131">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="21708-131">This property is read-only.</span></span>|
|<span data-ttu-id="21708-132">ендпоинтпротектионкаунт</span><span class="sxs-lookup"><span data-stu-id="21708-132">endpointProtectionCount</span></span>|<span data-ttu-id="21708-133">Int32</span><span class="sxs-lookup"><span data-stu-id="21708-133">Int32</span></span>|<span data-ttu-id="21708-134">Количество устройств с Ендпоинтпротектион свунг.</span><span class="sxs-lookup"><span data-stu-id="21708-134">Number of devices with EndpointProtection swung-over.</span></span> <span data-ttu-id="21708-135">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="21708-135">This property is read-only.</span></span>|
|<span data-ttu-id="21708-136">модернаппскаунт</span><span class="sxs-lookup"><span data-stu-id="21708-136">modernAppsCount</span></span>|<span data-ttu-id="21708-137">Int32</span><span class="sxs-lookup"><span data-stu-id="21708-137">Int32</span></span>|<span data-ttu-id="21708-138">Количество устройств с Модернаппс свунг.</span><span class="sxs-lookup"><span data-stu-id="21708-138">Number of devices with ModernApps swung-over.</span></span> <span data-ttu-id="21708-139">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="21708-139">This property is read-only.</span></span>|
|<span data-ttu-id="21708-140">оффицеаппскаунт</span><span class="sxs-lookup"><span data-stu-id="21708-140">officeAppsCount</span></span>|<span data-ttu-id="21708-141">Int32</span><span class="sxs-lookup"><span data-stu-id="21708-141">Int32</span></span>|<span data-ttu-id="21708-142">Количество устройств с Оффицеаппс свунг.</span><span class="sxs-lookup"><span data-stu-id="21708-142">Number of devices with OfficeApps swung-over.</span></span> <span data-ttu-id="21708-143">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="21708-143">This property is read-only.</span></span>|
|<span data-ttu-id="21708-144">тоталкоманажедкаунт</span><span class="sxs-lookup"><span data-stu-id="21708-144">totalComanagedCount</span></span>|<span data-ttu-id="21708-145">Int32</span><span class="sxs-lookup"><span data-stu-id="21708-145">Int32</span></span>|<span data-ttu-id="21708-146">Количество устройств Co-Managed.</span><span class="sxs-lookup"><span data-stu-id="21708-146">Number of Co-Managed Devices.</span></span> <span data-ttu-id="21708-147">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="21708-147">This property is read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="21708-148">Связи</span><span class="sxs-lookup"><span data-stu-id="21708-148">Relationships</span></span>
<span data-ttu-id="21708-149">Нет</span><span class="sxs-lookup"><span data-stu-id="21708-149">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="21708-150">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="21708-150">JSON Representation</span></span>
<span data-ttu-id="21708-151">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="21708-151">Here is a JSON representation of the resource.</span></span>
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






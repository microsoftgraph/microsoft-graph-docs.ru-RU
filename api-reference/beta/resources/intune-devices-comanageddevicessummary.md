---
title: Тип ресурса Команажеддевицессуммари
description: Сводные данные для совместно управляемых устройств
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 6f592ba7900f0761a24b02495dc337046b615bb1
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/18/2020
ms.locfileid: "44793467"
---
# <a name="comanageddevicessummary-resource-type"></a><span data-ttu-id="c8753-103">Тип ресурса Команажеддевицессуммари</span><span class="sxs-lookup"><span data-stu-id="c8753-103">comanagedDevicesSummary resource type</span></span>

<span data-ttu-id="c8753-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c8753-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c8753-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c8753-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c8753-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c8753-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c8753-107">Сводные данные для совместно управляемых устройств</span><span class="sxs-lookup"><span data-stu-id="c8753-107">Summary data for co managed devices</span></span>

## <a name="properties"></a><span data-ttu-id="c8753-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="c8753-108">Properties</span></span>
|<span data-ttu-id="c8753-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="c8753-109">Property</span></span>|<span data-ttu-id="c8753-110">Тип</span><span class="sxs-lookup"><span data-stu-id="c8753-110">Type</span></span>|<span data-ttu-id="c8753-111">Описание</span><span class="sxs-lookup"><span data-stu-id="c8753-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c8753-112">инвенторикаунт</span><span class="sxs-lookup"><span data-stu-id="c8753-112">inventoryCount</span></span>|<span data-ttu-id="c8753-113">Int32</span><span class="sxs-lookup"><span data-stu-id="c8753-113">Int32</span></span>|<span data-ttu-id="c8753-114">Количество устройств с свунгом инвентаризации.</span><span class="sxs-lookup"><span data-stu-id="c8753-114">Number of devices with Inventory swung-over.</span></span> <span data-ttu-id="c8753-115">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c8753-115">This property is read-only.</span></span>|
|<span data-ttu-id="c8753-116">комплианцеполицикаунт</span><span class="sxs-lookup"><span data-stu-id="c8753-116">compliancePolicyCount</span></span>|<span data-ttu-id="c8753-117">Int32</span><span class="sxs-lookup"><span data-stu-id="c8753-117">Int32</span></span>|<span data-ttu-id="c8753-118">Количество устройств с Комплианцеполици свунг.</span><span class="sxs-lookup"><span data-stu-id="c8753-118">Number of devices with CompliancePolicy swung-over.</span></span> <span data-ttu-id="c8753-119">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c8753-119">This property is read-only.</span></span>|
|<span data-ttu-id="c8753-120">ресаурцеакцесскаунт</span><span class="sxs-lookup"><span data-stu-id="c8753-120">resourceAccessCount</span></span>|<span data-ttu-id="c8753-121">Int32</span><span class="sxs-lookup"><span data-stu-id="c8753-121">Int32</span></span>|<span data-ttu-id="c8753-122">Количество устройств с Ресаурцеакцесс свунг.</span><span class="sxs-lookup"><span data-stu-id="c8753-122">Number of devices with ResourceAccess swung-over.</span></span> <span data-ttu-id="c8753-123">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c8753-123">This property is read-only.</span></span>|
|<span data-ttu-id="c8753-124">конфигуратионсеттингскаунт</span><span class="sxs-lookup"><span data-stu-id="c8753-124">configurationSettingsCount</span></span>|<span data-ttu-id="c8753-125">Int32</span><span class="sxs-lookup"><span data-stu-id="c8753-125">Int32</span></span>|<span data-ttu-id="c8753-126">Количество устройств с Конфигуратионсеттингс свунг.</span><span class="sxs-lookup"><span data-stu-id="c8753-126">Number of devices with ConfigurationSettings swung-over.</span></span> <span data-ttu-id="c8753-127">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c8753-127">This property is read-only.</span></span>|
|<span data-ttu-id="c8753-128">виндовсупдатефорбусинесскаунт</span><span class="sxs-lookup"><span data-stu-id="c8753-128">windowsUpdateForBusinessCount</span></span>|<span data-ttu-id="c8753-129">Int32</span><span class="sxs-lookup"><span data-stu-id="c8753-129">Int32</span></span>|<span data-ttu-id="c8753-130">Количество устройств с Виндовсупдатефорбусинесс свунг.</span><span class="sxs-lookup"><span data-stu-id="c8753-130">Number of devices with WindowsUpdateForBusiness swung-over.</span></span> <span data-ttu-id="c8753-131">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c8753-131">This property is read-only.</span></span>|
|<span data-ttu-id="c8753-132">ендпоинтпротектионкаунт</span><span class="sxs-lookup"><span data-stu-id="c8753-132">endpointProtectionCount</span></span>|<span data-ttu-id="c8753-133">Int32</span><span class="sxs-lookup"><span data-stu-id="c8753-133">Int32</span></span>|<span data-ttu-id="c8753-134">Количество устройств с Ендпоинтпротектион свунг.</span><span class="sxs-lookup"><span data-stu-id="c8753-134">Number of devices with EndpointProtection swung-over.</span></span> <span data-ttu-id="c8753-135">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c8753-135">This property is read-only.</span></span>|
|<span data-ttu-id="c8753-136">модернаппскаунт</span><span class="sxs-lookup"><span data-stu-id="c8753-136">modernAppsCount</span></span>|<span data-ttu-id="c8753-137">Int32</span><span class="sxs-lookup"><span data-stu-id="c8753-137">Int32</span></span>|<span data-ttu-id="c8753-138">Количество устройств с Модернаппс свунг.</span><span class="sxs-lookup"><span data-stu-id="c8753-138">Number of devices with ModernApps swung-over.</span></span> <span data-ttu-id="c8753-139">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c8753-139">This property is read-only.</span></span>|
|<span data-ttu-id="c8753-140">оффицеаппскаунт</span><span class="sxs-lookup"><span data-stu-id="c8753-140">officeAppsCount</span></span>|<span data-ttu-id="c8753-141">Int32</span><span class="sxs-lookup"><span data-stu-id="c8753-141">Int32</span></span>|<span data-ttu-id="c8753-142">Количество устройств с Оффицеаппс свунг.</span><span class="sxs-lookup"><span data-stu-id="c8753-142">Number of devices with OfficeApps swung-over.</span></span> <span data-ttu-id="c8753-143">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c8753-143">This property is read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c8753-144">Связи</span><span class="sxs-lookup"><span data-stu-id="c8753-144">Relationships</span></span>
<span data-ttu-id="c8753-145">Нет</span><span class="sxs-lookup"><span data-stu-id="c8753-145">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c8753-146">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c8753-146">JSON Representation</span></span>
<span data-ttu-id="c8753-147">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c8753-147">Here is a JSON representation of the resource.</span></span>
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
  "officeAppsCount": 1024
}
```




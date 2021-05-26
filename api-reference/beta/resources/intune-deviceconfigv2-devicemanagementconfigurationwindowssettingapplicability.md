---
title: тип ресурса deviceManagementConfigurationWindowsSettingApplicability
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 2302bcbae4af684efc159f269d639c50aeb99191
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/26/2021
ms.locfileid: "52666683"
---
# <a name="devicemanagementconfigurationwindowssettingapplicability-resource-type"></a><span data-ttu-id="20c3b-103">тип ресурса deviceManagementConfigurationWindowsSettingApplicability</span><span class="sxs-lookup"><span data-stu-id="20c3b-103">deviceManagementConfigurationWindowsSettingApplicability resource type</span></span>

<span data-ttu-id="20c3b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="20c3b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="20c3b-105">**Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="20c3b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="20c3b-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="20c3b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="20c3b-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="20c3b-107">Not yet documented</span></span>


<span data-ttu-id="20c3b-108">Наследует [от deviceManagementConfigurationSettingApplicability](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md)</span><span class="sxs-lookup"><span data-stu-id="20c3b-108">Inherits from [deviceManagementConfigurationSettingApplicability](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md)</span></span>

## <a name="properties"></a><span data-ttu-id="20c3b-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="20c3b-109">Properties</span></span>
|<span data-ttu-id="20c3b-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="20c3b-110">Property</span></span>|<span data-ttu-id="20c3b-111">Тип</span><span class="sxs-lookup"><span data-stu-id="20c3b-111">Type</span></span>|<span data-ttu-id="20c3b-112">Описание</span><span class="sxs-lookup"><span data-stu-id="20c3b-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="20c3b-113">description</span><span class="sxs-lookup"><span data-stu-id="20c3b-113">description</span></span>|<span data-ttu-id="20c3b-114">Строка</span><span class="sxs-lookup"><span data-stu-id="20c3b-114">String</span></span>|<span data-ttu-id="20c3b-115">описание параметра Inherited from [deviceManagementConfigurationSettingApplicability](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md)</span><span class="sxs-lookup"><span data-stu-id="20c3b-115">description of the setting Inherited from [deviceManagementConfigurationSettingApplicability](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md)</span></span>|
|<span data-ttu-id="20c3b-116">платформа</span><span class="sxs-lookup"><span data-stu-id="20c3b-116">platform</span></span>|[<span data-ttu-id="20c3b-117">deviceManagementConfigurationPlatforms</span><span class="sxs-lookup"><span data-stu-id="20c3b-117">deviceManagementConfigurationPlatforms</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationplatforms.md)|<span data-ttu-id="20c3b-118">Параметр платформы можно применять на унаследованной от [deviceManagementConfigurationSettingApplicability.](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md)</span><span class="sxs-lookup"><span data-stu-id="20c3b-118">Platform setting can be applied on Inherited from [deviceManagementConfigurationSettingApplicability](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md).</span></span> <span data-ttu-id="20c3b-119">Возможные значения: `none`, `macOS`, `windows10X`, `windows10`.</span><span class="sxs-lookup"><span data-stu-id="20c3b-119">Possible values are: `none`, `macOS`, `windows10X`, `windows10`.</span></span>|
|<span data-ttu-id="20c3b-120">deviceMode</span><span class="sxs-lookup"><span data-stu-id="20c3b-120">deviceMode</span></span>|[<span data-ttu-id="20c3b-121">deviceManagementConfigurationDeviceMode</span><span class="sxs-lookup"><span data-stu-id="20c3b-121">deviceManagementConfigurationDeviceMode</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationdevicemode.md)|<span data-ttu-id="20c3b-122">Режим устройства, который можно применить в режиме Inherited from [deviceManagementConfigurationSettingApplicability.](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md)</span><span class="sxs-lookup"><span data-stu-id="20c3b-122">Device Mode that setting can be applied on Inherited from [deviceManagementConfigurationSettingApplicability](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md).</span></span> <span data-ttu-id="20c3b-123">Возможные значения: `none`, `kiosk`.</span><span class="sxs-lookup"><span data-stu-id="20c3b-123">Possible values are: `none`, `kiosk`.</span></span>|
|<span data-ttu-id="20c3b-124">технологии</span><span class="sxs-lookup"><span data-stu-id="20c3b-124">technologies</span></span>|[<span data-ttu-id="20c3b-125">deviceManagementConfigurationTechnologies</span><span class="sxs-lookup"><span data-stu-id="20c3b-125">deviceManagementConfigurationTechnologies</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationtechnologies.md)|<span data-ttu-id="20c3b-126">Какие технологические каналы этого параметра можно развернуть с помощью inherited from [deviceManagementConfigurationSettingApplicability.](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md)</span><span class="sxs-lookup"><span data-stu-id="20c3b-126">Which technology channels this setting can be deployed through Inherited from [deviceManagementConfigurationSettingApplicability](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md).</span></span> <span data-ttu-id="20c3b-127">Возможные значения: `none`, `mdm`, `windows10XManagement`, `configManager`, `microsoftSense`.</span><span class="sxs-lookup"><span data-stu-id="20c3b-127">Possible values are: `none`, `mdm`, `windows10XManagement`, `configManager`, `microsoftSense`.</span></span>|
|<span data-ttu-id="20c3b-128">configurationServiceProviderVersion</span><span class="sxs-lookup"><span data-stu-id="20c3b-128">configurationServiceProviderVersion</span></span>|<span data-ttu-id="20c3b-129">Строка</span><span class="sxs-lookup"><span data-stu-id="20c3b-129">String</span></span>|<span data-ttu-id="20c3b-130">Версия параметра CSP является частью</span><span class="sxs-lookup"><span data-stu-id="20c3b-130">Version of CSP setting is a part of</span></span>|
|<span data-ttu-id="20c3b-131">maximumSupportedVersion</span><span class="sxs-lookup"><span data-stu-id="20c3b-131">maximumSupportedVersion</span></span>|<span data-ttu-id="20c3b-132">Строка</span><span class="sxs-lookup"><span data-stu-id="20c3b-132">String</span></span>|<span data-ttu-id="20c3b-133">Максимально поддерживаемая версия Windows</span><span class="sxs-lookup"><span data-stu-id="20c3b-133">Maximum supported version of Windows</span></span>|
|<span data-ttu-id="20c3b-134">minimumSupportedVersion</span><span class="sxs-lookup"><span data-stu-id="20c3b-134">minimumSupportedVersion</span></span>|<span data-ttu-id="20c3b-135">Строка</span><span class="sxs-lookup"><span data-stu-id="20c3b-135">String</span></span>|<span data-ttu-id="20c3b-136">Минимальная поддерживаемая версия Windows</span><span class="sxs-lookup"><span data-stu-id="20c3b-136">Minimum supported version of Windows</span></span>|
|<span data-ttu-id="20c3b-137">windowsSkus</span><span class="sxs-lookup"><span data-stu-id="20c3b-137">windowsSkus</span></span>|<span data-ttu-id="20c3b-138">[коллекция deviceManagementConfigurationWindowsSkus](../resources/intune-deviceconfigv2-devicemanagementconfigurationwindowsskus.md)</span><span class="sxs-lookup"><span data-stu-id="20c3b-138">[deviceManagementConfigurationWindowsSkus](../resources/intune-deviceconfigv2-devicemanagementconfigurationwindowsskus.md) collection</span></span>|<span data-ttu-id="20c3b-139">Список Windows, применимых к этому параметру</span><span class="sxs-lookup"><span data-stu-id="20c3b-139">List of Windows SKUs that the setting is applicable for</span></span>|
|<span data-ttu-id="20c3b-140">requiresAzureAd</span><span class="sxs-lookup"><span data-stu-id="20c3b-140">requiresAzureAd</span></span>|<span data-ttu-id="20c3b-141">Логический</span><span class="sxs-lookup"><span data-stu-id="20c3b-141">Boolean</span></span>|<span data-ttu-id="20c3b-142">Требование параметра AzureAD</span><span class="sxs-lookup"><span data-stu-id="20c3b-142">AzureAD setting requirement</span></span>|
|<span data-ttu-id="20c3b-143">requiredAzureAdTrustType</span><span class="sxs-lookup"><span data-stu-id="20c3b-143">requiredAzureAdTrustType</span></span>|[<span data-ttu-id="20c3b-144">deviceManagementConfigurationAzureAdTrustType</span><span class="sxs-lookup"><span data-stu-id="20c3b-144">deviceManagementConfigurationAzureAdTrustType</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationazureadtrusttype.md)|<span data-ttu-id="20c3b-145">Необходимый тип доверия AzureAD.</span><span class="sxs-lookup"><span data-stu-id="20c3b-145">Required AzureAD trust type.</span></span> <span data-ttu-id="20c3b-146">Возможные значения: `none`, `azureAdJoined`, `addWorkAccount`, `mdmOnly`.</span><span class="sxs-lookup"><span data-stu-id="20c3b-146">Possible values are: `none`, `azureAdJoined`, `addWorkAccount`, `mdmOnly`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="20c3b-147">Связи</span><span class="sxs-lookup"><span data-stu-id="20c3b-147">Relationships</span></span>
<span data-ttu-id="20c3b-148">Нет</span><span class="sxs-lookup"><span data-stu-id="20c3b-148">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="20c3b-149">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="20c3b-149">JSON Representation</span></span>
<span data-ttu-id="20c3b-150">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="20c3b-150">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationWindowsSettingApplicability"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationWindowsSettingApplicability",
  "description": "String",
  "platform": "String",
  "deviceMode": "String",
  "technologies": "String",
  "configurationServiceProviderVersion": "String",
  "maximumSupportedVersion": "String",
  "minimumSupportedVersion": "String",
  "windowsSkus": [
    "String"
  ],
  "requiresAzureAd": true,
  "requiredAzureAdTrustType": "String"
}
```





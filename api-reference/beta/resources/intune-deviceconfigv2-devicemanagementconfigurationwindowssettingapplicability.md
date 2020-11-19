---
title: Тип ресурса Девицеманажементконфигуратионвиндовссеттингаппликабилити
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ca3b520a194a09d178790f5a82f3ca21c1e00d2d
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49301930"
---
# <a name="devicemanagementconfigurationwindowssettingapplicability-resource-type"></a><span data-ttu-id="49986-103">Тип ресурса Девицеманажементконфигуратионвиндовссеттингаппликабилити</span><span class="sxs-lookup"><span data-stu-id="49986-103">deviceManagementConfigurationWindowsSettingApplicability resource type</span></span>

<span data-ttu-id="49986-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="49986-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="49986-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="49986-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="49986-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="49986-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="49986-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="49986-107">Not yet documented</span></span>


<span data-ttu-id="49986-108">Наследуется от [девицеманажементконфигуратионсеттингаппликабилити](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md)</span><span class="sxs-lookup"><span data-stu-id="49986-108">Inherits from [deviceManagementConfigurationSettingApplicability](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md)</span></span>

## <a name="properties"></a><span data-ttu-id="49986-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="49986-109">Properties</span></span>
|<span data-ttu-id="49986-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="49986-110">Property</span></span>|<span data-ttu-id="49986-111">Тип</span><span class="sxs-lookup"><span data-stu-id="49986-111">Type</span></span>|<span data-ttu-id="49986-112">Описание</span><span class="sxs-lookup"><span data-stu-id="49986-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="49986-113">description</span><span class="sxs-lookup"><span data-stu-id="49986-113">description</span></span>|<span data-ttu-id="49986-114">String</span><span class="sxs-lookup"><span data-stu-id="49986-114">String</span></span>|<span data-ttu-id="49986-115">Описание параметра, унаследованного от [девицеманажементконфигуратионсеттингаппликабилити](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md)</span><span class="sxs-lookup"><span data-stu-id="49986-115">description of the setting Inherited from [deviceManagementConfigurationSettingApplicability](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md)</span></span>|
|<span data-ttu-id="49986-116">платформа</span><span class="sxs-lookup"><span data-stu-id="49986-116">platform</span></span>|[<span data-ttu-id="49986-117">девицеманажементконфигуратионплатформс</span><span class="sxs-lookup"><span data-stu-id="49986-117">deviceManagementConfigurationPlatforms</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationplatforms.md)|<span data-ttu-id="49986-118">Параметр платформы можно применять для наследования от [девицеманажементконфигуратионсеттингаппликабилити](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md).</span><span class="sxs-lookup"><span data-stu-id="49986-118">Platform setting can be applied on Inherited from [deviceManagementConfigurationSettingApplicability](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md).</span></span> <span data-ttu-id="49986-119">Возможные значения: `none`, `macOS`, `windows10X`, `windows10`.</span><span class="sxs-lookup"><span data-stu-id="49986-119">Possible values are: `none`, `macOS`, `windows10X`, `windows10`.</span></span>|
|<span data-ttu-id="49986-120">девицемоде</span><span class="sxs-lookup"><span data-stu-id="49986-120">deviceMode</span></span>|[<span data-ttu-id="49986-121">девицеманажементконфигуратиондевицемоде</span><span class="sxs-lookup"><span data-stu-id="49986-121">deviceManagementConfigurationDeviceMode</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationdevicemode.md)|<span data-ttu-id="49986-122">Режим устройства, с которым можно применять параметры, наследуемые от [девицеманажементконфигуратионсеттингаппликабилити](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md).</span><span class="sxs-lookup"><span data-stu-id="49986-122">Device Mode that setting can be applied on Inherited from [deviceManagementConfigurationSettingApplicability](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md).</span></span> <span data-ttu-id="49986-123">Возможные значения: `none`, `kiosk`.</span><span class="sxs-lookup"><span data-stu-id="49986-123">Possible values are: `none`, `kiosk`.</span></span>|
|<span data-ttu-id="49986-124">технологически</span><span class="sxs-lookup"><span data-stu-id="49986-124">technologies</span></span>|[<span data-ttu-id="49986-125">девицеманажементконфигуратионтечнологиес</span><span class="sxs-lookup"><span data-stu-id="49986-125">deviceManagementConfigurationTechnologies</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationtechnologies.md)|<span data-ttu-id="49986-126">Какие технологические каналы этот параметр можно развернуть с помощью наследования от [девицеманажементконфигуратионсеттингаппликабилити](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md).</span><span class="sxs-lookup"><span data-stu-id="49986-126">Which technology channels this setting can be deployed through Inherited from [deviceManagementConfigurationSettingApplicability](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md).</span></span> <span data-ttu-id="49986-127">Возможные значения: `none`, `mdm`, `windows10XManagement`, `configManager`.</span><span class="sxs-lookup"><span data-stu-id="49986-127">Possible values are: `none`, `mdm`, `windows10XManagement`, `configManager`.</span></span>|
|<span data-ttu-id="49986-128">конфигуратионсервицепровидерверсион</span><span class="sxs-lookup"><span data-stu-id="49986-128">configurationServiceProviderVersion</span></span>|<span data-ttu-id="49986-129">String</span><span class="sxs-lookup"><span data-stu-id="49986-129">String</span></span>|<span data-ttu-id="49986-130">Версия параметра CSP является частью</span><span class="sxs-lookup"><span data-stu-id="49986-130">Version of CSP setting is a part of</span></span>|
|<span data-ttu-id="49986-131">максимумсуппортедверсион</span><span class="sxs-lookup"><span data-stu-id="49986-131">maximumSupportedVersion</span></span>|<span data-ttu-id="49986-132">String</span><span class="sxs-lookup"><span data-stu-id="49986-132">String</span></span>|<span data-ttu-id="49986-133">Максимальная поддерживаемая версия Windows</span><span class="sxs-lookup"><span data-stu-id="49986-133">Maximum supported version of Windows</span></span>|
|<span data-ttu-id="49986-134">минимумсуппортедверсион</span><span class="sxs-lookup"><span data-stu-id="49986-134">minimumSupportedVersion</span></span>|<span data-ttu-id="49986-135">String</span><span class="sxs-lookup"><span data-stu-id="49986-135">String</span></span>|<span data-ttu-id="49986-136">Минимальная поддерживаемая версия Windows</span><span class="sxs-lookup"><span data-stu-id="49986-136">Minimum supported version of Windows</span></span>|
|<span data-ttu-id="49986-137">виндовсскус</span><span class="sxs-lookup"><span data-stu-id="49986-137">windowsSkus</span></span>|<span data-ttu-id="49986-138">Коллекция [девицеманажементконфигуратионвиндовсскус](../resources/intune-deviceconfigv2-devicemanagementconfigurationwindowsskus.md)</span><span class="sxs-lookup"><span data-stu-id="49986-138">[deviceManagementConfigurationWindowsSkus](../resources/intune-deviceconfigv2-devicemanagementconfigurationwindowsskus.md) collection</span></span>|<span data-ttu-id="49986-139">Список SKU Windows, к которым применяется параметр</span><span class="sxs-lookup"><span data-stu-id="49986-139">List of Windows SKUs that the setting is applicable for</span></span>|
|<span data-ttu-id="49986-140">рекуиресазуреад</span><span class="sxs-lookup"><span data-stu-id="49986-140">requiresAzureAd</span></span>|<span data-ttu-id="49986-141">Boolean</span><span class="sxs-lookup"><span data-stu-id="49986-141">Boolean</span></span>|<span data-ttu-id="49986-142">Требование к параметру AzureAD</span><span class="sxs-lookup"><span data-stu-id="49986-142">AzureAD setting requirement</span></span>|
|<span data-ttu-id="49986-143">рекуиредазуреадтрусттипе</span><span class="sxs-lookup"><span data-stu-id="49986-143">requiredAzureAdTrustType</span></span>|[<span data-ttu-id="49986-144">девицеманажементконфигуратионазуреадтрусттипе</span><span class="sxs-lookup"><span data-stu-id="49986-144">deviceManagementConfigurationAzureAdTrustType</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationazureadtrusttype.md)|<span data-ttu-id="49986-145">Обязательный тип доверия AzureAD.</span><span class="sxs-lookup"><span data-stu-id="49986-145">Required AzureAD trust type.</span></span> <span data-ttu-id="49986-146">Возможные значения: `none`, `azureAdJoined`, `addWorkAccount`, `mdmOnly`.</span><span class="sxs-lookup"><span data-stu-id="49986-146">Possible values are: `none`, `azureAdJoined`, `addWorkAccount`, `mdmOnly`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="49986-147">Связи</span><span class="sxs-lookup"><span data-stu-id="49986-147">Relationships</span></span>
<span data-ttu-id="49986-148">Нет</span><span class="sxs-lookup"><span data-stu-id="49986-148">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="49986-149">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="49986-149">JSON Representation</span></span>
<span data-ttu-id="49986-150">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="49986-150">Here is a JSON representation of the resource.</span></span>
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





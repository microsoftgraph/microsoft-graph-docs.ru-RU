---
title: тип ресурса deviceManagementConfigurationSettingApplicability
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b95e92c7ee9d6e520a326cb8918dcbfe05f83725
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/26/2021
ms.locfileid: "52665079"
---
# <a name="devicemanagementconfigurationsettingapplicability-resource-type"></a><span data-ttu-id="ddf61-103">тип ресурса deviceManagementConfigurationSettingApplicability</span><span class="sxs-lookup"><span data-stu-id="ddf61-103">deviceManagementConfigurationSettingApplicability resource type</span></span>

<span data-ttu-id="ddf61-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ddf61-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ddf61-105">**Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ddf61-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ddf61-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ddf61-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ddf61-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="ddf61-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="ddf61-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="ddf61-108">Properties</span></span>
|<span data-ttu-id="ddf61-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="ddf61-109">Property</span></span>|<span data-ttu-id="ddf61-110">Тип</span><span class="sxs-lookup"><span data-stu-id="ddf61-110">Type</span></span>|<span data-ttu-id="ddf61-111">Описание</span><span class="sxs-lookup"><span data-stu-id="ddf61-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ddf61-112">description</span><span class="sxs-lookup"><span data-stu-id="ddf61-112">description</span></span>|<span data-ttu-id="ddf61-113">Строка</span><span class="sxs-lookup"><span data-stu-id="ddf61-113">String</span></span>|<span data-ttu-id="ddf61-114">описание параметра</span><span class="sxs-lookup"><span data-stu-id="ddf61-114">description of the setting</span></span>|
|<span data-ttu-id="ddf61-115">платформа</span><span class="sxs-lookup"><span data-stu-id="ddf61-115">platform</span></span>|[<span data-ttu-id="ddf61-116">deviceManagementConfigurationPlatforms</span><span class="sxs-lookup"><span data-stu-id="ddf61-116">deviceManagementConfigurationPlatforms</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationplatforms.md)|<span data-ttu-id="ddf61-117">Параметр платформы можно применить.</span><span class="sxs-lookup"><span data-stu-id="ddf61-117">Platform setting can be applied on.</span></span> <span data-ttu-id="ddf61-118">Возможные значения: `none`, `macOS`, `windows10X`, `windows10`.</span><span class="sxs-lookup"><span data-stu-id="ddf61-118">Possible values are: `none`, `macOS`, `windows10X`, `windows10`.</span></span>|
|<span data-ttu-id="ddf61-119">deviceMode</span><span class="sxs-lookup"><span data-stu-id="ddf61-119">deviceMode</span></span>|[<span data-ttu-id="ddf61-120">deviceManagementConfigurationDeviceMode</span><span class="sxs-lookup"><span data-stu-id="ddf61-120">deviceManagementConfigurationDeviceMode</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationdevicemode.md)|<span data-ttu-id="ddf61-121">Режим устройства, на который можно применить параметр.</span><span class="sxs-lookup"><span data-stu-id="ddf61-121">Device Mode that setting can be applied on.</span></span> <span data-ttu-id="ddf61-122">Возможные значения: `none`, `kiosk`.</span><span class="sxs-lookup"><span data-stu-id="ddf61-122">Possible values are: `none`, `kiosk`.</span></span>|
|<span data-ttu-id="ddf61-123">технологии</span><span class="sxs-lookup"><span data-stu-id="ddf61-123">technologies</span></span>|[<span data-ttu-id="ddf61-124">deviceManagementConfigurationTechnologies</span><span class="sxs-lookup"><span data-stu-id="ddf61-124">deviceManagementConfigurationTechnologies</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationtechnologies.md)|<span data-ttu-id="ddf61-125">Какие технологические каналы этот параметр можно развернуть.</span><span class="sxs-lookup"><span data-stu-id="ddf61-125">Which technology channels this setting can be deployed through.</span></span> <span data-ttu-id="ddf61-126">Возможные значения: `none`, `mdm`, `windows10XManagement`, `configManager`, `microsoftSense`.</span><span class="sxs-lookup"><span data-stu-id="ddf61-126">Possible values are: `none`, `mdm`, `windows10XManagement`, `configManager`, `microsoftSense`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ddf61-127">Связи</span><span class="sxs-lookup"><span data-stu-id="ddf61-127">Relationships</span></span>
<span data-ttu-id="ddf61-128">Нет</span><span class="sxs-lookup"><span data-stu-id="ddf61-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ddf61-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ddf61-129">JSON Representation</span></span>
<span data-ttu-id="ddf61-130">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ddf61-130">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingApplicability"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationSettingApplicability",
  "description": "String",
  "platform": "String",
  "deviceMode": "String",
  "technologies": "String"
}
```





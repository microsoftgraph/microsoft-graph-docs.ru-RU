---
title: Тип ресурса Девицеманажементконфигуратионсеттингаппликабилити
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f94bfffd8dd3149d11e7ada38a4c238f4ce618a4
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49242192"
---
# <a name="devicemanagementconfigurationsettingapplicability-resource-type"></a><span data-ttu-id="e065a-103">Тип ресурса Девицеманажементконфигуратионсеттингаппликабилити</span><span class="sxs-lookup"><span data-stu-id="e065a-103">deviceManagementConfigurationSettingApplicability resource type</span></span>

<span data-ttu-id="e065a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e065a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e065a-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e065a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e065a-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e065a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e065a-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="e065a-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="e065a-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="e065a-108">Properties</span></span>
|<span data-ttu-id="e065a-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="e065a-109">Property</span></span>|<span data-ttu-id="e065a-110">Тип</span><span class="sxs-lookup"><span data-stu-id="e065a-110">Type</span></span>|<span data-ttu-id="e065a-111">Описание</span><span class="sxs-lookup"><span data-stu-id="e065a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e065a-112">description</span><span class="sxs-lookup"><span data-stu-id="e065a-112">description</span></span>|<span data-ttu-id="e065a-113">String</span><span class="sxs-lookup"><span data-stu-id="e065a-113">String</span></span>|<span data-ttu-id="e065a-114">Описание параметра</span><span class="sxs-lookup"><span data-stu-id="e065a-114">description of the setting</span></span>|
|<span data-ttu-id="e065a-115">платформа</span><span class="sxs-lookup"><span data-stu-id="e065a-115">platform</span></span>|[<span data-ttu-id="e065a-116">девицеманажементконфигуратионплатформс</span><span class="sxs-lookup"><span data-stu-id="e065a-116">deviceManagementConfigurationPlatforms</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationplatforms.md)|<span data-ttu-id="e065a-117">Параметр платформы можно применить к.</span><span class="sxs-lookup"><span data-stu-id="e065a-117">Platform setting can be applied on.</span></span> <span data-ttu-id="e065a-118">Возможные значения: `none`, `macOS`, `windows10X`, `windows10`.</span><span class="sxs-lookup"><span data-stu-id="e065a-118">Possible values are: `none`, `macOS`, `windows10X`, `windows10`.</span></span>|
|<span data-ttu-id="e065a-119">девицемоде</span><span class="sxs-lookup"><span data-stu-id="e065a-119">deviceMode</span></span>|[<span data-ttu-id="e065a-120">девицеманажементконфигуратиондевицемоде</span><span class="sxs-lookup"><span data-stu-id="e065a-120">deviceManagementConfigurationDeviceMode</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationdevicemode.md)|<span data-ttu-id="e065a-121">Режим устройства, к которому можно применять параметры.</span><span class="sxs-lookup"><span data-stu-id="e065a-121">Device Mode that setting can be applied on.</span></span> <span data-ttu-id="e065a-122">Возможные значения: `none`, `kiosk`.</span><span class="sxs-lookup"><span data-stu-id="e065a-122">Possible values are: `none`, `kiosk`.</span></span>|
|<span data-ttu-id="e065a-123">технологически</span><span class="sxs-lookup"><span data-stu-id="e065a-123">technologies</span></span>|[<span data-ttu-id="e065a-124">девицеманажементконфигуратионтечнологиес</span><span class="sxs-lookup"><span data-stu-id="e065a-124">deviceManagementConfigurationTechnologies</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationtechnologies.md)|<span data-ttu-id="e065a-125">Какие технологические каналы можно развернуть с помощью этого параметра.</span><span class="sxs-lookup"><span data-stu-id="e065a-125">Which technology channels this setting can be deployed through.</span></span> <span data-ttu-id="e065a-126">Возможные значения: `none`, `mdm`, `windows10XManagement`, `configManager`.</span><span class="sxs-lookup"><span data-stu-id="e065a-126">Possible values are: `none`, `mdm`, `windows10XManagement`, `configManager`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e065a-127">Связи</span><span class="sxs-lookup"><span data-stu-id="e065a-127">Relationships</span></span>
<span data-ttu-id="e065a-128">Нет</span><span class="sxs-lookup"><span data-stu-id="e065a-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e065a-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e065a-129">JSON Representation</span></span>
<span data-ttu-id="e065a-130">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e065a-130">Here is a JSON representation of the resource.</span></span>
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





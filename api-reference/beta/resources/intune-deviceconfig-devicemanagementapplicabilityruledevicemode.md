---
title: Тип ресурса Девицеманажементаппликабилитируледевицемоде
description: Пока не задокументировано.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 099f6081366187e240bf8510fca30a548fea4fe3
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42792040"
---
# <a name="devicemanagementapplicabilityruledevicemode-resource-type"></a><span data-ttu-id="35687-103">Тип ресурса Девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="35687-103">deviceManagementApplicabilityRuleDeviceMode resource type</span></span>

> <span data-ttu-id="35687-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="35687-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="35687-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="35687-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="35687-106">Н/Д</span><span class="sxs-lookup"><span data-stu-id="35687-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="35687-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="35687-107">Properties</span></span>
|<span data-ttu-id="35687-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="35687-108">Property</span></span>|<span data-ttu-id="35687-109">Тип</span><span class="sxs-lookup"><span data-stu-id="35687-109">Type</span></span>|<span data-ttu-id="35687-110">Описание</span><span class="sxs-lookup"><span data-stu-id="35687-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="35687-111">девицемоде</span><span class="sxs-lookup"><span data-stu-id="35687-111">deviceMode</span></span>|[<span data-ttu-id="35687-112">windows10DeviceModeType</span><span class="sxs-lookup"><span data-stu-id="35687-112">windows10DeviceModeType</span></span>](../resources/intune-deviceconfig-windows10devicemodetype.md)|<span data-ttu-id="35687-113">Правило применимости для режима устройства.</span><span class="sxs-lookup"><span data-stu-id="35687-113">Applicability rule for device mode.</span></span> <span data-ttu-id="35687-114">Возможные значения: `standardConfiguration`, `sModeConfiguration`.</span><span class="sxs-lookup"><span data-stu-id="35687-114">Possible values are: `standardConfiguration`, `sModeConfiguration`.</span></span>|
|<span data-ttu-id="35687-115">name</span><span class="sxs-lookup"><span data-stu-id="35687-115">name</span></span>|<span data-ttu-id="35687-116">String</span><span class="sxs-lookup"><span data-stu-id="35687-116">String</span></span>|<span data-ttu-id="35687-117">Имя объекта.</span><span class="sxs-lookup"><span data-stu-id="35687-117">Name for object.</span></span>|
|<span data-ttu-id="35687-118">ruleType</span><span class="sxs-lookup"><span data-stu-id="35687-118">ruleType</span></span>|[<span data-ttu-id="35687-119">deviceManagementApplicabilityRuleType</span><span class="sxs-lookup"><span data-stu-id="35687-119">deviceManagementApplicabilityRuleType</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruletype.md)|<span data-ttu-id="35687-120">Тип правила применимости.</span><span class="sxs-lookup"><span data-stu-id="35687-120">Applicability Rule type.</span></span> <span data-ttu-id="35687-121">Возможные значения: `include`, `exclude`.</span><span class="sxs-lookup"><span data-stu-id="35687-121">Possible values are: `include`, `exclude`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="35687-122">Связи</span><span class="sxs-lookup"><span data-stu-id="35687-122">Relationships</span></span>
<span data-ttu-id="35687-123">Нет</span><span class="sxs-lookup"><span data-stu-id="35687-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="35687-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="35687-124">JSON Representation</span></span>
<span data-ttu-id="35687-125">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="35687-125">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
  "deviceMode": "String",
  "name": "String",
  "ruleType": "String"
}
```




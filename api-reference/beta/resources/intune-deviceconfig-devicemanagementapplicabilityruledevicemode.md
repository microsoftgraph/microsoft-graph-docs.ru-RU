---
title: Тип ресурса Девицеманажементаппликабилитируледевицемоде
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 660263e729c4de0603f7d683a585981e0a4fd98f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47985953"
---
# <a name="devicemanagementapplicabilityruledevicemode-resource-type"></a><span data-ttu-id="32263-103">Тип ресурса Девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="32263-103">deviceManagementApplicabilityRuleDeviceMode resource type</span></span>

<span data-ttu-id="32263-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="32263-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="32263-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="32263-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="32263-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="32263-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="32263-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="32263-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="32263-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="32263-108">Properties</span></span>
|<span data-ttu-id="32263-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="32263-109">Property</span></span>|<span data-ttu-id="32263-110">Тип</span><span class="sxs-lookup"><span data-stu-id="32263-110">Type</span></span>|<span data-ttu-id="32263-111">Описание</span><span class="sxs-lookup"><span data-stu-id="32263-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="32263-112">девицемоде</span><span class="sxs-lookup"><span data-stu-id="32263-112">deviceMode</span></span>|[<span data-ttu-id="32263-113">windows10DeviceModeType</span><span class="sxs-lookup"><span data-stu-id="32263-113">windows10DeviceModeType</span></span>](../resources/intune-deviceconfig-windows10devicemodetype.md)|<span data-ttu-id="32263-114">Правило применимости для режима устройства.</span><span class="sxs-lookup"><span data-stu-id="32263-114">Applicability rule for device mode.</span></span> <span data-ttu-id="32263-115">Возможные значения: `standardConfiguration`, `sModeConfiguration`.</span><span class="sxs-lookup"><span data-stu-id="32263-115">Possible values are: `standardConfiguration`, `sModeConfiguration`.</span></span>|
|<span data-ttu-id="32263-116">name</span><span class="sxs-lookup"><span data-stu-id="32263-116">name</span></span>|<span data-ttu-id="32263-117">String</span><span class="sxs-lookup"><span data-stu-id="32263-117">String</span></span>|<span data-ttu-id="32263-118">Имя объекта.</span><span class="sxs-lookup"><span data-stu-id="32263-118">Name for object.</span></span>|
|<span data-ttu-id="32263-119">ruleType</span><span class="sxs-lookup"><span data-stu-id="32263-119">ruleType</span></span>|[<span data-ttu-id="32263-120">deviceManagementApplicabilityRuleType</span><span class="sxs-lookup"><span data-stu-id="32263-120">deviceManagementApplicabilityRuleType</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruletype.md)|<span data-ttu-id="32263-121">Тип правила применимости.</span><span class="sxs-lookup"><span data-stu-id="32263-121">Applicability Rule type.</span></span> <span data-ttu-id="32263-122">Возможные значения: `include`, `exclude`.</span><span class="sxs-lookup"><span data-stu-id="32263-122">Possible values are: `include`, `exclude`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="32263-123">Связи</span><span class="sxs-lookup"><span data-stu-id="32263-123">Relationships</span></span>
<span data-ttu-id="32263-124">Нет</span><span class="sxs-lookup"><span data-stu-id="32263-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="32263-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="32263-125">JSON Representation</span></span>
<span data-ttu-id="32263-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="32263-126">Here is a JSON representation of the resource.</span></span>
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







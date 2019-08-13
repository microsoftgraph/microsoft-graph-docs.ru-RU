---
title: Тип ресурса Девицеманажементаппликабилитируледевицемоде
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: f53d9f676dd50c49fc5222f50c24c2c9a6d08e22
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36332864"
---
# <a name="devicemanagementapplicabilityruledevicemode-resource-type"></a><span data-ttu-id="683a6-103">Тип ресурса Девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="683a6-103">deviceManagementApplicabilityRuleDeviceMode resource type</span></span>

> <span data-ttu-id="683a6-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="683a6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="683a6-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="683a6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="683a6-106">Н/Д</span><span class="sxs-lookup"><span data-stu-id="683a6-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="683a6-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="683a6-107">Properties</span></span>
|<span data-ttu-id="683a6-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="683a6-108">Property</span></span>|<span data-ttu-id="683a6-109">Тип</span><span class="sxs-lookup"><span data-stu-id="683a6-109">Type</span></span>|<span data-ttu-id="683a6-110">Описание</span><span class="sxs-lookup"><span data-stu-id="683a6-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="683a6-111">девицемоде</span><span class="sxs-lookup"><span data-stu-id="683a6-111">deviceMode</span></span>|[<span data-ttu-id="683a6-112">windows10DeviceModeType</span><span class="sxs-lookup"><span data-stu-id="683a6-112">windows10DeviceModeType</span></span>](../resources/intune-deviceconfig-windows10devicemodetype.md)|<span data-ttu-id="683a6-113">Правило применимости для режима устройства.</span><span class="sxs-lookup"><span data-stu-id="683a6-113">Applicability rule for device mode.</span></span> <span data-ttu-id="683a6-114">Возможные значения: `standardConfiguration`, `sModeConfiguration`.</span><span class="sxs-lookup"><span data-stu-id="683a6-114">Possible values are: `standardConfiguration`, `sModeConfiguration`.</span></span>|
|<span data-ttu-id="683a6-115">name</span><span class="sxs-lookup"><span data-stu-id="683a6-115">name</span></span>|<span data-ttu-id="683a6-116">String</span><span class="sxs-lookup"><span data-stu-id="683a6-116">String</span></span>|<span data-ttu-id="683a6-117">Имя объекта.</span><span class="sxs-lookup"><span data-stu-id="683a6-117">Name for object.</span></span>|
|<span data-ttu-id="683a6-118">ruleType</span><span class="sxs-lookup"><span data-stu-id="683a6-118">ruleType</span></span>|[<span data-ttu-id="683a6-119">девицеманажементаппликабилитирулетипе</span><span class="sxs-lookup"><span data-stu-id="683a6-119">deviceManagementApplicabilityRuleType</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruletype.md)|<span data-ttu-id="683a6-120">Тип правила применимости.</span><span class="sxs-lookup"><span data-stu-id="683a6-120">Applicability Rule type.</span></span> <span data-ttu-id="683a6-121">Возможные значения: `include`, `exclude`.</span><span class="sxs-lookup"><span data-stu-id="683a6-121">Possible values are: `include`, `exclude`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="683a6-122">Отношения</span><span class="sxs-lookup"><span data-stu-id="683a6-122">Relationships</span></span>
<span data-ttu-id="683a6-123">Нет</span><span class="sxs-lookup"><span data-stu-id="683a6-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="683a6-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="683a6-124">JSON Representation</span></span>
<span data-ttu-id="683a6-125">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="683a6-125">Here is a JSON representation of the resource.</span></span>
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




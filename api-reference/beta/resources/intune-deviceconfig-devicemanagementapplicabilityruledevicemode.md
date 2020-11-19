---
title: Тип ресурса Девицеманажементаппликабилитируледевицемоде
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c6e85a8f634085442a02b47747c508266279e5cc
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49283597"
---
# <a name="devicemanagementapplicabilityruledevicemode-resource-type"></a><span data-ttu-id="92e84-103">Тип ресурса Девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="92e84-103">deviceManagementApplicabilityRuleDeviceMode resource type</span></span>

<span data-ttu-id="92e84-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="92e84-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="92e84-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="92e84-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="92e84-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="92e84-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="92e84-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="92e84-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="92e84-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="92e84-108">Properties</span></span>
|<span data-ttu-id="92e84-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="92e84-109">Property</span></span>|<span data-ttu-id="92e84-110">Тип</span><span class="sxs-lookup"><span data-stu-id="92e84-110">Type</span></span>|<span data-ttu-id="92e84-111">Описание</span><span class="sxs-lookup"><span data-stu-id="92e84-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="92e84-112">девицемоде</span><span class="sxs-lookup"><span data-stu-id="92e84-112">deviceMode</span></span>|[<span data-ttu-id="92e84-113">windows10DeviceModeType</span><span class="sxs-lookup"><span data-stu-id="92e84-113">windows10DeviceModeType</span></span>](../resources/intune-deviceconfig-windows10devicemodetype.md)|<span data-ttu-id="92e84-114">Правило применимости для режима устройства.</span><span class="sxs-lookup"><span data-stu-id="92e84-114">Applicability rule for device mode.</span></span> <span data-ttu-id="92e84-115">Возможные значения: `standardConfiguration`, `sModeConfiguration`.</span><span class="sxs-lookup"><span data-stu-id="92e84-115">Possible values are: `standardConfiguration`, `sModeConfiguration`.</span></span>|
|<span data-ttu-id="92e84-116">name</span><span class="sxs-lookup"><span data-stu-id="92e84-116">name</span></span>|<span data-ttu-id="92e84-117">String</span><span class="sxs-lookup"><span data-stu-id="92e84-117">String</span></span>|<span data-ttu-id="92e84-118">Имя объекта.</span><span class="sxs-lookup"><span data-stu-id="92e84-118">Name for object.</span></span>|
|<span data-ttu-id="92e84-119">ruleType</span><span class="sxs-lookup"><span data-stu-id="92e84-119">ruleType</span></span>|[<span data-ttu-id="92e84-120">deviceManagementApplicabilityRuleType</span><span class="sxs-lookup"><span data-stu-id="92e84-120">deviceManagementApplicabilityRuleType</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruletype.md)|<span data-ttu-id="92e84-121">Тип правила применимости.</span><span class="sxs-lookup"><span data-stu-id="92e84-121">Applicability Rule type.</span></span> <span data-ttu-id="92e84-122">Возможные значения: `include`, `exclude`.</span><span class="sxs-lookup"><span data-stu-id="92e84-122">Possible values are: `include`, `exclude`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="92e84-123">Связи</span><span class="sxs-lookup"><span data-stu-id="92e84-123">Relationships</span></span>
<span data-ttu-id="92e84-124">Нет</span><span class="sxs-lookup"><span data-stu-id="92e84-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="92e84-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="92e84-125">JSON Representation</span></span>
<span data-ttu-id="92e84-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="92e84-126">Here is a JSON representation of the resource.</span></span>
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





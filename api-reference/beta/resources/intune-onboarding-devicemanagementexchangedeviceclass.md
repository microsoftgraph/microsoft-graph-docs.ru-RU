---
title: Тип ресурса Девицеманажементексчанжедевицекласс
description: Класс устройства в Exchange.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 384fa172c255ec3f21ec0088c2b9f4ab025768ce
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42779032"
---
# <a name="devicemanagementexchangedeviceclass-resource-type"></a><span data-ttu-id="375b8-103">Тип ресурса Девицеманажементексчанжедевицекласс</span><span class="sxs-lookup"><span data-stu-id="375b8-103">deviceManagementExchangeDeviceClass resource type</span></span>

> <span data-ttu-id="375b8-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="375b8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="375b8-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="375b8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="375b8-106">Класс устройства в Exchange.</span><span class="sxs-lookup"><span data-stu-id="375b8-106">Device Class in Exchange.</span></span>

## <a name="properties"></a><span data-ttu-id="375b8-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="375b8-107">Properties</span></span>
|<span data-ttu-id="375b8-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="375b8-108">Property</span></span>|<span data-ttu-id="375b8-109">Тип</span><span class="sxs-lookup"><span data-stu-id="375b8-109">Type</span></span>|<span data-ttu-id="375b8-110">Описание</span><span class="sxs-lookup"><span data-stu-id="375b8-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="375b8-111">name</span><span class="sxs-lookup"><span data-stu-id="375b8-111">name</span></span>|<span data-ttu-id="375b8-112">String</span><span class="sxs-lookup"><span data-stu-id="375b8-112">String</span></span>|<span data-ttu-id="375b8-113">Имя класса устройств, на который влияет это правило.</span><span class="sxs-lookup"><span data-stu-id="375b8-113">Name of the device class which will be impacted by this rule.</span></span>|
|<span data-ttu-id="375b8-114">type</span><span class="sxs-lookup"><span data-stu-id="375b8-114">type</span></span>|[<span data-ttu-id="375b8-115">девицеманажементексчанжеакцессрулетипе</span><span class="sxs-lookup"><span data-stu-id="375b8-115">deviceManagementExchangeAccessRuleType</span></span>](../resources/intune-onboarding-devicemanagementexchangeaccessruletype.md)|<span data-ttu-id="375b8-116">Тип устройства, на которое влияет это правило, например Model, Family.</span><span class="sxs-lookup"><span data-stu-id="375b8-116">Type of device which is impacted by this rule e.g. Model, Family.</span></span> <span data-ttu-id="375b8-117">Возможные значения: `family`, `model`.</span><span class="sxs-lookup"><span data-stu-id="375b8-117">Possible values are: `family`, `model`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="375b8-118">Связи</span><span class="sxs-lookup"><span data-stu-id="375b8-118">Relationships</span></span>
<span data-ttu-id="375b8-119">Нет</span><span class="sxs-lookup"><span data-stu-id="375b8-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="375b8-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="375b8-120">JSON Representation</span></span>
<span data-ttu-id="375b8-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="375b8-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementExchangeDeviceClass"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementExchangeDeviceClass",
  "name": "String",
  "type": "String"
}
```




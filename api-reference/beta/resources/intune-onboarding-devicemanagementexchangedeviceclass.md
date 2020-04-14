---
title: Тип ресурса Девицеманажементексчанжедевицекласс
description: Класс устройства в Exchange.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 4099009c67e2c5b0ce8cc5b3c52dd00b1fd32aec
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43448045"
---
# <a name="devicemanagementexchangedeviceclass-resource-type"></a><span data-ttu-id="f928b-103">Тип ресурса Девицеманажементексчанжедевицекласс</span><span class="sxs-lookup"><span data-stu-id="f928b-103">deviceManagementExchangeDeviceClass resource type</span></span>

<span data-ttu-id="f928b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f928b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f928b-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f928b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f928b-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f928b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f928b-107">Класс устройства в Exchange.</span><span class="sxs-lookup"><span data-stu-id="f928b-107">Device Class in Exchange.</span></span>

## <a name="properties"></a><span data-ttu-id="f928b-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="f928b-108">Properties</span></span>
|<span data-ttu-id="f928b-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="f928b-109">Property</span></span>|<span data-ttu-id="f928b-110">Тип</span><span class="sxs-lookup"><span data-stu-id="f928b-110">Type</span></span>|<span data-ttu-id="f928b-111">Описание</span><span class="sxs-lookup"><span data-stu-id="f928b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f928b-112">name</span><span class="sxs-lookup"><span data-stu-id="f928b-112">name</span></span>|<span data-ttu-id="f928b-113">String</span><span class="sxs-lookup"><span data-stu-id="f928b-113">String</span></span>|<span data-ttu-id="f928b-114">Имя класса устройств, на который влияет это правило.</span><span class="sxs-lookup"><span data-stu-id="f928b-114">Name of the device class which will be impacted by this rule.</span></span>|
|<span data-ttu-id="f928b-115">type</span><span class="sxs-lookup"><span data-stu-id="f928b-115">type</span></span>|[<span data-ttu-id="f928b-116">девицеманажементексчанжеакцессрулетипе</span><span class="sxs-lookup"><span data-stu-id="f928b-116">deviceManagementExchangeAccessRuleType</span></span>](../resources/intune-onboarding-devicemanagementexchangeaccessruletype.md)|<span data-ttu-id="f928b-117">Тип устройства, на которое влияет это правило, например Model, Family.</span><span class="sxs-lookup"><span data-stu-id="f928b-117">Type of device which is impacted by this rule e.g. Model, Family.</span></span> <span data-ttu-id="f928b-118">Возможные значения: `family`, `model`.</span><span class="sxs-lookup"><span data-stu-id="f928b-118">Possible values are: `family`, `model`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f928b-119">Связи</span><span class="sxs-lookup"><span data-stu-id="f928b-119">Relationships</span></span>
<span data-ttu-id="f928b-120">Нет</span><span class="sxs-lookup"><span data-stu-id="f928b-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f928b-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f928b-121">JSON Representation</span></span>
<span data-ttu-id="f928b-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f928b-122">Here is a JSON representation of the resource.</span></span>
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




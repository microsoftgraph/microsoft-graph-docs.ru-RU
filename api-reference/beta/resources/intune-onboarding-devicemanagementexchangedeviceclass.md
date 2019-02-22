---
title: Тип ресурса Девицеманажементексчанжедевицекласс
description: Класс устройства в Exchange.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ffa5f9c9f54722711a2e38116c2f2a3e03a3171e
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30149569"
---
# <a name="devicemanagementexchangedeviceclass-resource-type"></a><span data-ttu-id="194cf-103">Тип ресурса Девицеманажементексчанжедевицекласс</span><span class="sxs-lookup"><span data-stu-id="194cf-103">deviceManagementExchangeDeviceClass resource type</span></span>

> <span data-ttu-id="194cf-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="194cf-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="194cf-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="194cf-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="194cf-106">Класс устройства в Exchange.</span><span class="sxs-lookup"><span data-stu-id="194cf-106">Device Class in Exchange.</span></span>

## <a name="properties"></a><span data-ttu-id="194cf-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="194cf-107">Properties</span></span>
|<span data-ttu-id="194cf-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="194cf-108">Property</span></span>|<span data-ttu-id="194cf-109">Тип</span><span class="sxs-lookup"><span data-stu-id="194cf-109">Type</span></span>|<span data-ttu-id="194cf-110">Описание</span><span class="sxs-lookup"><span data-stu-id="194cf-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="194cf-111">name</span><span class="sxs-lookup"><span data-stu-id="194cf-111">name</span></span>|<span data-ttu-id="194cf-112">String</span><span class="sxs-lookup"><span data-stu-id="194cf-112">String</span></span>|<span data-ttu-id="194cf-113">Имя класса устройств, на который влияет это правило.</span><span class="sxs-lookup"><span data-stu-id="194cf-113">Name of the device class which will be impacted by this rule.</span></span>|
|<span data-ttu-id="194cf-114">type</span><span class="sxs-lookup"><span data-stu-id="194cf-114">type</span></span>|[<span data-ttu-id="194cf-115">Девицеманажементексчанжеакцессрулетипе</span><span class="sxs-lookup"><span data-stu-id="194cf-115">deviceManagementExchangeAccessRuleType</span></span>](../resources/intune-onboarding-devicemanagementexchangeaccessruletype.md)|<span data-ttu-id="194cf-116">Тип устройства, на которое влияет это правило, например Model, Family.</span><span class="sxs-lookup"><span data-stu-id="194cf-116">Type of device which is impacted by this rule e.g. Model, Family.</span></span> <span data-ttu-id="194cf-117">Возможные значения: `family`, `model`.</span><span class="sxs-lookup"><span data-stu-id="194cf-117">Possible values are: `family`, `model`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="194cf-118">Связи</span><span class="sxs-lookup"><span data-stu-id="194cf-118">Relationships</span></span>
<span data-ttu-id="194cf-119">Нет</span><span class="sxs-lookup"><span data-stu-id="194cf-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="194cf-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="194cf-120">JSON Representation</span></span>
<span data-ttu-id="194cf-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="194cf-121">Here is a JSON representation of the resource.</span></span>
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





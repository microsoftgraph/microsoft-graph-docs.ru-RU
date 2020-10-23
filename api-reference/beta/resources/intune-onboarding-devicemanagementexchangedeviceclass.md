---
title: Тип ресурса Девицеманажементексчанжедевицекласс
description: Класс устройства в Exchange.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c50a15e6c58b5526f773b783887acfed25ed58e7
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48736095"
---
# <a name="devicemanagementexchangedeviceclass-resource-type"></a><span data-ttu-id="7d7a1-103">Тип ресурса Девицеманажементексчанжедевицекласс</span><span class="sxs-lookup"><span data-stu-id="7d7a1-103">deviceManagementExchangeDeviceClass resource type</span></span>

<span data-ttu-id="7d7a1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7d7a1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7d7a1-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7d7a1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7d7a1-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7d7a1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7d7a1-107">Класс устройства в Exchange.</span><span class="sxs-lookup"><span data-stu-id="7d7a1-107">Device Class in Exchange.</span></span>

## <a name="properties"></a><span data-ttu-id="7d7a1-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="7d7a1-108">Properties</span></span>
|<span data-ttu-id="7d7a1-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="7d7a1-109">Property</span></span>|<span data-ttu-id="7d7a1-110">Тип</span><span class="sxs-lookup"><span data-stu-id="7d7a1-110">Type</span></span>|<span data-ttu-id="7d7a1-111">Описание</span><span class="sxs-lookup"><span data-stu-id="7d7a1-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7d7a1-112">name</span><span class="sxs-lookup"><span data-stu-id="7d7a1-112">name</span></span>|<span data-ttu-id="7d7a1-113">String</span><span class="sxs-lookup"><span data-stu-id="7d7a1-113">String</span></span>|<span data-ttu-id="7d7a1-114">Имя класса устройств, на который влияет это правило.</span><span class="sxs-lookup"><span data-stu-id="7d7a1-114">Name of the device class which will be impacted by this rule.</span></span>|
|<span data-ttu-id="7d7a1-115">type</span><span class="sxs-lookup"><span data-stu-id="7d7a1-115">type</span></span>|[<span data-ttu-id="7d7a1-116">девицеманажементексчанжеакцессрулетипе</span><span class="sxs-lookup"><span data-stu-id="7d7a1-116">deviceManagementExchangeAccessRuleType</span></span>](../resources/intune-onboarding-devicemanagementexchangeaccessruletype.md)|<span data-ttu-id="7d7a1-117">Тип устройства, на которое влияет это правило, например Model, Family.</span><span class="sxs-lookup"><span data-stu-id="7d7a1-117">Type of device which is impacted by this rule e.g. Model, Family.</span></span> <span data-ttu-id="7d7a1-118">Возможные значения: `family`, `model`.</span><span class="sxs-lookup"><span data-stu-id="7d7a1-118">Possible values are: `family`, `model`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7d7a1-119">Связи</span><span class="sxs-lookup"><span data-stu-id="7d7a1-119">Relationships</span></span>
<span data-ttu-id="7d7a1-120">Нет</span><span class="sxs-lookup"><span data-stu-id="7d7a1-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7d7a1-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7d7a1-121">JSON Representation</span></span>
<span data-ttu-id="7d7a1-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7d7a1-122">Here is a JSON representation of the resource.</span></span>
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






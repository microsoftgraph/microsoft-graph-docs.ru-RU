---
title: Тип ресурса Девицеманажементексчанжедевицекласс
description: Класс устройства в Exchange.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 8e881c827d4f357679b20095a75d7ac4b4ea4c37
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36372876"
---
# <a name="devicemanagementexchangedeviceclass-resource-type"></a><span data-ttu-id="bc068-103">Тип ресурса Девицеманажементексчанжедевицекласс</span><span class="sxs-lookup"><span data-stu-id="bc068-103">deviceManagementExchangeDeviceClass resource type</span></span>

> <span data-ttu-id="bc068-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bc068-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bc068-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bc068-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bc068-106">Класс устройства в Exchange.</span><span class="sxs-lookup"><span data-stu-id="bc068-106">Device Class in Exchange.</span></span>

## <a name="properties"></a><span data-ttu-id="bc068-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="bc068-107">Properties</span></span>
|<span data-ttu-id="bc068-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="bc068-108">Property</span></span>|<span data-ttu-id="bc068-109">Тип</span><span class="sxs-lookup"><span data-stu-id="bc068-109">Type</span></span>|<span data-ttu-id="bc068-110">Описание</span><span class="sxs-lookup"><span data-stu-id="bc068-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bc068-111">name</span><span class="sxs-lookup"><span data-stu-id="bc068-111">name</span></span>|<span data-ttu-id="bc068-112">String</span><span class="sxs-lookup"><span data-stu-id="bc068-112">String</span></span>|<span data-ttu-id="bc068-113">Имя класса устройств, на который влияет это правило.</span><span class="sxs-lookup"><span data-stu-id="bc068-113">Name of the device class which will be impacted by this rule.</span></span>|
|<span data-ttu-id="bc068-114">type</span><span class="sxs-lookup"><span data-stu-id="bc068-114">type</span></span>|[<span data-ttu-id="bc068-115">девицеманажементексчанжеакцессрулетипе</span><span class="sxs-lookup"><span data-stu-id="bc068-115">deviceManagementExchangeAccessRuleType</span></span>](../resources/intune-onboarding-devicemanagementexchangeaccessruletype.md)|<span data-ttu-id="bc068-116">Тип устройства, на которое влияет это правило, например Model, Family.</span><span class="sxs-lookup"><span data-stu-id="bc068-116">Type of device which is impacted by this rule e.g. Model, Family.</span></span> <span data-ttu-id="bc068-117">Возможные значения: `family`, `model`.</span><span class="sxs-lookup"><span data-stu-id="bc068-117">Possible values are: `family`, `model`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bc068-118">Отношения</span><span class="sxs-lookup"><span data-stu-id="bc068-118">Relationships</span></span>
<span data-ttu-id="bc068-119">Нет</span><span class="sxs-lookup"><span data-stu-id="bc068-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bc068-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bc068-120">JSON Representation</span></span>
<span data-ttu-id="bc068-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bc068-121">Here is a JSON representation of the resource.</span></span>
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




---
title: Тип ресурса Девицеманажементексчанжедевицекласс
description: Класс устройства в Exchange.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 4304fb138ede5cf35db07bbb08814f3d8fcf532f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42527745"
---
# <a name="devicemanagementexchangedeviceclass-resource-type"></a><span data-ttu-id="3f5e7-103">Тип ресурса Девицеманажементексчанжедевицекласс</span><span class="sxs-lookup"><span data-stu-id="3f5e7-103">deviceManagementExchangeDeviceClass resource type</span></span>

<span data-ttu-id="3f5e7-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="3f5e7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3f5e7-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3f5e7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3f5e7-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3f5e7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3f5e7-107">Класс устройства в Exchange.</span><span class="sxs-lookup"><span data-stu-id="3f5e7-107">Device Class in Exchange.</span></span>

## <a name="properties"></a><span data-ttu-id="3f5e7-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="3f5e7-108">Properties</span></span>
|<span data-ttu-id="3f5e7-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="3f5e7-109">Property</span></span>|<span data-ttu-id="3f5e7-110">Тип</span><span class="sxs-lookup"><span data-stu-id="3f5e7-110">Type</span></span>|<span data-ttu-id="3f5e7-111">Описание</span><span class="sxs-lookup"><span data-stu-id="3f5e7-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3f5e7-112">name</span><span class="sxs-lookup"><span data-stu-id="3f5e7-112">name</span></span>|<span data-ttu-id="3f5e7-113">String</span><span class="sxs-lookup"><span data-stu-id="3f5e7-113">String</span></span>|<span data-ttu-id="3f5e7-114">Имя класса устройств, на который влияет это правило.</span><span class="sxs-lookup"><span data-stu-id="3f5e7-114">Name of the device class which will be impacted by this rule.</span></span>|
|<span data-ttu-id="3f5e7-115">type</span><span class="sxs-lookup"><span data-stu-id="3f5e7-115">type</span></span>|[<span data-ttu-id="3f5e7-116">девицеманажементексчанжеакцессрулетипе</span><span class="sxs-lookup"><span data-stu-id="3f5e7-116">deviceManagementExchangeAccessRuleType</span></span>](../resources/intune-onboarding-devicemanagementexchangeaccessruletype.md)|<span data-ttu-id="3f5e7-117">Тип устройства, на которое влияет это правило, например Model, Family.</span><span class="sxs-lookup"><span data-stu-id="3f5e7-117">Type of device which is impacted by this rule e.g. Model, Family.</span></span> <span data-ttu-id="3f5e7-118">Возможные значения: `family`, `model`.</span><span class="sxs-lookup"><span data-stu-id="3f5e7-118">Possible values are: `family`, `model`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3f5e7-119">Связи</span><span class="sxs-lookup"><span data-stu-id="3f5e7-119">Relationships</span></span>
<span data-ttu-id="3f5e7-120">Нет</span><span class="sxs-lookup"><span data-stu-id="3f5e7-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3f5e7-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3f5e7-121">JSON Representation</span></span>
<span data-ttu-id="3f5e7-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3f5e7-122">Here is a JSON representation of the resource.</span></span>
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




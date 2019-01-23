---
title: Тип ресурса deviceManagementExchangeDeviceClass
description: Класс устройств в Exchange.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 3e512253a9b9bc4228d41c369501bec1e7a5e031
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29413733"
---
# <a name="devicemanagementexchangedeviceclass-resource-type"></a><span data-ttu-id="dc388-103">Тип ресурса deviceManagementExchangeDeviceClass</span><span class="sxs-lookup"><span data-stu-id="dc388-103">deviceManagementExchangeDeviceClass resource type</span></span>

> <span data-ttu-id="dc388-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="dc388-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="dc388-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dc388-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="dc388-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="dc388-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dc388-107">Класс устройств в Exchange.</span><span class="sxs-lookup"><span data-stu-id="dc388-107">Device Class in Exchange.</span></span>

## <a name="properties"></a><span data-ttu-id="dc388-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="dc388-108">Properties</span></span>
|<span data-ttu-id="dc388-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="dc388-109">Property</span></span>|<span data-ttu-id="dc388-110">Тип</span><span class="sxs-lookup"><span data-stu-id="dc388-110">Type</span></span>|<span data-ttu-id="dc388-111">Описание</span><span class="sxs-lookup"><span data-stu-id="dc388-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dc388-112">name</span><span class="sxs-lookup"><span data-stu-id="dc388-112">name</span></span>|<span data-ttu-id="dc388-113">String</span><span class="sxs-lookup"><span data-stu-id="dc388-113">String</span></span>|<span data-ttu-id="dc388-114">Имя класса устройства, которое будет затронут этого правила.</span><span class="sxs-lookup"><span data-stu-id="dc388-114">Name of the device class which will be impacted by this rule.</span></span>|
|<span data-ttu-id="dc388-115">type</span><span class="sxs-lookup"><span data-stu-id="dc388-115">type</span></span>|[<span data-ttu-id="dc388-116">deviceManagementExchangeAccessRuleType</span><span class="sxs-lookup"><span data-stu-id="dc388-116">deviceManagementExchangeAccessRuleType</span></span>](../resources/intune-onboarding-devicemanagementexchangeaccessruletype.md)|<span data-ttu-id="dc388-117">Тип устройства, который влияет этот правило семейства, например модели.</span><span class="sxs-lookup"><span data-stu-id="dc388-117">Type of device which is impacted by this rule e.g. Model, Family.</span></span> <span data-ttu-id="dc388-118">Возможные значения: `family`, `model`.</span><span class="sxs-lookup"><span data-stu-id="dc388-118">Possible values are: `family`, `model`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="dc388-119">Связи</span><span class="sxs-lookup"><span data-stu-id="dc388-119">Relationships</span></span>
<span data-ttu-id="dc388-120">Нет</span><span class="sxs-lookup"><span data-stu-id="dc388-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="dc388-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="dc388-121">JSON Representation</span></span>
<span data-ttu-id="dc388-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="dc388-122">Here is a JSON representation of the resource.</span></span>
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





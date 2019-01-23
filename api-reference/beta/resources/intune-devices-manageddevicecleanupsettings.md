---
title: Тип ресурса managedDeviceCleanupSettings
description: Определение правила, когда администратор хочет устройств, чтобы очистить.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 4bf756072dcc3cd13bda2fda59b8688b63f3cd43
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29424569"
---
# <a name="manageddevicecleanupsettings-resource-type"></a><span data-ttu-id="d3c5e-103">Тип ресурса managedDeviceCleanupSettings</span><span class="sxs-lookup"><span data-stu-id="d3c5e-103">managedDeviceCleanupSettings resource type</span></span>

> <span data-ttu-id="d3c5e-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="d3c5e-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="d3c5e-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d3c5e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d3c5e-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d3c5e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d3c5e-107">Определение правила, когда администратор хочет устройств, чтобы очистить.</span><span class="sxs-lookup"><span data-stu-id="d3c5e-107">Define the rule when the admin wants the devices to be cleaned up.</span></span>

## <a name="properties"></a><span data-ttu-id="d3c5e-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="d3c5e-108">Properties</span></span>
|<span data-ttu-id="d3c5e-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="d3c5e-109">Property</span></span>|<span data-ttu-id="d3c5e-110">Тип</span><span class="sxs-lookup"><span data-stu-id="d3c5e-110">Type</span></span>|<span data-ttu-id="d3c5e-111">Описание</span><span class="sxs-lookup"><span data-stu-id="d3c5e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d3c5e-112">deviceInactivityBeforeRetirementInDays</span><span class="sxs-lookup"><span data-stu-id="d3c5e-112">deviceInactivityBeforeRetirementInDays</span></span>|<span data-ttu-id="d3c5e-113">String</span><span class="sxs-lookup"><span data-stu-id="d3c5e-113">String</span></span>|<span data-ttu-id="d3c5e-114">Количество дней, когда устройство имеет не связаться с Intune.</span><span class="sxs-lookup"><span data-stu-id="d3c5e-114">Number of days when the device has not contacted Intune.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d3c5e-115">Отношения</span><span class="sxs-lookup"><span data-stu-id="d3c5e-115">Relationships</span></span>
<span data-ttu-id="d3c5e-116">Нет</span><span class="sxs-lookup"><span data-stu-id="d3c5e-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d3c5e-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d3c5e-117">JSON Representation</span></span>
<span data-ttu-id="d3c5e-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d3c5e-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedDeviceCleanupSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDeviceCleanupSettings",
  "deviceInactivityBeforeRetirementInDays": "String"
}
```





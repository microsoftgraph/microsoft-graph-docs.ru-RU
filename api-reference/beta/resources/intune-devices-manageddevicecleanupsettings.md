---
title: Тип ресурса Манажеддевицеклеанупсеттингс
description: Определите правило, когда администратор хочет очистить устройства.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 86003dfd0121b6d4056377e8cf340497f41ccbd9
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42783965"
---
# <a name="manageddevicecleanupsettings-resource-type"></a><span data-ttu-id="cdb1a-103">Тип ресурса Манажеддевицеклеанупсеттингс</span><span class="sxs-lookup"><span data-stu-id="cdb1a-103">managedDeviceCleanupSettings resource type</span></span>

> <span data-ttu-id="cdb1a-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cdb1a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cdb1a-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="cdb1a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cdb1a-106">Определите правило, когда администратор хочет очистить устройства.</span><span class="sxs-lookup"><span data-stu-id="cdb1a-106">Define the rule when the admin wants the devices to be cleaned up.</span></span>

## <a name="properties"></a><span data-ttu-id="cdb1a-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="cdb1a-107">Properties</span></span>
|<span data-ttu-id="cdb1a-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="cdb1a-108">Property</span></span>|<span data-ttu-id="cdb1a-109">Тип</span><span class="sxs-lookup"><span data-stu-id="cdb1a-109">Type</span></span>|<span data-ttu-id="cdb1a-110">Описание</span><span class="sxs-lookup"><span data-stu-id="cdb1a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cdb1a-111">девицеинактивитибефореретирементиндайс</span><span class="sxs-lookup"><span data-stu-id="cdb1a-111">deviceInactivityBeforeRetirementInDays</span></span>|<span data-ttu-id="cdb1a-112">String</span><span class="sxs-lookup"><span data-stu-id="cdb1a-112">String</span></span>|<span data-ttu-id="cdb1a-113">Количество дней, когда устройство не связывалось с Intune.</span><span class="sxs-lookup"><span data-stu-id="cdb1a-113">Number of days when the device has not contacted Intune.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cdb1a-114">Связи</span><span class="sxs-lookup"><span data-stu-id="cdb1a-114">Relationships</span></span>
<span data-ttu-id="cdb1a-115">Нет</span><span class="sxs-lookup"><span data-stu-id="cdb1a-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="cdb1a-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="cdb1a-116">JSON Representation</span></span>
<span data-ttu-id="cdb1a-117">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cdb1a-117">Here is a JSON representation of the resource.</span></span>
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




---
title: Тип ресурса Манажеддевицеклеанупсеттингс
description: Определите правило, когда администратор хочет очистить устройства.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5070de01324b25332d42b63a4d1d787989b86c4f
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33941963"
---
# <a name="manageddevicecleanupsettings-resource-type"></a><span data-ttu-id="748d9-103">Тип ресурса Манажеддевицеклеанупсеттингс</span><span class="sxs-lookup"><span data-stu-id="748d9-103">managedDeviceCleanupSettings resource type</span></span>

> <span data-ttu-id="748d9-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="748d9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="748d9-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="748d9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="748d9-106">Определите правило, когда администратор хочет очистить устройства.</span><span class="sxs-lookup"><span data-stu-id="748d9-106">Define the rule when the admin wants the devices to be cleaned up.</span></span>

## <a name="properties"></a><span data-ttu-id="748d9-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="748d9-107">Properties</span></span>
|<span data-ttu-id="748d9-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="748d9-108">Property</span></span>|<span data-ttu-id="748d9-109">Тип</span><span class="sxs-lookup"><span data-stu-id="748d9-109">Type</span></span>|<span data-ttu-id="748d9-110">Описание</span><span class="sxs-lookup"><span data-stu-id="748d9-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="748d9-111">Девицеинактивитибефореретирементиндайс</span><span class="sxs-lookup"><span data-stu-id="748d9-111">deviceInactivityBeforeRetirementInDays</span></span>|<span data-ttu-id="748d9-112">Строка</span><span class="sxs-lookup"><span data-stu-id="748d9-112">String</span></span>|<span data-ttu-id="748d9-113">Количество дней, когда устройство не связывалось с Intune.</span><span class="sxs-lookup"><span data-stu-id="748d9-113">Number of days when the device has not contacted Intune.</span></span>|

## <a name="relationships"></a><span data-ttu-id="748d9-114">Связи</span><span class="sxs-lookup"><span data-stu-id="748d9-114">Relationships</span></span>
<span data-ttu-id="748d9-115">Нет</span><span class="sxs-lookup"><span data-stu-id="748d9-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="748d9-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="748d9-116">JSON Representation</span></span>
<span data-ttu-id="748d9-117">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="748d9-117">Here is a JSON representation of the resource.</span></span>
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





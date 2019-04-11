---
title: Тип ресурса Манажеддевицеклеанупсеттингс
description: Определите правило, когда администратор хочет очистить устройства.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0d7e91d632860e47275cda158acf4d816c64e835
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31804559"
---
# <a name="manageddevicecleanupsettings-resource-type"></a><span data-ttu-id="8aed2-103">Тип ресурса Манажеддевицеклеанупсеттингс</span><span class="sxs-lookup"><span data-stu-id="8aed2-103">managedDeviceCleanupSettings resource type</span></span>

> <span data-ttu-id="8aed2-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8aed2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8aed2-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8aed2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8aed2-106">Определите правило, когда администратор хочет очистить устройства.</span><span class="sxs-lookup"><span data-stu-id="8aed2-106">Define the rule when the admin wants the devices to be cleaned up.</span></span>

## <a name="properties"></a><span data-ttu-id="8aed2-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="8aed2-107">Properties</span></span>
|<span data-ttu-id="8aed2-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="8aed2-108">Property</span></span>|<span data-ttu-id="8aed2-109">Тип</span><span class="sxs-lookup"><span data-stu-id="8aed2-109">Type</span></span>|<span data-ttu-id="8aed2-110">Описание</span><span class="sxs-lookup"><span data-stu-id="8aed2-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8aed2-111">Девицеинактивитибефореретирементиндайс</span><span class="sxs-lookup"><span data-stu-id="8aed2-111">deviceInactivityBeforeRetirementInDays</span></span>|<span data-ttu-id="8aed2-112">String</span><span class="sxs-lookup"><span data-stu-id="8aed2-112">String</span></span>|<span data-ttu-id="8aed2-113">Количество дней, когда устройство не связывалось с Intune.</span><span class="sxs-lookup"><span data-stu-id="8aed2-113">Number of days when the device has not contacted Intune.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8aed2-114">Отношения</span><span class="sxs-lookup"><span data-stu-id="8aed2-114">Relationships</span></span>
<span data-ttu-id="8aed2-115">Нет</span><span class="sxs-lookup"><span data-stu-id="8aed2-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8aed2-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8aed2-116">JSON Representation</span></span>
<span data-ttu-id="8aed2-117">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8aed2-117">Here is a JSON representation of the resource.</span></span>
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






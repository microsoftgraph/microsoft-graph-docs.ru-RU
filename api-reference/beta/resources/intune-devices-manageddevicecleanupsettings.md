---
title: Тип ресурса Манажеддевицеклеанупсеттингс
description: Определите правило, когда администратор хочет очистить устройства.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0d7e91d632860e47275cda158acf4d816c64e835
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32522120"
---
# <a name="manageddevicecleanupsettings-resource-type"></a><span data-ttu-id="2896c-103">Тип ресурса Манажеддевицеклеанупсеттингс</span><span class="sxs-lookup"><span data-stu-id="2896c-103">managedDeviceCleanupSettings resource type</span></span>

> <span data-ttu-id="2896c-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2896c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2896c-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2896c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2896c-106">Определите правило, когда администратор хочет очистить устройства.</span><span class="sxs-lookup"><span data-stu-id="2896c-106">Define the rule when the admin wants the devices to be cleaned up.</span></span>

## <a name="properties"></a><span data-ttu-id="2896c-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="2896c-107">Properties</span></span>
|<span data-ttu-id="2896c-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="2896c-108">Property</span></span>|<span data-ttu-id="2896c-109">Тип</span><span class="sxs-lookup"><span data-stu-id="2896c-109">Type</span></span>|<span data-ttu-id="2896c-110">Описание</span><span class="sxs-lookup"><span data-stu-id="2896c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2896c-111">Девицеинактивитибефореретирементиндайс</span><span class="sxs-lookup"><span data-stu-id="2896c-111">deviceInactivityBeforeRetirementInDays</span></span>|<span data-ttu-id="2896c-112">String</span><span class="sxs-lookup"><span data-stu-id="2896c-112">String</span></span>|<span data-ttu-id="2896c-113">Количество дней, когда устройство не связывалось с Intune.</span><span class="sxs-lookup"><span data-stu-id="2896c-113">Number of days when the device has not contacted Intune.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2896c-114">Отношения</span><span class="sxs-lookup"><span data-stu-id="2896c-114">Relationships</span></span>
<span data-ttu-id="2896c-115">Нет</span><span class="sxs-lookup"><span data-stu-id="2896c-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2896c-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2896c-116">JSON Representation</span></span>
<span data-ttu-id="2896c-117">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2896c-117">Here is a JSON representation of the resource.</span></span>
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






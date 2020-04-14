---
title: Тип ресурса Манажеддевицеклеанупсеттингс
description: Определите правило, когда администратор хочет очистить устройства.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: e37b45c61bdc96b47b0b8ca29dd5bc44689addc9
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43443963"
---
# <a name="manageddevicecleanupsettings-resource-type"></a><span data-ttu-id="59c38-103">Тип ресурса Манажеддевицеклеанупсеттингс</span><span class="sxs-lookup"><span data-stu-id="59c38-103">managedDeviceCleanupSettings resource type</span></span>

<span data-ttu-id="59c38-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="59c38-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="59c38-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="59c38-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="59c38-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="59c38-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="59c38-107">Определите правило, когда администратор хочет очистить устройства.</span><span class="sxs-lookup"><span data-stu-id="59c38-107">Define the rule when the admin wants the devices to be cleaned up.</span></span>

## <a name="properties"></a><span data-ttu-id="59c38-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="59c38-108">Properties</span></span>
|<span data-ttu-id="59c38-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="59c38-109">Property</span></span>|<span data-ttu-id="59c38-110">Тип</span><span class="sxs-lookup"><span data-stu-id="59c38-110">Type</span></span>|<span data-ttu-id="59c38-111">Описание</span><span class="sxs-lookup"><span data-stu-id="59c38-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="59c38-112">девицеинактивитибефореретирементиндайс</span><span class="sxs-lookup"><span data-stu-id="59c38-112">deviceInactivityBeforeRetirementInDays</span></span>|<span data-ttu-id="59c38-113">String</span><span class="sxs-lookup"><span data-stu-id="59c38-113">String</span></span>|<span data-ttu-id="59c38-114">Количество дней, когда устройство не связывалось с Intune.</span><span class="sxs-lookup"><span data-stu-id="59c38-114">Number of days when the device has not contacted Intune.</span></span>|

## <a name="relationships"></a><span data-ttu-id="59c38-115">Связи</span><span class="sxs-lookup"><span data-stu-id="59c38-115">Relationships</span></span>
<span data-ttu-id="59c38-116">Нет</span><span class="sxs-lookup"><span data-stu-id="59c38-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="59c38-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="59c38-117">JSON Representation</span></span>
<span data-ttu-id="59c38-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="59c38-118">Here is a JSON representation of the resource.</span></span>
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




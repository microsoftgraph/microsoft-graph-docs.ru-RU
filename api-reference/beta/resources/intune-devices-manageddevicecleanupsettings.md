---
title: Тип ресурса Манажеддевицеклеанупсеттингс
description: Определите правило, когда администратор хочет очистить устройства.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 67e911cb5e1b31e3be2cc20378ebe77ff305204a
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48725486"
---
# <a name="manageddevicecleanupsettings-resource-type"></a><span data-ttu-id="3222c-103">Тип ресурса Манажеддевицеклеанупсеттингс</span><span class="sxs-lookup"><span data-stu-id="3222c-103">managedDeviceCleanupSettings resource type</span></span>

<span data-ttu-id="3222c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3222c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3222c-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3222c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3222c-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3222c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3222c-107">Определите правило, когда администратор хочет очистить устройства.</span><span class="sxs-lookup"><span data-stu-id="3222c-107">Define the rule when the admin wants the devices to be cleaned up.</span></span>

## <a name="properties"></a><span data-ttu-id="3222c-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="3222c-108">Properties</span></span>
|<span data-ttu-id="3222c-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="3222c-109">Property</span></span>|<span data-ttu-id="3222c-110">Тип</span><span class="sxs-lookup"><span data-stu-id="3222c-110">Type</span></span>|<span data-ttu-id="3222c-111">Описание</span><span class="sxs-lookup"><span data-stu-id="3222c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3222c-112">девицеинактивитибефореретирементиндайс</span><span class="sxs-lookup"><span data-stu-id="3222c-112">deviceInactivityBeforeRetirementInDays</span></span>|<span data-ttu-id="3222c-113">Строка</span><span class="sxs-lookup"><span data-stu-id="3222c-113">String</span></span>|<span data-ttu-id="3222c-114">Количество дней, когда устройство не связывалось с Intune.</span><span class="sxs-lookup"><span data-stu-id="3222c-114">Number of days when the device has not contacted Intune.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3222c-115">Связи</span><span class="sxs-lookup"><span data-stu-id="3222c-115">Relationships</span></span>
<span data-ttu-id="3222c-116">Нет</span><span class="sxs-lookup"><span data-stu-id="3222c-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3222c-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3222c-117">JSON Representation</span></span>
<span data-ttu-id="3222c-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3222c-118">Here is a JSON representation of the resource.</span></span>
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






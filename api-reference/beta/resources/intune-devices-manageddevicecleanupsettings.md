---
title: Тип ресурса Манажеддевицеклеанупсеттингс
description: Определите правило, когда администратор хочет очистить устройства.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 8091c873c18c1af0344cae9f6800e26e85181c19
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48081225"
---
# <a name="manageddevicecleanupsettings-resource-type"></a><span data-ttu-id="7ed12-103">Тип ресурса Манажеддевицеклеанупсеттингс</span><span class="sxs-lookup"><span data-stu-id="7ed12-103">managedDeviceCleanupSettings resource type</span></span>

<span data-ttu-id="7ed12-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7ed12-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7ed12-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7ed12-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7ed12-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7ed12-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7ed12-107">Определите правило, когда администратор хочет очистить устройства.</span><span class="sxs-lookup"><span data-stu-id="7ed12-107">Define the rule when the admin wants the devices to be cleaned up.</span></span>

## <a name="properties"></a><span data-ttu-id="7ed12-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="7ed12-108">Properties</span></span>
|<span data-ttu-id="7ed12-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="7ed12-109">Property</span></span>|<span data-ttu-id="7ed12-110">Тип</span><span class="sxs-lookup"><span data-stu-id="7ed12-110">Type</span></span>|<span data-ttu-id="7ed12-111">Описание</span><span class="sxs-lookup"><span data-stu-id="7ed12-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7ed12-112">девицеинактивитибефореретирементиндайс</span><span class="sxs-lookup"><span data-stu-id="7ed12-112">deviceInactivityBeforeRetirementInDays</span></span>|<span data-ttu-id="7ed12-113">Строка</span><span class="sxs-lookup"><span data-stu-id="7ed12-113">String</span></span>|<span data-ttu-id="7ed12-114">Количество дней, когда устройство не связывалось с Intune.</span><span class="sxs-lookup"><span data-stu-id="7ed12-114">Number of days when the device has not contacted Intune.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7ed12-115">Связи</span><span class="sxs-lookup"><span data-stu-id="7ed12-115">Relationships</span></span>
<span data-ttu-id="7ed12-116">Нет</span><span class="sxs-lookup"><span data-stu-id="7ed12-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7ed12-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7ed12-117">JSON Representation</span></span>
<span data-ttu-id="7ed12-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7ed12-118">Here is a JSON representation of the resource.</span></span>
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







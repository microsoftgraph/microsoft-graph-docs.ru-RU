---
title: Тип ресурса Девицехеалсскриптремедиатионсуммари
description: Количество развернутых сценариев работоспособности устройств и количество устройств, которые были исправлены в сценариях.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b59f2d057f258e60a8182194c1ac930e95012b93
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42784946"
---
# <a name="devicehealthscriptremediationsummary-resource-type"></a><span data-ttu-id="9a4b9-103">Тип ресурса Девицехеалсскриптремедиатионсуммари</span><span class="sxs-lookup"><span data-stu-id="9a4b9-103">deviceHealthScriptRemediationSummary resource type</span></span>

> <span data-ttu-id="9a4b9-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9a4b9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9a4b9-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9a4b9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9a4b9-106">Количество развернутых сценариев работоспособности устройств и количество устройств, которые были исправлены в сценариях.</span><span class="sxs-lookup"><span data-stu-id="9a4b9-106">The number of device health scripts deployed and the number of devices the scripts remediated.</span></span>

## <a name="properties"></a><span data-ttu-id="9a4b9-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="9a4b9-107">Properties</span></span>
|<span data-ttu-id="9a4b9-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="9a4b9-108">Property</span></span>|<span data-ttu-id="9a4b9-109">Тип</span><span class="sxs-lookup"><span data-stu-id="9a4b9-109">Type</span></span>|<span data-ttu-id="9a4b9-110">Описание</span><span class="sxs-lookup"><span data-stu-id="9a4b9-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9a4b9-111">скрипткаунт</span><span class="sxs-lookup"><span data-stu-id="9a4b9-111">scriptCount</span></span>|<span data-ttu-id="9a4b9-112">Int32</span><span class="sxs-lookup"><span data-stu-id="9a4b9-112">Int32</span></span>|<span data-ttu-id="9a4b9-113">Количество развернутых сценариев работоспособности устройств.</span><span class="sxs-lookup"><span data-stu-id="9a4b9-113">The number of device health scripts deployed.</span></span>|
|<span data-ttu-id="9a4b9-114">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="9a4b9-114">remediatedDeviceCount</span></span>|<span data-ttu-id="9a4b9-115">Int32</span><span class="sxs-lookup"><span data-stu-id="9a4b9-115">Int32</span></span>|<span data-ttu-id="9a4b9-116">Количество устройств, исправленных сценариями работоспособности устройства.</span><span class="sxs-lookup"><span data-stu-id="9a4b9-116">The number of devices remediated by device health scripts.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9a4b9-117">Связи</span><span class="sxs-lookup"><span data-stu-id="9a4b9-117">Relationships</span></span>
<span data-ttu-id="9a4b9-118">Нет</span><span class="sxs-lookup"><span data-stu-id="9a4b9-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9a4b9-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9a4b9-119">JSON Representation</span></span>
<span data-ttu-id="9a4b9-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9a4b9-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceHealthScriptRemediationSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceHealthScriptRemediationSummary",
  "scriptCount": 1024,
  "remediatedDeviceCount": 1024
}
```




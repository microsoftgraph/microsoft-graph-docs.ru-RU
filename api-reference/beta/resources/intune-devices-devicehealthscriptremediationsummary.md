---
title: Тип ресурса Девицехеалсскриптремедиатионсуммари
description: Количество развернутых сценариев работоспособности устройств и количество устройств, которые были исправлены в сценариях.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: e538ba04a9dc5007331b8dde3f4d6ec854938e91
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48690625"
---
# <a name="devicehealthscriptremediationsummary-resource-type"></a><span data-ttu-id="86101-103">Тип ресурса Девицехеалсскриптремедиатионсуммари</span><span class="sxs-lookup"><span data-stu-id="86101-103">deviceHealthScriptRemediationSummary resource type</span></span>

<span data-ttu-id="86101-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="86101-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="86101-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="86101-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="86101-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="86101-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="86101-107">Количество развернутых сценариев работоспособности устройств и количество устройств, которые были исправлены в сценариях.</span><span class="sxs-lookup"><span data-stu-id="86101-107">The number of device health scripts deployed and the number of devices the scripts remediated.</span></span>

## <a name="properties"></a><span data-ttu-id="86101-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="86101-108">Properties</span></span>
|<span data-ttu-id="86101-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="86101-109">Property</span></span>|<span data-ttu-id="86101-110">Тип</span><span class="sxs-lookup"><span data-stu-id="86101-110">Type</span></span>|<span data-ttu-id="86101-111">Описание</span><span class="sxs-lookup"><span data-stu-id="86101-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="86101-112">скрипткаунт</span><span class="sxs-lookup"><span data-stu-id="86101-112">scriptCount</span></span>|<span data-ttu-id="86101-113">Int32</span><span class="sxs-lookup"><span data-stu-id="86101-113">Int32</span></span>|<span data-ttu-id="86101-114">Количество развернутых сценариев работоспособности устройств.</span><span class="sxs-lookup"><span data-stu-id="86101-114">The number of device health scripts deployed.</span></span>|
|<span data-ttu-id="86101-115">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="86101-115">remediatedDeviceCount</span></span>|<span data-ttu-id="86101-116">Int32</span><span class="sxs-lookup"><span data-stu-id="86101-116">Int32</span></span>|<span data-ttu-id="86101-117">Количество устройств, исправленных сценариями работоспособности устройства.</span><span class="sxs-lookup"><span data-stu-id="86101-117">The number of devices remediated by device health scripts.</span></span>|

## <a name="relationships"></a><span data-ttu-id="86101-118">Связи</span><span class="sxs-lookup"><span data-stu-id="86101-118">Relationships</span></span>
<span data-ttu-id="86101-119">Нет</span><span class="sxs-lookup"><span data-stu-id="86101-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="86101-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="86101-120">JSON Representation</span></span>
<span data-ttu-id="86101-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="86101-121">Here is a JSON representation of the resource.</span></span>
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






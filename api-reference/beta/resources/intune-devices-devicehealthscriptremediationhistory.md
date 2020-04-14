---
title: Тип ресурса Девицехеалсскриптремедиатионхистори
description: Количество устройств, исправленных сценарием работоспособности устройства на указанную дату в последний момент времени изменения.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 72df8bdf3ab5dca917d6eee1ff60fc24327245e2
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43388518"
---
# <a name="devicehealthscriptremediationhistory-resource-type"></a><span data-ttu-id="1dfed-103">Тип ресурса Девицехеалсскриптремедиатионхистори</span><span class="sxs-lookup"><span data-stu-id="1dfed-103">deviceHealthScriptRemediationHistory resource type</span></span>

<span data-ttu-id="1dfed-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1dfed-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1dfed-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1dfed-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1dfed-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1dfed-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1dfed-107">Количество устройств, исправленных сценарием работоспособности устройства на указанную дату в последний момент времени изменения.</span><span class="sxs-lookup"><span data-stu-id="1dfed-107">The number of devices remediated by a device health script on a given date with the last modified time.</span></span>

## <a name="properties"></a><span data-ttu-id="1dfed-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="1dfed-108">Properties</span></span>
|<span data-ttu-id="1dfed-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="1dfed-109">Property</span></span>|<span data-ttu-id="1dfed-110">Тип</span><span class="sxs-lookup"><span data-stu-id="1dfed-110">Type</span></span>|<span data-ttu-id="1dfed-111">Описание</span><span class="sxs-lookup"><span data-stu-id="1dfed-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1dfed-112">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1dfed-112">lastModifiedDateTime</span></span>|<span data-ttu-id="1dfed-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1dfed-113">DateTimeOffset</span></span>|<span data-ttu-id="1dfed-114">Дата, на которую рассчитывается журнал результатов для хеалсскрипт.</span><span class="sxs-lookup"><span data-stu-id="1dfed-114">The date on which the results history is calculated for the healthscript.</span></span>|
|<span data-ttu-id="1dfed-115">хисторидата</span><span class="sxs-lookup"><span data-stu-id="1dfed-115">historyData</span></span>|<span data-ttu-id="1dfed-116">Коллекция [девицехеалсскриптремедиатионхисторидата](../resources/intune-devices-devicehealthscriptremediationhistorydata.md)</span><span class="sxs-lookup"><span data-stu-id="1dfed-116">[deviceHealthScriptRemediationHistoryData](../resources/intune-devices-devicehealthscriptremediationhistorydata.md) collection</span></span>|<span data-ttu-id="1dfed-117">Количество устройств, исправленных сценарием работоспособности устройства на указанную дату.</span><span class="sxs-lookup"><span data-stu-id="1dfed-117">The number of devices remediated by the device health script on the given date.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1dfed-118">Связи</span><span class="sxs-lookup"><span data-stu-id="1dfed-118">Relationships</span></span>
<span data-ttu-id="1dfed-119">Нет</span><span class="sxs-lookup"><span data-stu-id="1dfed-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1dfed-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1dfed-120">JSON Representation</span></span>
<span data-ttu-id="1dfed-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1dfed-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceHealthScriptRemediationHistory"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceHealthScriptRemediationHistory",
  "lastModifiedDateTime": "String (timestamp)",
  "historyData": [
    {
      "@odata.type": "microsoft.graph.deviceHealthScriptRemediationHistoryData",
      "date": "<Unknown Primitive Type Edm.Date>",
      "remediatedDeviceCount": 1024,
      "noIssueDeviceCount": 1024
    }
  ]
}
```




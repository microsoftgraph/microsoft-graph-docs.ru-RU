---
title: Тип ресурса Девицехеалсскриптремедиатионхистори
description: Количество устройств, исправленных сценарием работоспособности устройства на указанную дату в последний момент времени изменения.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 1ca94403decdc183748c8b147fae678e88aac264
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48697702"
---
# <a name="devicehealthscriptremediationhistory-resource-type"></a><span data-ttu-id="cae07-103">Тип ресурса Девицехеалсскриптремедиатионхистори</span><span class="sxs-lookup"><span data-stu-id="cae07-103">deviceHealthScriptRemediationHistory resource type</span></span>

<span data-ttu-id="cae07-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cae07-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cae07-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cae07-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cae07-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="cae07-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cae07-107">Количество устройств, исправленных сценарием работоспособности устройства на указанную дату в последний момент времени изменения.</span><span class="sxs-lookup"><span data-stu-id="cae07-107">The number of devices remediated by a device health script on a given date with the last modified time.</span></span>

## <a name="properties"></a><span data-ttu-id="cae07-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="cae07-108">Properties</span></span>
|<span data-ttu-id="cae07-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="cae07-109">Property</span></span>|<span data-ttu-id="cae07-110">Тип</span><span class="sxs-lookup"><span data-stu-id="cae07-110">Type</span></span>|<span data-ttu-id="cae07-111">Описание</span><span class="sxs-lookup"><span data-stu-id="cae07-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cae07-112">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="cae07-112">lastModifiedDateTime</span></span>|<span data-ttu-id="cae07-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cae07-113">DateTimeOffset</span></span>|<span data-ttu-id="cae07-114">Дата, на которую рассчитывается журнал результатов для хеалсскрипт.</span><span class="sxs-lookup"><span data-stu-id="cae07-114">The date on which the results history is calculated for the healthscript.</span></span>|
|<span data-ttu-id="cae07-115">хисторидата</span><span class="sxs-lookup"><span data-stu-id="cae07-115">historyData</span></span>|<span data-ttu-id="cae07-116">Коллекция [девицехеалсскриптремедиатионхисторидата](../resources/intune-devices-devicehealthscriptremediationhistorydata.md)</span><span class="sxs-lookup"><span data-stu-id="cae07-116">[deviceHealthScriptRemediationHistoryData](../resources/intune-devices-devicehealthscriptremediationhistorydata.md) collection</span></span>|<span data-ttu-id="cae07-117">Количество устройств, исправленных сценарием работоспособности устройства на указанную дату.</span><span class="sxs-lookup"><span data-stu-id="cae07-117">The number of devices remediated by the device health script on the given date.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cae07-118">Связи</span><span class="sxs-lookup"><span data-stu-id="cae07-118">Relationships</span></span>
<span data-ttu-id="cae07-119">Нет</span><span class="sxs-lookup"><span data-stu-id="cae07-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="cae07-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="cae07-120">JSON Representation</span></span>
<span data-ttu-id="cae07-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cae07-121">Here is a JSON representation of the resource.</span></span>
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
      "date": "String (Date)",
      "remediatedDeviceCount": 1024,
      "noIssueDeviceCount": 1024
    }
  ]
}
```






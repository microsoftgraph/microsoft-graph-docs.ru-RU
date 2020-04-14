---
title: Тип ресурса Девицехеалсскриптремедиатионхисторидата
description: Количество устройств, исправленных сценарием работоспособности устройства на заданную дату.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 396c52cbf797b0e0028e9f7ed71ca1e9fe05d34c
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43388504"
---
# <a name="devicehealthscriptremediationhistorydata-resource-type"></a><span data-ttu-id="9bee5-103">Тип ресурса Девицехеалсскриптремедиатионхисторидата</span><span class="sxs-lookup"><span data-stu-id="9bee5-103">deviceHealthScriptRemediationHistoryData resource type</span></span>

<span data-ttu-id="9bee5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9bee5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9bee5-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9bee5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9bee5-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9bee5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9bee5-107">Количество устройств, исправленных сценарием работоспособности устройства на заданную дату.</span><span class="sxs-lookup"><span data-stu-id="9bee5-107">The number of devices remediated by a device health script on a given date.</span></span>

## <a name="properties"></a><span data-ttu-id="9bee5-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="9bee5-108">Properties</span></span>
|<span data-ttu-id="9bee5-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="9bee5-109">Property</span></span>|<span data-ttu-id="9bee5-110">Тип</span><span class="sxs-lookup"><span data-stu-id="9bee5-110">Type</span></span>|<span data-ttu-id="9bee5-111">Описание</span><span class="sxs-lookup"><span data-stu-id="9bee5-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9bee5-112">date</span><span class="sxs-lookup"><span data-stu-id="9bee5-112">date</span></span>|<span data-ttu-id="9bee5-113">Date</span><span class="sxs-lookup"><span data-stu-id="9bee5-113">Date</span></span>|<span data-ttu-id="9bee5-114">Дата исправления устройств с помощью сценария работоспособности устройства.</span><span class="sxs-lookup"><span data-stu-id="9bee5-114">The date on which devices were remediated by the device health script.</span></span>|
|<span data-ttu-id="9bee5-115">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="9bee5-115">remediatedDeviceCount</span></span>|<span data-ttu-id="9bee5-116">Int32</span><span class="sxs-lookup"><span data-stu-id="9bee5-116">Int32</span></span>|<span data-ttu-id="9bee5-117">Количество устройств, исправленных сценарием работоспособности устройства.</span><span class="sxs-lookup"><span data-stu-id="9bee5-117">The number of devices remediated by the device health script.</span></span>|
|<span data-ttu-id="9bee5-118">ноиссуедевицекаунт</span><span class="sxs-lookup"><span data-stu-id="9bee5-118">noIssueDeviceCount</span></span>|<span data-ttu-id="9bee5-119">Int32</span><span class="sxs-lookup"><span data-stu-id="9bee5-119">Int32</span></span>|<span data-ttu-id="9bee5-120">Количество устройств, для которых было обнаружено отсутствие ошибок в сценарии работоспособности устройства.</span><span class="sxs-lookup"><span data-stu-id="9bee5-120">The number of devices that were found to have no issue by the device health script.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9bee5-121">Связи</span><span class="sxs-lookup"><span data-stu-id="9bee5-121">Relationships</span></span>
<span data-ttu-id="9bee5-122">Нет</span><span class="sxs-lookup"><span data-stu-id="9bee5-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9bee5-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9bee5-123">JSON Representation</span></span>
<span data-ttu-id="9bee5-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9bee5-124">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceHealthScriptRemediationHistoryData"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceHealthScriptRemediationHistoryData",
  "date": "<Unknown Primitive Type Edm.Date>",
  "remediatedDeviceCount": 1024,
  "noIssueDeviceCount": 1024
}
```




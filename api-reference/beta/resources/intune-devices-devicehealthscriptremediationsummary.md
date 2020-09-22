---
title: Тип ресурса Девицехеалсскриптремедиатионсуммари
description: Количество развернутых сценариев работоспособности устройств и количество устройств, которые были исправлены в сценариях.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 06e48973305dbbdf7ae276e4d14d3307da74c36e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48060294"
---
# <a name="devicehealthscriptremediationsummary-resource-type"></a><span data-ttu-id="07de8-103">Тип ресурса Девицехеалсскриптремедиатионсуммари</span><span class="sxs-lookup"><span data-stu-id="07de8-103">deviceHealthScriptRemediationSummary resource type</span></span>

<span data-ttu-id="07de8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="07de8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="07de8-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="07de8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="07de8-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="07de8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="07de8-107">Количество развернутых сценариев работоспособности устройств и количество устройств, которые были исправлены в сценариях.</span><span class="sxs-lookup"><span data-stu-id="07de8-107">The number of device health scripts deployed and the number of devices the scripts remediated.</span></span>

## <a name="properties"></a><span data-ttu-id="07de8-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="07de8-108">Properties</span></span>
|<span data-ttu-id="07de8-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="07de8-109">Property</span></span>|<span data-ttu-id="07de8-110">Тип</span><span class="sxs-lookup"><span data-stu-id="07de8-110">Type</span></span>|<span data-ttu-id="07de8-111">Описание</span><span class="sxs-lookup"><span data-stu-id="07de8-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="07de8-112">скрипткаунт</span><span class="sxs-lookup"><span data-stu-id="07de8-112">scriptCount</span></span>|<span data-ttu-id="07de8-113">Int32</span><span class="sxs-lookup"><span data-stu-id="07de8-113">Int32</span></span>|<span data-ttu-id="07de8-114">Количество развернутых сценариев работоспособности устройств.</span><span class="sxs-lookup"><span data-stu-id="07de8-114">The number of device health scripts deployed.</span></span>|
|<span data-ttu-id="07de8-115">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="07de8-115">remediatedDeviceCount</span></span>|<span data-ttu-id="07de8-116">Int32</span><span class="sxs-lookup"><span data-stu-id="07de8-116">Int32</span></span>|<span data-ttu-id="07de8-117">Количество устройств, исправленных сценариями работоспособности устройства.</span><span class="sxs-lookup"><span data-stu-id="07de8-117">The number of devices remediated by device health scripts.</span></span>|

## <a name="relationships"></a><span data-ttu-id="07de8-118">Связи</span><span class="sxs-lookup"><span data-stu-id="07de8-118">Relationships</span></span>
<span data-ttu-id="07de8-119">Нет</span><span class="sxs-lookup"><span data-stu-id="07de8-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="07de8-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="07de8-120">JSON Representation</span></span>
<span data-ttu-id="07de8-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="07de8-121">Here is a JSON representation of the resource.</span></span>
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







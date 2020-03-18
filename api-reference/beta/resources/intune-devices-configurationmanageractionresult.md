---
title: Тип ресурса Конфигуратионманажерактионресулт
description: Результат действия Конфигуратионманажер
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: de187585e7e8dd74f4495d7143030e30acf46c4a
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42785086"
---
# <a name="configurationmanageractionresult-resource-type"></a><span data-ttu-id="7256d-103">Тип ресурса Конфигуратионманажерактионресулт</span><span class="sxs-lookup"><span data-stu-id="7256d-103">configurationManagerActionResult resource type</span></span>

> <span data-ttu-id="7256d-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7256d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7256d-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7256d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7256d-106">Результат действия Конфигуратионманажер</span><span class="sxs-lookup"><span data-stu-id="7256d-106">Result of the ConfigurationManager action</span></span>


<span data-ttu-id="7256d-107">Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="7256d-107">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="7256d-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="7256d-108">Properties</span></span>
|<span data-ttu-id="7256d-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="7256d-109">Property</span></span>|<span data-ttu-id="7256d-110">Тип</span><span class="sxs-lookup"><span data-stu-id="7256d-110">Type</span></span>|<span data-ttu-id="7256d-111">Описание</span><span class="sxs-lookup"><span data-stu-id="7256d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7256d-112">actionName</span><span class="sxs-lookup"><span data-stu-id="7256d-112">actionName</span></span>|<span data-ttu-id="7256d-113">String</span><span class="sxs-lookup"><span data-stu-id="7256d-113">String</span></span>|<span data-ttu-id="7256d-114">Название действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="7256d-114">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="7256d-115">actionState</span><span class="sxs-lookup"><span data-stu-id="7256d-115">actionState</span></span>|[<span data-ttu-id="7256d-116">actionState</span><span class="sxs-lookup"><span data-stu-id="7256d-116">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="7256d-117">Состояние действия, унаследованного от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="7256d-117">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="7256d-118">Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="7256d-118">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="7256d-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="7256d-119">startDateTime</span></span>|<span data-ttu-id="7256d-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7256d-120">DateTimeOffset</span></span>|<span data-ttu-id="7256d-121">Время начала действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="7256d-121">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="7256d-122">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="7256d-122">lastUpdatedDateTime</span></span>|<span data-ttu-id="7256d-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7256d-123">DateTimeOffset</span></span>|<span data-ttu-id="7256d-124">Время последнего обновления действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="7256d-124">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="7256d-125">актионделиверистатус</span><span class="sxs-lookup"><span data-stu-id="7256d-125">actionDeliveryStatus</span></span>|[<span data-ttu-id="7256d-126">конфигуратионманажерактионделиверистатус</span><span class="sxs-lookup"><span data-stu-id="7256d-126">configurationManagerActionDeliveryStatus</span></span>](../resources/intune-devices-configurationmanageractiondeliverystatus.md)|<span data-ttu-id="7256d-127">Состояние действия, которое доставляется на локальный сервер.</span><span class="sxs-lookup"><span data-stu-id="7256d-127">State of the action being delivered to on-prem server.</span></span> <span data-ttu-id="7256d-128">Возможные значения: `unknown`, `pendingDelivery`, `deliveredToConnectorService`, `failedToDeliverToConnectorService`, `deliveredToOnPremisesServer`.</span><span class="sxs-lookup"><span data-stu-id="7256d-128">Possible values are: `unknown`, `pendingDelivery`, `deliveredToConnectorService`, `failedToDeliverToConnectorService`, `deliveredToOnPremisesServer`.</span></span>|
|<span data-ttu-id="7256d-129">errorCode</span><span class="sxs-lookup"><span data-stu-id="7256d-129">errorCode</span></span>|<span data-ttu-id="7256d-130">Int32</span><span class="sxs-lookup"><span data-stu-id="7256d-130">Int32</span></span>|<span data-ttu-id="7256d-131">Код ошибки действия Configuration Manager от клиента</span><span class="sxs-lookup"><span data-stu-id="7256d-131">Error code of Configuration Manager action from client</span></span>|

## <a name="relationships"></a><span data-ttu-id="7256d-132">Связи</span><span class="sxs-lookup"><span data-stu-id="7256d-132">Relationships</span></span>
<span data-ttu-id="7256d-133">Нет</span><span class="sxs-lookup"><span data-stu-id="7256d-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7256d-134">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7256d-134">JSON Representation</span></span>
<span data-ttu-id="7256d-135">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7256d-135">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.configurationManagerActionResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.configurationManagerActionResult",
  "actionName": "String",
  "actionState": "String",
  "startDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)",
  "actionDeliveryStatus": "String",
  "errorCode": 1024
}
```




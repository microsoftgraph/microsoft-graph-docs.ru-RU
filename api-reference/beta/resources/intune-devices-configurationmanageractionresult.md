---
title: Тип ресурса Конфигуратионманажерактионресулт
description: Результат действия Конфигуратионманажер
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 8512f383396b235d80fa16b7bc122e42b89c041a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48060680"
---
# <a name="configurationmanageractionresult-resource-type"></a><span data-ttu-id="5e48b-103">Тип ресурса Конфигуратионманажерактионресулт</span><span class="sxs-lookup"><span data-stu-id="5e48b-103">configurationManagerActionResult resource type</span></span>

<span data-ttu-id="5e48b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5e48b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5e48b-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5e48b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5e48b-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5e48b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5e48b-107">Результат действия Конфигуратионманажер</span><span class="sxs-lookup"><span data-stu-id="5e48b-107">Result of the ConfigurationManager action</span></span>


<span data-ttu-id="5e48b-108">Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="5e48b-108">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="5e48b-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="5e48b-109">Properties</span></span>
|<span data-ttu-id="5e48b-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="5e48b-110">Property</span></span>|<span data-ttu-id="5e48b-111">Тип</span><span class="sxs-lookup"><span data-stu-id="5e48b-111">Type</span></span>|<span data-ttu-id="5e48b-112">Описание</span><span class="sxs-lookup"><span data-stu-id="5e48b-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5e48b-113">actionName</span><span class="sxs-lookup"><span data-stu-id="5e48b-113">actionName</span></span>|<span data-ttu-id="5e48b-114">String</span><span class="sxs-lookup"><span data-stu-id="5e48b-114">String</span></span>|<span data-ttu-id="5e48b-115">Название действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="5e48b-115">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="5e48b-116">actionState</span><span class="sxs-lookup"><span data-stu-id="5e48b-116">actionState</span></span>|[<span data-ttu-id="5e48b-117">actionState</span><span class="sxs-lookup"><span data-stu-id="5e48b-117">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="5e48b-118">Состояние действия, унаследованного от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="5e48b-118">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="5e48b-119">Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="5e48b-119">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="5e48b-120">startDateTime</span><span class="sxs-lookup"><span data-stu-id="5e48b-120">startDateTime</span></span>|<span data-ttu-id="5e48b-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5e48b-121">DateTimeOffset</span></span>|<span data-ttu-id="5e48b-122">Время начала действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="5e48b-122">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="5e48b-123">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="5e48b-123">lastUpdatedDateTime</span></span>|<span data-ttu-id="5e48b-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5e48b-124">DateTimeOffset</span></span>|<span data-ttu-id="5e48b-125">Время последнего обновления действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="5e48b-125">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="5e48b-126">актионделиверистатус</span><span class="sxs-lookup"><span data-stu-id="5e48b-126">actionDeliveryStatus</span></span>|[<span data-ttu-id="5e48b-127">configurationManagerActionDeliveryStatus</span><span class="sxs-lookup"><span data-stu-id="5e48b-127">configurationManagerActionDeliveryStatus</span></span>](../resources/intune-devices-configurationmanageractiondeliverystatus.md)|<span data-ttu-id="5e48b-128">Состояние действия, которое доставляется на локальный сервер.</span><span class="sxs-lookup"><span data-stu-id="5e48b-128">State of the action being delivered to on-prem server.</span></span> <span data-ttu-id="5e48b-129">Возможные значения: `unknown`, `pendingDelivery`, `deliveredToConnectorService`, `failedToDeliverToConnectorService`, `deliveredToOnPremisesServer`.</span><span class="sxs-lookup"><span data-stu-id="5e48b-129">Possible values are: `unknown`, `pendingDelivery`, `deliveredToConnectorService`, `failedToDeliverToConnectorService`, `deliveredToOnPremisesServer`.</span></span>|
|<span data-ttu-id="5e48b-130">errorCode</span><span class="sxs-lookup"><span data-stu-id="5e48b-130">errorCode</span></span>|<span data-ttu-id="5e48b-131">Int32</span><span class="sxs-lookup"><span data-stu-id="5e48b-131">Int32</span></span>|<span data-ttu-id="5e48b-132">Код ошибки действия Configuration Manager от клиента</span><span class="sxs-lookup"><span data-stu-id="5e48b-132">Error code of Configuration Manager action from client</span></span>|

## <a name="relationships"></a><span data-ttu-id="5e48b-133">Связи</span><span class="sxs-lookup"><span data-stu-id="5e48b-133">Relationships</span></span>
<span data-ttu-id="5e48b-134">Нет</span><span class="sxs-lookup"><span data-stu-id="5e48b-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5e48b-135">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5e48b-135">JSON Representation</span></span>
<span data-ttu-id="5e48b-136">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5e48b-136">Here is a JSON representation of the resource.</span></span>
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







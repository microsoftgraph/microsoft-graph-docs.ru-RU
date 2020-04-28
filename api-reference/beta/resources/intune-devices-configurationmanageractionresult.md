---
title: Тип ресурса Конфигуратионманажерактионресулт
description: Результат действия Конфигуратионманажер
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 5c5450eb4178181d7bbf2c76bd978e91cbdf0cb2
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43465084"
---
# <a name="configurationmanageractionresult-resource-type"></a><span data-ttu-id="3ccd8-103">Тип ресурса Конфигуратионманажерактионресулт</span><span class="sxs-lookup"><span data-stu-id="3ccd8-103">configurationManagerActionResult resource type</span></span>

<span data-ttu-id="3ccd8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3ccd8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3ccd8-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3ccd8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3ccd8-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3ccd8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3ccd8-107">Результат действия Конфигуратионманажер</span><span class="sxs-lookup"><span data-stu-id="3ccd8-107">Result of the ConfigurationManager action</span></span>


<span data-ttu-id="3ccd8-108">Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="3ccd8-108">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="3ccd8-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="3ccd8-109">Properties</span></span>
|<span data-ttu-id="3ccd8-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="3ccd8-110">Property</span></span>|<span data-ttu-id="3ccd8-111">Тип</span><span class="sxs-lookup"><span data-stu-id="3ccd8-111">Type</span></span>|<span data-ttu-id="3ccd8-112">Описание</span><span class="sxs-lookup"><span data-stu-id="3ccd8-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3ccd8-113">actionName</span><span class="sxs-lookup"><span data-stu-id="3ccd8-113">actionName</span></span>|<span data-ttu-id="3ccd8-114">String</span><span class="sxs-lookup"><span data-stu-id="3ccd8-114">String</span></span>|<span data-ttu-id="3ccd8-115">Название действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="3ccd8-115">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="3ccd8-116">actionState</span><span class="sxs-lookup"><span data-stu-id="3ccd8-116">actionState</span></span>|[<span data-ttu-id="3ccd8-117">actionState</span><span class="sxs-lookup"><span data-stu-id="3ccd8-117">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="3ccd8-118">Состояние действия, унаследованного от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="3ccd8-118">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="3ccd8-119">Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="3ccd8-119">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="3ccd8-120">startDateTime</span><span class="sxs-lookup"><span data-stu-id="3ccd8-120">startDateTime</span></span>|<span data-ttu-id="3ccd8-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3ccd8-121">DateTimeOffset</span></span>|<span data-ttu-id="3ccd8-122">Время начала действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="3ccd8-122">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="3ccd8-123">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="3ccd8-123">lastUpdatedDateTime</span></span>|<span data-ttu-id="3ccd8-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3ccd8-124">DateTimeOffset</span></span>|<span data-ttu-id="3ccd8-125">Время последнего обновления действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="3ccd8-125">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="3ccd8-126">актионделиверистатус</span><span class="sxs-lookup"><span data-stu-id="3ccd8-126">actionDeliveryStatus</span></span>|[<span data-ttu-id="3ccd8-127">configurationManagerActionDeliveryStatus</span><span class="sxs-lookup"><span data-stu-id="3ccd8-127">configurationManagerActionDeliveryStatus</span></span>](../resources/intune-devices-configurationmanageractiondeliverystatus.md)|<span data-ttu-id="3ccd8-128">Состояние действия, которое доставляется на локальный сервер.</span><span class="sxs-lookup"><span data-stu-id="3ccd8-128">State of the action being delivered to on-prem server.</span></span> <span data-ttu-id="3ccd8-129">Возможные значения: `unknown`, `pendingDelivery`, `deliveredToConnectorService`, `failedToDeliverToConnectorService`, `deliveredToOnPremisesServer`.</span><span class="sxs-lookup"><span data-stu-id="3ccd8-129">Possible values are: `unknown`, `pendingDelivery`, `deliveredToConnectorService`, `failedToDeliverToConnectorService`, `deliveredToOnPremisesServer`.</span></span>|
|<span data-ttu-id="3ccd8-130">errorCode</span><span class="sxs-lookup"><span data-stu-id="3ccd8-130">errorCode</span></span>|<span data-ttu-id="3ccd8-131">Int32</span><span class="sxs-lookup"><span data-stu-id="3ccd8-131">Int32</span></span>|<span data-ttu-id="3ccd8-132">Код ошибки действия Configuration Manager от клиента</span><span class="sxs-lookup"><span data-stu-id="3ccd8-132">Error code of Configuration Manager action from client</span></span>|

## <a name="relationships"></a><span data-ttu-id="3ccd8-133">Связи</span><span class="sxs-lookup"><span data-stu-id="3ccd8-133">Relationships</span></span>
<span data-ttu-id="3ccd8-134">Нет</span><span class="sxs-lookup"><span data-stu-id="3ccd8-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3ccd8-135">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3ccd8-135">JSON Representation</span></span>
<span data-ttu-id="3ccd8-136">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3ccd8-136">Here is a JSON representation of the resource.</span></span>
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




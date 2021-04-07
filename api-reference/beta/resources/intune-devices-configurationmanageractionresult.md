---
title: тип ресурса configurationManagerActionResult
description: Результат действия ConfigurationManager
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 9fbe2827194403c8295e9ef59a1089c698f14092
ms.sourcegitcommit: fe1b4d098af604cc34596f595e799911ea672532
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/07/2021
ms.locfileid: "51611981"
---
# <a name="configurationmanageractionresult-resource-type"></a><span data-ttu-id="c724f-103">тип ресурса configurationManagerActionResult</span><span class="sxs-lookup"><span data-stu-id="c724f-103">configurationManagerActionResult resource type</span></span>

<span data-ttu-id="c724f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c724f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c724f-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c724f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c724f-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c724f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c724f-107">Результат действия ConfigurationManager</span><span class="sxs-lookup"><span data-stu-id="c724f-107">Result of the ConfigurationManager action</span></span>


<span data-ttu-id="c724f-108">Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="c724f-108">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c724f-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="c724f-109">Properties</span></span>
|<span data-ttu-id="c724f-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="c724f-110">Property</span></span>|<span data-ttu-id="c724f-111">Тип</span><span class="sxs-lookup"><span data-stu-id="c724f-111">Type</span></span>|<span data-ttu-id="c724f-112">Описание</span><span class="sxs-lookup"><span data-stu-id="c724f-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c724f-113">actionName</span><span class="sxs-lookup"><span data-stu-id="c724f-113">actionName</span></span>|<span data-ttu-id="c724f-114">String</span><span class="sxs-lookup"><span data-stu-id="c724f-114">String</span></span>|<span data-ttu-id="c724f-115">Название действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="c724f-115">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="c724f-116">actionState</span><span class="sxs-lookup"><span data-stu-id="c724f-116">actionState</span></span>|[<span data-ttu-id="c724f-117">actionState</span><span class="sxs-lookup"><span data-stu-id="c724f-117">actionState</span></span>](../resources/intune-devices-actionstate.md)|<span data-ttu-id="c724f-118">Состояние действия, унаследованной от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="c724f-118">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="c724f-119">Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="c724f-119">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="c724f-120">startDateTime</span><span class="sxs-lookup"><span data-stu-id="c724f-120">startDateTime</span></span>|<span data-ttu-id="c724f-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c724f-121">DateTimeOffset</span></span>|<span data-ttu-id="c724f-122">Время начала действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="c724f-122">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="c724f-123">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="c724f-123">lastUpdatedDateTime</span></span>|<span data-ttu-id="c724f-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c724f-124">DateTimeOffset</span></span>|<span data-ttu-id="c724f-125">Время последнего обновления действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="c724f-125">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="c724f-126">actionDeliveryStatus</span><span class="sxs-lookup"><span data-stu-id="c724f-126">actionDeliveryStatus</span></span>|[<span data-ttu-id="c724f-127">configurationManagerActionDeliveryStatus</span><span class="sxs-lookup"><span data-stu-id="c724f-127">configurationManagerActionDeliveryStatus</span></span>](../resources/intune-devices-configurationmanageractiondeliverystatus.md)|<span data-ttu-id="c724f-128">Состояние действия, доставляемого на предварительном сервере.</span><span class="sxs-lookup"><span data-stu-id="c724f-128">State of the action being delivered to on-prem server.</span></span> <span data-ttu-id="c724f-129">Возможные значения: `unknown`, `pendingDelivery`, `deliveredToConnectorService`, `failedToDeliverToConnectorService`, `deliveredToOnPremisesServer`.</span><span class="sxs-lookup"><span data-stu-id="c724f-129">Possible values are: `unknown`, `pendingDelivery`, `deliveredToConnectorService`, `failedToDeliverToConnectorService`, `deliveredToOnPremisesServer`.</span></span>|
|<span data-ttu-id="c724f-130">errorCode</span><span class="sxs-lookup"><span data-stu-id="c724f-130">errorCode</span></span>|<span data-ttu-id="c724f-131">Int32</span><span class="sxs-lookup"><span data-stu-id="c724f-131">Int32</span></span>|<span data-ttu-id="c724f-132">Код ошибки действия Configuration Manager от клиента</span><span class="sxs-lookup"><span data-stu-id="c724f-132">Error code of Configuration Manager action from client</span></span>|

## <a name="relationships"></a><span data-ttu-id="c724f-133">Связи</span><span class="sxs-lookup"><span data-stu-id="c724f-133">Relationships</span></span>
<span data-ttu-id="c724f-134">Нет</span><span class="sxs-lookup"><span data-stu-id="c724f-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c724f-135">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c724f-135">JSON Representation</span></span>
<span data-ttu-id="c724f-136">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c724f-136">Here is a JSON representation of the resource.</span></span>
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





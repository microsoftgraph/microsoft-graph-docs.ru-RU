---
title: Тип ресурса Ревокеапплевпплиценсесактионресулт
description: Отзыв результатов действий для лицензий Apple VPP
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b86cdd0f52e885efec712448236bc8ba7c2d23d9
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48081078"
---
# <a name="revokeapplevpplicensesactionresult-resource-type"></a><span data-ttu-id="9a924-103">Тип ресурса Ревокеапплевпплиценсесактионресулт</span><span class="sxs-lookup"><span data-stu-id="9a924-103">revokeAppleVppLicensesActionResult resource type</span></span>

<span data-ttu-id="9a924-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9a924-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9a924-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9a924-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9a924-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9a924-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9a924-107">Отзыв результатов действий для лицензий Apple VPP</span><span class="sxs-lookup"><span data-stu-id="9a924-107">Revoke Apple Vpp licenses action result</span></span>


<span data-ttu-id="9a924-108">Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="9a924-108">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="9a924-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="9a924-109">Properties</span></span>
|<span data-ttu-id="9a924-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="9a924-110">Property</span></span>|<span data-ttu-id="9a924-111">Тип</span><span class="sxs-lookup"><span data-stu-id="9a924-111">Type</span></span>|<span data-ttu-id="9a924-112">Описание</span><span class="sxs-lookup"><span data-stu-id="9a924-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9a924-113">actionName</span><span class="sxs-lookup"><span data-stu-id="9a924-113">actionName</span></span>|<span data-ttu-id="9a924-114">String</span><span class="sxs-lookup"><span data-stu-id="9a924-114">String</span></span>|<span data-ttu-id="9a924-115">Название действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="9a924-115">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="9a924-116">actionState</span><span class="sxs-lookup"><span data-stu-id="9a924-116">actionState</span></span>|[<span data-ttu-id="9a924-117">actionState</span><span class="sxs-lookup"><span data-stu-id="9a924-117">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="9a924-118">Состояние действия, унаследованного от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="9a924-118">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="9a924-119">Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="9a924-119">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="9a924-120">startDateTime</span><span class="sxs-lookup"><span data-stu-id="9a924-120">startDateTime</span></span>|<span data-ttu-id="9a924-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9a924-121">DateTimeOffset</span></span>|<span data-ttu-id="9a924-122">Время начала действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="9a924-122">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="9a924-123">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="9a924-123">lastUpdatedDateTime</span></span>|<span data-ttu-id="9a924-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9a924-124">DateTimeOffset</span></span>|<span data-ttu-id="9a924-125">Время последнего обновления действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="9a924-125">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="9a924-126">тоталлиценсескаунт</span><span class="sxs-lookup"><span data-stu-id="9a924-126">totalLicensesCount</span></span>|<span data-ttu-id="9a924-127">Int32</span><span class="sxs-lookup"><span data-stu-id="9a924-127">Int32</span></span>|<span data-ttu-id="9a924-128">Общее количество связанных лицензий Apple VPP</span><span class="sxs-lookup"><span data-stu-id="9a924-128">Total number of Apple Vpp licenses associated</span></span>|
|<span data-ttu-id="9a924-129">фаиледлиценсескаунт</span><span class="sxs-lookup"><span data-stu-id="9a924-129">failedLicensesCount</span></span>|<span data-ttu-id="9a924-130">Int32</span><span class="sxs-lookup"><span data-stu-id="9a924-130">Int32</span></span>|<span data-ttu-id="9a924-131">Общее количество лицензий Apple VPP, которые не удалось отозвать</span><span class="sxs-lookup"><span data-stu-id="9a924-131">Total number of Apple Vpp licenses that failed to revoke</span></span>|

## <a name="relationships"></a><span data-ttu-id="9a924-132">Связи</span><span class="sxs-lookup"><span data-stu-id="9a924-132">Relationships</span></span>
<span data-ttu-id="9a924-133">Нет</span><span class="sxs-lookup"><span data-stu-id="9a924-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9a924-134">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9a924-134">JSON Representation</span></span>
<span data-ttu-id="9a924-135">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9a924-135">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.revokeAppleVppLicensesActionResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.revokeAppleVppLicensesActionResult",
  "actionName": "String",
  "actionState": "String",
  "startDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)",
  "totalLicensesCount": 1024,
  "failedLicensesCount": 1024
}
```







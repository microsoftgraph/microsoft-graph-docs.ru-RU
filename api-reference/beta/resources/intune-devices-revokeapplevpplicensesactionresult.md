---
title: Тип ресурса Ревокеапплевпплиценсесактионресулт
description: Отзыв результатов действий для лицензий Apple VPP
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 09843bbce769594e2729421121b7a936dcd19c4a
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48724504"
---
# <a name="revokeapplevpplicensesactionresult-resource-type"></a><span data-ttu-id="c1093-103">Тип ресурса Ревокеапплевпплиценсесактионресулт</span><span class="sxs-lookup"><span data-stu-id="c1093-103">revokeAppleVppLicensesActionResult resource type</span></span>

<span data-ttu-id="c1093-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c1093-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c1093-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c1093-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c1093-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c1093-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c1093-107">Отзыв результатов действий для лицензий Apple VPP</span><span class="sxs-lookup"><span data-stu-id="c1093-107">Revoke Apple Vpp licenses action result</span></span>


<span data-ttu-id="c1093-108">Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="c1093-108">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c1093-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="c1093-109">Properties</span></span>
|<span data-ttu-id="c1093-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="c1093-110">Property</span></span>|<span data-ttu-id="c1093-111">Тип</span><span class="sxs-lookup"><span data-stu-id="c1093-111">Type</span></span>|<span data-ttu-id="c1093-112">Описание</span><span class="sxs-lookup"><span data-stu-id="c1093-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c1093-113">actionName</span><span class="sxs-lookup"><span data-stu-id="c1093-113">actionName</span></span>|<span data-ttu-id="c1093-114">String</span><span class="sxs-lookup"><span data-stu-id="c1093-114">String</span></span>|<span data-ttu-id="c1093-115">Название действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="c1093-115">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="c1093-116">actionState</span><span class="sxs-lookup"><span data-stu-id="c1093-116">actionState</span></span>|[<span data-ttu-id="c1093-117">actionState</span><span class="sxs-lookup"><span data-stu-id="c1093-117">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="c1093-118">Состояние действия, унаследованного от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="c1093-118">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="c1093-119">Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="c1093-119">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="c1093-120">startDateTime</span><span class="sxs-lookup"><span data-stu-id="c1093-120">startDateTime</span></span>|<span data-ttu-id="c1093-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c1093-121">DateTimeOffset</span></span>|<span data-ttu-id="c1093-122">Время начала действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="c1093-122">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="c1093-123">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="c1093-123">lastUpdatedDateTime</span></span>|<span data-ttu-id="c1093-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c1093-124">DateTimeOffset</span></span>|<span data-ttu-id="c1093-125">Время последнего обновления действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="c1093-125">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="c1093-126">тоталлиценсескаунт</span><span class="sxs-lookup"><span data-stu-id="c1093-126">totalLicensesCount</span></span>|<span data-ttu-id="c1093-127">Int32</span><span class="sxs-lookup"><span data-stu-id="c1093-127">Int32</span></span>|<span data-ttu-id="c1093-128">Общее количество связанных лицензий Apple VPP</span><span class="sxs-lookup"><span data-stu-id="c1093-128">Total number of Apple Vpp licenses associated</span></span>|
|<span data-ttu-id="c1093-129">фаиледлиценсескаунт</span><span class="sxs-lookup"><span data-stu-id="c1093-129">failedLicensesCount</span></span>|<span data-ttu-id="c1093-130">Int32</span><span class="sxs-lookup"><span data-stu-id="c1093-130">Int32</span></span>|<span data-ttu-id="c1093-131">Общее количество лицензий Apple VPP, которые не удалось отозвать</span><span class="sxs-lookup"><span data-stu-id="c1093-131">Total number of Apple Vpp licenses that failed to revoke</span></span>|

## <a name="relationships"></a><span data-ttu-id="c1093-132">Связи</span><span class="sxs-lookup"><span data-stu-id="c1093-132">Relationships</span></span>
<span data-ttu-id="c1093-133">Нет</span><span class="sxs-lookup"><span data-stu-id="c1093-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c1093-134">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c1093-134">JSON Representation</span></span>
<span data-ttu-id="c1093-135">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c1093-135">Here is a JSON representation of the resource.</span></span>
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






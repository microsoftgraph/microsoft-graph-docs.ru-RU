---
title: Тип ресурса Ревокеапплевпплиценсесактионресулт
description: Отзыв результатов действий для лицензий Apple VPP
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c5315c2061eafbe87b6a5292237828c65999433e
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31789306"
---
# <a name="revokeapplevpplicensesactionresult-resource-type"></a><span data-ttu-id="cf6c7-103">Тип ресурса Ревокеапплевпплиценсесактионресулт</span><span class="sxs-lookup"><span data-stu-id="cf6c7-103">revokeAppleVppLicensesActionResult resource type</span></span>

> <span data-ttu-id="cf6c7-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cf6c7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cf6c7-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="cf6c7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cf6c7-106">Отзыв результатов действий для лицензий Apple VPP</span><span class="sxs-lookup"><span data-stu-id="cf6c7-106">Revoke Apple Vpp licenses action result</span></span>


<span data-ttu-id="cf6c7-107">Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="cf6c7-107">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="cf6c7-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="cf6c7-108">Properties</span></span>
|<span data-ttu-id="cf6c7-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="cf6c7-109">Property</span></span>|<span data-ttu-id="cf6c7-110">Тип</span><span class="sxs-lookup"><span data-stu-id="cf6c7-110">Type</span></span>|<span data-ttu-id="cf6c7-111">Описание</span><span class="sxs-lookup"><span data-stu-id="cf6c7-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cf6c7-112">actionName</span><span class="sxs-lookup"><span data-stu-id="cf6c7-112">actionName</span></span>|<span data-ttu-id="cf6c7-113">String</span><span class="sxs-lookup"><span data-stu-id="cf6c7-113">String</span></span>|<span data-ttu-id="cf6c7-114">Название действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="cf6c7-114">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="cf6c7-115">actionState</span><span class="sxs-lookup"><span data-stu-id="cf6c7-115">actionState</span></span>|[<span data-ttu-id="cf6c7-116">actionState</span><span class="sxs-lookup"><span data-stu-id="cf6c7-116">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="cf6c7-117">Состояние действия, унаследованного от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="cf6c7-117">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="cf6c7-118">Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="cf6c7-118">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="cf6c7-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="cf6c7-119">startDateTime</span></span>|<span data-ttu-id="cf6c7-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cf6c7-120">DateTimeOffset</span></span>|<span data-ttu-id="cf6c7-121">Время начала действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="cf6c7-121">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="cf6c7-122">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="cf6c7-122">lastUpdatedDateTime</span></span>|<span data-ttu-id="cf6c7-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cf6c7-123">DateTimeOffset</span></span>|<span data-ttu-id="cf6c7-124">Время последнего обновления действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="cf6c7-124">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="cf6c7-125">Тоталлиценсескаунт</span><span class="sxs-lookup"><span data-stu-id="cf6c7-125">totalLicensesCount</span></span>|<span data-ttu-id="cf6c7-126">Int32</span><span class="sxs-lookup"><span data-stu-id="cf6c7-126">Int32</span></span>|<span data-ttu-id="cf6c7-127">Общее количество связанных лицензий Apple VPP</span><span class="sxs-lookup"><span data-stu-id="cf6c7-127">Total number of Apple Vpp licenses associated</span></span>|
|<span data-ttu-id="cf6c7-128">Фаиледлиценсескаунт</span><span class="sxs-lookup"><span data-stu-id="cf6c7-128">failedLicensesCount</span></span>|<span data-ttu-id="cf6c7-129">Int32</span><span class="sxs-lookup"><span data-stu-id="cf6c7-129">Int32</span></span>|<span data-ttu-id="cf6c7-130">Общее количество лицензий Apple VPP, которые не удалось отозвать</span><span class="sxs-lookup"><span data-stu-id="cf6c7-130">Total number of Apple Vpp licenses that failed to revoke</span></span>|

## <a name="relationships"></a><span data-ttu-id="cf6c7-131">Отношения</span><span class="sxs-lookup"><span data-stu-id="cf6c7-131">Relationships</span></span>
<span data-ttu-id="cf6c7-132">Нет</span><span class="sxs-lookup"><span data-stu-id="cf6c7-132">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="cf6c7-133">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="cf6c7-133">JSON Representation</span></span>
<span data-ttu-id="cf6c7-134">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cf6c7-134">Here is a JSON representation of the resource.</span></span>
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






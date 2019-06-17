---
title: Тип ресурса Ревокеапплевпплиценсесактионресулт
description: Отзыв результатов действий для лицензий Apple VPP
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fe831c36af1cfbe29d4b5bcc0dd2daa2a148a01a
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34963830"
---
# <a name="revokeapplevpplicensesactionresult-resource-type"></a><span data-ttu-id="ff6c6-103">Тип ресурса Ревокеапплевпплиценсесактионресулт</span><span class="sxs-lookup"><span data-stu-id="ff6c6-103">revokeAppleVppLicensesActionResult resource type</span></span>

> <span data-ttu-id="ff6c6-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ff6c6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ff6c6-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ff6c6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ff6c6-106">Отзыв результатов действий для лицензий Apple VPP</span><span class="sxs-lookup"><span data-stu-id="ff6c6-106">Revoke Apple Vpp licenses action result</span></span>


<span data-ttu-id="ff6c6-107">Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="ff6c6-107">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="ff6c6-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="ff6c6-108">Properties</span></span>
|<span data-ttu-id="ff6c6-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="ff6c6-109">Property</span></span>|<span data-ttu-id="ff6c6-110">Тип</span><span class="sxs-lookup"><span data-stu-id="ff6c6-110">Type</span></span>|<span data-ttu-id="ff6c6-111">Описание</span><span class="sxs-lookup"><span data-stu-id="ff6c6-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ff6c6-112">actionName</span><span class="sxs-lookup"><span data-stu-id="ff6c6-112">actionName</span></span>|<span data-ttu-id="ff6c6-113">String</span><span class="sxs-lookup"><span data-stu-id="ff6c6-113">String</span></span>|<span data-ttu-id="ff6c6-114">Название действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="ff6c6-114">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="ff6c6-115">actionState</span><span class="sxs-lookup"><span data-stu-id="ff6c6-115">actionState</span></span>|[<span data-ttu-id="ff6c6-116">actionState</span><span class="sxs-lookup"><span data-stu-id="ff6c6-116">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="ff6c6-117">Состояние действия, унаследованного от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="ff6c6-117">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="ff6c6-118">Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="ff6c6-118">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="ff6c6-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="ff6c6-119">startDateTime</span></span>|<span data-ttu-id="ff6c6-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ff6c6-120">DateTimeOffset</span></span>|<span data-ttu-id="ff6c6-121">Время начала действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="ff6c6-121">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="ff6c6-122">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="ff6c6-122">lastUpdatedDateTime</span></span>|<span data-ttu-id="ff6c6-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ff6c6-123">DateTimeOffset</span></span>|<span data-ttu-id="ff6c6-124">Время последнего обновления действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="ff6c6-124">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="ff6c6-125">Тоталлиценсескаунт</span><span class="sxs-lookup"><span data-stu-id="ff6c6-125">totalLicensesCount</span></span>|<span data-ttu-id="ff6c6-126">Int32</span><span class="sxs-lookup"><span data-stu-id="ff6c6-126">Int32</span></span>|<span data-ttu-id="ff6c6-127">Общее количество связанных лицензий Apple VPP</span><span class="sxs-lookup"><span data-stu-id="ff6c6-127">Total number of Apple Vpp licenses associated</span></span>|
|<span data-ttu-id="ff6c6-128">Фаиледлиценсескаунт</span><span class="sxs-lookup"><span data-stu-id="ff6c6-128">failedLicensesCount</span></span>|<span data-ttu-id="ff6c6-129">Int32</span><span class="sxs-lookup"><span data-stu-id="ff6c6-129">Int32</span></span>|<span data-ttu-id="ff6c6-130">Общее количество лицензий Apple VPP, которые не удалось отозвать</span><span class="sxs-lookup"><span data-stu-id="ff6c6-130">Total number of Apple Vpp licenses that failed to revoke</span></span>|

## <a name="relationships"></a><span data-ttu-id="ff6c6-131">Отношения</span><span class="sxs-lookup"><span data-stu-id="ff6c6-131">Relationships</span></span>
<span data-ttu-id="ff6c6-132">Нет</span><span class="sxs-lookup"><span data-stu-id="ff6c6-132">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ff6c6-133">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ff6c6-133">JSON Representation</span></span>
<span data-ttu-id="ff6c6-134">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ff6c6-134">Here is a JSON representation of the resource.</span></span>
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






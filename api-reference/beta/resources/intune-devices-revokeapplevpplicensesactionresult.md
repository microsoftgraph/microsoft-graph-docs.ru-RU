---
title: Тип ресурса Ревокеапплевпплиценсесактионресулт
description: Отзыв результатов действий для лицензий Apple VPP
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 68a01df03814ea2fd0b52ecfc681490777b46d54
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43383153"
---
# <a name="revokeapplevpplicensesactionresult-resource-type"></a><span data-ttu-id="b0a96-103">Тип ресурса Ревокеапплевпплиценсесактионресулт</span><span class="sxs-lookup"><span data-stu-id="b0a96-103">revokeAppleVppLicensesActionResult resource type</span></span>

<span data-ttu-id="b0a96-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b0a96-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b0a96-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b0a96-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b0a96-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b0a96-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b0a96-107">Отзыв результатов действий для лицензий Apple VPP</span><span class="sxs-lookup"><span data-stu-id="b0a96-107">Revoke Apple Vpp licenses action result</span></span>


<span data-ttu-id="b0a96-108">Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="b0a96-108">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="b0a96-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="b0a96-109">Properties</span></span>
|<span data-ttu-id="b0a96-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="b0a96-110">Property</span></span>|<span data-ttu-id="b0a96-111">Тип</span><span class="sxs-lookup"><span data-stu-id="b0a96-111">Type</span></span>|<span data-ttu-id="b0a96-112">Описание</span><span class="sxs-lookup"><span data-stu-id="b0a96-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b0a96-113">actionName</span><span class="sxs-lookup"><span data-stu-id="b0a96-113">actionName</span></span>|<span data-ttu-id="b0a96-114">String</span><span class="sxs-lookup"><span data-stu-id="b0a96-114">String</span></span>|<span data-ttu-id="b0a96-115">Название действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="b0a96-115">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="b0a96-116">actionState</span><span class="sxs-lookup"><span data-stu-id="b0a96-116">actionState</span></span>|[<span data-ttu-id="b0a96-117">actionState</span><span class="sxs-lookup"><span data-stu-id="b0a96-117">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="b0a96-118">Состояние действия, унаследованного от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="b0a96-118">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="b0a96-119">Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="b0a96-119">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="b0a96-120">startDateTime</span><span class="sxs-lookup"><span data-stu-id="b0a96-120">startDateTime</span></span>|<span data-ttu-id="b0a96-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b0a96-121">DateTimeOffset</span></span>|<span data-ttu-id="b0a96-122">Время начала действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="b0a96-122">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="b0a96-123">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="b0a96-123">lastUpdatedDateTime</span></span>|<span data-ttu-id="b0a96-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b0a96-124">DateTimeOffset</span></span>|<span data-ttu-id="b0a96-125">Время последнего обновления действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="b0a96-125">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="b0a96-126">тоталлиценсескаунт</span><span class="sxs-lookup"><span data-stu-id="b0a96-126">totalLicensesCount</span></span>|<span data-ttu-id="b0a96-127">Int32</span><span class="sxs-lookup"><span data-stu-id="b0a96-127">Int32</span></span>|<span data-ttu-id="b0a96-128">Общее количество связанных лицензий Apple VPP</span><span class="sxs-lookup"><span data-stu-id="b0a96-128">Total number of Apple Vpp licenses associated</span></span>|
|<span data-ttu-id="b0a96-129">фаиледлиценсескаунт</span><span class="sxs-lookup"><span data-stu-id="b0a96-129">failedLicensesCount</span></span>|<span data-ttu-id="b0a96-130">Int32</span><span class="sxs-lookup"><span data-stu-id="b0a96-130">Int32</span></span>|<span data-ttu-id="b0a96-131">Общее количество лицензий Apple VPP, которые не удалось отозвать</span><span class="sxs-lookup"><span data-stu-id="b0a96-131">Total number of Apple Vpp licenses that failed to revoke</span></span>|

## <a name="relationships"></a><span data-ttu-id="b0a96-132">Связи</span><span class="sxs-lookup"><span data-stu-id="b0a96-132">Relationships</span></span>
<span data-ttu-id="b0a96-133">Нет</span><span class="sxs-lookup"><span data-stu-id="b0a96-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b0a96-134">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b0a96-134">JSON Representation</span></span>
<span data-ttu-id="b0a96-135">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b0a96-135">Here is a JSON representation of the resource.</span></span>
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




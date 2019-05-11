---
title: Тип ресурса Макосвппаппревокелиценсесактионресулт
description: Определяет результаты для действий в приложениях MacOS VPP, содержит унаследованные свойства для Актионресулт.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ad7ad1a2cdf8eabd67c1578c387b424f3e6f6c85
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33950223"
---
# <a name="macosvppapprevokelicensesactionresult-resource-type"></a><span data-ttu-id="dc457-103">Тип ресурса Макосвппаппревокелиценсесактионресулт</span><span class="sxs-lookup"><span data-stu-id="dc457-103">macOsVppAppRevokeLicensesActionResult resource type</span></span>

> <span data-ttu-id="dc457-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dc457-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dc457-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="dc457-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dc457-106">Определяет результаты для действий в приложениях MacOS VPP, содержит унаследованные свойства для Актионресулт.</span><span class="sxs-lookup"><span data-stu-id="dc457-106">Defines results for actions on MacOS Vpp Apps, contains inherited properties for ActionResult.</span></span>

## <a name="properties"></a><span data-ttu-id="dc457-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="dc457-107">Properties</span></span>
|<span data-ttu-id="dc457-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="dc457-108">Property</span></span>|<span data-ttu-id="dc457-109">Тип</span><span class="sxs-lookup"><span data-stu-id="dc457-109">Type</span></span>|<span data-ttu-id="dc457-110">Описание</span><span class="sxs-lookup"><span data-stu-id="dc457-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dc457-111">userId</span><span class="sxs-lookup"><span data-stu-id="dc457-111">userId</span></span>|<span data-ttu-id="dc457-112">String</span><span class="sxs-lookup"><span data-stu-id="dc457-112">String</span></span>|<span data-ttu-id="dc457-113">UserId, связанный с действием.</span><span class="sxs-lookup"><span data-stu-id="dc457-113">UserId associated with the action.</span></span>|
|<span data-ttu-id="dc457-114">Манажеддевицеид</span><span class="sxs-lookup"><span data-stu-id="dc457-114">managedDeviceId</span></span>|<span data-ttu-id="dc457-115">Строка</span><span class="sxs-lookup"><span data-stu-id="dc457-115">String</span></span>|<span data-ttu-id="dc457-116">DeviceId, связанный с действием.</span><span class="sxs-lookup"><span data-stu-id="dc457-116">DeviceId associated with the action.</span></span>|
|<span data-ttu-id="dc457-117">Тоталлиценсескаунт</span><span class="sxs-lookup"><span data-stu-id="dc457-117">totalLicensesCount</span></span>|<span data-ttu-id="dc457-118">Int32</span><span class="sxs-lookup"><span data-stu-id="dc457-118">Int32</span></span>|<span data-ttu-id="dc457-119">Количество лицензий, для которых была предпринята попытка отзыва.</span><span class="sxs-lookup"><span data-stu-id="dc457-119">A count of the number of licenses for which revoke was attempted.</span></span>|
|<span data-ttu-id="dc457-120">Фаиледлиценсескаунт</span><span class="sxs-lookup"><span data-stu-id="dc457-120">failedLicensesCount</span></span>|<span data-ttu-id="dc457-121">Int32</span><span class="sxs-lookup"><span data-stu-id="dc457-121">Int32</span></span>|<span data-ttu-id="dc457-122">Количество лицензий, для которых произошел сбой при отзыве.</span><span class="sxs-lookup"><span data-stu-id="dc457-122">A count of the number of licenses for which revoke failed.</span></span>|
|<span data-ttu-id="dc457-123">Актионфаилуререасон</span><span class="sxs-lookup"><span data-stu-id="dc457-123">actionFailureReason</span></span>|[<span data-ttu-id="dc457-124">Впптокенактионфаилуререасон</span><span class="sxs-lookup"><span data-stu-id="dc457-124">vppTokenActionFailureReason</span></span>](../resources/intune-shared-vpptokenactionfailurereason.md)|<span data-ttu-id="dc457-125">Причина сбоя действия "отзыв лицензий".</span><span class="sxs-lookup"><span data-stu-id="dc457-125">The reason for the revoke licenses action failure.</span></span> <span data-ttu-id="dc457-126">Возможные значения: `none`, `appleFailure`, `internalError`, `expiredVppToken`, `expiredApplePushNotificationCertificate`.</span><span class="sxs-lookup"><span data-stu-id="dc457-126">Possible values are: `none`, `appleFailure`, `internalError`, `expiredVppToken`, `expiredApplePushNotificationCertificate`.</span></span>|
|<span data-ttu-id="dc457-127">actionName</span><span class="sxs-lookup"><span data-stu-id="dc457-127">actionName</span></span>|<span data-ttu-id="dc457-128">String</span><span class="sxs-lookup"><span data-stu-id="dc457-128">String</span></span>|<span data-ttu-id="dc457-129">Название действия</span><span class="sxs-lookup"><span data-stu-id="dc457-129">Action name</span></span>|
|<span data-ttu-id="dc457-130">actionState</span><span class="sxs-lookup"><span data-stu-id="dc457-130">actionState</span></span>|[<span data-ttu-id="dc457-131">actionState</span><span class="sxs-lookup"><span data-stu-id="dc457-131">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="dc457-132">Состояние действия.</span><span class="sxs-lookup"><span data-stu-id="dc457-132">State of the action.</span></span> <span data-ttu-id="dc457-133">Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="dc457-133">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="dc457-134">startDateTime</span><span class="sxs-lookup"><span data-stu-id="dc457-134">startDateTime</span></span>|<span data-ttu-id="dc457-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dc457-135">DateTimeOffset</span></span>|<span data-ttu-id="dc457-136">Время начала действия</span><span class="sxs-lookup"><span data-stu-id="dc457-136">Time the action was initiated</span></span>|
|<span data-ttu-id="dc457-137">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="dc457-137">lastUpdatedDateTime</span></span>|<span data-ttu-id="dc457-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dc457-138">DateTimeOffset</span></span>|<span data-ttu-id="dc457-139">Время последнего обновления состояния действия</span><span class="sxs-lookup"><span data-stu-id="dc457-139">Time the action state was last updated</span></span>|

## <a name="relationships"></a><span data-ttu-id="dc457-140">Связи</span><span class="sxs-lookup"><span data-stu-id="dc457-140">Relationships</span></span>
<span data-ttu-id="dc457-141">Нет</span><span class="sxs-lookup"><span data-stu-id="dc457-141">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="dc457-142">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="dc457-142">JSON Representation</span></span>
<span data-ttu-id="dc457-143">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="dc457-143">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.macOsVppAppRevokeLicensesActionResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOsVppAppRevokeLicensesActionResult",
  "userId": "String",
  "managedDeviceId": "String",
  "totalLicensesCount": 1024,
  "failedLicensesCount": 1024,
  "actionFailureReason": "String",
  "actionName": "String",
  "actionState": "String",
  "startDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)"
}
```





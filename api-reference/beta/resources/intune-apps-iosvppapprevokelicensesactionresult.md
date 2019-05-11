---
title: Тип ресурса Иосвппаппревокелиценсесактионресулт
description: Определяет результаты действий в приложениях для iOS VPP, содержит унаследованные свойства для Актионресулт.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6e28e21baa4dc0461d9b54f206810a969a153c15
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33950244"
---
# <a name="iosvppapprevokelicensesactionresult-resource-type"></a><span data-ttu-id="f9750-103">Тип ресурса Иосвппаппревокелиценсесактионресулт</span><span class="sxs-lookup"><span data-stu-id="f9750-103">iosVppAppRevokeLicensesActionResult resource type</span></span>

> <span data-ttu-id="f9750-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f9750-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f9750-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f9750-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f9750-106">Определяет результаты действий в приложениях для iOS VPP, содержит унаследованные свойства для Актионресулт.</span><span class="sxs-lookup"><span data-stu-id="f9750-106">Defines results for actions on iOS Vpp Apps, contains inherited properties for ActionResult.</span></span>

## <a name="properties"></a><span data-ttu-id="f9750-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="f9750-107">Properties</span></span>
|<span data-ttu-id="f9750-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="f9750-108">Property</span></span>|<span data-ttu-id="f9750-109">Тип</span><span class="sxs-lookup"><span data-stu-id="f9750-109">Type</span></span>|<span data-ttu-id="f9750-110">Описание</span><span class="sxs-lookup"><span data-stu-id="f9750-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f9750-111">userId</span><span class="sxs-lookup"><span data-stu-id="f9750-111">userId</span></span>|<span data-ttu-id="f9750-112">String</span><span class="sxs-lookup"><span data-stu-id="f9750-112">String</span></span>|<span data-ttu-id="f9750-113">UserId, связанный с действием.</span><span class="sxs-lookup"><span data-stu-id="f9750-113">UserId associated with the action.</span></span>|
|<span data-ttu-id="f9750-114">Манажеддевицеид</span><span class="sxs-lookup"><span data-stu-id="f9750-114">managedDeviceId</span></span>|<span data-ttu-id="f9750-115">Строка</span><span class="sxs-lookup"><span data-stu-id="f9750-115">String</span></span>|<span data-ttu-id="f9750-116">DeviceId, связанный с действием.</span><span class="sxs-lookup"><span data-stu-id="f9750-116">DeviceId associated with the action.</span></span>|
|<span data-ttu-id="f9750-117">Тоталлиценсескаунт</span><span class="sxs-lookup"><span data-stu-id="f9750-117">totalLicensesCount</span></span>|<span data-ttu-id="f9750-118">Int32</span><span class="sxs-lookup"><span data-stu-id="f9750-118">Int32</span></span>|<span data-ttu-id="f9750-119">Количество лицензий, для которых была предпринята попытка отзыва.</span><span class="sxs-lookup"><span data-stu-id="f9750-119">A count of the number of licenses for which revoke was attempted.</span></span>|
|<span data-ttu-id="f9750-120">Фаиледлиценсескаунт</span><span class="sxs-lookup"><span data-stu-id="f9750-120">failedLicensesCount</span></span>|<span data-ttu-id="f9750-121">Int32</span><span class="sxs-lookup"><span data-stu-id="f9750-121">Int32</span></span>|<span data-ttu-id="f9750-122">Количество лицензий, для которых произошел сбой при отзыве.</span><span class="sxs-lookup"><span data-stu-id="f9750-122">A count of the number of licenses for which revoke failed.</span></span>|
|<span data-ttu-id="f9750-123">Актионфаилуререасон</span><span class="sxs-lookup"><span data-stu-id="f9750-123">actionFailureReason</span></span>|[<span data-ttu-id="f9750-124">Впптокенактионфаилуререасон</span><span class="sxs-lookup"><span data-stu-id="f9750-124">vppTokenActionFailureReason</span></span>](../resources/intune-shared-vpptokenactionfailurereason.md)|<span data-ttu-id="f9750-125">Причина сбоя действия "отзыв лицензий".</span><span class="sxs-lookup"><span data-stu-id="f9750-125">The reason for the revoke licenses action failure.</span></span> <span data-ttu-id="f9750-126">Возможные значения: `none`, `appleFailure`, `internalError`, `expiredVppToken`, `expiredApplePushNotificationCertificate`.</span><span class="sxs-lookup"><span data-stu-id="f9750-126">Possible values are: `none`, `appleFailure`, `internalError`, `expiredVppToken`, `expiredApplePushNotificationCertificate`.</span></span>|
|<span data-ttu-id="f9750-127">actionName</span><span class="sxs-lookup"><span data-stu-id="f9750-127">actionName</span></span>|<span data-ttu-id="f9750-128">String</span><span class="sxs-lookup"><span data-stu-id="f9750-128">String</span></span>|<span data-ttu-id="f9750-129">Название действия</span><span class="sxs-lookup"><span data-stu-id="f9750-129">Action name</span></span>|
|<span data-ttu-id="f9750-130">actionState</span><span class="sxs-lookup"><span data-stu-id="f9750-130">actionState</span></span>|[<span data-ttu-id="f9750-131">actionState</span><span class="sxs-lookup"><span data-stu-id="f9750-131">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="f9750-132">Состояние действия.</span><span class="sxs-lookup"><span data-stu-id="f9750-132">State of the action.</span></span> <span data-ttu-id="f9750-133">Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="f9750-133">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="f9750-134">startDateTime</span><span class="sxs-lookup"><span data-stu-id="f9750-134">startDateTime</span></span>|<span data-ttu-id="f9750-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f9750-135">DateTimeOffset</span></span>|<span data-ttu-id="f9750-136">Время начала действия</span><span class="sxs-lookup"><span data-stu-id="f9750-136">Time the action was initiated</span></span>|
|<span data-ttu-id="f9750-137">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="f9750-137">lastUpdatedDateTime</span></span>|<span data-ttu-id="f9750-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f9750-138">DateTimeOffset</span></span>|<span data-ttu-id="f9750-139">Время последнего обновления состояния действия</span><span class="sxs-lookup"><span data-stu-id="f9750-139">Time the action state was last updated</span></span>|

## <a name="relationships"></a><span data-ttu-id="f9750-140">Связи</span><span class="sxs-lookup"><span data-stu-id="f9750-140">Relationships</span></span>
<span data-ttu-id="f9750-141">Нет</span><span class="sxs-lookup"><span data-stu-id="f9750-141">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f9750-142">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f9750-142">JSON Representation</span></span>
<span data-ttu-id="f9750-143">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f9750-143">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosVppAppRevokeLicensesActionResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosVppAppRevokeLicensesActionResult",
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





---
title: Тип ресурса Иосвппаппревокелиценсесактионресулт
description: Определяет результаты действий в приложениях для iOS VPP, содержит унаследованные свойства для Актионресулт.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 3f101784808e20566deb59b2e3f61cb886371c17
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36005466"
---
# <a name="iosvppapprevokelicensesactionresult-resource-type"></a><span data-ttu-id="6d8df-103">Тип ресурса Иосвппаппревокелиценсесактионресулт</span><span class="sxs-lookup"><span data-stu-id="6d8df-103">iosVppAppRevokeLicensesActionResult resource type</span></span>

> <span data-ttu-id="6d8df-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6d8df-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6d8df-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6d8df-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6d8df-106">Определяет результаты действий в приложениях для iOS VPP, содержит унаследованные свойства для Актионресулт.</span><span class="sxs-lookup"><span data-stu-id="6d8df-106">Defines results for actions on iOS Vpp Apps, contains inherited properties for ActionResult.</span></span>

## <a name="properties"></a><span data-ttu-id="6d8df-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="6d8df-107">Properties</span></span>
|<span data-ttu-id="6d8df-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="6d8df-108">Property</span></span>|<span data-ttu-id="6d8df-109">Тип</span><span class="sxs-lookup"><span data-stu-id="6d8df-109">Type</span></span>|<span data-ttu-id="6d8df-110">Описание</span><span class="sxs-lookup"><span data-stu-id="6d8df-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6d8df-111">userId</span><span class="sxs-lookup"><span data-stu-id="6d8df-111">userId</span></span>|<span data-ttu-id="6d8df-112">String</span><span class="sxs-lookup"><span data-stu-id="6d8df-112">String</span></span>|<span data-ttu-id="6d8df-113">UserId, связанный с действием.</span><span class="sxs-lookup"><span data-stu-id="6d8df-113">UserId associated with the action.</span></span>|
|<span data-ttu-id="6d8df-114">Манажеддевицеид</span><span class="sxs-lookup"><span data-stu-id="6d8df-114">managedDeviceId</span></span>|<span data-ttu-id="6d8df-115">String</span><span class="sxs-lookup"><span data-stu-id="6d8df-115">String</span></span>|<span data-ttu-id="6d8df-116">DeviceId, связанный с действием.</span><span class="sxs-lookup"><span data-stu-id="6d8df-116">DeviceId associated with the action.</span></span>|
|<span data-ttu-id="6d8df-117">Тоталлиценсескаунт</span><span class="sxs-lookup"><span data-stu-id="6d8df-117">totalLicensesCount</span></span>|<span data-ttu-id="6d8df-118">Int32</span><span class="sxs-lookup"><span data-stu-id="6d8df-118">Int32</span></span>|<span data-ttu-id="6d8df-119">Количество лицензий, для которых была предпринята попытка отзыва.</span><span class="sxs-lookup"><span data-stu-id="6d8df-119">A count of the number of licenses for which revoke was attempted.</span></span>|
|<span data-ttu-id="6d8df-120">Фаиледлиценсескаунт</span><span class="sxs-lookup"><span data-stu-id="6d8df-120">failedLicensesCount</span></span>|<span data-ttu-id="6d8df-121">Int32</span><span class="sxs-lookup"><span data-stu-id="6d8df-121">Int32</span></span>|<span data-ttu-id="6d8df-122">Количество лицензий, для которых произошел сбой при отзыве.</span><span class="sxs-lookup"><span data-stu-id="6d8df-122">A count of the number of licenses for which revoke failed.</span></span>|
|<span data-ttu-id="6d8df-123">Актионфаилуререасон</span><span class="sxs-lookup"><span data-stu-id="6d8df-123">actionFailureReason</span></span>|[<span data-ttu-id="6d8df-124">Впптокенактионфаилуререасон</span><span class="sxs-lookup"><span data-stu-id="6d8df-124">vppTokenActionFailureReason</span></span>](../resources/intune-shared-vpptokenactionfailurereason.md)|<span data-ttu-id="6d8df-125">Причина сбоя действия "отзыв лицензий".</span><span class="sxs-lookup"><span data-stu-id="6d8df-125">The reason for the revoke licenses action failure.</span></span> <span data-ttu-id="6d8df-126">Возможные значения: `none`, `appleFailure`, `internalError`, `expiredVppToken`, `expiredApplePushNotificationCertificate`.</span><span class="sxs-lookup"><span data-stu-id="6d8df-126">Possible values are: `none`, `appleFailure`, `internalError`, `expiredVppToken`, `expiredApplePushNotificationCertificate`.</span></span>|
|<span data-ttu-id="6d8df-127">actionName</span><span class="sxs-lookup"><span data-stu-id="6d8df-127">actionName</span></span>|<span data-ttu-id="6d8df-128">String</span><span class="sxs-lookup"><span data-stu-id="6d8df-128">String</span></span>|<span data-ttu-id="6d8df-129">Название действия</span><span class="sxs-lookup"><span data-stu-id="6d8df-129">Action name</span></span>|
|<span data-ttu-id="6d8df-130">actionState</span><span class="sxs-lookup"><span data-stu-id="6d8df-130">actionState</span></span>|[<span data-ttu-id="6d8df-131">actionState</span><span class="sxs-lookup"><span data-stu-id="6d8df-131">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="6d8df-132">Состояние действия.</span><span class="sxs-lookup"><span data-stu-id="6d8df-132">State of the action.</span></span> <span data-ttu-id="6d8df-133">Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="6d8df-133">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="6d8df-134">startDateTime</span><span class="sxs-lookup"><span data-stu-id="6d8df-134">startDateTime</span></span>|<span data-ttu-id="6d8df-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6d8df-135">DateTimeOffset</span></span>|<span data-ttu-id="6d8df-136">Время начала действия</span><span class="sxs-lookup"><span data-stu-id="6d8df-136">Time the action was initiated</span></span>|
|<span data-ttu-id="6d8df-137">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="6d8df-137">lastUpdatedDateTime</span></span>|<span data-ttu-id="6d8df-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6d8df-138">DateTimeOffset</span></span>|<span data-ttu-id="6d8df-139">Время последнего обновления состояния действия</span><span class="sxs-lookup"><span data-stu-id="6d8df-139">Time the action state was last updated</span></span>|

## <a name="relationships"></a><span data-ttu-id="6d8df-140">Отношения</span><span class="sxs-lookup"><span data-stu-id="6d8df-140">Relationships</span></span>
<span data-ttu-id="6d8df-141">Нет</span><span class="sxs-lookup"><span data-stu-id="6d8df-141">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6d8df-142">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6d8df-142">JSON Representation</span></span>
<span data-ttu-id="6d8df-143">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6d8df-143">Here is a JSON representation of the resource.</span></span>
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






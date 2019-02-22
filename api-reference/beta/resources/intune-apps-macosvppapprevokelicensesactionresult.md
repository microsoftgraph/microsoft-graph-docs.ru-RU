---
title: Тип ресурса Макосвппаппревокелиценсесактионресулт
description: Определяет результаты для действий в приложениях MacOS VPP, содержит унаследованные свойства для Актионресулт.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7cf8390dc2c1541525e288b81defd073144f4132
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30166509"
---
# <a name="macosvppapprevokelicensesactionresult-resource-type"></a><span data-ttu-id="208e1-103">Тип ресурса Макосвппаппревокелиценсесактионресулт</span><span class="sxs-lookup"><span data-stu-id="208e1-103">macOsVppAppRevokeLicensesActionResult resource type</span></span>

> <span data-ttu-id="208e1-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="208e1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="208e1-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="208e1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="208e1-106">Определяет результаты для действий в приложениях MacOS VPP, содержит унаследованные свойства для Актионресулт.</span><span class="sxs-lookup"><span data-stu-id="208e1-106">Defines results for actions on MacOS Vpp Apps, contains inherited properties for ActionResult.</span></span>

## <a name="properties"></a><span data-ttu-id="208e1-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="208e1-107">Properties</span></span>
|<span data-ttu-id="208e1-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="208e1-108">Property</span></span>|<span data-ttu-id="208e1-109">Тип</span><span class="sxs-lookup"><span data-stu-id="208e1-109">Type</span></span>|<span data-ttu-id="208e1-110">Описание</span><span class="sxs-lookup"><span data-stu-id="208e1-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="208e1-111">userId</span><span class="sxs-lookup"><span data-stu-id="208e1-111">userId</span></span>|<span data-ttu-id="208e1-112">String</span><span class="sxs-lookup"><span data-stu-id="208e1-112">String</span></span>|<span data-ttu-id="208e1-113">UserId, связанный с действием.</span><span class="sxs-lookup"><span data-stu-id="208e1-113">UserId associated with the action.</span></span>|
|<span data-ttu-id="208e1-114">Манажеддевицеид</span><span class="sxs-lookup"><span data-stu-id="208e1-114">managedDeviceId</span></span>|<span data-ttu-id="208e1-115">String</span><span class="sxs-lookup"><span data-stu-id="208e1-115">String</span></span>|<span data-ttu-id="208e1-116">DeviceId, связанный с действием.</span><span class="sxs-lookup"><span data-stu-id="208e1-116">DeviceId associated with the action.</span></span>|
|<span data-ttu-id="208e1-117">Тоталлиценсескаунт</span><span class="sxs-lookup"><span data-stu-id="208e1-117">totalLicensesCount</span></span>|<span data-ttu-id="208e1-118">Int32</span><span class="sxs-lookup"><span data-stu-id="208e1-118">Int32</span></span>|<span data-ttu-id="208e1-119">Количество лицензий, для которых была предпринята попытка отзыва.</span><span class="sxs-lookup"><span data-stu-id="208e1-119">A count of the number of licenses for which revoke was attempted.</span></span>|
|<span data-ttu-id="208e1-120">Фаиледлиценсескаунт</span><span class="sxs-lookup"><span data-stu-id="208e1-120">failedLicensesCount</span></span>|<span data-ttu-id="208e1-121">Int32</span><span class="sxs-lookup"><span data-stu-id="208e1-121">Int32</span></span>|<span data-ttu-id="208e1-122">Количество лицензий, для которых произошел сбой при отзыве.</span><span class="sxs-lookup"><span data-stu-id="208e1-122">A count of the number of licenses for which revoke failed.</span></span>|
|<span data-ttu-id="208e1-123">Актионфаилуререасон</span><span class="sxs-lookup"><span data-stu-id="208e1-123">actionFailureReason</span></span>|[<span data-ttu-id="208e1-124">Впптокенактионфаилуререасон</span><span class="sxs-lookup"><span data-stu-id="208e1-124">vppTokenActionFailureReason</span></span>](../resources/intune-shared-vpptokenactionfailurereason.md)|<span data-ttu-id="208e1-125">Причина сбоя действия "отзыв лицензий".</span><span class="sxs-lookup"><span data-stu-id="208e1-125">The reason for the revoke licenses action failure.</span></span> <span data-ttu-id="208e1-126">Возможные значения: `none`, `appleFailure`, `internalError`, `expiredVppToken`, `expiredApplePushNotificationCertificate`.</span><span class="sxs-lookup"><span data-stu-id="208e1-126">Possible values are: `none`, `appleFailure`, `internalError`, `expiredVppToken`, `expiredApplePushNotificationCertificate`.</span></span>|
|<span data-ttu-id="208e1-127">actionName</span><span class="sxs-lookup"><span data-stu-id="208e1-127">actionName</span></span>|<span data-ttu-id="208e1-128">String</span><span class="sxs-lookup"><span data-stu-id="208e1-128">String</span></span>|<span data-ttu-id="208e1-129">Название действия</span><span class="sxs-lookup"><span data-stu-id="208e1-129">Action name</span></span>|
|<span data-ttu-id="208e1-130">actionState</span><span class="sxs-lookup"><span data-stu-id="208e1-130">actionState</span></span>|[<span data-ttu-id="208e1-131">actionState</span><span class="sxs-lookup"><span data-stu-id="208e1-131">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="208e1-132">Состояние действия.</span><span class="sxs-lookup"><span data-stu-id="208e1-132">State of the action.</span></span> <span data-ttu-id="208e1-133">Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="208e1-133">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="208e1-134">startDateTime</span><span class="sxs-lookup"><span data-stu-id="208e1-134">startDateTime</span></span>|<span data-ttu-id="208e1-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="208e1-135">DateTimeOffset</span></span>|<span data-ttu-id="208e1-136">Время начала действия</span><span class="sxs-lookup"><span data-stu-id="208e1-136">Time the action was initiated</span></span>|
|<span data-ttu-id="208e1-137">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="208e1-137">lastUpdatedDateTime</span></span>|<span data-ttu-id="208e1-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="208e1-138">DateTimeOffset</span></span>|<span data-ttu-id="208e1-139">Время последнего обновления состояния действия</span><span class="sxs-lookup"><span data-stu-id="208e1-139">Time the action state was last updated</span></span>|

## <a name="relationships"></a><span data-ttu-id="208e1-140">Связи</span><span class="sxs-lookup"><span data-stu-id="208e1-140">Relationships</span></span>
<span data-ttu-id="208e1-141">Нет</span><span class="sxs-lookup"><span data-stu-id="208e1-141">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="208e1-142">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="208e1-142">JSON Representation</span></span>
<span data-ttu-id="208e1-143">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="208e1-143">Here is a JSON representation of the resource.</span></span>
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





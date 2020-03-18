---
title: Тип ресурса Иосвппаппревокелиценсесактионресулт
description: Определяет результаты действий в приложениях для iOS VPP, содержит унаследованные свойства для Актионресулт.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ebb4af4c9cd6b9f58a3e0ee341b7e43192094d29
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42798058"
---
# <a name="iosvppapprevokelicensesactionresult-resource-type"></a><span data-ttu-id="7f08a-103">Тип ресурса Иосвппаппревокелиценсесактионресулт</span><span class="sxs-lookup"><span data-stu-id="7f08a-103">iosVppAppRevokeLicensesActionResult resource type</span></span>

> <span data-ttu-id="7f08a-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7f08a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7f08a-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7f08a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7f08a-106">Определяет результаты действий в приложениях для iOS VPP, содержит унаследованные свойства для Актионресулт.</span><span class="sxs-lookup"><span data-stu-id="7f08a-106">Defines results for actions on iOS Vpp Apps, contains inherited properties for ActionResult.</span></span>

## <a name="properties"></a><span data-ttu-id="7f08a-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="7f08a-107">Properties</span></span>
|<span data-ttu-id="7f08a-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="7f08a-108">Property</span></span>|<span data-ttu-id="7f08a-109">Тип</span><span class="sxs-lookup"><span data-stu-id="7f08a-109">Type</span></span>|<span data-ttu-id="7f08a-110">Описание</span><span class="sxs-lookup"><span data-stu-id="7f08a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7f08a-111">userId</span><span class="sxs-lookup"><span data-stu-id="7f08a-111">userId</span></span>|<span data-ttu-id="7f08a-112">String</span><span class="sxs-lookup"><span data-stu-id="7f08a-112">String</span></span>|<span data-ttu-id="7f08a-113">UserId, связанный с действием.</span><span class="sxs-lookup"><span data-stu-id="7f08a-113">UserId associated with the action.</span></span>|
|<span data-ttu-id="7f08a-114">манажеддевицеид</span><span class="sxs-lookup"><span data-stu-id="7f08a-114">managedDeviceId</span></span>|<span data-ttu-id="7f08a-115">String</span><span class="sxs-lookup"><span data-stu-id="7f08a-115">String</span></span>|<span data-ttu-id="7f08a-116">DeviceId, связанный с действием.</span><span class="sxs-lookup"><span data-stu-id="7f08a-116">DeviceId associated with the action.</span></span>|
|<span data-ttu-id="7f08a-117">тоталлиценсескаунт</span><span class="sxs-lookup"><span data-stu-id="7f08a-117">totalLicensesCount</span></span>|<span data-ttu-id="7f08a-118">Int32</span><span class="sxs-lookup"><span data-stu-id="7f08a-118">Int32</span></span>|<span data-ttu-id="7f08a-119">Количество лицензий, для которых была предпринята попытка отзыва.</span><span class="sxs-lookup"><span data-stu-id="7f08a-119">A count of the number of licenses for which revoke was attempted.</span></span>|
|<span data-ttu-id="7f08a-120">фаиледлиценсескаунт</span><span class="sxs-lookup"><span data-stu-id="7f08a-120">failedLicensesCount</span></span>|<span data-ttu-id="7f08a-121">Int32</span><span class="sxs-lookup"><span data-stu-id="7f08a-121">Int32</span></span>|<span data-ttu-id="7f08a-122">Количество лицензий, для которых произошел сбой при отзыве.</span><span class="sxs-lookup"><span data-stu-id="7f08a-122">A count of the number of licenses for which revoke failed.</span></span>|
|<span data-ttu-id="7f08a-123">актионфаилуререасон</span><span class="sxs-lookup"><span data-stu-id="7f08a-123">actionFailureReason</span></span>|[<span data-ttu-id="7f08a-124">впптокенактионфаилуререасон</span><span class="sxs-lookup"><span data-stu-id="7f08a-124">vppTokenActionFailureReason</span></span>](../resources/intune-shared-vpptokenactionfailurereason.md)|<span data-ttu-id="7f08a-125">Причина сбоя действия "отзыв лицензий".</span><span class="sxs-lookup"><span data-stu-id="7f08a-125">The reason for the revoke licenses action failure.</span></span> <span data-ttu-id="7f08a-126">Возможные значения: `none`, `appleFailure`, `internalError`, `expiredVppToken`, `expiredApplePushNotificationCertificate`.</span><span class="sxs-lookup"><span data-stu-id="7f08a-126">Possible values are: `none`, `appleFailure`, `internalError`, `expiredVppToken`, `expiredApplePushNotificationCertificate`.</span></span>|
|<span data-ttu-id="7f08a-127">actionName</span><span class="sxs-lookup"><span data-stu-id="7f08a-127">actionName</span></span>|<span data-ttu-id="7f08a-128">String</span><span class="sxs-lookup"><span data-stu-id="7f08a-128">String</span></span>|<span data-ttu-id="7f08a-129">Название действия</span><span class="sxs-lookup"><span data-stu-id="7f08a-129">Action name</span></span>|
|<span data-ttu-id="7f08a-130">actionState</span><span class="sxs-lookup"><span data-stu-id="7f08a-130">actionState</span></span>|[<span data-ttu-id="7f08a-131">actionState</span><span class="sxs-lookup"><span data-stu-id="7f08a-131">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="7f08a-132">Состояние действия.</span><span class="sxs-lookup"><span data-stu-id="7f08a-132">State of the action.</span></span> <span data-ttu-id="7f08a-133">Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="7f08a-133">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="7f08a-134">startDateTime</span><span class="sxs-lookup"><span data-stu-id="7f08a-134">startDateTime</span></span>|<span data-ttu-id="7f08a-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7f08a-135">DateTimeOffset</span></span>|<span data-ttu-id="7f08a-136">Время начала действия</span><span class="sxs-lookup"><span data-stu-id="7f08a-136">Time the action was initiated</span></span>|
|<span data-ttu-id="7f08a-137">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="7f08a-137">lastUpdatedDateTime</span></span>|<span data-ttu-id="7f08a-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7f08a-138">DateTimeOffset</span></span>|<span data-ttu-id="7f08a-139">Время последнего обновления состояния действия</span><span class="sxs-lookup"><span data-stu-id="7f08a-139">Time the action state was last updated</span></span>|

## <a name="relationships"></a><span data-ttu-id="7f08a-140">Связи</span><span class="sxs-lookup"><span data-stu-id="7f08a-140">Relationships</span></span>
<span data-ttu-id="7f08a-141">Нет</span><span class="sxs-lookup"><span data-stu-id="7f08a-141">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7f08a-142">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7f08a-142">JSON Representation</span></span>
<span data-ttu-id="7f08a-143">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7f08a-143">Here is a JSON representation of the resource.</span></span>
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




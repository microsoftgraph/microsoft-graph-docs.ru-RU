---
title: Тип ресурса Иосвппаппревокелиценсесактионресулт
description: Определяет результаты действий в приложениях для iOS VPP, содержит унаследованные свойства для Актионресулт.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 16945bcb0043a07821803964b245319fb10b5c8a
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43458948"
---
# <a name="iosvppapprevokelicensesactionresult-resource-type"></a><span data-ttu-id="34c14-103">Тип ресурса Иосвппаппревокелиценсесактионресулт</span><span class="sxs-lookup"><span data-stu-id="34c14-103">iosVppAppRevokeLicensesActionResult resource type</span></span>

<span data-ttu-id="34c14-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="34c14-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="34c14-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="34c14-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="34c14-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="34c14-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="34c14-107">Определяет результаты действий в приложениях для iOS VPP, содержит унаследованные свойства для Актионресулт.</span><span class="sxs-lookup"><span data-stu-id="34c14-107">Defines results for actions on iOS Vpp Apps, contains inherited properties for ActionResult.</span></span>

## <a name="properties"></a><span data-ttu-id="34c14-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="34c14-108">Properties</span></span>
|<span data-ttu-id="34c14-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="34c14-109">Property</span></span>|<span data-ttu-id="34c14-110">Тип</span><span class="sxs-lookup"><span data-stu-id="34c14-110">Type</span></span>|<span data-ttu-id="34c14-111">Описание</span><span class="sxs-lookup"><span data-stu-id="34c14-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="34c14-112">userId</span><span class="sxs-lookup"><span data-stu-id="34c14-112">userId</span></span>|<span data-ttu-id="34c14-113">String</span><span class="sxs-lookup"><span data-stu-id="34c14-113">String</span></span>|<span data-ttu-id="34c14-114">UserId, связанный с действием.</span><span class="sxs-lookup"><span data-stu-id="34c14-114">UserId associated with the action.</span></span>|
|<span data-ttu-id="34c14-115">манажеддевицеид</span><span class="sxs-lookup"><span data-stu-id="34c14-115">managedDeviceId</span></span>|<span data-ttu-id="34c14-116">String</span><span class="sxs-lookup"><span data-stu-id="34c14-116">String</span></span>|<span data-ttu-id="34c14-117">DeviceId, связанный с действием.</span><span class="sxs-lookup"><span data-stu-id="34c14-117">DeviceId associated with the action.</span></span>|
|<span data-ttu-id="34c14-118">тоталлиценсескаунт</span><span class="sxs-lookup"><span data-stu-id="34c14-118">totalLicensesCount</span></span>|<span data-ttu-id="34c14-119">Int32</span><span class="sxs-lookup"><span data-stu-id="34c14-119">Int32</span></span>|<span data-ttu-id="34c14-120">Количество лицензий, для которых была предпринята попытка отзыва.</span><span class="sxs-lookup"><span data-stu-id="34c14-120">A count of the number of licenses for which revoke was attempted.</span></span>|
|<span data-ttu-id="34c14-121">фаиледлиценсескаунт</span><span class="sxs-lookup"><span data-stu-id="34c14-121">failedLicensesCount</span></span>|<span data-ttu-id="34c14-122">Int32</span><span class="sxs-lookup"><span data-stu-id="34c14-122">Int32</span></span>|<span data-ttu-id="34c14-123">Количество лицензий, для которых произошел сбой при отзыве.</span><span class="sxs-lookup"><span data-stu-id="34c14-123">A count of the number of licenses for which revoke failed.</span></span>|
|<span data-ttu-id="34c14-124">актионфаилуререасон</span><span class="sxs-lookup"><span data-stu-id="34c14-124">actionFailureReason</span></span>|[<span data-ttu-id="34c14-125">впптокенактионфаилуререасон</span><span class="sxs-lookup"><span data-stu-id="34c14-125">vppTokenActionFailureReason</span></span>](../resources/intune-shared-vpptokenactionfailurereason.md)|<span data-ttu-id="34c14-126">Причина сбоя действия "отзыв лицензий".</span><span class="sxs-lookup"><span data-stu-id="34c14-126">The reason for the revoke licenses action failure.</span></span> <span data-ttu-id="34c14-127">Возможные значения: `none`, `appleFailure`, `internalError`, `expiredVppToken`, `expiredApplePushNotificationCertificate`.</span><span class="sxs-lookup"><span data-stu-id="34c14-127">Possible values are: `none`, `appleFailure`, `internalError`, `expiredVppToken`, `expiredApplePushNotificationCertificate`.</span></span>|
|<span data-ttu-id="34c14-128">actionName</span><span class="sxs-lookup"><span data-stu-id="34c14-128">actionName</span></span>|<span data-ttu-id="34c14-129">String</span><span class="sxs-lookup"><span data-stu-id="34c14-129">String</span></span>|<span data-ttu-id="34c14-130">Название действия</span><span class="sxs-lookup"><span data-stu-id="34c14-130">Action name</span></span>|
|<span data-ttu-id="34c14-131">actionState</span><span class="sxs-lookup"><span data-stu-id="34c14-131">actionState</span></span>|[<span data-ttu-id="34c14-132">actionState</span><span class="sxs-lookup"><span data-stu-id="34c14-132">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="34c14-133">Состояние действия.</span><span class="sxs-lookup"><span data-stu-id="34c14-133">State of the action.</span></span> <span data-ttu-id="34c14-134">Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="34c14-134">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="34c14-135">startDateTime</span><span class="sxs-lookup"><span data-stu-id="34c14-135">startDateTime</span></span>|<span data-ttu-id="34c14-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="34c14-136">DateTimeOffset</span></span>|<span data-ttu-id="34c14-137">Время начала действия</span><span class="sxs-lookup"><span data-stu-id="34c14-137">Time the action was initiated</span></span>|
|<span data-ttu-id="34c14-138">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="34c14-138">lastUpdatedDateTime</span></span>|<span data-ttu-id="34c14-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="34c14-139">DateTimeOffset</span></span>|<span data-ttu-id="34c14-140">Время последнего обновления состояния действия</span><span class="sxs-lookup"><span data-stu-id="34c14-140">Time the action state was last updated</span></span>|

## <a name="relationships"></a><span data-ttu-id="34c14-141">Связи</span><span class="sxs-lookup"><span data-stu-id="34c14-141">Relationships</span></span>
<span data-ttu-id="34c14-142">Нет</span><span class="sxs-lookup"><span data-stu-id="34c14-142">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="34c14-143">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="34c14-143">JSON Representation</span></span>
<span data-ttu-id="34c14-144">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="34c14-144">Here is a JSON representation of the resource.</span></span>
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




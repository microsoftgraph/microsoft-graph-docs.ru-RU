---
title: Тип ресурса Иосвппаппревокелиценсесактионресулт
description: Определяет результаты действий в приложениях для iOS VPP, содержит унаследованные свойства для Актионресулт.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: eb297bff4c51a23076fb2d6ff2c4505be017989b
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36365953"
---
# <a name="iosvppapprevokelicensesactionresult-resource-type"></a><span data-ttu-id="fdc42-103">Тип ресурса Иосвппаппревокелиценсесактионресулт</span><span class="sxs-lookup"><span data-stu-id="fdc42-103">iosVppAppRevokeLicensesActionResult resource type</span></span>

> <span data-ttu-id="fdc42-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fdc42-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fdc42-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fdc42-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fdc42-106">Определяет результаты действий в приложениях для iOS VPP, содержит унаследованные свойства для Актионресулт.</span><span class="sxs-lookup"><span data-stu-id="fdc42-106">Defines results for actions on iOS Vpp Apps, contains inherited properties for ActionResult.</span></span>

## <a name="properties"></a><span data-ttu-id="fdc42-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="fdc42-107">Properties</span></span>
|<span data-ttu-id="fdc42-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="fdc42-108">Property</span></span>|<span data-ttu-id="fdc42-109">Тип</span><span class="sxs-lookup"><span data-stu-id="fdc42-109">Type</span></span>|<span data-ttu-id="fdc42-110">Описание</span><span class="sxs-lookup"><span data-stu-id="fdc42-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fdc42-111">userId</span><span class="sxs-lookup"><span data-stu-id="fdc42-111">userId</span></span>|<span data-ttu-id="fdc42-112">String</span><span class="sxs-lookup"><span data-stu-id="fdc42-112">String</span></span>|<span data-ttu-id="fdc42-113">UserId, связанный с действием.</span><span class="sxs-lookup"><span data-stu-id="fdc42-113">UserId associated with the action.</span></span>|
|<span data-ttu-id="fdc42-114">манажеддевицеид</span><span class="sxs-lookup"><span data-stu-id="fdc42-114">managedDeviceId</span></span>|<span data-ttu-id="fdc42-115">String</span><span class="sxs-lookup"><span data-stu-id="fdc42-115">String</span></span>|<span data-ttu-id="fdc42-116">DeviceId, связанный с действием.</span><span class="sxs-lookup"><span data-stu-id="fdc42-116">DeviceId associated with the action.</span></span>|
|<span data-ttu-id="fdc42-117">тоталлиценсескаунт</span><span class="sxs-lookup"><span data-stu-id="fdc42-117">totalLicensesCount</span></span>|<span data-ttu-id="fdc42-118">Int32</span><span class="sxs-lookup"><span data-stu-id="fdc42-118">Int32</span></span>|<span data-ttu-id="fdc42-119">Количество лицензий, для которых была предпринята попытка отзыва.</span><span class="sxs-lookup"><span data-stu-id="fdc42-119">A count of the number of licenses for which revoke was attempted.</span></span>|
|<span data-ttu-id="fdc42-120">фаиледлиценсескаунт</span><span class="sxs-lookup"><span data-stu-id="fdc42-120">failedLicensesCount</span></span>|<span data-ttu-id="fdc42-121">Int32</span><span class="sxs-lookup"><span data-stu-id="fdc42-121">Int32</span></span>|<span data-ttu-id="fdc42-122">Количество лицензий, для которых произошел сбой при отзыве.</span><span class="sxs-lookup"><span data-stu-id="fdc42-122">A count of the number of licenses for which revoke failed.</span></span>|
|<span data-ttu-id="fdc42-123">актионфаилуререасон</span><span class="sxs-lookup"><span data-stu-id="fdc42-123">actionFailureReason</span></span>|[<span data-ttu-id="fdc42-124">впптокенактионфаилуререасон</span><span class="sxs-lookup"><span data-stu-id="fdc42-124">vppTokenActionFailureReason</span></span>](../resources/intune-shared-vpptokenactionfailurereason.md)|<span data-ttu-id="fdc42-125">Причина сбоя действия "отзыв лицензий".</span><span class="sxs-lookup"><span data-stu-id="fdc42-125">The reason for the revoke licenses action failure.</span></span> <span data-ttu-id="fdc42-126">Возможные значения: `none`, `appleFailure`, `internalError`, `expiredVppToken`, `expiredApplePushNotificationCertificate`.</span><span class="sxs-lookup"><span data-stu-id="fdc42-126">Possible values are: `none`, `appleFailure`, `internalError`, `expiredVppToken`, `expiredApplePushNotificationCertificate`.</span></span>|
|<span data-ttu-id="fdc42-127">actionName</span><span class="sxs-lookup"><span data-stu-id="fdc42-127">actionName</span></span>|<span data-ttu-id="fdc42-128">String</span><span class="sxs-lookup"><span data-stu-id="fdc42-128">String</span></span>|<span data-ttu-id="fdc42-129">Название действия</span><span class="sxs-lookup"><span data-stu-id="fdc42-129">Action name</span></span>|
|<span data-ttu-id="fdc42-130">actionState</span><span class="sxs-lookup"><span data-stu-id="fdc42-130">actionState</span></span>|[<span data-ttu-id="fdc42-131">actionState</span><span class="sxs-lookup"><span data-stu-id="fdc42-131">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="fdc42-132">Состояние действия.</span><span class="sxs-lookup"><span data-stu-id="fdc42-132">State of the action.</span></span> <span data-ttu-id="fdc42-133">Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="fdc42-133">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="fdc42-134">startDateTime</span><span class="sxs-lookup"><span data-stu-id="fdc42-134">startDateTime</span></span>|<span data-ttu-id="fdc42-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fdc42-135">DateTimeOffset</span></span>|<span data-ttu-id="fdc42-136">Время начала действия</span><span class="sxs-lookup"><span data-stu-id="fdc42-136">Time the action was initiated</span></span>|
|<span data-ttu-id="fdc42-137">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="fdc42-137">lastUpdatedDateTime</span></span>|<span data-ttu-id="fdc42-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fdc42-138">DateTimeOffset</span></span>|<span data-ttu-id="fdc42-139">Время последнего обновления состояния действия</span><span class="sxs-lookup"><span data-stu-id="fdc42-139">Time the action state was last updated</span></span>|

## <a name="relationships"></a><span data-ttu-id="fdc42-140">Отношения</span><span class="sxs-lookup"><span data-stu-id="fdc42-140">Relationships</span></span>
<span data-ttu-id="fdc42-141">Нет</span><span class="sxs-lookup"><span data-stu-id="fdc42-141">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fdc42-142">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="fdc42-142">JSON Representation</span></span>
<span data-ttu-id="fdc42-143">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fdc42-143">Here is a JSON representation of the resource.</span></span>
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




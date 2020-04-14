---
title: Тип ресурса Макосвппаппревокелиценсесактионресулт
description: Определяет результаты для действий в приложениях MacOS VPP, содержит унаследованные свойства для Актионресулт.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 07cef42eab31c82e49a07abd4e85e933027eb93b
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43458823"
---
# <a name="macosvppapprevokelicensesactionresult-resource-type"></a><span data-ttu-id="a1b31-103">Тип ресурса Макосвппаппревокелиценсесактионресулт</span><span class="sxs-lookup"><span data-stu-id="a1b31-103">macOsVppAppRevokeLicensesActionResult resource type</span></span>

<span data-ttu-id="a1b31-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a1b31-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a1b31-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a1b31-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a1b31-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a1b31-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a1b31-107">Определяет результаты для действий в приложениях MacOS VPP, содержит унаследованные свойства для Актионресулт.</span><span class="sxs-lookup"><span data-stu-id="a1b31-107">Defines results for actions on MacOS Vpp Apps, contains inherited properties for ActionResult.</span></span>

## <a name="properties"></a><span data-ttu-id="a1b31-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="a1b31-108">Properties</span></span>
|<span data-ttu-id="a1b31-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="a1b31-109">Property</span></span>|<span data-ttu-id="a1b31-110">Тип</span><span class="sxs-lookup"><span data-stu-id="a1b31-110">Type</span></span>|<span data-ttu-id="a1b31-111">Описание</span><span class="sxs-lookup"><span data-stu-id="a1b31-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a1b31-112">userId</span><span class="sxs-lookup"><span data-stu-id="a1b31-112">userId</span></span>|<span data-ttu-id="a1b31-113">String</span><span class="sxs-lookup"><span data-stu-id="a1b31-113">String</span></span>|<span data-ttu-id="a1b31-114">UserId, связанный с действием.</span><span class="sxs-lookup"><span data-stu-id="a1b31-114">UserId associated with the action.</span></span>|
|<span data-ttu-id="a1b31-115">манажеддевицеид</span><span class="sxs-lookup"><span data-stu-id="a1b31-115">managedDeviceId</span></span>|<span data-ttu-id="a1b31-116">String</span><span class="sxs-lookup"><span data-stu-id="a1b31-116">String</span></span>|<span data-ttu-id="a1b31-117">DeviceId, связанный с действием.</span><span class="sxs-lookup"><span data-stu-id="a1b31-117">DeviceId associated with the action.</span></span>|
|<span data-ttu-id="a1b31-118">тоталлиценсескаунт</span><span class="sxs-lookup"><span data-stu-id="a1b31-118">totalLicensesCount</span></span>|<span data-ttu-id="a1b31-119">Int32</span><span class="sxs-lookup"><span data-stu-id="a1b31-119">Int32</span></span>|<span data-ttu-id="a1b31-120">Количество лицензий, для которых была предпринята попытка отзыва.</span><span class="sxs-lookup"><span data-stu-id="a1b31-120">A count of the number of licenses for which revoke was attempted.</span></span>|
|<span data-ttu-id="a1b31-121">фаиледлиценсескаунт</span><span class="sxs-lookup"><span data-stu-id="a1b31-121">failedLicensesCount</span></span>|<span data-ttu-id="a1b31-122">Int32</span><span class="sxs-lookup"><span data-stu-id="a1b31-122">Int32</span></span>|<span data-ttu-id="a1b31-123">Количество лицензий, для которых произошел сбой при отзыве.</span><span class="sxs-lookup"><span data-stu-id="a1b31-123">A count of the number of licenses for which revoke failed.</span></span>|
|<span data-ttu-id="a1b31-124">актионфаилуререасон</span><span class="sxs-lookup"><span data-stu-id="a1b31-124">actionFailureReason</span></span>|[<span data-ttu-id="a1b31-125">впптокенактионфаилуререасон</span><span class="sxs-lookup"><span data-stu-id="a1b31-125">vppTokenActionFailureReason</span></span>](../resources/intune-shared-vpptokenactionfailurereason.md)|<span data-ttu-id="a1b31-126">Причина сбоя действия "отзыв лицензий".</span><span class="sxs-lookup"><span data-stu-id="a1b31-126">The reason for the revoke licenses action failure.</span></span> <span data-ttu-id="a1b31-127">Возможные значения: `none`, `appleFailure`, `internalError`, `expiredVppToken`, `expiredApplePushNotificationCertificate`.</span><span class="sxs-lookup"><span data-stu-id="a1b31-127">Possible values are: `none`, `appleFailure`, `internalError`, `expiredVppToken`, `expiredApplePushNotificationCertificate`.</span></span>|
|<span data-ttu-id="a1b31-128">actionName</span><span class="sxs-lookup"><span data-stu-id="a1b31-128">actionName</span></span>|<span data-ttu-id="a1b31-129">String</span><span class="sxs-lookup"><span data-stu-id="a1b31-129">String</span></span>|<span data-ttu-id="a1b31-130">Название действия</span><span class="sxs-lookup"><span data-stu-id="a1b31-130">Action name</span></span>|
|<span data-ttu-id="a1b31-131">actionState</span><span class="sxs-lookup"><span data-stu-id="a1b31-131">actionState</span></span>|[<span data-ttu-id="a1b31-132">actionState</span><span class="sxs-lookup"><span data-stu-id="a1b31-132">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="a1b31-133">Состояние действия.</span><span class="sxs-lookup"><span data-stu-id="a1b31-133">State of the action.</span></span> <span data-ttu-id="a1b31-134">Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="a1b31-134">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="a1b31-135">startDateTime</span><span class="sxs-lookup"><span data-stu-id="a1b31-135">startDateTime</span></span>|<span data-ttu-id="a1b31-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a1b31-136">DateTimeOffset</span></span>|<span data-ttu-id="a1b31-137">Время начала действия</span><span class="sxs-lookup"><span data-stu-id="a1b31-137">Time the action was initiated</span></span>|
|<span data-ttu-id="a1b31-138">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="a1b31-138">lastUpdatedDateTime</span></span>|<span data-ttu-id="a1b31-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a1b31-139">DateTimeOffset</span></span>|<span data-ttu-id="a1b31-140">Время последнего обновления состояния действия</span><span class="sxs-lookup"><span data-stu-id="a1b31-140">Time the action state was last updated</span></span>|

## <a name="relationships"></a><span data-ttu-id="a1b31-141">Связи</span><span class="sxs-lookup"><span data-stu-id="a1b31-141">Relationships</span></span>
<span data-ttu-id="a1b31-142">Нет</span><span class="sxs-lookup"><span data-stu-id="a1b31-142">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a1b31-143">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a1b31-143">JSON Representation</span></span>
<span data-ttu-id="a1b31-144">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a1b31-144">Here is a JSON representation of the resource.</span></span>
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




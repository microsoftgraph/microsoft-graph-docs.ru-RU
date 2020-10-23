---
title: Тип ресурса Макосвппаппревокелиценсесактионресулт
description: Определяет результаты для действий в приложениях MacOS VPP, содержит унаследованные свойства для Актионресулт.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 97daa2d7c156664f359bc454067981b71c5e4d5b
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48707208"
---
# <a name="macosvppapprevokelicensesactionresult-resource-type"></a><span data-ttu-id="b6268-103">Тип ресурса Макосвппаппревокелиценсесактионресулт</span><span class="sxs-lookup"><span data-stu-id="b6268-103">macOsVppAppRevokeLicensesActionResult resource type</span></span>

<span data-ttu-id="b6268-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b6268-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b6268-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b6268-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b6268-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b6268-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b6268-107">Определяет результаты для действий в приложениях MacOS VPP, содержит унаследованные свойства для Актионресулт.</span><span class="sxs-lookup"><span data-stu-id="b6268-107">Defines results for actions on MacOS Vpp Apps, contains inherited properties for ActionResult.</span></span>

## <a name="properties"></a><span data-ttu-id="b6268-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="b6268-108">Properties</span></span>
|<span data-ttu-id="b6268-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="b6268-109">Property</span></span>|<span data-ttu-id="b6268-110">Тип</span><span class="sxs-lookup"><span data-stu-id="b6268-110">Type</span></span>|<span data-ttu-id="b6268-111">Описание</span><span class="sxs-lookup"><span data-stu-id="b6268-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b6268-112">userId</span><span class="sxs-lookup"><span data-stu-id="b6268-112">userId</span></span>|<span data-ttu-id="b6268-113">String</span><span class="sxs-lookup"><span data-stu-id="b6268-113">String</span></span>|<span data-ttu-id="b6268-114">UserId, связанный с действием.</span><span class="sxs-lookup"><span data-stu-id="b6268-114">UserId associated with the action.</span></span>|
|<span data-ttu-id="b6268-115">манажеддевицеид</span><span class="sxs-lookup"><span data-stu-id="b6268-115">managedDeviceId</span></span>|<span data-ttu-id="b6268-116">Строка</span><span class="sxs-lookup"><span data-stu-id="b6268-116">String</span></span>|<span data-ttu-id="b6268-117">DeviceId, связанный с действием.</span><span class="sxs-lookup"><span data-stu-id="b6268-117">DeviceId associated with the action.</span></span>|
|<span data-ttu-id="b6268-118">тоталлиценсескаунт</span><span class="sxs-lookup"><span data-stu-id="b6268-118">totalLicensesCount</span></span>|<span data-ttu-id="b6268-119">Int32</span><span class="sxs-lookup"><span data-stu-id="b6268-119">Int32</span></span>|<span data-ttu-id="b6268-120">Количество лицензий, для которых была предпринята попытка отзыва.</span><span class="sxs-lookup"><span data-stu-id="b6268-120">A count of the number of licenses for which revoke was attempted.</span></span>|
|<span data-ttu-id="b6268-121">фаиледлиценсескаунт</span><span class="sxs-lookup"><span data-stu-id="b6268-121">failedLicensesCount</span></span>|<span data-ttu-id="b6268-122">Int32</span><span class="sxs-lookup"><span data-stu-id="b6268-122">Int32</span></span>|<span data-ttu-id="b6268-123">Количество лицензий, для которых произошел сбой при отзыве.</span><span class="sxs-lookup"><span data-stu-id="b6268-123">A count of the number of licenses for which revoke failed.</span></span>|
|<span data-ttu-id="b6268-124">актионфаилуререасон</span><span class="sxs-lookup"><span data-stu-id="b6268-124">actionFailureReason</span></span>|[<span data-ttu-id="b6268-125">впптокенактионфаилуререасон</span><span class="sxs-lookup"><span data-stu-id="b6268-125">vppTokenActionFailureReason</span></span>](../resources/intune-shared-vpptokenactionfailurereason.md)|<span data-ttu-id="b6268-126">Причина сбоя действия "отзыв лицензий".</span><span class="sxs-lookup"><span data-stu-id="b6268-126">The reason for the revoke licenses action failure.</span></span> <span data-ttu-id="b6268-127">Возможные значения: `none`, `appleFailure`, `internalError`, `expiredVppToken`, `expiredApplePushNotificationCertificate`.</span><span class="sxs-lookup"><span data-stu-id="b6268-127">Possible values are: `none`, `appleFailure`, `internalError`, `expiredVppToken`, `expiredApplePushNotificationCertificate`.</span></span>|
|<span data-ttu-id="b6268-128">actionName</span><span class="sxs-lookup"><span data-stu-id="b6268-128">actionName</span></span>|<span data-ttu-id="b6268-129">String</span><span class="sxs-lookup"><span data-stu-id="b6268-129">String</span></span>|<span data-ttu-id="b6268-130">Название действия</span><span class="sxs-lookup"><span data-stu-id="b6268-130">Action name</span></span>|
|<span data-ttu-id="b6268-131">actionState</span><span class="sxs-lookup"><span data-stu-id="b6268-131">actionState</span></span>|[<span data-ttu-id="b6268-132">actionState</span><span class="sxs-lookup"><span data-stu-id="b6268-132">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="b6268-133">Состояние действия.</span><span class="sxs-lookup"><span data-stu-id="b6268-133">State of the action.</span></span> <span data-ttu-id="b6268-134">Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="b6268-134">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="b6268-135">startDateTime</span><span class="sxs-lookup"><span data-stu-id="b6268-135">startDateTime</span></span>|<span data-ttu-id="b6268-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b6268-136">DateTimeOffset</span></span>|<span data-ttu-id="b6268-137">Время начала действия</span><span class="sxs-lookup"><span data-stu-id="b6268-137">Time the action was initiated</span></span>|
|<span data-ttu-id="b6268-138">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="b6268-138">lastUpdatedDateTime</span></span>|<span data-ttu-id="b6268-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b6268-139">DateTimeOffset</span></span>|<span data-ttu-id="b6268-140">Время последнего обновления состояния действия</span><span class="sxs-lookup"><span data-stu-id="b6268-140">Time the action state was last updated</span></span>|

## <a name="relationships"></a><span data-ttu-id="b6268-141">Связи</span><span class="sxs-lookup"><span data-stu-id="b6268-141">Relationships</span></span>
<span data-ttu-id="b6268-142">Нет</span><span class="sxs-lookup"><span data-stu-id="b6268-142">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b6268-143">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b6268-143">JSON Representation</span></span>
<span data-ttu-id="b6268-144">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b6268-144">Here is a JSON representation of the resource.</span></span>
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






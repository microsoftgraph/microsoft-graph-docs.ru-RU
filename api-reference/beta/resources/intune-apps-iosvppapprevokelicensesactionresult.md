---
title: Тип ресурса iosVppAppRevokeLicensesActionResult
description: Определяет результаты для действий на iOS Vpp приложений, содержащий наследуемые свойства для ActionResult.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 1f64f2df709d5332be46dd76216b1a1457d27a61
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29418906"
---
# <a name="iosvppapprevokelicensesactionresult-resource-type"></a><span data-ttu-id="029d9-103">Тип ресурса iosVppAppRevokeLicensesActionResult</span><span class="sxs-lookup"><span data-stu-id="029d9-103">iosVppAppRevokeLicensesActionResult resource type</span></span>

> <span data-ttu-id="029d9-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="029d9-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="029d9-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="029d9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="029d9-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="029d9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="029d9-107">Определяет результаты для действий на iOS Vpp приложений, содержащий наследуемые свойства для ActionResult.</span><span class="sxs-lookup"><span data-stu-id="029d9-107">Defines results for actions on iOS Vpp Apps, contains inherited properties for ActionResult.</span></span>

## <a name="properties"></a><span data-ttu-id="029d9-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="029d9-108">Properties</span></span>
|<span data-ttu-id="029d9-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="029d9-109">Property</span></span>|<span data-ttu-id="029d9-110">Тип</span><span class="sxs-lookup"><span data-stu-id="029d9-110">Type</span></span>|<span data-ttu-id="029d9-111">Описание</span><span class="sxs-lookup"><span data-stu-id="029d9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="029d9-112">userId</span><span class="sxs-lookup"><span data-stu-id="029d9-112">userId</span></span>|<span data-ttu-id="029d9-113">String</span><span class="sxs-lookup"><span data-stu-id="029d9-113">String</span></span>|<span data-ttu-id="029d9-114">Идентификатор пользователя, связанные с действием.</span><span class="sxs-lookup"><span data-stu-id="029d9-114">UserId associated with the action.</span></span>|
|<span data-ttu-id="029d9-115">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="029d9-115">managedDeviceId</span></span>|<span data-ttu-id="029d9-116">String</span><span class="sxs-lookup"><span data-stu-id="029d9-116">String</span></span>|<span data-ttu-id="029d9-117">DeviceId, связанные с действием.</span><span class="sxs-lookup"><span data-stu-id="029d9-117">DeviceId associated with the action.</span></span>|
|<span data-ttu-id="029d9-118">totalLicensesCount</span><span class="sxs-lookup"><span data-stu-id="029d9-118">totalLicensesCount</span></span>|<span data-ttu-id="029d9-119">Int32</span><span class="sxs-lookup"><span data-stu-id="029d9-119">Int32</span></span>|<span data-ttu-id="029d9-120">Подсчет числа лицензий, для которых осуществляется попытка revoke.</span><span class="sxs-lookup"><span data-stu-id="029d9-120">A count of the number of licenses for which revoke was attempted.</span></span>|
|<span data-ttu-id="029d9-121">failedLicensesCount</span><span class="sxs-lookup"><span data-stu-id="029d9-121">failedLicensesCount</span></span>|<span data-ttu-id="029d9-122">Int32</span><span class="sxs-lookup"><span data-stu-id="029d9-122">Int32</span></span>|<span data-ttu-id="029d9-123">Подсчет числа лицензий, для которых не удалось revoke.</span><span class="sxs-lookup"><span data-stu-id="029d9-123">A count of the number of licenses for which revoke failed.</span></span>|
|<span data-ttu-id="029d9-124">actionFailureReason</span><span class="sxs-lookup"><span data-stu-id="029d9-124">actionFailureReason</span></span>|[<span data-ttu-id="029d9-125">vppTokenActionFailureReason</span><span class="sxs-lookup"><span data-stu-id="029d9-125">vppTokenActionFailureReason</span></span>](../resources/intune-shared-vpptokenactionfailurereason.md)|<span data-ttu-id="029d9-126">Причина ошибки действие revoke лицензий.</span><span class="sxs-lookup"><span data-stu-id="029d9-126">The reason for the revoke licenses action failure.</span></span> <span data-ttu-id="029d9-127">Возможные значения: `none`, `appleFailure`, `internalError`, `expiredVppToken`, `expiredApplePushNotificationCertificate`.</span><span class="sxs-lookup"><span data-stu-id="029d9-127">Possible values are: `none`, `appleFailure`, `internalError`, `expiredVppToken`, `expiredApplePushNotificationCertificate`.</span></span>|
|<span data-ttu-id="029d9-128">actionName</span><span class="sxs-lookup"><span data-stu-id="029d9-128">actionName</span></span>|<span data-ttu-id="029d9-129">String</span><span class="sxs-lookup"><span data-stu-id="029d9-129">String</span></span>|<span data-ttu-id="029d9-130">Название действия</span><span class="sxs-lookup"><span data-stu-id="029d9-130">Action name</span></span>|
|<span data-ttu-id="029d9-131">actionState</span><span class="sxs-lookup"><span data-stu-id="029d9-131">actionState</span></span>|[<span data-ttu-id="029d9-132">actionState</span><span class="sxs-lookup"><span data-stu-id="029d9-132">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="029d9-133">Состояние действия.</span><span class="sxs-lookup"><span data-stu-id="029d9-133">State of the action.</span></span> <span data-ttu-id="029d9-134">Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="029d9-134">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="029d9-135">startDateTime</span><span class="sxs-lookup"><span data-stu-id="029d9-135">startDateTime</span></span>|<span data-ttu-id="029d9-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="029d9-136">DateTimeOffset</span></span>|<span data-ttu-id="029d9-137">Время начала действия</span><span class="sxs-lookup"><span data-stu-id="029d9-137">Time the action was initiated</span></span>|
|<span data-ttu-id="029d9-138">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="029d9-138">lastUpdatedDateTime</span></span>|<span data-ttu-id="029d9-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="029d9-139">DateTimeOffset</span></span>|<span data-ttu-id="029d9-140">Время последнего обновления состояния действия</span><span class="sxs-lookup"><span data-stu-id="029d9-140">Time the action state was last updated</span></span>|

## <a name="relationships"></a><span data-ttu-id="029d9-141">Связи</span><span class="sxs-lookup"><span data-stu-id="029d9-141">Relationships</span></span>
<span data-ttu-id="029d9-142">Нет</span><span class="sxs-lookup"><span data-stu-id="029d9-142">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="029d9-143">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="029d9-143">JSON Representation</span></span>
<span data-ttu-id="029d9-144">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="029d9-144">Here is a JSON representation of the resource.</span></span>
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





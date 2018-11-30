---
title: Тип ресурса iosVppAppRevokeLicensesActionResult
description: Определяет результаты для действий на iOS Vpp приложений, содержащий наследуемые свойства для ActionResult.
ms.openlocfilehash: 1c6c1486d63ba5ce7c866dc2697d1a3eb2ee8e38
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27081561"
---
# <a name="iosvppapprevokelicensesactionresult-resource-type"></a><span data-ttu-id="a8390-103">Тип ресурса iosVppAppRevokeLicensesActionResult</span><span class="sxs-lookup"><span data-stu-id="a8390-103">iosVppAppRevokeLicensesActionResult resource type</span></span>

> <span data-ttu-id="a8390-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="a8390-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a8390-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a8390-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a8390-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="a8390-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a8390-107">Определяет результаты для действий на iOS Vpp приложений, содержащий наследуемые свойства для ActionResult.</span><span class="sxs-lookup"><span data-stu-id="a8390-107">Defines results for actions on iOS Vpp Apps, contains inherited properties for ActionResult.</span></span>
## <a name="properties"></a><span data-ttu-id="a8390-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="a8390-108">Properties</span></span>
|<span data-ttu-id="a8390-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="a8390-109">Property</span></span>|<span data-ttu-id="a8390-110">Тип</span><span class="sxs-lookup"><span data-stu-id="a8390-110">Type</span></span>|<span data-ttu-id="a8390-111">Description</span><span class="sxs-lookup"><span data-stu-id="a8390-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a8390-112">userId</span><span class="sxs-lookup"><span data-stu-id="a8390-112">userId</span></span>|<span data-ttu-id="a8390-113">String</span><span class="sxs-lookup"><span data-stu-id="a8390-113">String</span></span>|<span data-ttu-id="a8390-114">Идентификатор пользователя, связанные с действием.</span><span class="sxs-lookup"><span data-stu-id="a8390-114">UserId associated with the action.</span></span>|
|<span data-ttu-id="a8390-115">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="a8390-115">managedDeviceId</span></span>|<span data-ttu-id="a8390-116">String</span><span class="sxs-lookup"><span data-stu-id="a8390-116">String</span></span>|<span data-ttu-id="a8390-117">DeviceId, связанные с действием.</span><span class="sxs-lookup"><span data-stu-id="a8390-117">DeviceId associated with the action.</span></span>|
|<span data-ttu-id="a8390-118">totalLicensesCount</span><span class="sxs-lookup"><span data-stu-id="a8390-118">totalLicensesCount</span></span>|<span data-ttu-id="a8390-119">Int32</span><span class="sxs-lookup"><span data-stu-id="a8390-119">Int32</span></span>|<span data-ttu-id="a8390-120">Подсчет числа лицензий, для которых осуществляется попытка revoke.</span><span class="sxs-lookup"><span data-stu-id="a8390-120">A count of the number of licenses for which revoke was attempted.</span></span>|
|<span data-ttu-id="a8390-121">failedLicensesCount</span><span class="sxs-lookup"><span data-stu-id="a8390-121">failedLicensesCount</span></span>|<span data-ttu-id="a8390-122">Int32</span><span class="sxs-lookup"><span data-stu-id="a8390-122">Int32</span></span>|<span data-ttu-id="a8390-123">Подсчет числа лицензий, для которых не удалось revoke.</span><span class="sxs-lookup"><span data-stu-id="a8390-123">A count of the number of licenses for which revoke failed.</span></span>|
|<span data-ttu-id="a8390-124">actionFailureReason</span><span class="sxs-lookup"><span data-stu-id="a8390-124">actionFailureReason</span></span>|[<span data-ttu-id="a8390-125">vppTokenActionFailureReason</span><span class="sxs-lookup"><span data-stu-id="a8390-125">vppTokenActionFailureReason</span></span>](../resources/intune-shared-vpptokenactionfailurereason.md)|<span data-ttu-id="a8390-126">Причина ошибки действие revoke лицензий.</span><span class="sxs-lookup"><span data-stu-id="a8390-126">The reason for the revoke licenses action failure.</span></span> <span data-ttu-id="a8390-127">Возможные значения: `none`, `appleFailure`, `internalError`, `expiredVppToken`, `expiredApplePushNotificationCertificate`.</span><span class="sxs-lookup"><span data-stu-id="a8390-127">Possible values are: `none`, `appleFailure`, `internalError`, `expiredVppToken`, `expiredApplePushNotificationCertificate`.</span></span>|
|<span data-ttu-id="a8390-128">actionName</span><span class="sxs-lookup"><span data-stu-id="a8390-128">actionName</span></span>|<span data-ttu-id="a8390-129">String</span><span class="sxs-lookup"><span data-stu-id="a8390-129">String</span></span>|<span data-ttu-id="a8390-130">Название действия</span><span class="sxs-lookup"><span data-stu-id="a8390-130">Action name</span></span>|
|<span data-ttu-id="a8390-131">actionState</span><span class="sxs-lookup"><span data-stu-id="a8390-131">actionState</span></span>|[<span data-ttu-id="a8390-132">actionState</span><span class="sxs-lookup"><span data-stu-id="a8390-132">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="a8390-133">Состояние действия.</span><span class="sxs-lookup"><span data-stu-id="a8390-133">State of the action.</span></span> <span data-ttu-id="a8390-134">Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="a8390-134">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="a8390-135">startDateTime</span><span class="sxs-lookup"><span data-stu-id="a8390-135">startDateTime</span></span>|<span data-ttu-id="a8390-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a8390-136">DateTimeOffset</span></span>|<span data-ttu-id="a8390-137">Время начала действия</span><span class="sxs-lookup"><span data-stu-id="a8390-137">Time the action was initiated</span></span>|
|<span data-ttu-id="a8390-138">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="a8390-138">lastUpdatedDateTime</span></span>|<span data-ttu-id="a8390-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a8390-139">DateTimeOffset</span></span>|<span data-ttu-id="a8390-140">Время последнего обновления состояния действия</span><span class="sxs-lookup"><span data-stu-id="a8390-140">Time the action state was last updated</span></span>|

## <a name="relationships"></a><span data-ttu-id="a8390-141">Связи</span><span class="sxs-lookup"><span data-stu-id="a8390-141">Relationships</span></span>
<span data-ttu-id="a8390-142">Нет</span><span class="sxs-lookup"><span data-stu-id="a8390-142">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="a8390-143">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a8390-143">JSON Representation</span></span>
<span data-ttu-id="a8390-144">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a8390-144">Here is a JSON representation of the resource.</span></span>
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






---
title: Тип ресурса iosVppAppRevokeLicensesActionResult
description: Определяет результаты для действий на iOS Vpp приложений, содержащий наследуемые свойства для ActionResult.
localization_priority: Normal
ms.openlocfilehash: 8ed57465e263245cfc18ca22899c2142d949855d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27842086"
---
# <a name="iosvppapprevokelicensesactionresult-resource-type"></a><span data-ttu-id="6eb18-103">Тип ресурса iosVppAppRevokeLicensesActionResult</span><span class="sxs-lookup"><span data-stu-id="6eb18-103">iosVppAppRevokeLicensesActionResult resource type</span></span>

> <span data-ttu-id="6eb18-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="6eb18-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6eb18-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6eb18-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6eb18-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="6eb18-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6eb18-107">Определяет результаты для действий на iOS Vpp приложений, содержащий наследуемые свойства для ActionResult.</span><span class="sxs-lookup"><span data-stu-id="6eb18-107">Defines results for actions on iOS Vpp Apps, contains inherited properties for ActionResult.</span></span>
## <a name="properties"></a><span data-ttu-id="6eb18-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="6eb18-108">Properties</span></span>
|<span data-ttu-id="6eb18-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="6eb18-109">Property</span></span>|<span data-ttu-id="6eb18-110">Тип</span><span class="sxs-lookup"><span data-stu-id="6eb18-110">Type</span></span>|<span data-ttu-id="6eb18-111">Описание</span><span class="sxs-lookup"><span data-stu-id="6eb18-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6eb18-112">userId</span><span class="sxs-lookup"><span data-stu-id="6eb18-112">userId</span></span>|<span data-ttu-id="6eb18-113">String</span><span class="sxs-lookup"><span data-stu-id="6eb18-113">String</span></span>|<span data-ttu-id="6eb18-114">Идентификатор пользователя, связанные с действием.</span><span class="sxs-lookup"><span data-stu-id="6eb18-114">UserId associated with the action.</span></span>|
|<span data-ttu-id="6eb18-115">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="6eb18-115">managedDeviceId</span></span>|<span data-ttu-id="6eb18-116">Строка</span><span class="sxs-lookup"><span data-stu-id="6eb18-116">String</span></span>|<span data-ttu-id="6eb18-117">DeviceId, связанные с действием.</span><span class="sxs-lookup"><span data-stu-id="6eb18-117">DeviceId associated with the action.</span></span>|
|<span data-ttu-id="6eb18-118">totalLicensesCount</span><span class="sxs-lookup"><span data-stu-id="6eb18-118">totalLicensesCount</span></span>|<span data-ttu-id="6eb18-119">Int32</span><span class="sxs-lookup"><span data-stu-id="6eb18-119">Int32</span></span>|<span data-ttu-id="6eb18-120">Подсчет числа лицензий, для которых осуществляется попытка revoke.</span><span class="sxs-lookup"><span data-stu-id="6eb18-120">A count of the number of licenses for which revoke was attempted.</span></span>|
|<span data-ttu-id="6eb18-121">failedLicensesCount</span><span class="sxs-lookup"><span data-stu-id="6eb18-121">failedLicensesCount</span></span>|<span data-ttu-id="6eb18-122">Int32</span><span class="sxs-lookup"><span data-stu-id="6eb18-122">Int32</span></span>|<span data-ttu-id="6eb18-123">Подсчет числа лицензий, для которых не удалось revoke.</span><span class="sxs-lookup"><span data-stu-id="6eb18-123">A count of the number of licenses for which revoke failed.</span></span>|
|<span data-ttu-id="6eb18-124">actionFailureReason</span><span class="sxs-lookup"><span data-stu-id="6eb18-124">actionFailureReason</span></span>|[<span data-ttu-id="6eb18-125">vppTokenActionFailureReason</span><span class="sxs-lookup"><span data-stu-id="6eb18-125">vppTokenActionFailureReason</span></span>](../resources/intune-shared-vpptokenactionfailurereason.md)|<span data-ttu-id="6eb18-126">Причина ошибки действие revoke лицензий.</span><span class="sxs-lookup"><span data-stu-id="6eb18-126">The reason for the revoke licenses action failure.</span></span> <span data-ttu-id="6eb18-127">Возможные значения: `none`, `appleFailure`, `internalError`, `expiredVppToken`, `expiredApplePushNotificationCertificate`.</span><span class="sxs-lookup"><span data-stu-id="6eb18-127">Possible values are: `none`, `appleFailure`, `internalError`, `expiredVppToken`, `expiredApplePushNotificationCertificate`.</span></span>|
|<span data-ttu-id="6eb18-128">actionName</span><span class="sxs-lookup"><span data-stu-id="6eb18-128">actionName</span></span>|<span data-ttu-id="6eb18-129">String</span><span class="sxs-lookup"><span data-stu-id="6eb18-129">String</span></span>|<span data-ttu-id="6eb18-130">Название действия</span><span class="sxs-lookup"><span data-stu-id="6eb18-130">Action name</span></span>|
|<span data-ttu-id="6eb18-131">actionState</span><span class="sxs-lookup"><span data-stu-id="6eb18-131">actionState</span></span>|[<span data-ttu-id="6eb18-132">actionState</span><span class="sxs-lookup"><span data-stu-id="6eb18-132">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="6eb18-133">Состояние действия.</span><span class="sxs-lookup"><span data-stu-id="6eb18-133">State of the action.</span></span> <span data-ttu-id="6eb18-134">Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="6eb18-134">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="6eb18-135">startDateTime</span><span class="sxs-lookup"><span data-stu-id="6eb18-135">startDateTime</span></span>|<span data-ttu-id="6eb18-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6eb18-136">DateTimeOffset</span></span>|<span data-ttu-id="6eb18-137">Время начала действия</span><span class="sxs-lookup"><span data-stu-id="6eb18-137">Time the action was initiated</span></span>|
|<span data-ttu-id="6eb18-138">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="6eb18-138">lastUpdatedDateTime</span></span>|<span data-ttu-id="6eb18-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6eb18-139">DateTimeOffset</span></span>|<span data-ttu-id="6eb18-140">Время последнего обновления состояния действия</span><span class="sxs-lookup"><span data-stu-id="6eb18-140">Time the action state was last updated</span></span>|

## <a name="relationships"></a><span data-ttu-id="6eb18-141">Связи</span><span class="sxs-lookup"><span data-stu-id="6eb18-141">Relationships</span></span>
<span data-ttu-id="6eb18-142">Нет</span><span class="sxs-lookup"><span data-stu-id="6eb18-142">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="6eb18-143">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6eb18-143">JSON Representation</span></span>
<span data-ttu-id="6eb18-144">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6eb18-144">Here is a JSON representation of the resource.</span></span>
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






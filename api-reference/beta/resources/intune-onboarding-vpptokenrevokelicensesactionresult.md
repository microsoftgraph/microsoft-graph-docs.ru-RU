---
title: Тип ресурса vppTokenRevokeLicensesActionResult
description: Состояние действия лицензий revoke выполнить на маркер покупки программы корпоративного Apple.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 75c75c6b8bcdc06ede0f71b19956155becc4d478
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29418227"
---
# <a name="vpptokenrevokelicensesactionresult-resource-type"></a><span data-ttu-id="bd118-103">Тип ресурса vppTokenRevokeLicensesActionResult</span><span class="sxs-lookup"><span data-stu-id="bd118-103">vppTokenRevokeLicensesActionResult resource type</span></span>

> <span data-ttu-id="bd118-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="bd118-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="bd118-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bd118-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bd118-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bd118-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bd118-107">Состояние действия лицензий revoke выполнить на маркер покупки программы корпоративного Apple.</span><span class="sxs-lookup"><span data-stu-id="bd118-107">The status of the revoke licenses action performed on the Apple Volume Purchase Program token.</span></span>


<span data-ttu-id="bd118-108">Наследуется от [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="bd118-108">Inherits from [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="bd118-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="bd118-109">Properties</span></span>
|<span data-ttu-id="bd118-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="bd118-110">Property</span></span>|<span data-ttu-id="bd118-111">Тип</span><span class="sxs-lookup"><span data-stu-id="bd118-111">Type</span></span>|<span data-ttu-id="bd118-112">Описание</span><span class="sxs-lookup"><span data-stu-id="bd118-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bd118-113">actionName</span><span class="sxs-lookup"><span data-stu-id="bd118-113">actionName</span></span>|<span data-ttu-id="bd118-114">String</span><span class="sxs-lookup"><span data-stu-id="bd118-114">String</span></span>|<span data-ttu-id="bd118-115">Имя действия унаследованные от [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="bd118-115">Action name Inherited from [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span></span>|
|<span data-ttu-id="bd118-116">actionState</span><span class="sxs-lookup"><span data-stu-id="bd118-116">actionState</span></span>|[<span data-ttu-id="bd118-117">actionState</span><span class="sxs-lookup"><span data-stu-id="bd118-117">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="bd118-118">Состояние действие унаследованные от [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="bd118-118">State of the action Inherited from [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md).</span></span> <span data-ttu-id="bd118-119">Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="bd118-119">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="bd118-120">startDateTime</span><span class="sxs-lookup"><span data-stu-id="bd118-120">startDateTime</span></span>|<span data-ttu-id="bd118-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bd118-121">DateTimeOffset</span></span>|<span data-ttu-id="bd118-122">Время началось наследуется от [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="bd118-122">Time the action was initiated Inherited from [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span></span>|
|<span data-ttu-id="bd118-123">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="bd118-123">lastUpdatedDateTime</span></span>|<span data-ttu-id="bd118-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bd118-124">DateTimeOffset</span></span>|<span data-ttu-id="bd118-125">Время последнего состояния действия обновления унаследованные от [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="bd118-125">Time the action state was last updated Inherited from [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span></span>|
|<span data-ttu-id="bd118-126">totalLicensesCount</span><span class="sxs-lookup"><span data-stu-id="bd118-126">totalLicensesCount</span></span>|<span data-ttu-id="bd118-127">Int32</span><span class="sxs-lookup"><span data-stu-id="bd118-127">Int32</span></span>|<span data-ttu-id="bd118-128">Подсчет числа лицензий, которые были пытались отменить.</span><span class="sxs-lookup"><span data-stu-id="bd118-128">A count of the number of licenses that were attempted to revoke.</span></span>|
|<span data-ttu-id="bd118-129">failedLicensesCount</span><span class="sxs-lookup"><span data-stu-id="bd118-129">failedLicensesCount</span></span>|<span data-ttu-id="bd118-130">Int32</span><span class="sxs-lookup"><span data-stu-id="bd118-130">Int32</span></span>|<span data-ttu-id="bd118-131">Подсчет числа лицензий, которые не удалось отозвать.</span><span class="sxs-lookup"><span data-stu-id="bd118-131">A count of the number of licenses that failed to revoke.</span></span>|
|<span data-ttu-id="bd118-132">actionFailureReason</span><span class="sxs-lookup"><span data-stu-id="bd118-132">actionFailureReason</span></span>|[<span data-ttu-id="bd118-133">vppTokenActionFailureReason</span><span class="sxs-lookup"><span data-stu-id="bd118-133">vppTokenActionFailureReason</span></span>](../resources/intune-shared-vpptokenactionfailurereason.md)|<span data-ttu-id="bd118-134">Причина ошибки действие revoke лицензий.</span><span class="sxs-lookup"><span data-stu-id="bd118-134">The reason for the revoke licenses action failure.</span></span> <span data-ttu-id="bd118-135">Возможные значения: `none`, `appleFailure`, `internalError`, `expiredVppToken`, `expiredApplePushNotificationCertificate`.</span><span class="sxs-lookup"><span data-stu-id="bd118-135">Possible values are: `none`, `appleFailure`, `internalError`, `expiredVppToken`, `expiredApplePushNotificationCertificate`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bd118-136">Отношения</span><span class="sxs-lookup"><span data-stu-id="bd118-136">Relationships</span></span>
<span data-ttu-id="bd118-137">Нет</span><span class="sxs-lookup"><span data-stu-id="bd118-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bd118-138">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bd118-138">JSON Representation</span></span>
<span data-ttu-id="bd118-139">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bd118-139">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.vppTokenRevokeLicensesActionResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vppTokenRevokeLicensesActionResult",
  "actionName": "String",
  "actionState": "String",
  "startDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)",
  "totalLicensesCount": 1024,
  "failedLicensesCount": 1024,
  "actionFailureReason": "String"
}
```





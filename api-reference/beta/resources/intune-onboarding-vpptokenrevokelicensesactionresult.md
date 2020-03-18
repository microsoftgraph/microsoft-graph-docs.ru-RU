---
title: Тип ресурса Впптокенревокелиценсесактионресулт
description: Состояние действия отзыва лицензий, выполняемого в токене Apple Volume Purchase Program.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: d2ec896504435c644767af1ff04a74f4eaf4aa17
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42777504"
---
# <a name="vpptokenrevokelicensesactionresult-resource-type"></a><span data-ttu-id="bd9e0-103">Тип ресурса Впптокенревокелиценсесактионресулт</span><span class="sxs-lookup"><span data-stu-id="bd9e0-103">vppTokenRevokeLicensesActionResult resource type</span></span>

> <span data-ttu-id="bd9e0-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bd9e0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bd9e0-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bd9e0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bd9e0-106">Состояние действия отзыва лицензий, выполняемого в токене Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="bd9e0-106">The status of the revoke licenses action performed on the Apple Volume Purchase Program token.</span></span>


<span data-ttu-id="bd9e0-107">Наследуется от [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="bd9e0-107">Inherits from [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="bd9e0-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="bd9e0-108">Properties</span></span>
|<span data-ttu-id="bd9e0-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="bd9e0-109">Property</span></span>|<span data-ttu-id="bd9e0-110">Тип</span><span class="sxs-lookup"><span data-stu-id="bd9e0-110">Type</span></span>|<span data-ttu-id="bd9e0-111">Описание</span><span class="sxs-lookup"><span data-stu-id="bd9e0-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bd9e0-112">actionName</span><span class="sxs-lookup"><span data-stu-id="bd9e0-112">actionName</span></span>|<span data-ttu-id="bd9e0-113">String</span><span class="sxs-lookup"><span data-stu-id="bd9e0-113">String</span></span>|<span data-ttu-id="bd9e0-114">Имя действия наследуется от [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="bd9e0-114">Action name Inherited from [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span></span>|
|<span data-ttu-id="bd9e0-115">actionState</span><span class="sxs-lookup"><span data-stu-id="bd9e0-115">actionState</span></span>|[<span data-ttu-id="bd9e0-116">actionState</span><span class="sxs-lookup"><span data-stu-id="bd9e0-116">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="bd9e0-117">Состояние действия, унаследованного от [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="bd9e0-117">State of the action Inherited from [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md).</span></span> <span data-ttu-id="bd9e0-118">Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="bd9e0-118">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="bd9e0-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="bd9e0-119">startDateTime</span></span>|<span data-ttu-id="bd9e0-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bd9e0-120">DateTimeOffset</span></span>|<span data-ttu-id="bd9e0-121">Время начала действия, унаследованное от [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="bd9e0-121">Time the action was initiated Inherited from [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span></span>|
|<span data-ttu-id="bd9e0-122">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="bd9e0-122">lastUpdatedDateTime</span></span>|<span data-ttu-id="bd9e0-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bd9e0-123">DateTimeOffset</span></span>|<span data-ttu-id="bd9e0-124">Время последнего обновления состояния действия, унаследованного от [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="bd9e0-124">Time the action state was last updated Inherited from [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span></span>|
|<span data-ttu-id="bd9e0-125">тоталлиценсескаунт</span><span class="sxs-lookup"><span data-stu-id="bd9e0-125">totalLicensesCount</span></span>|<span data-ttu-id="bd9e0-126">Int32</span><span class="sxs-lookup"><span data-stu-id="bd9e0-126">Int32</span></span>|<span data-ttu-id="bd9e0-127">Число неудачных попыток отзыва лицензий.</span><span class="sxs-lookup"><span data-stu-id="bd9e0-127">A count of the number of licenses that were attempted to revoke.</span></span>|
|<span data-ttu-id="bd9e0-128">фаиледлиценсескаунт</span><span class="sxs-lookup"><span data-stu-id="bd9e0-128">failedLicensesCount</span></span>|<span data-ttu-id="bd9e0-129">Int32</span><span class="sxs-lookup"><span data-stu-id="bd9e0-129">Int32</span></span>|<span data-ttu-id="bd9e0-130">Количество лицензий, которые не удалось отозвать.</span><span class="sxs-lookup"><span data-stu-id="bd9e0-130">A count of the number of licenses that failed to revoke.</span></span>|
|<span data-ttu-id="bd9e0-131">актионфаилуререасон</span><span class="sxs-lookup"><span data-stu-id="bd9e0-131">actionFailureReason</span></span>|[<span data-ttu-id="bd9e0-132">впптокенактионфаилуререасон</span><span class="sxs-lookup"><span data-stu-id="bd9e0-132">vppTokenActionFailureReason</span></span>](../resources/intune-shared-vpptokenactionfailurereason.md)|<span data-ttu-id="bd9e0-133">Причина сбоя действия "отзыв лицензий".</span><span class="sxs-lookup"><span data-stu-id="bd9e0-133">The reason for the revoke licenses action failure.</span></span> <span data-ttu-id="bd9e0-134">Возможные значения: `none`, `appleFailure`, `internalError`, `expiredVppToken`, `expiredApplePushNotificationCertificate`.</span><span class="sxs-lookup"><span data-stu-id="bd9e0-134">Possible values are: `none`, `appleFailure`, `internalError`, `expiredVppToken`, `expiredApplePushNotificationCertificate`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bd9e0-135">Связи</span><span class="sxs-lookup"><span data-stu-id="bd9e0-135">Relationships</span></span>
<span data-ttu-id="bd9e0-136">Нет</span><span class="sxs-lookup"><span data-stu-id="bd9e0-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bd9e0-137">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bd9e0-137">JSON Representation</span></span>
<span data-ttu-id="bd9e0-138">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bd9e0-138">Here is a JSON representation of the resource.</span></span>
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




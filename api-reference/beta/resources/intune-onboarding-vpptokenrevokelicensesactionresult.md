---
title: Тип ресурса Впптокенревокелиценсесактионресулт
description: Состояние действия отзыва лицензий, выполняемого в токене Apple Volume Purchase Program.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 432419f337750362256140b8d13a1841b49907d4
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32566467"
---
# <a name="vpptokenrevokelicensesactionresult-resource-type"></a><span data-ttu-id="cae15-103">Тип ресурса Впптокенревокелиценсесактионресулт</span><span class="sxs-lookup"><span data-stu-id="cae15-103">vppTokenRevokeLicensesActionResult resource type</span></span>

> <span data-ttu-id="cae15-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cae15-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cae15-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="cae15-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cae15-106">Состояние действия отзыва лицензий, выполняемого в токене Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="cae15-106">The status of the revoke licenses action performed on the Apple Volume Purchase Program token.</span></span>


<span data-ttu-id="cae15-107">НаСледуется от [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="cae15-107">Inherits from [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="cae15-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="cae15-108">Properties</span></span>
|<span data-ttu-id="cae15-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="cae15-109">Property</span></span>|<span data-ttu-id="cae15-110">Тип</span><span class="sxs-lookup"><span data-stu-id="cae15-110">Type</span></span>|<span data-ttu-id="cae15-111">Описание</span><span class="sxs-lookup"><span data-stu-id="cae15-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cae15-112">actionName</span><span class="sxs-lookup"><span data-stu-id="cae15-112">actionName</span></span>|<span data-ttu-id="cae15-113">String</span><span class="sxs-lookup"><span data-stu-id="cae15-113">String</span></span>|<span data-ttu-id="cae15-114">Имя действия наСледуется от [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="cae15-114">Action name Inherited from [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span></span>|
|<span data-ttu-id="cae15-115">actionState</span><span class="sxs-lookup"><span data-stu-id="cae15-115">actionState</span></span>|[<span data-ttu-id="cae15-116">actionState</span><span class="sxs-lookup"><span data-stu-id="cae15-116">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="cae15-117">Состояние действия, унаследованного от [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="cae15-117">State of the action Inherited from [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md).</span></span> <span data-ttu-id="cae15-118">Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="cae15-118">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="cae15-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="cae15-119">startDateTime</span></span>|<span data-ttu-id="cae15-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cae15-120">DateTimeOffset</span></span>|<span data-ttu-id="cae15-121">Время начала действия, унаследованное от [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="cae15-121">Time the action was initiated Inherited from [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span></span>|
|<span data-ttu-id="cae15-122">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="cae15-122">lastUpdatedDateTime</span></span>|<span data-ttu-id="cae15-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cae15-123">DateTimeOffset</span></span>|<span data-ttu-id="cae15-124">Время последнего обновления состояния действия, унаследованного от [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="cae15-124">Time the action state was last updated Inherited from [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span></span>|
|<span data-ttu-id="cae15-125">Тоталлиценсескаунт</span><span class="sxs-lookup"><span data-stu-id="cae15-125">totalLicensesCount</span></span>|<span data-ttu-id="cae15-126">Int32</span><span class="sxs-lookup"><span data-stu-id="cae15-126">Int32</span></span>|<span data-ttu-id="cae15-127">Число неудачных попыток отзыва лицензий.</span><span class="sxs-lookup"><span data-stu-id="cae15-127">A count of the number of licenses that were attempted to revoke.</span></span>|
|<span data-ttu-id="cae15-128">Фаиледлиценсескаунт</span><span class="sxs-lookup"><span data-stu-id="cae15-128">failedLicensesCount</span></span>|<span data-ttu-id="cae15-129">Int32</span><span class="sxs-lookup"><span data-stu-id="cae15-129">Int32</span></span>|<span data-ttu-id="cae15-130">Количество лицензий, которые не удалось отозвать.</span><span class="sxs-lookup"><span data-stu-id="cae15-130">A count of the number of licenses that failed to revoke.</span></span>|
|<span data-ttu-id="cae15-131">Актионфаилуререасон</span><span class="sxs-lookup"><span data-stu-id="cae15-131">actionFailureReason</span></span>|[<span data-ttu-id="cae15-132">Впптокенактионфаилуререасон</span><span class="sxs-lookup"><span data-stu-id="cae15-132">vppTokenActionFailureReason</span></span>](../resources/intune-shared-vpptokenactionfailurereason.md)|<span data-ttu-id="cae15-133">Причина сбоя действия "отзыв лицензий".</span><span class="sxs-lookup"><span data-stu-id="cae15-133">The reason for the revoke licenses action failure.</span></span> <span data-ttu-id="cae15-134">Возможные значения: `none`, `appleFailure`, `internalError`, `expiredVppToken`, `expiredApplePushNotificationCertificate`.</span><span class="sxs-lookup"><span data-stu-id="cae15-134">Possible values are: `none`, `appleFailure`, `internalError`, `expiredVppToken`, `expiredApplePushNotificationCertificate`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cae15-135">Отношения</span><span class="sxs-lookup"><span data-stu-id="cae15-135">Relationships</span></span>
<span data-ttu-id="cae15-136">Нет</span><span class="sxs-lookup"><span data-stu-id="cae15-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="cae15-137">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="cae15-137">JSON Representation</span></span>
<span data-ttu-id="cae15-138">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cae15-138">Here is a JSON representation of the resource.</span></span>
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






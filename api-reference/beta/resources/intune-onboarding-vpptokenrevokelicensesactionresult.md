---
title: Тип ресурса Впптокенревокелиценсесактионресулт
description: Состояние действия отзыва лицензий, выполняемого в токене Apple Volume Purchase Program.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ec3ccf2bfd72ae9f6aeb85e3a7228faac09a8b2c
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30158172"
---
# <a name="vpptokenrevokelicensesactionresult-resource-type"></a><span data-ttu-id="32e96-103">Тип ресурса Впптокенревокелиценсесактионресулт</span><span class="sxs-lookup"><span data-stu-id="32e96-103">vppTokenRevokeLicensesActionResult resource type</span></span>

> <span data-ttu-id="32e96-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="32e96-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="32e96-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="32e96-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="32e96-106">Состояние действия отзыва лицензий, выполняемого в токене Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="32e96-106">The status of the revoke licenses action performed on the Apple Volume Purchase Program token.</span></span>


<span data-ttu-id="32e96-107">НаСледуется от [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="32e96-107">Inherits from [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="32e96-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="32e96-108">Properties</span></span>
|<span data-ttu-id="32e96-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="32e96-109">Property</span></span>|<span data-ttu-id="32e96-110">Тип</span><span class="sxs-lookup"><span data-stu-id="32e96-110">Type</span></span>|<span data-ttu-id="32e96-111">Описание</span><span class="sxs-lookup"><span data-stu-id="32e96-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="32e96-112">actionName</span><span class="sxs-lookup"><span data-stu-id="32e96-112">actionName</span></span>|<span data-ttu-id="32e96-113">String</span><span class="sxs-lookup"><span data-stu-id="32e96-113">String</span></span>|<span data-ttu-id="32e96-114">Имя действия наСледуется от [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="32e96-114">Action name Inherited from [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span></span>|
|<span data-ttu-id="32e96-115">actionState</span><span class="sxs-lookup"><span data-stu-id="32e96-115">actionState</span></span>|[<span data-ttu-id="32e96-116">actionState</span><span class="sxs-lookup"><span data-stu-id="32e96-116">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="32e96-117">Состояние действия, унаследованного от [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="32e96-117">State of the action Inherited from [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md).</span></span> <span data-ttu-id="32e96-118">Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="32e96-118">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="32e96-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="32e96-119">startDateTime</span></span>|<span data-ttu-id="32e96-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="32e96-120">DateTimeOffset</span></span>|<span data-ttu-id="32e96-121">Время начала действия, унаследованное от [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="32e96-121">Time the action was initiated Inherited from [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span></span>|
|<span data-ttu-id="32e96-122">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="32e96-122">lastUpdatedDateTime</span></span>|<span data-ttu-id="32e96-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="32e96-123">DateTimeOffset</span></span>|<span data-ttu-id="32e96-124">Время последнего обновления состояния действия, унаследованного от [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="32e96-124">Time the action state was last updated Inherited from [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span></span>|
|<span data-ttu-id="32e96-125">Тоталлиценсескаунт</span><span class="sxs-lookup"><span data-stu-id="32e96-125">totalLicensesCount</span></span>|<span data-ttu-id="32e96-126">Int32</span><span class="sxs-lookup"><span data-stu-id="32e96-126">Int32</span></span>|<span data-ttu-id="32e96-127">Число неудачных попыток отзыва лицензий.</span><span class="sxs-lookup"><span data-stu-id="32e96-127">A count of the number of licenses that were attempted to revoke.</span></span>|
|<span data-ttu-id="32e96-128">Фаиледлиценсескаунт</span><span class="sxs-lookup"><span data-stu-id="32e96-128">failedLicensesCount</span></span>|<span data-ttu-id="32e96-129">Int32</span><span class="sxs-lookup"><span data-stu-id="32e96-129">Int32</span></span>|<span data-ttu-id="32e96-130">Количество лицензий, которые не удалось отозвать.</span><span class="sxs-lookup"><span data-stu-id="32e96-130">A count of the number of licenses that failed to revoke.</span></span>|
|<span data-ttu-id="32e96-131">Актионфаилуререасон</span><span class="sxs-lookup"><span data-stu-id="32e96-131">actionFailureReason</span></span>|[<span data-ttu-id="32e96-132">Впптокенактионфаилуререасон</span><span class="sxs-lookup"><span data-stu-id="32e96-132">vppTokenActionFailureReason</span></span>](../resources/intune-shared-vpptokenactionfailurereason.md)|<span data-ttu-id="32e96-133">Причина сбоя действия "отзыв лицензий".</span><span class="sxs-lookup"><span data-stu-id="32e96-133">The reason for the revoke licenses action failure.</span></span> <span data-ttu-id="32e96-134">Возможные значения: `none`, `appleFailure`, `internalError`, `expiredVppToken`, `expiredApplePushNotificationCertificate`.</span><span class="sxs-lookup"><span data-stu-id="32e96-134">Possible values are: `none`, `appleFailure`, `internalError`, `expiredVppToken`, `expiredApplePushNotificationCertificate`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="32e96-135">Отношения</span><span class="sxs-lookup"><span data-stu-id="32e96-135">Relationships</span></span>
<span data-ttu-id="32e96-136">Нет</span><span class="sxs-lookup"><span data-stu-id="32e96-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="32e96-137">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="32e96-137">JSON Representation</span></span>
<span data-ttu-id="32e96-138">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="32e96-138">Here is a JSON representation of the resource.</span></span>
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





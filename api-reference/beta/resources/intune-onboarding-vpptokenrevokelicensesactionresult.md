---
title: Тип ресурса Впптокенревокелиценсесактионресулт
description: Состояние действия отзыва лицензий, выполняемого в токене Apple Volume Purchase Program.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 4be11b14c51f7de9f03de6705a9b2cf71fc0c362
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36369390"
---
# <a name="vpptokenrevokelicensesactionresult-resource-type"></a><span data-ttu-id="55fcc-103">Тип ресурса Впптокенревокелиценсесактионресулт</span><span class="sxs-lookup"><span data-stu-id="55fcc-103">vppTokenRevokeLicensesActionResult resource type</span></span>

> <span data-ttu-id="55fcc-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="55fcc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="55fcc-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="55fcc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="55fcc-106">Состояние действия отзыва лицензий, выполняемого в токене Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="55fcc-106">The status of the revoke licenses action performed on the Apple Volume Purchase Program token.</span></span>


<span data-ttu-id="55fcc-107">Наследуется от [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="55fcc-107">Inherits from [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="55fcc-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="55fcc-108">Properties</span></span>
|<span data-ttu-id="55fcc-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="55fcc-109">Property</span></span>|<span data-ttu-id="55fcc-110">Тип</span><span class="sxs-lookup"><span data-stu-id="55fcc-110">Type</span></span>|<span data-ttu-id="55fcc-111">Описание</span><span class="sxs-lookup"><span data-stu-id="55fcc-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="55fcc-112">actionName</span><span class="sxs-lookup"><span data-stu-id="55fcc-112">actionName</span></span>|<span data-ttu-id="55fcc-113">String</span><span class="sxs-lookup"><span data-stu-id="55fcc-113">String</span></span>|<span data-ttu-id="55fcc-114">Имя действия наследуется от [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="55fcc-114">Action name Inherited from [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span></span>|
|<span data-ttu-id="55fcc-115">actionState</span><span class="sxs-lookup"><span data-stu-id="55fcc-115">actionState</span></span>|[<span data-ttu-id="55fcc-116">actionState</span><span class="sxs-lookup"><span data-stu-id="55fcc-116">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="55fcc-117">Состояние действия, унаследованного от [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="55fcc-117">State of the action Inherited from [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md).</span></span> <span data-ttu-id="55fcc-118">Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="55fcc-118">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="55fcc-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="55fcc-119">startDateTime</span></span>|<span data-ttu-id="55fcc-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="55fcc-120">DateTimeOffset</span></span>|<span data-ttu-id="55fcc-121">Время начала действия, унаследованное от [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="55fcc-121">Time the action was initiated Inherited from [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span></span>|
|<span data-ttu-id="55fcc-122">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="55fcc-122">lastUpdatedDateTime</span></span>|<span data-ttu-id="55fcc-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="55fcc-123">DateTimeOffset</span></span>|<span data-ttu-id="55fcc-124">Время последнего обновления состояния действия, унаследованного от [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="55fcc-124">Time the action state was last updated Inherited from [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span></span>|
|<span data-ttu-id="55fcc-125">тоталлиценсескаунт</span><span class="sxs-lookup"><span data-stu-id="55fcc-125">totalLicensesCount</span></span>|<span data-ttu-id="55fcc-126">Int32</span><span class="sxs-lookup"><span data-stu-id="55fcc-126">Int32</span></span>|<span data-ttu-id="55fcc-127">Число неудачных попыток отзыва лицензий.</span><span class="sxs-lookup"><span data-stu-id="55fcc-127">A count of the number of licenses that were attempted to revoke.</span></span>|
|<span data-ttu-id="55fcc-128">фаиледлиценсескаунт</span><span class="sxs-lookup"><span data-stu-id="55fcc-128">failedLicensesCount</span></span>|<span data-ttu-id="55fcc-129">Int32</span><span class="sxs-lookup"><span data-stu-id="55fcc-129">Int32</span></span>|<span data-ttu-id="55fcc-130">Количество лицензий, которые не удалось отозвать.</span><span class="sxs-lookup"><span data-stu-id="55fcc-130">A count of the number of licenses that failed to revoke.</span></span>|
|<span data-ttu-id="55fcc-131">актионфаилуререасон</span><span class="sxs-lookup"><span data-stu-id="55fcc-131">actionFailureReason</span></span>|[<span data-ttu-id="55fcc-132">впптокенактионфаилуререасон</span><span class="sxs-lookup"><span data-stu-id="55fcc-132">vppTokenActionFailureReason</span></span>](../resources/intune-shared-vpptokenactionfailurereason.md)|<span data-ttu-id="55fcc-133">Причина сбоя действия "отзыв лицензий".</span><span class="sxs-lookup"><span data-stu-id="55fcc-133">The reason for the revoke licenses action failure.</span></span> <span data-ttu-id="55fcc-134">Возможные значения: `none`, `appleFailure`, `internalError`, `expiredVppToken`, `expiredApplePushNotificationCertificate`.</span><span class="sxs-lookup"><span data-stu-id="55fcc-134">Possible values are: `none`, `appleFailure`, `internalError`, `expiredVppToken`, `expiredApplePushNotificationCertificate`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="55fcc-135">Отношения</span><span class="sxs-lookup"><span data-stu-id="55fcc-135">Relationships</span></span>
<span data-ttu-id="55fcc-136">Нет</span><span class="sxs-lookup"><span data-stu-id="55fcc-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="55fcc-137">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="55fcc-137">JSON Representation</span></span>
<span data-ttu-id="55fcc-138">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="55fcc-138">Here is a JSON representation of the resource.</span></span>
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




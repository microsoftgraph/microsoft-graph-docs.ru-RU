---
title: Тип ресурса Впптокенревокелиценсесактионресулт
description: Состояние действия отзыва лицензий, выполняемого в токене Apple Volume Purchase Program.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 91e86ad5dd490aa4f42a01c369b8597fde030857
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36010632"
---
# <a name="vpptokenrevokelicensesactionresult-resource-type"></a><span data-ttu-id="ee955-103">Тип ресурса Впптокенревокелиценсесактионресулт</span><span class="sxs-lookup"><span data-stu-id="ee955-103">vppTokenRevokeLicensesActionResult resource type</span></span>

> <span data-ttu-id="ee955-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ee955-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ee955-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ee955-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ee955-106">Состояние действия отзыва лицензий, выполняемого в токене Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="ee955-106">The status of the revoke licenses action performed on the Apple Volume Purchase Program token.</span></span>


<span data-ttu-id="ee955-107">Наследуется от [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="ee955-107">Inherits from [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="ee955-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="ee955-108">Properties</span></span>
|<span data-ttu-id="ee955-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="ee955-109">Property</span></span>|<span data-ttu-id="ee955-110">Тип</span><span class="sxs-lookup"><span data-stu-id="ee955-110">Type</span></span>|<span data-ttu-id="ee955-111">Описание</span><span class="sxs-lookup"><span data-stu-id="ee955-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ee955-112">actionName</span><span class="sxs-lookup"><span data-stu-id="ee955-112">actionName</span></span>|<span data-ttu-id="ee955-113">String</span><span class="sxs-lookup"><span data-stu-id="ee955-113">String</span></span>|<span data-ttu-id="ee955-114">Имя действия наследуется от [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="ee955-114">Action name Inherited from [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span></span>|
|<span data-ttu-id="ee955-115">actionState</span><span class="sxs-lookup"><span data-stu-id="ee955-115">actionState</span></span>|[<span data-ttu-id="ee955-116">actionState</span><span class="sxs-lookup"><span data-stu-id="ee955-116">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="ee955-117">Состояние действия, унаследованного от [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="ee955-117">State of the action Inherited from [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md).</span></span> <span data-ttu-id="ee955-118">Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="ee955-118">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="ee955-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="ee955-119">startDateTime</span></span>|<span data-ttu-id="ee955-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ee955-120">DateTimeOffset</span></span>|<span data-ttu-id="ee955-121">Время начала действия, унаследованное от [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="ee955-121">Time the action was initiated Inherited from [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span></span>|
|<span data-ttu-id="ee955-122">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="ee955-122">lastUpdatedDateTime</span></span>|<span data-ttu-id="ee955-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ee955-123">DateTimeOffset</span></span>|<span data-ttu-id="ee955-124">Время последнего обновления состояния действия, унаследованного от [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="ee955-124">Time the action state was last updated Inherited from [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span></span>|
|<span data-ttu-id="ee955-125">Тоталлиценсескаунт</span><span class="sxs-lookup"><span data-stu-id="ee955-125">totalLicensesCount</span></span>|<span data-ttu-id="ee955-126">Int32</span><span class="sxs-lookup"><span data-stu-id="ee955-126">Int32</span></span>|<span data-ttu-id="ee955-127">Число неудачных попыток отзыва лицензий.</span><span class="sxs-lookup"><span data-stu-id="ee955-127">A count of the number of licenses that were attempted to revoke.</span></span>|
|<span data-ttu-id="ee955-128">Фаиледлиценсескаунт</span><span class="sxs-lookup"><span data-stu-id="ee955-128">failedLicensesCount</span></span>|<span data-ttu-id="ee955-129">Int32</span><span class="sxs-lookup"><span data-stu-id="ee955-129">Int32</span></span>|<span data-ttu-id="ee955-130">Количество лицензий, которые не удалось отозвать.</span><span class="sxs-lookup"><span data-stu-id="ee955-130">A count of the number of licenses that failed to revoke.</span></span>|
|<span data-ttu-id="ee955-131">Актионфаилуререасон</span><span class="sxs-lookup"><span data-stu-id="ee955-131">actionFailureReason</span></span>|[<span data-ttu-id="ee955-132">Впптокенактионфаилуререасон</span><span class="sxs-lookup"><span data-stu-id="ee955-132">vppTokenActionFailureReason</span></span>](../resources/intune-shared-vpptokenactionfailurereason.md)|<span data-ttu-id="ee955-133">Причина сбоя действия "отзыв лицензий".</span><span class="sxs-lookup"><span data-stu-id="ee955-133">The reason for the revoke licenses action failure.</span></span> <span data-ttu-id="ee955-134">Возможные значения: `none`, `appleFailure`, `internalError`, `expiredVppToken`, `expiredApplePushNotificationCertificate`.</span><span class="sxs-lookup"><span data-stu-id="ee955-134">Possible values are: `none`, `appleFailure`, `internalError`, `expiredVppToken`, `expiredApplePushNotificationCertificate`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ee955-135">Отношения</span><span class="sxs-lookup"><span data-stu-id="ee955-135">Relationships</span></span>
<span data-ttu-id="ee955-136">Нет</span><span class="sxs-lookup"><span data-stu-id="ee955-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ee955-137">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ee955-137">JSON Representation</span></span>
<span data-ttu-id="ee955-138">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ee955-138">Here is a JSON representation of the resource.</span></span>
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






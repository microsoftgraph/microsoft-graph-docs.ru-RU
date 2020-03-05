---
title: Тип ресурса Впптокенревокелиценсесактионресулт
description: Состояние действия отзыва лицензий, выполняемого в токене Apple Volume Purchase Program.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 82a7374b610c880eae52cc1ecc7185156aa11aa4
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42524071"
---
# <a name="vpptokenrevokelicensesactionresult-resource-type"></a><span data-ttu-id="8d97c-103">Тип ресурса Впптокенревокелиценсесактионресулт</span><span class="sxs-lookup"><span data-stu-id="8d97c-103">vppTokenRevokeLicensesActionResult resource type</span></span>

<span data-ttu-id="8d97c-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="8d97c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8d97c-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8d97c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8d97c-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8d97c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8d97c-107">Состояние действия отзыва лицензий, выполняемого в токене Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="8d97c-107">The status of the revoke licenses action performed on the Apple Volume Purchase Program token.</span></span>


<span data-ttu-id="8d97c-108">Наследуется от [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="8d97c-108">Inherits from [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="8d97c-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="8d97c-109">Properties</span></span>
|<span data-ttu-id="8d97c-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="8d97c-110">Property</span></span>|<span data-ttu-id="8d97c-111">Тип</span><span class="sxs-lookup"><span data-stu-id="8d97c-111">Type</span></span>|<span data-ttu-id="8d97c-112">Описание</span><span class="sxs-lookup"><span data-stu-id="8d97c-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8d97c-113">actionName</span><span class="sxs-lookup"><span data-stu-id="8d97c-113">actionName</span></span>|<span data-ttu-id="8d97c-114">String</span><span class="sxs-lookup"><span data-stu-id="8d97c-114">String</span></span>|<span data-ttu-id="8d97c-115">Имя действия наследуется от [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="8d97c-115">Action name Inherited from [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span></span>|
|<span data-ttu-id="8d97c-116">actionState</span><span class="sxs-lookup"><span data-stu-id="8d97c-116">actionState</span></span>|[<span data-ttu-id="8d97c-117">actionState</span><span class="sxs-lookup"><span data-stu-id="8d97c-117">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="8d97c-118">Состояние действия, унаследованного от [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="8d97c-118">State of the action Inherited from [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md).</span></span> <span data-ttu-id="8d97c-119">Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="8d97c-119">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="8d97c-120">startDateTime</span><span class="sxs-lookup"><span data-stu-id="8d97c-120">startDateTime</span></span>|<span data-ttu-id="8d97c-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8d97c-121">DateTimeOffset</span></span>|<span data-ttu-id="8d97c-122">Время начала действия, унаследованное от [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="8d97c-122">Time the action was initiated Inherited from [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span></span>|
|<span data-ttu-id="8d97c-123">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="8d97c-123">lastUpdatedDateTime</span></span>|<span data-ttu-id="8d97c-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8d97c-124">DateTimeOffset</span></span>|<span data-ttu-id="8d97c-125">Время последнего обновления состояния действия, унаследованного от [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="8d97c-125">Time the action state was last updated Inherited from [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span></span>|
|<span data-ttu-id="8d97c-126">тоталлиценсескаунт</span><span class="sxs-lookup"><span data-stu-id="8d97c-126">totalLicensesCount</span></span>|<span data-ttu-id="8d97c-127">Int32</span><span class="sxs-lookup"><span data-stu-id="8d97c-127">Int32</span></span>|<span data-ttu-id="8d97c-128">Число неудачных попыток отзыва лицензий.</span><span class="sxs-lookup"><span data-stu-id="8d97c-128">A count of the number of licenses that were attempted to revoke.</span></span>|
|<span data-ttu-id="8d97c-129">фаиледлиценсескаунт</span><span class="sxs-lookup"><span data-stu-id="8d97c-129">failedLicensesCount</span></span>|<span data-ttu-id="8d97c-130">Int32</span><span class="sxs-lookup"><span data-stu-id="8d97c-130">Int32</span></span>|<span data-ttu-id="8d97c-131">Количество лицензий, которые не удалось отозвать.</span><span class="sxs-lookup"><span data-stu-id="8d97c-131">A count of the number of licenses that failed to revoke.</span></span>|
|<span data-ttu-id="8d97c-132">актионфаилуререасон</span><span class="sxs-lookup"><span data-stu-id="8d97c-132">actionFailureReason</span></span>|[<span data-ttu-id="8d97c-133">впптокенактионфаилуререасон</span><span class="sxs-lookup"><span data-stu-id="8d97c-133">vppTokenActionFailureReason</span></span>](../resources/intune-shared-vpptokenactionfailurereason.md)|<span data-ttu-id="8d97c-134">Причина сбоя действия "отзыв лицензий".</span><span class="sxs-lookup"><span data-stu-id="8d97c-134">The reason for the revoke licenses action failure.</span></span> <span data-ttu-id="8d97c-135">Возможные значения: `none`, `appleFailure`, `internalError`, `expiredVppToken`, `expiredApplePushNotificationCertificate`.</span><span class="sxs-lookup"><span data-stu-id="8d97c-135">Possible values are: `none`, `appleFailure`, `internalError`, `expiredVppToken`, `expiredApplePushNotificationCertificate`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8d97c-136">Связи</span><span class="sxs-lookup"><span data-stu-id="8d97c-136">Relationships</span></span>
<span data-ttu-id="8d97c-137">Нет</span><span class="sxs-lookup"><span data-stu-id="8d97c-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8d97c-138">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8d97c-138">JSON Representation</span></span>
<span data-ttu-id="8d97c-139">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8d97c-139">Here is a JSON representation of the resource.</span></span>
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




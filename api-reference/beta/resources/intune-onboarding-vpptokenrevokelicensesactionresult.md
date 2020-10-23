---
title: Тип ресурса Впптокенревокелиценсесактионресулт
description: Состояние действия отзыва лицензий, выполняемого в токене Apple Volume Purchase Program.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 216bdffc1fae14633174301dbd183871048f0051
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48703617"
---
# <a name="vpptokenrevokelicensesactionresult-resource-type"></a><span data-ttu-id="7d5ab-103">Тип ресурса Впптокенревокелиценсесактионресулт</span><span class="sxs-lookup"><span data-stu-id="7d5ab-103">vppTokenRevokeLicensesActionResult resource type</span></span>

<span data-ttu-id="7d5ab-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7d5ab-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7d5ab-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7d5ab-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7d5ab-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7d5ab-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7d5ab-107">Состояние действия отзыва лицензий, выполняемого в токене Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="7d5ab-107">The status of the revoke licenses action performed on the Apple Volume Purchase Program token.</span></span>


<span data-ttu-id="7d5ab-108">Наследуется от [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="7d5ab-108">Inherits from [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="7d5ab-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="7d5ab-109">Properties</span></span>
|<span data-ttu-id="7d5ab-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="7d5ab-110">Property</span></span>|<span data-ttu-id="7d5ab-111">Тип</span><span class="sxs-lookup"><span data-stu-id="7d5ab-111">Type</span></span>|<span data-ttu-id="7d5ab-112">Описание</span><span class="sxs-lookup"><span data-stu-id="7d5ab-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7d5ab-113">actionName</span><span class="sxs-lookup"><span data-stu-id="7d5ab-113">actionName</span></span>|<span data-ttu-id="7d5ab-114">String</span><span class="sxs-lookup"><span data-stu-id="7d5ab-114">String</span></span>|<span data-ttu-id="7d5ab-115">Имя действия наследуется от [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="7d5ab-115">Action name Inherited from [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span></span>|
|<span data-ttu-id="7d5ab-116">actionState</span><span class="sxs-lookup"><span data-stu-id="7d5ab-116">actionState</span></span>|[<span data-ttu-id="7d5ab-117">actionState</span><span class="sxs-lookup"><span data-stu-id="7d5ab-117">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="7d5ab-118">Состояние действия, унаследованного от [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="7d5ab-118">State of the action Inherited from [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md).</span></span> <span data-ttu-id="7d5ab-119">Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="7d5ab-119">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="7d5ab-120">startDateTime</span><span class="sxs-lookup"><span data-stu-id="7d5ab-120">startDateTime</span></span>|<span data-ttu-id="7d5ab-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7d5ab-121">DateTimeOffset</span></span>|<span data-ttu-id="7d5ab-122">Время начала действия, унаследованное от [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="7d5ab-122">Time the action was initiated Inherited from [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span></span>|
|<span data-ttu-id="7d5ab-123">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="7d5ab-123">lastUpdatedDateTime</span></span>|<span data-ttu-id="7d5ab-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7d5ab-124">DateTimeOffset</span></span>|<span data-ttu-id="7d5ab-125">Время последнего обновления состояния действия, унаследованного от [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="7d5ab-125">Time the action state was last updated Inherited from [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span></span>|
|<span data-ttu-id="7d5ab-126">тоталлиценсескаунт</span><span class="sxs-lookup"><span data-stu-id="7d5ab-126">totalLicensesCount</span></span>|<span data-ttu-id="7d5ab-127">Int32</span><span class="sxs-lookup"><span data-stu-id="7d5ab-127">Int32</span></span>|<span data-ttu-id="7d5ab-128">Число неудачных попыток отзыва лицензий.</span><span class="sxs-lookup"><span data-stu-id="7d5ab-128">A count of the number of licenses that were attempted to revoke.</span></span>|
|<span data-ttu-id="7d5ab-129">фаиледлиценсескаунт</span><span class="sxs-lookup"><span data-stu-id="7d5ab-129">failedLicensesCount</span></span>|<span data-ttu-id="7d5ab-130">Int32</span><span class="sxs-lookup"><span data-stu-id="7d5ab-130">Int32</span></span>|<span data-ttu-id="7d5ab-131">Количество лицензий, которые не удалось отозвать.</span><span class="sxs-lookup"><span data-stu-id="7d5ab-131">A count of the number of licenses that failed to revoke.</span></span>|
|<span data-ttu-id="7d5ab-132">актионфаилуререасон</span><span class="sxs-lookup"><span data-stu-id="7d5ab-132">actionFailureReason</span></span>|[<span data-ttu-id="7d5ab-133">впптокенактионфаилуререасон</span><span class="sxs-lookup"><span data-stu-id="7d5ab-133">vppTokenActionFailureReason</span></span>](../resources/intune-shared-vpptokenactionfailurereason.md)|<span data-ttu-id="7d5ab-134">Причина сбоя действия "отзыв лицензий".</span><span class="sxs-lookup"><span data-stu-id="7d5ab-134">The reason for the revoke licenses action failure.</span></span> <span data-ttu-id="7d5ab-135">Возможные значения: `none`, `appleFailure`, `internalError`, `expiredVppToken`, `expiredApplePushNotificationCertificate`.</span><span class="sxs-lookup"><span data-stu-id="7d5ab-135">Possible values are: `none`, `appleFailure`, `internalError`, `expiredVppToken`, `expiredApplePushNotificationCertificate`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7d5ab-136">Связи</span><span class="sxs-lookup"><span data-stu-id="7d5ab-136">Relationships</span></span>
<span data-ttu-id="7d5ab-137">Нет</span><span class="sxs-lookup"><span data-stu-id="7d5ab-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7d5ab-138">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7d5ab-138">JSON Representation</span></span>
<span data-ttu-id="7d5ab-139">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7d5ab-139">Here is a JSON representation of the resource.</span></span>
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






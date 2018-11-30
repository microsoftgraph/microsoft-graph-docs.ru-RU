---
title: Тип ресурса vppTokenRevokeLicensesActionResult
description: Состояние действия лицензий revoke выполнить на маркер покупки программы корпоративного Apple.
ms.openlocfilehash: 89baf69ba89ac11c52b8e05b35f38aca422cc1b2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27078184"
---
# <a name="vpptokenrevokelicensesactionresult-resource-type"></a><span data-ttu-id="bf9ed-103">Тип ресурса vppTokenRevokeLicensesActionResult</span><span class="sxs-lookup"><span data-stu-id="bf9ed-103">vppTokenRevokeLicensesActionResult resource type</span></span>

> <span data-ttu-id="bf9ed-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="bf9ed-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bf9ed-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bf9ed-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bf9ed-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="bf9ed-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bf9ed-107">Состояние действия лицензий revoke выполнить на маркер покупки программы корпоративного Apple.</span><span class="sxs-lookup"><span data-stu-id="bf9ed-107">The status of the revoke licenses action performed on the Apple Volume Purchase Program token.</span></span>

<span data-ttu-id="bf9ed-108">Наследуется от [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="bf9ed-108">Inherits from [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="bf9ed-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="bf9ed-109">Properties</span></span>
|<span data-ttu-id="bf9ed-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="bf9ed-110">Property</span></span>|<span data-ttu-id="bf9ed-111">Тип</span><span class="sxs-lookup"><span data-stu-id="bf9ed-111">Type</span></span>|<span data-ttu-id="bf9ed-112">Описание</span><span class="sxs-lookup"><span data-stu-id="bf9ed-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bf9ed-113">actionName</span><span class="sxs-lookup"><span data-stu-id="bf9ed-113">actionName</span></span>|<span data-ttu-id="bf9ed-114">String</span><span class="sxs-lookup"><span data-stu-id="bf9ed-114">String</span></span>|<span data-ttu-id="bf9ed-115">Имя действия унаследованные от [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="bf9ed-115">Action name Inherited from [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span></span>|
|<span data-ttu-id="bf9ed-116">actionState</span><span class="sxs-lookup"><span data-stu-id="bf9ed-116">actionState</span></span>|[<span data-ttu-id="bf9ed-117">actionState</span><span class="sxs-lookup"><span data-stu-id="bf9ed-117">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="bf9ed-118">Состояние действие унаследованные от [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="bf9ed-118">State of the action Inherited from [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md).</span></span> <span data-ttu-id="bf9ed-119">Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="bf9ed-119">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="bf9ed-120">startDateTime</span><span class="sxs-lookup"><span data-stu-id="bf9ed-120">startDateTime</span></span>|<span data-ttu-id="bf9ed-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bf9ed-121">DateTimeOffset</span></span>|<span data-ttu-id="bf9ed-122">Время началось наследуется от [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="bf9ed-122">Time the action was initiated Inherited from [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span></span>|
|<span data-ttu-id="bf9ed-123">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="bf9ed-123">lastUpdatedDateTime</span></span>|<span data-ttu-id="bf9ed-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bf9ed-124">DateTimeOffset</span></span>|<span data-ttu-id="bf9ed-125">Время последнего состояния действия обновления унаследованные от [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="bf9ed-125">Time the action state was last updated Inherited from [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span></span>|
|<span data-ttu-id="bf9ed-126">totalLicensesCount</span><span class="sxs-lookup"><span data-stu-id="bf9ed-126">totalLicensesCount</span></span>|<span data-ttu-id="bf9ed-127">Int32</span><span class="sxs-lookup"><span data-stu-id="bf9ed-127">Int32</span></span>|<span data-ttu-id="bf9ed-128">Подсчет числа лицензий, которые были пытались отменить.</span><span class="sxs-lookup"><span data-stu-id="bf9ed-128">A count of the number of licenses that were attempted to revoke.</span></span>|
|<span data-ttu-id="bf9ed-129">failedLicensesCount</span><span class="sxs-lookup"><span data-stu-id="bf9ed-129">failedLicensesCount</span></span>|<span data-ttu-id="bf9ed-130">Int32</span><span class="sxs-lookup"><span data-stu-id="bf9ed-130">Int32</span></span>|<span data-ttu-id="bf9ed-131">Подсчет числа лицензий, которые не удалось отозвать.</span><span class="sxs-lookup"><span data-stu-id="bf9ed-131">A count of the number of licenses that failed to revoke.</span></span>|
|<span data-ttu-id="bf9ed-132">actionFailureReason</span><span class="sxs-lookup"><span data-stu-id="bf9ed-132">actionFailureReason</span></span>|[<span data-ttu-id="bf9ed-133">vppTokenActionFailureReason</span><span class="sxs-lookup"><span data-stu-id="bf9ed-133">vppTokenActionFailureReason</span></span>](../resources/intune-shared-vpptokenactionfailurereason.md)|<span data-ttu-id="bf9ed-134">Причина ошибки действие revoke лицензий.</span><span class="sxs-lookup"><span data-stu-id="bf9ed-134">The reason for the revoke licenses action failure.</span></span> <span data-ttu-id="bf9ed-135">Возможные значения: `none`, `appleFailure`, `internalError`, `expiredVppToken`, `expiredApplePushNotificationCertificate`.</span><span class="sxs-lookup"><span data-stu-id="bf9ed-135">Possible values are: `none`, `appleFailure`, `internalError`, `expiredVppToken`, `expiredApplePushNotificationCertificate`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bf9ed-136">Связи</span><span class="sxs-lookup"><span data-stu-id="bf9ed-136">Relationships</span></span>
<span data-ttu-id="bf9ed-137">Нет</span><span class="sxs-lookup"><span data-stu-id="bf9ed-137">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="bf9ed-138">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bf9ed-138">JSON Representation</span></span>
<span data-ttu-id="bf9ed-139">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bf9ed-139">Here is a JSON representation of the resource.</span></span>
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






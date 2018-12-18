---
title: Тип ресурса vppTokenRevokeLicensesActionResult
description: Состояние действия лицензий revoke выполнить на маркер покупки программы корпоративного Apple.
author: tfitzmac
ms.openlocfilehash: a4188a269f9273b955fd29b32348dec82023b181
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27351459"
---
# <a name="vpptokenrevokelicensesactionresult-resource-type"></a><span data-ttu-id="ff51a-103">Тип ресурса vppTokenRevokeLicensesActionResult</span><span class="sxs-lookup"><span data-stu-id="ff51a-103">vppTokenRevokeLicensesActionResult resource type</span></span>

> <span data-ttu-id="ff51a-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="ff51a-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ff51a-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ff51a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ff51a-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="ff51a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ff51a-107">Состояние действия лицензий revoke выполнить на маркер покупки программы корпоративного Apple.</span><span class="sxs-lookup"><span data-stu-id="ff51a-107">The status of the revoke licenses action performed on the Apple Volume Purchase Program token.</span></span>

<span data-ttu-id="ff51a-108">Наследуется от [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="ff51a-108">Inherits from [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="ff51a-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="ff51a-109">Properties</span></span>
|<span data-ttu-id="ff51a-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="ff51a-110">Property</span></span>|<span data-ttu-id="ff51a-111">Тип</span><span class="sxs-lookup"><span data-stu-id="ff51a-111">Type</span></span>|<span data-ttu-id="ff51a-112">Описание</span><span class="sxs-lookup"><span data-stu-id="ff51a-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ff51a-113">actionName</span><span class="sxs-lookup"><span data-stu-id="ff51a-113">actionName</span></span>|<span data-ttu-id="ff51a-114">String</span><span class="sxs-lookup"><span data-stu-id="ff51a-114">String</span></span>|<span data-ttu-id="ff51a-115">Имя действия унаследованные от [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="ff51a-115">Action name Inherited from [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span></span>|
|<span data-ttu-id="ff51a-116">actionState</span><span class="sxs-lookup"><span data-stu-id="ff51a-116">actionState</span></span>|[<span data-ttu-id="ff51a-117">actionState</span><span class="sxs-lookup"><span data-stu-id="ff51a-117">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="ff51a-118">Состояние действие унаследованные от [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="ff51a-118">State of the action Inherited from [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md).</span></span> <span data-ttu-id="ff51a-119">Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="ff51a-119">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="ff51a-120">startDateTime</span><span class="sxs-lookup"><span data-stu-id="ff51a-120">startDateTime</span></span>|<span data-ttu-id="ff51a-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ff51a-121">DateTimeOffset</span></span>|<span data-ttu-id="ff51a-122">Время началось наследуется от [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="ff51a-122">Time the action was initiated Inherited from [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span></span>|
|<span data-ttu-id="ff51a-123">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="ff51a-123">lastUpdatedDateTime</span></span>|<span data-ttu-id="ff51a-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ff51a-124">DateTimeOffset</span></span>|<span data-ttu-id="ff51a-125">Время последнего состояния действия обновления унаследованные от [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="ff51a-125">Time the action state was last updated Inherited from [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span></span>|
|<span data-ttu-id="ff51a-126">totalLicensesCount</span><span class="sxs-lookup"><span data-stu-id="ff51a-126">totalLicensesCount</span></span>|<span data-ttu-id="ff51a-127">Int32</span><span class="sxs-lookup"><span data-stu-id="ff51a-127">Int32</span></span>|<span data-ttu-id="ff51a-128">Подсчет числа лицензий, которые были пытались отменить.</span><span class="sxs-lookup"><span data-stu-id="ff51a-128">A count of the number of licenses that were attempted to revoke.</span></span>|
|<span data-ttu-id="ff51a-129">failedLicensesCount</span><span class="sxs-lookup"><span data-stu-id="ff51a-129">failedLicensesCount</span></span>|<span data-ttu-id="ff51a-130">Int32</span><span class="sxs-lookup"><span data-stu-id="ff51a-130">Int32</span></span>|<span data-ttu-id="ff51a-131">Подсчет числа лицензий, которые не удалось отозвать.</span><span class="sxs-lookup"><span data-stu-id="ff51a-131">A count of the number of licenses that failed to revoke.</span></span>|
|<span data-ttu-id="ff51a-132">actionFailureReason</span><span class="sxs-lookup"><span data-stu-id="ff51a-132">actionFailureReason</span></span>|[<span data-ttu-id="ff51a-133">vppTokenActionFailureReason</span><span class="sxs-lookup"><span data-stu-id="ff51a-133">vppTokenActionFailureReason</span></span>](../resources/intune-shared-vpptokenactionfailurereason.md)|<span data-ttu-id="ff51a-134">Причина ошибки действие revoke лицензий.</span><span class="sxs-lookup"><span data-stu-id="ff51a-134">The reason for the revoke licenses action failure.</span></span> <span data-ttu-id="ff51a-135">Возможные значения: `none`, `appleFailure`, `internalError`, `expiredVppToken`, `expiredApplePushNotificationCertificate`.</span><span class="sxs-lookup"><span data-stu-id="ff51a-135">Possible values are: `none`, `appleFailure`, `internalError`, `expiredVppToken`, `expiredApplePushNotificationCertificate`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ff51a-136">Связи</span><span class="sxs-lookup"><span data-stu-id="ff51a-136">Relationships</span></span>
<span data-ttu-id="ff51a-137">Нет</span><span class="sxs-lookup"><span data-stu-id="ff51a-137">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="ff51a-138">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ff51a-138">JSON Representation</span></span>
<span data-ttu-id="ff51a-139">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ff51a-139">Here is a JSON representation of the resource.</span></span>
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






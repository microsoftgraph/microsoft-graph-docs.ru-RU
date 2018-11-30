---
title: Тип ресурса revokeAppleVppLicensesActionResult
description: Отменить результат действия лицензий на Apple Vpp
ms.openlocfilehash: f751f90b90bbf282fa05a59a4a1c59d04ccfbb99
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27078088"
---
# <a name="revokeapplevpplicensesactionresult-resource-type"></a><span data-ttu-id="cc3e0-103">Тип ресурса revokeAppleVppLicensesActionResult</span><span class="sxs-lookup"><span data-stu-id="cc3e0-103">revokeAppleVppLicensesActionResult resource type</span></span>

> <span data-ttu-id="cc3e0-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="cc3e0-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cc3e0-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cc3e0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="cc3e0-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="cc3e0-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cc3e0-107">Отменить результат действия лицензий на Apple Vpp</span><span class="sxs-lookup"><span data-stu-id="cc3e0-107">Revoke Apple Vpp licenses action result</span></span>

<span data-ttu-id="cc3e0-108">Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="cc3e0-108">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="cc3e0-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="cc3e0-109">Properties</span></span>
|<span data-ttu-id="cc3e0-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="cc3e0-110">Property</span></span>|<span data-ttu-id="cc3e0-111">Тип</span><span class="sxs-lookup"><span data-stu-id="cc3e0-111">Type</span></span>|<span data-ttu-id="cc3e0-112">Описание</span><span class="sxs-lookup"><span data-stu-id="cc3e0-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cc3e0-113">actionName</span><span class="sxs-lookup"><span data-stu-id="cc3e0-113">actionName</span></span>|<span data-ttu-id="cc3e0-114">String</span><span class="sxs-lookup"><span data-stu-id="cc3e0-114">String</span></span>|<span data-ttu-id="cc3e0-115">Название действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="cc3e0-115">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="cc3e0-116">actionState</span><span class="sxs-lookup"><span data-stu-id="cc3e0-116">actionState</span></span>|[<span data-ttu-id="cc3e0-117">actionState</span><span class="sxs-lookup"><span data-stu-id="cc3e0-117">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="cc3e0-118">Состояние действие унаследованные от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="cc3e0-118">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="cc3e0-119">Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="cc3e0-119">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="cc3e0-120">startDateTime</span><span class="sxs-lookup"><span data-stu-id="cc3e0-120">startDateTime</span></span>|<span data-ttu-id="cc3e0-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cc3e0-121">DateTimeOffset</span></span>|<span data-ttu-id="cc3e0-122">Время начала действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="cc3e0-122">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="cc3e0-123">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="cc3e0-123">lastUpdatedDateTime</span></span>|<span data-ttu-id="cc3e0-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cc3e0-124">DateTimeOffset</span></span>|<span data-ttu-id="cc3e0-125">Время последнего обновления действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="cc3e0-125">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="cc3e0-126">totalLicensesCount</span><span class="sxs-lookup"><span data-stu-id="cc3e0-126">totalLicensesCount</span></span>|<span data-ttu-id="cc3e0-127">Int32</span><span class="sxs-lookup"><span data-stu-id="cc3e0-127">Int32</span></span>|<span data-ttu-id="cc3e0-128">Общее число лицензий Apple Vpp связанный</span><span class="sxs-lookup"><span data-stu-id="cc3e0-128">Total number of Apple Vpp licenses associated</span></span>|
|<span data-ttu-id="cc3e0-129">failedLicensesCount</span><span class="sxs-lookup"><span data-stu-id="cc3e0-129">failedLicensesCount</span></span>|<span data-ttu-id="cc3e0-130">Int32</span><span class="sxs-lookup"><span data-stu-id="cc3e0-130">Int32</span></span>|<span data-ttu-id="cc3e0-131">Общее число лицензий Apple Vpp, которые не удалось отозвать</span><span class="sxs-lookup"><span data-stu-id="cc3e0-131">Total number of Apple Vpp licenses that failed to revoke</span></span>|

## <a name="relationships"></a><span data-ttu-id="cc3e0-132">Связи</span><span class="sxs-lookup"><span data-stu-id="cc3e0-132">Relationships</span></span>
<span data-ttu-id="cc3e0-133">Нет</span><span class="sxs-lookup"><span data-stu-id="cc3e0-133">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="cc3e0-134">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="cc3e0-134">JSON Representation</span></span>
<span data-ttu-id="cc3e0-135">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cc3e0-135">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.revokeAppleVppLicensesActionResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.revokeAppleVppLicensesActionResult",
  "actionName": "String",
  "actionState": "String",
  "startDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)",
  "totalLicensesCount": 1024,
  "failedLicensesCount": 1024
}
```






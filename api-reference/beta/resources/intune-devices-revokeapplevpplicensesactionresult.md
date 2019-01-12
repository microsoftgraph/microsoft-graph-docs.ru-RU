---
title: Тип ресурса revokeAppleVppLicensesActionResult
description: Отменить результат действия лицензий на Apple Vpp
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: dfb2c18f89dde36ef0fbda7a6ad3221e2ad3728f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27944483"
---
# <a name="revokeapplevpplicensesactionresult-resource-type"></a><span data-ttu-id="47a16-103">Тип ресурса revokeAppleVppLicensesActionResult</span><span class="sxs-lookup"><span data-stu-id="47a16-103">revokeAppleVppLicensesActionResult resource type</span></span>

> <span data-ttu-id="47a16-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="47a16-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="47a16-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="47a16-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="47a16-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="47a16-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="47a16-107">Отменить результат действия лицензий на Apple Vpp</span><span class="sxs-lookup"><span data-stu-id="47a16-107">Revoke Apple Vpp licenses action result</span></span>

<span data-ttu-id="47a16-108">Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="47a16-108">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="47a16-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="47a16-109">Properties</span></span>
|<span data-ttu-id="47a16-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="47a16-110">Property</span></span>|<span data-ttu-id="47a16-111">Тип</span><span class="sxs-lookup"><span data-stu-id="47a16-111">Type</span></span>|<span data-ttu-id="47a16-112">Описание</span><span class="sxs-lookup"><span data-stu-id="47a16-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="47a16-113">actionName</span><span class="sxs-lookup"><span data-stu-id="47a16-113">actionName</span></span>|<span data-ttu-id="47a16-114">String</span><span class="sxs-lookup"><span data-stu-id="47a16-114">String</span></span>|<span data-ttu-id="47a16-115">Название действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="47a16-115">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="47a16-116">actionState</span><span class="sxs-lookup"><span data-stu-id="47a16-116">actionState</span></span>|[<span data-ttu-id="47a16-117">actionState</span><span class="sxs-lookup"><span data-stu-id="47a16-117">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="47a16-118">Состояние действие унаследованные от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="47a16-118">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="47a16-119">Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="47a16-119">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="47a16-120">startDateTime</span><span class="sxs-lookup"><span data-stu-id="47a16-120">startDateTime</span></span>|<span data-ttu-id="47a16-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="47a16-121">DateTimeOffset</span></span>|<span data-ttu-id="47a16-122">Время начала действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="47a16-122">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="47a16-123">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="47a16-123">lastUpdatedDateTime</span></span>|<span data-ttu-id="47a16-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="47a16-124">DateTimeOffset</span></span>|<span data-ttu-id="47a16-125">Время последнего обновления действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="47a16-125">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="47a16-126">totalLicensesCount</span><span class="sxs-lookup"><span data-stu-id="47a16-126">totalLicensesCount</span></span>|<span data-ttu-id="47a16-127">Int32</span><span class="sxs-lookup"><span data-stu-id="47a16-127">Int32</span></span>|<span data-ttu-id="47a16-128">Общее число лицензий Apple Vpp связанный</span><span class="sxs-lookup"><span data-stu-id="47a16-128">Total number of Apple Vpp licenses associated</span></span>|
|<span data-ttu-id="47a16-129">failedLicensesCount</span><span class="sxs-lookup"><span data-stu-id="47a16-129">failedLicensesCount</span></span>|<span data-ttu-id="47a16-130">Int32</span><span class="sxs-lookup"><span data-stu-id="47a16-130">Int32</span></span>|<span data-ttu-id="47a16-131">Общее число лицензий Apple Vpp, которые не удалось отозвать</span><span class="sxs-lookup"><span data-stu-id="47a16-131">Total number of Apple Vpp licenses that failed to revoke</span></span>|

## <a name="relationships"></a><span data-ttu-id="47a16-132">Связи</span><span class="sxs-lookup"><span data-stu-id="47a16-132">Relationships</span></span>
<span data-ttu-id="47a16-133">Нет</span><span class="sxs-lookup"><span data-stu-id="47a16-133">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="47a16-134">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="47a16-134">JSON Representation</span></span>
<span data-ttu-id="47a16-135">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="47a16-135">Here is a JSON representation of the resource.</span></span>
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






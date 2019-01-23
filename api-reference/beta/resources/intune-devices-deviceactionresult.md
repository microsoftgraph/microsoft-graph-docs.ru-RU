---
title: Тип ресурса deviceActionResult
description: Результат действия, касающегося устройства
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 518d0d09d7ef4f9fea67ce8d600f97be0345fa63
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29404710"
---
# <a name="deviceactionresult-resource-type"></a><span data-ttu-id="e1971-103">Тип ресурса deviceActionResult</span><span class="sxs-lookup"><span data-stu-id="e1971-103">deviceActionResult resource type</span></span>

> <span data-ttu-id="e1971-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="e1971-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="e1971-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e1971-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e1971-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e1971-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e1971-107">Результат действия, касающегося устройства</span><span class="sxs-lookup"><span data-stu-id="e1971-107">Device action result</span></span>

## <a name="properties"></a><span data-ttu-id="e1971-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="e1971-108">Properties</span></span>
|<span data-ttu-id="e1971-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="e1971-109">Property</span></span>|<span data-ttu-id="e1971-110">Тип</span><span class="sxs-lookup"><span data-stu-id="e1971-110">Type</span></span>|<span data-ttu-id="e1971-111">Описание</span><span class="sxs-lookup"><span data-stu-id="e1971-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e1971-112">actionName</span><span class="sxs-lookup"><span data-stu-id="e1971-112">actionName</span></span>|<span data-ttu-id="e1971-113">String</span><span class="sxs-lookup"><span data-stu-id="e1971-113">String</span></span>|<span data-ttu-id="e1971-114">Название действия</span><span class="sxs-lookup"><span data-stu-id="e1971-114">Action name</span></span>|
|<span data-ttu-id="e1971-115">actionState</span><span class="sxs-lookup"><span data-stu-id="e1971-115">actionState</span></span>|[<span data-ttu-id="e1971-116">actionState</span><span class="sxs-lookup"><span data-stu-id="e1971-116">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="e1971-117">Состояние действия.</span><span class="sxs-lookup"><span data-stu-id="e1971-117">State of the action.</span></span> <span data-ttu-id="e1971-118">Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="e1971-118">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="e1971-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="e1971-119">startDateTime</span></span>|<span data-ttu-id="e1971-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e1971-120">DateTimeOffset</span></span>|<span data-ttu-id="e1971-121">Время начала действия</span><span class="sxs-lookup"><span data-stu-id="e1971-121">Time the action was initiated</span></span>|
|<span data-ttu-id="e1971-122">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="e1971-122">lastUpdatedDateTime</span></span>|<span data-ttu-id="e1971-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e1971-123">DateTimeOffset</span></span>|<span data-ttu-id="e1971-124">Время последнего обновления состояния действия</span><span class="sxs-lookup"><span data-stu-id="e1971-124">Time the action state was last updated</span></span>|

## <a name="relationships"></a><span data-ttu-id="e1971-125">Связи</span><span class="sxs-lookup"><span data-stu-id="e1971-125">Relationships</span></span>
<span data-ttu-id="e1971-126">Нет</span><span class="sxs-lookup"><span data-stu-id="e1971-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e1971-127">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e1971-127">JSON Representation</span></span>
<span data-ttu-id="e1971-128">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e1971-128">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceActionResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceActionResult",
  "actionName": "String",
  "actionState": "String",
  "startDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)"
}
```





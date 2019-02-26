---
title: Тип ресурса deviceActionResult
description: Результат действия с устройством
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d08b4285f81c7b6f7e4962c4738279f84ba37b7d
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30261049"
---
# <a name="deviceactionresult-resource-type"></a><span data-ttu-id="bbf22-103">Тип ресурса deviceActionResult</span><span class="sxs-lookup"><span data-stu-id="bbf22-103">deviceActionResult resource type</span></span>

> <span data-ttu-id="bbf22-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bbf22-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bbf22-105">Результат действия, касающегося устройства</span><span class="sxs-lookup"><span data-stu-id="bbf22-105">Device action result</span></span>

## <a name="properties"></a><span data-ttu-id="bbf22-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="bbf22-106">Properties</span></span>
|<span data-ttu-id="bbf22-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="bbf22-107">Property</span></span>|<span data-ttu-id="bbf22-108">Тип</span><span class="sxs-lookup"><span data-stu-id="bbf22-108">Type</span></span>|<span data-ttu-id="bbf22-109">Описание</span><span class="sxs-lookup"><span data-stu-id="bbf22-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bbf22-110">actionName</span><span class="sxs-lookup"><span data-stu-id="bbf22-110">actionName</span></span>|<span data-ttu-id="bbf22-111">String</span><span class="sxs-lookup"><span data-stu-id="bbf22-111">String</span></span>|<span data-ttu-id="bbf22-112">Название действия</span><span class="sxs-lookup"><span data-stu-id="bbf22-112">Action name</span></span>|
|<span data-ttu-id="bbf22-113">actionState</span><span class="sxs-lookup"><span data-stu-id="bbf22-113">actionState</span></span>|[<span data-ttu-id="bbf22-114">actionState</span><span class="sxs-lookup"><span data-stu-id="bbf22-114">actionState</span></span>](../resources/intune-devices-actionstate.md)|<span data-ttu-id="bbf22-115">Состояние действия.</span><span class="sxs-lookup"><span data-stu-id="bbf22-115">State of the action.</span></span> <span data-ttu-id="bbf22-116">Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="bbf22-116">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="bbf22-117">startDateTime</span><span class="sxs-lookup"><span data-stu-id="bbf22-117">startDateTime</span></span>|<span data-ttu-id="bbf22-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bbf22-118">DateTimeOffset</span></span>|<span data-ttu-id="bbf22-119">Время начала действия</span><span class="sxs-lookup"><span data-stu-id="bbf22-119">Time the action was initiated</span></span>|
|<span data-ttu-id="bbf22-120">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="bbf22-120">lastUpdatedDateTime</span></span>|<span data-ttu-id="bbf22-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bbf22-121">DateTimeOffset</span></span>|<span data-ttu-id="bbf22-122">Время последнего обновления состояния действия</span><span class="sxs-lookup"><span data-stu-id="bbf22-122">Time the action state was last updated</span></span>|

## <a name="relationships"></a><span data-ttu-id="bbf22-123">Связи</span><span class="sxs-lookup"><span data-stu-id="bbf22-123">Relationships</span></span>
<span data-ttu-id="bbf22-124">Нет</span><span class="sxs-lookup"><span data-stu-id="bbf22-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bbf22-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bbf22-125">JSON Representation</span></span>
<span data-ttu-id="bbf22-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bbf22-126">Here is a JSON representation of the resource.</span></span>
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




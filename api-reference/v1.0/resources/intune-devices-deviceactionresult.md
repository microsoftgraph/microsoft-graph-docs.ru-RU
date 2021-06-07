---
title: Тип ресурса deviceActionResult
description: Результат действия с устройством
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 808d9e559494338a7831626fd6d4d77f20092dcb
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52755779"
---
# <a name="deviceactionresult-resource-type"></a><span data-ttu-id="b0a7a-103">Тип ресурса deviceActionResult</span><span class="sxs-lookup"><span data-stu-id="b0a7a-103">deviceActionResult resource type</span></span>

<span data-ttu-id="b0a7a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b0a7a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b0a7a-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b0a7a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b0a7a-106">Результат действия, касающегося устройства</span><span class="sxs-lookup"><span data-stu-id="b0a7a-106">Device action result</span></span>

## <a name="properties"></a><span data-ttu-id="b0a7a-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="b0a7a-107">Properties</span></span>
|<span data-ttu-id="b0a7a-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="b0a7a-108">Property</span></span>|<span data-ttu-id="b0a7a-109">Тип</span><span class="sxs-lookup"><span data-stu-id="b0a7a-109">Type</span></span>|<span data-ttu-id="b0a7a-110">Описание</span><span class="sxs-lookup"><span data-stu-id="b0a7a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b0a7a-111">actionName</span><span class="sxs-lookup"><span data-stu-id="b0a7a-111">actionName</span></span>|<span data-ttu-id="b0a7a-112">String</span><span class="sxs-lookup"><span data-stu-id="b0a7a-112">String</span></span>|<span data-ttu-id="b0a7a-113">Название действия</span><span class="sxs-lookup"><span data-stu-id="b0a7a-113">Action name</span></span>|
|<span data-ttu-id="b0a7a-114">actionState</span><span class="sxs-lookup"><span data-stu-id="b0a7a-114">actionState</span></span>|[<span data-ttu-id="b0a7a-115">actionState</span><span class="sxs-lookup"><span data-stu-id="b0a7a-115">actionState</span></span>](../resources/intune-devices-actionstate.md)|<span data-ttu-id="b0a7a-116">Состояние действия.</span><span class="sxs-lookup"><span data-stu-id="b0a7a-116">State of the action.</span></span> <span data-ttu-id="b0a7a-117">Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="b0a7a-117">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="b0a7a-118">startDateTime</span><span class="sxs-lookup"><span data-stu-id="b0a7a-118">startDateTime</span></span>|<span data-ttu-id="b0a7a-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b0a7a-119">DateTimeOffset</span></span>|<span data-ttu-id="b0a7a-120">Время начала действия</span><span class="sxs-lookup"><span data-stu-id="b0a7a-120">Time the action was initiated</span></span>|
|<span data-ttu-id="b0a7a-121">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="b0a7a-121">lastUpdatedDateTime</span></span>|<span data-ttu-id="b0a7a-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b0a7a-122">DateTimeOffset</span></span>|<span data-ttu-id="b0a7a-123">Время последнего обновления состояния действия</span><span class="sxs-lookup"><span data-stu-id="b0a7a-123">Time the action state was last updated</span></span>|

## <a name="relationships"></a><span data-ttu-id="b0a7a-124">Отношения</span><span class="sxs-lookup"><span data-stu-id="b0a7a-124">Relationships</span></span>
<span data-ttu-id="b0a7a-125">Нет</span><span class="sxs-lookup"><span data-stu-id="b0a7a-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b0a7a-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b0a7a-126">JSON Representation</span></span>
<span data-ttu-id="b0a7a-127">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b0a7a-127">Here is a JSON representation of the resource.</span></span>
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





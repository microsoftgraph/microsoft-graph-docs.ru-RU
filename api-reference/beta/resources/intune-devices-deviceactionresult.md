---
title: Тип ресурса deviceActionResult
description: Результат действия с устройством
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c187a8b40fcafc9e79331544cb1df468012e79e4
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42785016"
---
# <a name="deviceactionresult-resource-type"></a><span data-ttu-id="a186b-103">Тип ресурса deviceActionResult</span><span class="sxs-lookup"><span data-stu-id="a186b-103">deviceActionResult resource type</span></span>

> <span data-ttu-id="a186b-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a186b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a186b-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a186b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a186b-106">Результат действия, касающегося устройства</span><span class="sxs-lookup"><span data-stu-id="a186b-106">Device action result</span></span>

## <a name="properties"></a><span data-ttu-id="a186b-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="a186b-107">Properties</span></span>
|<span data-ttu-id="a186b-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="a186b-108">Property</span></span>|<span data-ttu-id="a186b-109">Тип</span><span class="sxs-lookup"><span data-stu-id="a186b-109">Type</span></span>|<span data-ttu-id="a186b-110">Описание</span><span class="sxs-lookup"><span data-stu-id="a186b-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a186b-111">actionName</span><span class="sxs-lookup"><span data-stu-id="a186b-111">actionName</span></span>|<span data-ttu-id="a186b-112">String</span><span class="sxs-lookup"><span data-stu-id="a186b-112">String</span></span>|<span data-ttu-id="a186b-113">Название действия</span><span class="sxs-lookup"><span data-stu-id="a186b-113">Action name</span></span>|
|<span data-ttu-id="a186b-114">actionState</span><span class="sxs-lookup"><span data-stu-id="a186b-114">actionState</span></span>|[<span data-ttu-id="a186b-115">actionState</span><span class="sxs-lookup"><span data-stu-id="a186b-115">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="a186b-116">Состояние действия.</span><span class="sxs-lookup"><span data-stu-id="a186b-116">State of the action.</span></span> <span data-ttu-id="a186b-117">Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="a186b-117">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="a186b-118">startDateTime</span><span class="sxs-lookup"><span data-stu-id="a186b-118">startDateTime</span></span>|<span data-ttu-id="a186b-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a186b-119">DateTimeOffset</span></span>|<span data-ttu-id="a186b-120">Время начала действия</span><span class="sxs-lookup"><span data-stu-id="a186b-120">Time the action was initiated</span></span>|
|<span data-ttu-id="a186b-121">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="a186b-121">lastUpdatedDateTime</span></span>|<span data-ttu-id="a186b-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a186b-122">DateTimeOffset</span></span>|<span data-ttu-id="a186b-123">Время последнего обновления состояния действия</span><span class="sxs-lookup"><span data-stu-id="a186b-123">Time the action state was last updated</span></span>|

## <a name="relationships"></a><span data-ttu-id="a186b-124">Связи</span><span class="sxs-lookup"><span data-stu-id="a186b-124">Relationships</span></span>
<span data-ttu-id="a186b-125">Нет</span><span class="sxs-lookup"><span data-stu-id="a186b-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a186b-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a186b-126">JSON Representation</span></span>
<span data-ttu-id="a186b-127">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a186b-127">Here is a JSON representation of the resource.</span></span>
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




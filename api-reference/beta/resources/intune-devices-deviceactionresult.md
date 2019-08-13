---
title: Тип ресурса deviceActionResult
description: Результат действия с устройством
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 5cad8171e2c85a719c485e0fc7beec38d71e2e03
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36370181"
---
# <a name="deviceactionresult-resource-type"></a><span data-ttu-id="5a54f-103">Тип ресурса deviceActionResult</span><span class="sxs-lookup"><span data-stu-id="5a54f-103">deviceActionResult resource type</span></span>

> <span data-ttu-id="5a54f-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5a54f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5a54f-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5a54f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5a54f-106">Результат действия, касающегося устройства</span><span class="sxs-lookup"><span data-stu-id="5a54f-106">Device action result</span></span>

## <a name="properties"></a><span data-ttu-id="5a54f-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="5a54f-107">Properties</span></span>
|<span data-ttu-id="5a54f-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="5a54f-108">Property</span></span>|<span data-ttu-id="5a54f-109">Тип</span><span class="sxs-lookup"><span data-stu-id="5a54f-109">Type</span></span>|<span data-ttu-id="5a54f-110">Описание</span><span class="sxs-lookup"><span data-stu-id="5a54f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5a54f-111">actionName</span><span class="sxs-lookup"><span data-stu-id="5a54f-111">actionName</span></span>|<span data-ttu-id="5a54f-112">String</span><span class="sxs-lookup"><span data-stu-id="5a54f-112">String</span></span>|<span data-ttu-id="5a54f-113">Название действия</span><span class="sxs-lookup"><span data-stu-id="5a54f-113">Action name</span></span>|
|<span data-ttu-id="5a54f-114">actionState</span><span class="sxs-lookup"><span data-stu-id="5a54f-114">actionState</span></span>|[<span data-ttu-id="5a54f-115">actionState</span><span class="sxs-lookup"><span data-stu-id="5a54f-115">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="5a54f-116">Состояние действия.</span><span class="sxs-lookup"><span data-stu-id="5a54f-116">State of the action.</span></span> <span data-ttu-id="5a54f-117">Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="5a54f-117">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="5a54f-118">startDateTime</span><span class="sxs-lookup"><span data-stu-id="5a54f-118">startDateTime</span></span>|<span data-ttu-id="5a54f-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5a54f-119">DateTimeOffset</span></span>|<span data-ttu-id="5a54f-120">Время начала действия</span><span class="sxs-lookup"><span data-stu-id="5a54f-120">Time the action was initiated</span></span>|
|<span data-ttu-id="5a54f-121">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="5a54f-121">lastUpdatedDateTime</span></span>|<span data-ttu-id="5a54f-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5a54f-122">DateTimeOffset</span></span>|<span data-ttu-id="5a54f-123">Время последнего обновления состояния действия</span><span class="sxs-lookup"><span data-stu-id="5a54f-123">Time the action state was last updated</span></span>|

## <a name="relationships"></a><span data-ttu-id="5a54f-124">Отношения</span><span class="sxs-lookup"><span data-stu-id="5a54f-124">Relationships</span></span>
<span data-ttu-id="5a54f-125">Нет</span><span class="sxs-lookup"><span data-stu-id="5a54f-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5a54f-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5a54f-126">JSON Representation</span></span>
<span data-ttu-id="5a54f-127">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5a54f-127">Here is a JSON representation of the resource.</span></span>
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




---
title: Тип ресурса vppTokenActionResult
description: Состояние действия, выполняемого с помощью маркера Apple Volume Purchase Program.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b840d37963d8d8b56b0fe2ecd461b32f12368ae5
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36373576"
---
# <a name="vpptokenactionresult-resource-type"></a><span data-ttu-id="7ba66-103">Тип ресурса vppTokenActionResult</span><span class="sxs-lookup"><span data-stu-id="7ba66-103">vppTokenActionResult resource type</span></span>

> <span data-ttu-id="7ba66-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7ba66-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7ba66-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7ba66-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7ba66-106">Состояние действия, выполняемого с помощью маркера Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="7ba66-106">The status of the action performed with an Apple Volume Purchase Program token.</span></span>

## <a name="properties"></a><span data-ttu-id="7ba66-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="7ba66-107">Properties</span></span>
|<span data-ttu-id="7ba66-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="7ba66-108">Property</span></span>|<span data-ttu-id="7ba66-109">Тип</span><span class="sxs-lookup"><span data-stu-id="7ba66-109">Type</span></span>|<span data-ttu-id="7ba66-110">Описание</span><span class="sxs-lookup"><span data-stu-id="7ba66-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7ba66-111">actionName</span><span class="sxs-lookup"><span data-stu-id="7ba66-111">actionName</span></span>|<span data-ttu-id="7ba66-112">String</span><span class="sxs-lookup"><span data-stu-id="7ba66-112">String</span></span>|<span data-ttu-id="7ba66-113">Название действия</span><span class="sxs-lookup"><span data-stu-id="7ba66-113">Action name</span></span>|
|<span data-ttu-id="7ba66-114">actionState</span><span class="sxs-lookup"><span data-stu-id="7ba66-114">actionState</span></span>|[<span data-ttu-id="7ba66-115">actionState</span><span class="sxs-lookup"><span data-stu-id="7ba66-115">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="7ba66-116">Состояние действия.</span><span class="sxs-lookup"><span data-stu-id="7ba66-116">State of the action.</span></span> <span data-ttu-id="7ba66-117">Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="7ba66-117">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="7ba66-118">startDateTime</span><span class="sxs-lookup"><span data-stu-id="7ba66-118">startDateTime</span></span>|<span data-ttu-id="7ba66-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7ba66-119">DateTimeOffset</span></span>|<span data-ttu-id="7ba66-120">Время начала действия</span><span class="sxs-lookup"><span data-stu-id="7ba66-120">Time the action was initiated</span></span>|
|<span data-ttu-id="7ba66-121">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="7ba66-121">lastUpdatedDateTime</span></span>|<span data-ttu-id="7ba66-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7ba66-122">DateTimeOffset</span></span>|<span data-ttu-id="7ba66-123">Время последнего обновления состояния действия</span><span class="sxs-lookup"><span data-stu-id="7ba66-123">Time the action state was last updated</span></span>|

## <a name="relationships"></a><span data-ttu-id="7ba66-124">Отношения</span><span class="sxs-lookup"><span data-stu-id="7ba66-124">Relationships</span></span>
<span data-ttu-id="7ba66-125">Нет</span><span class="sxs-lookup"><span data-stu-id="7ba66-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7ba66-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7ba66-126">JSON Representation</span></span>
<span data-ttu-id="7ba66-127">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7ba66-127">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.vppTokenActionResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vppTokenActionResult",
  "actionName": "String",
  "actionState": "String",
  "startDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)"
}
```




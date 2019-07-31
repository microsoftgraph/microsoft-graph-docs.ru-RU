---
title: Тип ресурса vppTokenActionResult
description: Состояние действия, выполняемого с помощью маркера Apple Volume Purchase Program.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 7195289f52a13d327d98aad1c93fbab622f9960b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36010660"
---
# <a name="vpptokenactionresult-resource-type"></a><span data-ttu-id="1ceaf-103">Тип ресурса vppTokenActionResult</span><span class="sxs-lookup"><span data-stu-id="1ceaf-103">vppTokenActionResult resource type</span></span>

> <span data-ttu-id="1ceaf-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1ceaf-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1ceaf-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1ceaf-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1ceaf-106">Состояние действия, выполняемого с помощью маркера Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="1ceaf-106">The status of the action performed with an Apple Volume Purchase Program token.</span></span>

## <a name="properties"></a><span data-ttu-id="1ceaf-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="1ceaf-107">Properties</span></span>
|<span data-ttu-id="1ceaf-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="1ceaf-108">Property</span></span>|<span data-ttu-id="1ceaf-109">Тип</span><span class="sxs-lookup"><span data-stu-id="1ceaf-109">Type</span></span>|<span data-ttu-id="1ceaf-110">Описание</span><span class="sxs-lookup"><span data-stu-id="1ceaf-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1ceaf-111">actionName</span><span class="sxs-lookup"><span data-stu-id="1ceaf-111">actionName</span></span>|<span data-ttu-id="1ceaf-112">String</span><span class="sxs-lookup"><span data-stu-id="1ceaf-112">String</span></span>|<span data-ttu-id="1ceaf-113">Название действия</span><span class="sxs-lookup"><span data-stu-id="1ceaf-113">Action name</span></span>|
|<span data-ttu-id="1ceaf-114">actionState</span><span class="sxs-lookup"><span data-stu-id="1ceaf-114">actionState</span></span>|[<span data-ttu-id="1ceaf-115">actionState</span><span class="sxs-lookup"><span data-stu-id="1ceaf-115">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="1ceaf-116">Состояние действия.</span><span class="sxs-lookup"><span data-stu-id="1ceaf-116">State of the action.</span></span> <span data-ttu-id="1ceaf-117">Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="1ceaf-117">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="1ceaf-118">startDateTime</span><span class="sxs-lookup"><span data-stu-id="1ceaf-118">startDateTime</span></span>|<span data-ttu-id="1ceaf-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1ceaf-119">DateTimeOffset</span></span>|<span data-ttu-id="1ceaf-120">Время начала действия</span><span class="sxs-lookup"><span data-stu-id="1ceaf-120">Time the action was initiated</span></span>|
|<span data-ttu-id="1ceaf-121">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="1ceaf-121">lastUpdatedDateTime</span></span>|<span data-ttu-id="1ceaf-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1ceaf-122">DateTimeOffset</span></span>|<span data-ttu-id="1ceaf-123">Время последнего обновления состояния действия</span><span class="sxs-lookup"><span data-stu-id="1ceaf-123">Time the action state was last updated</span></span>|

## <a name="relationships"></a><span data-ttu-id="1ceaf-124">Отношения</span><span class="sxs-lookup"><span data-stu-id="1ceaf-124">Relationships</span></span>
<span data-ttu-id="1ceaf-125">Нет</span><span class="sxs-lookup"><span data-stu-id="1ceaf-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1ceaf-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1ceaf-126">JSON Representation</span></span>
<span data-ttu-id="1ceaf-127">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1ceaf-127">Here is a JSON representation of the resource.</span></span>
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






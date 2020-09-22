---
title: Тип ресурса vppTokenActionResult
description: Состояние действия, выполняемого с помощью маркера Apple Volume Purchase Program.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 0cc4856901af4f97fde87acc57916742a27186ce
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48029353"
---
# <a name="vpptokenactionresult-resource-type"></a><span data-ttu-id="d7d35-103">Тип ресурса vppTokenActionResult</span><span class="sxs-lookup"><span data-stu-id="d7d35-103">vppTokenActionResult resource type</span></span>

<span data-ttu-id="d7d35-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d7d35-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d7d35-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d7d35-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d7d35-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d7d35-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d7d35-107">Состояние действия, выполняемого с помощью маркера Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="d7d35-107">The status of the action performed with an Apple Volume Purchase Program token.</span></span>

## <a name="properties"></a><span data-ttu-id="d7d35-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="d7d35-108">Properties</span></span>
|<span data-ttu-id="d7d35-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="d7d35-109">Property</span></span>|<span data-ttu-id="d7d35-110">Тип</span><span class="sxs-lookup"><span data-stu-id="d7d35-110">Type</span></span>|<span data-ttu-id="d7d35-111">Описание</span><span class="sxs-lookup"><span data-stu-id="d7d35-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d7d35-112">actionName</span><span class="sxs-lookup"><span data-stu-id="d7d35-112">actionName</span></span>|<span data-ttu-id="d7d35-113">String</span><span class="sxs-lookup"><span data-stu-id="d7d35-113">String</span></span>|<span data-ttu-id="d7d35-114">Название действия</span><span class="sxs-lookup"><span data-stu-id="d7d35-114">Action name</span></span>|
|<span data-ttu-id="d7d35-115">actionState</span><span class="sxs-lookup"><span data-stu-id="d7d35-115">actionState</span></span>|[<span data-ttu-id="d7d35-116">actionState</span><span class="sxs-lookup"><span data-stu-id="d7d35-116">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="d7d35-117">Состояние действия.</span><span class="sxs-lookup"><span data-stu-id="d7d35-117">State of the action.</span></span> <span data-ttu-id="d7d35-118">Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="d7d35-118">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="d7d35-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="d7d35-119">startDateTime</span></span>|<span data-ttu-id="d7d35-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d7d35-120">DateTimeOffset</span></span>|<span data-ttu-id="d7d35-121">Время начала действия</span><span class="sxs-lookup"><span data-stu-id="d7d35-121">Time the action was initiated</span></span>|
|<span data-ttu-id="d7d35-122">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="d7d35-122">lastUpdatedDateTime</span></span>|<span data-ttu-id="d7d35-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d7d35-123">DateTimeOffset</span></span>|<span data-ttu-id="d7d35-124">Время последнего обновления состояния действия</span><span class="sxs-lookup"><span data-stu-id="d7d35-124">Time the action state was last updated</span></span>|

## <a name="relationships"></a><span data-ttu-id="d7d35-125">Отношения</span><span class="sxs-lookup"><span data-stu-id="d7d35-125">Relationships</span></span>
<span data-ttu-id="d7d35-126">Нет</span><span class="sxs-lookup"><span data-stu-id="d7d35-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d7d35-127">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d7d35-127">JSON Representation</span></span>
<span data-ttu-id="d7d35-128">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d7d35-128">Here is a JSON representation of the resource.</span></span>
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







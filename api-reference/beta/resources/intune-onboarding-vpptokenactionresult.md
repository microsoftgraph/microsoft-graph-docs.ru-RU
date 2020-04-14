---
title: Тип ресурса vppTokenActionResult
description: Состояние действия, выполняемого с помощью маркера Apple Volume Purchase Program.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ff272e6dea9a4778c9f2cb33f3c59f411b257da7
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43446839"
---
# <a name="vpptokenactionresult-resource-type"></a><span data-ttu-id="9b03b-103">Тип ресурса vppTokenActionResult</span><span class="sxs-lookup"><span data-stu-id="9b03b-103">vppTokenActionResult resource type</span></span>

<span data-ttu-id="9b03b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9b03b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9b03b-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9b03b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9b03b-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9b03b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9b03b-107">Состояние действия, выполняемого с помощью маркера Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="9b03b-107">The status of the action performed with an Apple Volume Purchase Program token.</span></span>

## <a name="properties"></a><span data-ttu-id="9b03b-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="9b03b-108">Properties</span></span>
|<span data-ttu-id="9b03b-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="9b03b-109">Property</span></span>|<span data-ttu-id="9b03b-110">Тип</span><span class="sxs-lookup"><span data-stu-id="9b03b-110">Type</span></span>|<span data-ttu-id="9b03b-111">Описание</span><span class="sxs-lookup"><span data-stu-id="9b03b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9b03b-112">actionName</span><span class="sxs-lookup"><span data-stu-id="9b03b-112">actionName</span></span>|<span data-ttu-id="9b03b-113">String</span><span class="sxs-lookup"><span data-stu-id="9b03b-113">String</span></span>|<span data-ttu-id="9b03b-114">Название действия</span><span class="sxs-lookup"><span data-stu-id="9b03b-114">Action name</span></span>|
|<span data-ttu-id="9b03b-115">actionState</span><span class="sxs-lookup"><span data-stu-id="9b03b-115">actionState</span></span>|[<span data-ttu-id="9b03b-116">actionState</span><span class="sxs-lookup"><span data-stu-id="9b03b-116">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="9b03b-117">Состояние действия.</span><span class="sxs-lookup"><span data-stu-id="9b03b-117">State of the action.</span></span> <span data-ttu-id="9b03b-118">Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="9b03b-118">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="9b03b-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="9b03b-119">startDateTime</span></span>|<span data-ttu-id="9b03b-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9b03b-120">DateTimeOffset</span></span>|<span data-ttu-id="9b03b-121">Время начала действия</span><span class="sxs-lookup"><span data-stu-id="9b03b-121">Time the action was initiated</span></span>|
|<span data-ttu-id="9b03b-122">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="9b03b-122">lastUpdatedDateTime</span></span>|<span data-ttu-id="9b03b-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9b03b-123">DateTimeOffset</span></span>|<span data-ttu-id="9b03b-124">Время последнего обновления состояния действия</span><span class="sxs-lookup"><span data-stu-id="9b03b-124">Time the action state was last updated</span></span>|

## <a name="relationships"></a><span data-ttu-id="9b03b-125">Связи</span><span class="sxs-lookup"><span data-stu-id="9b03b-125">Relationships</span></span>
<span data-ttu-id="9b03b-126">Нет</span><span class="sxs-lookup"><span data-stu-id="9b03b-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9b03b-127">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9b03b-127">JSON Representation</span></span>
<span data-ttu-id="9b03b-128">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9b03b-128">Here is a JSON representation of the resource.</span></span>
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




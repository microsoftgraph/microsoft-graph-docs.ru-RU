---
title: Тип ресурса vppTokenActionResult
description: Состояние действия, выполняемого с помощью маркера Apple Volume Purchase Program.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 87394bfebdda564a4f6eff1ff0efff077f681fbf
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48703630"
---
# <a name="vpptokenactionresult-resource-type"></a><span data-ttu-id="4898c-103">Тип ресурса vppTokenActionResult</span><span class="sxs-lookup"><span data-stu-id="4898c-103">vppTokenActionResult resource type</span></span>

<span data-ttu-id="4898c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4898c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4898c-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4898c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4898c-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4898c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4898c-107">Состояние действия, выполняемого с помощью маркера Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="4898c-107">The status of the action performed with an Apple Volume Purchase Program token.</span></span>

## <a name="properties"></a><span data-ttu-id="4898c-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="4898c-108">Properties</span></span>
|<span data-ttu-id="4898c-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="4898c-109">Property</span></span>|<span data-ttu-id="4898c-110">Тип</span><span class="sxs-lookup"><span data-stu-id="4898c-110">Type</span></span>|<span data-ttu-id="4898c-111">Описание</span><span class="sxs-lookup"><span data-stu-id="4898c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4898c-112">actionName</span><span class="sxs-lookup"><span data-stu-id="4898c-112">actionName</span></span>|<span data-ttu-id="4898c-113">String</span><span class="sxs-lookup"><span data-stu-id="4898c-113">String</span></span>|<span data-ttu-id="4898c-114">Название действия</span><span class="sxs-lookup"><span data-stu-id="4898c-114">Action name</span></span>|
|<span data-ttu-id="4898c-115">actionState</span><span class="sxs-lookup"><span data-stu-id="4898c-115">actionState</span></span>|[<span data-ttu-id="4898c-116">actionState</span><span class="sxs-lookup"><span data-stu-id="4898c-116">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="4898c-117">Состояние действия.</span><span class="sxs-lookup"><span data-stu-id="4898c-117">State of the action.</span></span> <span data-ttu-id="4898c-118">Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="4898c-118">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="4898c-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="4898c-119">startDateTime</span></span>|<span data-ttu-id="4898c-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4898c-120">DateTimeOffset</span></span>|<span data-ttu-id="4898c-121">Время начала действия</span><span class="sxs-lookup"><span data-stu-id="4898c-121">Time the action was initiated</span></span>|
|<span data-ttu-id="4898c-122">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="4898c-122">lastUpdatedDateTime</span></span>|<span data-ttu-id="4898c-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4898c-123">DateTimeOffset</span></span>|<span data-ttu-id="4898c-124">Время последнего обновления состояния действия</span><span class="sxs-lookup"><span data-stu-id="4898c-124">Time the action state was last updated</span></span>|

## <a name="relationships"></a><span data-ttu-id="4898c-125">Связи</span><span class="sxs-lookup"><span data-stu-id="4898c-125">Relationships</span></span>
<span data-ttu-id="4898c-126">Нет</span><span class="sxs-lookup"><span data-stu-id="4898c-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4898c-127">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4898c-127">JSON Representation</span></span>
<span data-ttu-id="4898c-128">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4898c-128">Here is a JSON representation of the resource.</span></span>
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






---
title: Тип ресурса vppTokenActionResult
description: Состояние действия выполняется с маркером покупки программы корпоративного Apple.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 2fb78ea991ed43bd100a424ea7ddd7e23b22412d
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29414293"
---
# <a name="vpptokenactionresult-resource-type"></a><span data-ttu-id="f54b9-103">Тип ресурса vppTokenActionResult</span><span class="sxs-lookup"><span data-stu-id="f54b9-103">vppTokenActionResult resource type</span></span>

> <span data-ttu-id="f54b9-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="f54b9-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="f54b9-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f54b9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f54b9-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f54b9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f54b9-107">Состояние действия выполняется с маркером покупки программы корпоративного Apple.</span><span class="sxs-lookup"><span data-stu-id="f54b9-107">The status of the action performed with an Apple Volume Purchase Program token.</span></span>

## <a name="properties"></a><span data-ttu-id="f54b9-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="f54b9-108">Properties</span></span>
|<span data-ttu-id="f54b9-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="f54b9-109">Property</span></span>|<span data-ttu-id="f54b9-110">Тип</span><span class="sxs-lookup"><span data-stu-id="f54b9-110">Type</span></span>|<span data-ttu-id="f54b9-111">Описание</span><span class="sxs-lookup"><span data-stu-id="f54b9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f54b9-112">actionName</span><span class="sxs-lookup"><span data-stu-id="f54b9-112">actionName</span></span>|<span data-ttu-id="f54b9-113">String</span><span class="sxs-lookup"><span data-stu-id="f54b9-113">String</span></span>|<span data-ttu-id="f54b9-114">Название действия</span><span class="sxs-lookup"><span data-stu-id="f54b9-114">Action name</span></span>|
|<span data-ttu-id="f54b9-115">actionState</span><span class="sxs-lookup"><span data-stu-id="f54b9-115">actionState</span></span>|[<span data-ttu-id="f54b9-116">actionState</span><span class="sxs-lookup"><span data-stu-id="f54b9-116">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="f54b9-117">Состояние действия.</span><span class="sxs-lookup"><span data-stu-id="f54b9-117">State of the action.</span></span> <span data-ttu-id="f54b9-118">Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="f54b9-118">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="f54b9-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="f54b9-119">startDateTime</span></span>|<span data-ttu-id="f54b9-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f54b9-120">DateTimeOffset</span></span>|<span data-ttu-id="f54b9-121">Время начала действия</span><span class="sxs-lookup"><span data-stu-id="f54b9-121">Time the action was initiated</span></span>|
|<span data-ttu-id="f54b9-122">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="f54b9-122">lastUpdatedDateTime</span></span>|<span data-ttu-id="f54b9-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f54b9-123">DateTimeOffset</span></span>|<span data-ttu-id="f54b9-124">Время последнего обновления состояния действия</span><span class="sxs-lookup"><span data-stu-id="f54b9-124">Time the action state was last updated</span></span>|

## <a name="relationships"></a><span data-ttu-id="f54b9-125">Связи</span><span class="sxs-lookup"><span data-stu-id="f54b9-125">Relationships</span></span>
<span data-ttu-id="f54b9-126">Нет</span><span class="sxs-lookup"><span data-stu-id="f54b9-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f54b9-127">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f54b9-127">JSON Representation</span></span>
<span data-ttu-id="f54b9-128">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f54b9-128">Here is a JSON representation of the resource.</span></span>
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





---
title: Тип ресурса deviceActionResult
description: Результат действия с устройством
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 8ff7a02d9bace4e686f77c1173569360af1145b3
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48060568"
---
# <a name="deviceactionresult-resource-type"></a><span data-ttu-id="cef8b-103">Тип ресурса deviceActionResult</span><span class="sxs-lookup"><span data-stu-id="cef8b-103">deviceActionResult resource type</span></span>

<span data-ttu-id="cef8b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cef8b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cef8b-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cef8b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cef8b-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="cef8b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cef8b-107">Результат действия, касающегося устройства</span><span class="sxs-lookup"><span data-stu-id="cef8b-107">Device action result</span></span>

## <a name="properties"></a><span data-ttu-id="cef8b-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="cef8b-108">Properties</span></span>
|<span data-ttu-id="cef8b-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="cef8b-109">Property</span></span>|<span data-ttu-id="cef8b-110">Тип</span><span class="sxs-lookup"><span data-stu-id="cef8b-110">Type</span></span>|<span data-ttu-id="cef8b-111">Описание</span><span class="sxs-lookup"><span data-stu-id="cef8b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cef8b-112">actionName</span><span class="sxs-lookup"><span data-stu-id="cef8b-112">actionName</span></span>|<span data-ttu-id="cef8b-113">String</span><span class="sxs-lookup"><span data-stu-id="cef8b-113">String</span></span>|<span data-ttu-id="cef8b-114">Название действия</span><span class="sxs-lookup"><span data-stu-id="cef8b-114">Action name</span></span>|
|<span data-ttu-id="cef8b-115">actionState</span><span class="sxs-lookup"><span data-stu-id="cef8b-115">actionState</span></span>|[<span data-ttu-id="cef8b-116">actionState</span><span class="sxs-lookup"><span data-stu-id="cef8b-116">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="cef8b-117">Состояние действия.</span><span class="sxs-lookup"><span data-stu-id="cef8b-117">State of the action.</span></span> <span data-ttu-id="cef8b-118">Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="cef8b-118">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="cef8b-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="cef8b-119">startDateTime</span></span>|<span data-ttu-id="cef8b-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cef8b-120">DateTimeOffset</span></span>|<span data-ttu-id="cef8b-121">Время начала действия</span><span class="sxs-lookup"><span data-stu-id="cef8b-121">Time the action was initiated</span></span>|
|<span data-ttu-id="cef8b-122">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="cef8b-122">lastUpdatedDateTime</span></span>|<span data-ttu-id="cef8b-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cef8b-123">DateTimeOffset</span></span>|<span data-ttu-id="cef8b-124">Время последнего обновления состояния действия</span><span class="sxs-lookup"><span data-stu-id="cef8b-124">Time the action state was last updated</span></span>|

## <a name="relationships"></a><span data-ttu-id="cef8b-125">Связи</span><span class="sxs-lookup"><span data-stu-id="cef8b-125">Relationships</span></span>
<span data-ttu-id="cef8b-126">Нет</span><span class="sxs-lookup"><span data-stu-id="cef8b-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="cef8b-127">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="cef8b-127">JSON Representation</span></span>
<span data-ttu-id="cef8b-128">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cef8b-128">Here is a JSON representation of the resource.</span></span>
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







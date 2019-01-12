---
title: Тип ресурса deviceActionResult
description: Результат действия, касающегося устройства
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 22fd8e1bc338191bba54ba9f655f03899054ae86
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27912304"
---
# <a name="deviceactionresult-resource-type"></a><span data-ttu-id="1ea46-103">Тип ресурса deviceActionResult</span><span class="sxs-lookup"><span data-stu-id="1ea46-103">deviceActionResult resource type</span></span>

> <span data-ttu-id="1ea46-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="1ea46-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1ea46-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1ea46-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1ea46-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="1ea46-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1ea46-107">Результат действия, касающегося устройства</span><span class="sxs-lookup"><span data-stu-id="1ea46-107">Device action result</span></span>
## <a name="properties"></a><span data-ttu-id="1ea46-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="1ea46-108">Properties</span></span>
|<span data-ttu-id="1ea46-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="1ea46-109">Property</span></span>|<span data-ttu-id="1ea46-110">Тип</span><span class="sxs-lookup"><span data-stu-id="1ea46-110">Type</span></span>|<span data-ttu-id="1ea46-111">Описание</span><span class="sxs-lookup"><span data-stu-id="1ea46-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1ea46-112">actionName</span><span class="sxs-lookup"><span data-stu-id="1ea46-112">actionName</span></span>|<span data-ttu-id="1ea46-113">String</span><span class="sxs-lookup"><span data-stu-id="1ea46-113">String</span></span>|<span data-ttu-id="1ea46-114">Название действия</span><span class="sxs-lookup"><span data-stu-id="1ea46-114">Action name</span></span>|
|<span data-ttu-id="1ea46-115">actionState</span><span class="sxs-lookup"><span data-stu-id="1ea46-115">actionState</span></span>|[<span data-ttu-id="1ea46-116">actionState</span><span class="sxs-lookup"><span data-stu-id="1ea46-116">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="1ea46-117">Состояние действия.</span><span class="sxs-lookup"><span data-stu-id="1ea46-117">State of the action.</span></span> <span data-ttu-id="1ea46-118">Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="1ea46-118">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="1ea46-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="1ea46-119">startDateTime</span></span>|<span data-ttu-id="1ea46-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1ea46-120">DateTimeOffset</span></span>|<span data-ttu-id="1ea46-121">Время начала действия</span><span class="sxs-lookup"><span data-stu-id="1ea46-121">Time the action was initiated</span></span>|
|<span data-ttu-id="1ea46-122">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="1ea46-122">lastUpdatedDateTime</span></span>|<span data-ttu-id="1ea46-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1ea46-123">DateTimeOffset</span></span>|<span data-ttu-id="1ea46-124">Время последнего обновления состояния действия</span><span class="sxs-lookup"><span data-stu-id="1ea46-124">Time the action state was last updated</span></span>|

## <a name="relationships"></a><span data-ttu-id="1ea46-125">Связи</span><span class="sxs-lookup"><span data-stu-id="1ea46-125">Relationships</span></span>
<span data-ttu-id="1ea46-126">Нет</span><span class="sxs-lookup"><span data-stu-id="1ea46-126">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="1ea46-127">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1ea46-127">JSON Representation</span></span>
<span data-ttu-id="1ea46-128">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1ea46-128">Here is a JSON representation of the resource.</span></span>
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






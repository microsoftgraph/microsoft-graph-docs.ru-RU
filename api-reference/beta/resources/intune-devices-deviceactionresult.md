---
title: Тип ресурса deviceActionResult
description: Результат действия, касающегося устройства
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 051d5f381e27e4901f7e2fb9280cea3dc0bb71c4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27806106"
---
# <a name="deviceactionresult-resource-type"></a><span data-ttu-id="b9cec-103">Тип ресурса deviceActionResult</span><span class="sxs-lookup"><span data-stu-id="b9cec-103">deviceActionResult resource type</span></span>

> <span data-ttu-id="b9cec-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="b9cec-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b9cec-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b9cec-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b9cec-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="b9cec-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b9cec-107">Результат действия, касающегося устройства</span><span class="sxs-lookup"><span data-stu-id="b9cec-107">Device action result</span></span>
## <a name="properties"></a><span data-ttu-id="b9cec-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="b9cec-108">Properties</span></span>
|<span data-ttu-id="b9cec-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="b9cec-109">Property</span></span>|<span data-ttu-id="b9cec-110">Тип</span><span class="sxs-lookup"><span data-stu-id="b9cec-110">Type</span></span>|<span data-ttu-id="b9cec-111">Описание</span><span class="sxs-lookup"><span data-stu-id="b9cec-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b9cec-112">actionName</span><span class="sxs-lookup"><span data-stu-id="b9cec-112">actionName</span></span>|<span data-ttu-id="b9cec-113">String</span><span class="sxs-lookup"><span data-stu-id="b9cec-113">String</span></span>|<span data-ttu-id="b9cec-114">Название действия</span><span class="sxs-lookup"><span data-stu-id="b9cec-114">Action name</span></span>|
|<span data-ttu-id="b9cec-115">actionState</span><span class="sxs-lookup"><span data-stu-id="b9cec-115">actionState</span></span>|[<span data-ttu-id="b9cec-116">actionState</span><span class="sxs-lookup"><span data-stu-id="b9cec-116">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="b9cec-117">Состояние действия.</span><span class="sxs-lookup"><span data-stu-id="b9cec-117">State of the action.</span></span> <span data-ttu-id="b9cec-118">Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="b9cec-118">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="b9cec-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="b9cec-119">startDateTime</span></span>|<span data-ttu-id="b9cec-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b9cec-120">DateTimeOffset</span></span>|<span data-ttu-id="b9cec-121">Время начала действия</span><span class="sxs-lookup"><span data-stu-id="b9cec-121">Time the action was initiated</span></span>|
|<span data-ttu-id="b9cec-122">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="b9cec-122">lastUpdatedDateTime</span></span>|<span data-ttu-id="b9cec-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b9cec-123">DateTimeOffset</span></span>|<span data-ttu-id="b9cec-124">Время последнего обновления состояния действия</span><span class="sxs-lookup"><span data-stu-id="b9cec-124">Time the action state was last updated</span></span>|

## <a name="relationships"></a><span data-ttu-id="b9cec-125">Связи</span><span class="sxs-lookup"><span data-stu-id="b9cec-125">Relationships</span></span>
<span data-ttu-id="b9cec-126">Нет</span><span class="sxs-lookup"><span data-stu-id="b9cec-126">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="b9cec-127">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b9cec-127">JSON Representation</span></span>
<span data-ttu-id="b9cec-128">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b9cec-128">Here is a JSON representation of the resource.</span></span>
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






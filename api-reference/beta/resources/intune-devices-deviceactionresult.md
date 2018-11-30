---
title: Тип ресурса deviceActionResult
description: Результат действия, касающегося устройства
ms.openlocfilehash: ac37cdff8ec323dfb8a2019b383d506c1b7e1076
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27076075"
---
# <a name="deviceactionresult-resource-type"></a><span data-ttu-id="09ba8-103">Тип ресурса deviceActionResult</span><span class="sxs-lookup"><span data-stu-id="09ba8-103">deviceActionResult resource type</span></span>

> <span data-ttu-id="09ba8-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="09ba8-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="09ba8-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="09ba8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="09ba8-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="09ba8-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="09ba8-107">Результат действия, касающегося устройства</span><span class="sxs-lookup"><span data-stu-id="09ba8-107">Device action result</span></span>
## <a name="properties"></a><span data-ttu-id="09ba8-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="09ba8-108">Properties</span></span>
|<span data-ttu-id="09ba8-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="09ba8-109">Property</span></span>|<span data-ttu-id="09ba8-110">Тип</span><span class="sxs-lookup"><span data-stu-id="09ba8-110">Type</span></span>|<span data-ttu-id="09ba8-111">Описание</span><span class="sxs-lookup"><span data-stu-id="09ba8-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="09ba8-112">actionName</span><span class="sxs-lookup"><span data-stu-id="09ba8-112">actionName</span></span>|<span data-ttu-id="09ba8-113">String</span><span class="sxs-lookup"><span data-stu-id="09ba8-113">String</span></span>|<span data-ttu-id="09ba8-114">Название действия</span><span class="sxs-lookup"><span data-stu-id="09ba8-114">Action name</span></span>|
|<span data-ttu-id="09ba8-115">actionState</span><span class="sxs-lookup"><span data-stu-id="09ba8-115">actionState</span></span>|[<span data-ttu-id="09ba8-116">actionState</span><span class="sxs-lookup"><span data-stu-id="09ba8-116">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="09ba8-117">Состояние действия.</span><span class="sxs-lookup"><span data-stu-id="09ba8-117">State of the action.</span></span> <span data-ttu-id="09ba8-118">Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="09ba8-118">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="09ba8-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="09ba8-119">startDateTime</span></span>|<span data-ttu-id="09ba8-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="09ba8-120">DateTimeOffset</span></span>|<span data-ttu-id="09ba8-121">Время начала действия</span><span class="sxs-lookup"><span data-stu-id="09ba8-121">Time the action was initiated</span></span>|
|<span data-ttu-id="09ba8-122">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="09ba8-122">lastUpdatedDateTime</span></span>|<span data-ttu-id="09ba8-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="09ba8-123">DateTimeOffset</span></span>|<span data-ttu-id="09ba8-124">Время последнего обновления состояния действия</span><span class="sxs-lookup"><span data-stu-id="09ba8-124">Time the action state was last updated</span></span>|

## <a name="relationships"></a><span data-ttu-id="09ba8-125">Связи</span><span class="sxs-lookup"><span data-stu-id="09ba8-125">Relationships</span></span>
<span data-ttu-id="09ba8-126">Нет</span><span class="sxs-lookup"><span data-stu-id="09ba8-126">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="09ba8-127">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="09ba8-127">JSON Representation</span></span>
<span data-ttu-id="09ba8-128">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="09ba8-128">Here is a JSON representation of the resource.</span></span>
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






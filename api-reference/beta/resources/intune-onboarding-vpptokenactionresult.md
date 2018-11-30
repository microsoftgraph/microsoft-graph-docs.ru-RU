---
title: Тип ресурса vppTokenActionResult
description: Состояние действия выполняется с маркером покупки программы корпоративного Apple.
ms.openlocfilehash: d0cb9e21b04ccb8748d1f9e78f0a3e9dd465ce81
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27082385"
---
# <a name="vpptokenactionresult-resource-type"></a><span data-ttu-id="0c0f3-103">Тип ресурса vppTokenActionResult</span><span class="sxs-lookup"><span data-stu-id="0c0f3-103">vppTokenActionResult resource type</span></span>

> <span data-ttu-id="0c0f3-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="0c0f3-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0c0f3-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0c0f3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0c0f3-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="0c0f3-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0c0f3-107">Состояние действия выполняется с маркером покупки программы корпоративного Apple.</span><span class="sxs-lookup"><span data-stu-id="0c0f3-107">The status of the action performed with an Apple Volume Purchase Program token.</span></span>
## <a name="properties"></a><span data-ttu-id="0c0f3-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="0c0f3-108">Properties</span></span>
|<span data-ttu-id="0c0f3-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="0c0f3-109">Property</span></span>|<span data-ttu-id="0c0f3-110">Тип</span><span class="sxs-lookup"><span data-stu-id="0c0f3-110">Type</span></span>|<span data-ttu-id="0c0f3-111">Описание</span><span class="sxs-lookup"><span data-stu-id="0c0f3-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0c0f3-112">actionName</span><span class="sxs-lookup"><span data-stu-id="0c0f3-112">actionName</span></span>|<span data-ttu-id="0c0f3-113">String</span><span class="sxs-lookup"><span data-stu-id="0c0f3-113">String</span></span>|<span data-ttu-id="0c0f3-114">Название действия</span><span class="sxs-lookup"><span data-stu-id="0c0f3-114">Action name</span></span>|
|<span data-ttu-id="0c0f3-115">actionState</span><span class="sxs-lookup"><span data-stu-id="0c0f3-115">actionState</span></span>|[<span data-ttu-id="0c0f3-116">actionState</span><span class="sxs-lookup"><span data-stu-id="0c0f3-116">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="0c0f3-117">Состояние действия.</span><span class="sxs-lookup"><span data-stu-id="0c0f3-117">State of the action.</span></span> <span data-ttu-id="0c0f3-118">Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="0c0f3-118">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="0c0f3-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="0c0f3-119">startDateTime</span></span>|<span data-ttu-id="0c0f3-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0c0f3-120">DateTimeOffset</span></span>|<span data-ttu-id="0c0f3-121">Время начала действия</span><span class="sxs-lookup"><span data-stu-id="0c0f3-121">Time the action was initiated</span></span>|
|<span data-ttu-id="0c0f3-122">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="0c0f3-122">lastUpdatedDateTime</span></span>|<span data-ttu-id="0c0f3-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0c0f3-123">DateTimeOffset</span></span>|<span data-ttu-id="0c0f3-124">Время последнего обновления состояния действия</span><span class="sxs-lookup"><span data-stu-id="0c0f3-124">Time the action state was last updated</span></span>|

## <a name="relationships"></a><span data-ttu-id="0c0f3-125">Связи</span><span class="sxs-lookup"><span data-stu-id="0c0f3-125">Relationships</span></span>
<span data-ttu-id="0c0f3-126">Нет</span><span class="sxs-lookup"><span data-stu-id="0c0f3-126">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="0c0f3-127">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0c0f3-127">JSON Representation</span></span>
<span data-ttu-id="0c0f3-128">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0c0f3-128">Here is a JSON representation of the resource.</span></span>
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






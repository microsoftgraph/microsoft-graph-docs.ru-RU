---
title: Тип ресурса windows10AppsForceUpdateSchedule
description: Расписание принудительного обновления Windows 10 для приложений
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 980503e9316e5ae1d0083f2226519004fa802afd
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42787231"
---
# <a name="windows10appsforceupdateschedule-resource-type"></a><span data-ttu-id="d6d2a-103">Тип ресурса windows10AppsForceUpdateSchedule</span><span class="sxs-lookup"><span data-stu-id="d6d2a-103">windows10AppsForceUpdateSchedule resource type</span></span>

> <span data-ttu-id="d6d2a-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d6d2a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d6d2a-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d6d2a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d6d2a-106">Расписание принудительного обновления Windows 10 для приложений</span><span class="sxs-lookup"><span data-stu-id="d6d2a-106">Windows 10 force update schedule for Apps</span></span>

## <a name="properties"></a><span data-ttu-id="d6d2a-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="d6d2a-107">Properties</span></span>
|<span data-ttu-id="d6d2a-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="d6d2a-108">Property</span></span>|<span data-ttu-id="d6d2a-109">Тип</span><span class="sxs-lookup"><span data-stu-id="d6d2a-109">Type</span></span>|<span data-ttu-id="d6d2a-110">Описание</span><span class="sxs-lookup"><span data-stu-id="d6d2a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d6d2a-111">startDateTime</span><span class="sxs-lookup"><span data-stu-id="d6d2a-111">startDateTime</span></span>|<span data-ttu-id="d6d2a-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d6d2a-112">DateTimeOffset</span></span>|<span data-ttu-id="d6d2a-113">Время начала принудительного перезапуска.</span><span class="sxs-lookup"><span data-stu-id="d6d2a-113">The start time for the force restart.</span></span>|
|<span data-ttu-id="d6d2a-114">recurrence</span><span class="sxs-lookup"><span data-stu-id="d6d2a-114">recurrence</span></span>|[<span data-ttu-id="d6d2a-115">windows10AppsUpdateRecurrence</span><span class="sxs-lookup"><span data-stu-id="d6d2a-115">windows10AppsUpdateRecurrence</span></span>](../resources/intune-deviceconfig-windows10appsupdaterecurrence.md)|<span data-ttu-id="d6d2a-116">Расписание повторения.</span><span class="sxs-lookup"><span data-stu-id="d6d2a-116">Recurrence schedule.</span></span> <span data-ttu-id="d6d2a-117">Возможные значения: `none`, `daily`, `weekly`, `monthly`.</span><span class="sxs-lookup"><span data-stu-id="d6d2a-117">Possible values are: `none`, `daily`, `weekly`, `monthly`.</span></span>|
|<span data-ttu-id="d6d2a-118">руниммедиателифафтерстартдатетиме</span><span class="sxs-lookup"><span data-stu-id="d6d2a-118">runImmediatelyIfAfterStartDateTime</span></span>|<span data-ttu-id="d6d2a-119">Логический</span><span class="sxs-lookup"><span data-stu-id="d6d2a-119">Boolean</span></span>|<span data-ttu-id="d6d2a-120">Если этот параметр имеет значение true, задача выполняется немедленно, если StartDateTime находится в прошлое, иначе — выполняется при следующем повторении.</span><span class="sxs-lookup"><span data-stu-id="d6d2a-120">If true, runs the task immediately if StartDateTime is in the past, else, runs at the next recurrence.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d6d2a-121">Связи</span><span class="sxs-lookup"><span data-stu-id="d6d2a-121">Relationships</span></span>
<span data-ttu-id="d6d2a-122">Нет</span><span class="sxs-lookup"><span data-stu-id="d6d2a-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d6d2a-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d6d2a-123">JSON Representation</span></span>
<span data-ttu-id="d6d2a-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d6d2a-124">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windows10AppsForceUpdateSchedule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windows10AppsForceUpdateSchedule",
  "startDateTime": "String (timestamp)",
  "recurrence": "String",
  "runImmediatelyIfAfterStartDateTime": true
}
```




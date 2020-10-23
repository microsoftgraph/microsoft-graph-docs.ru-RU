---
title: Тип ресурса windows10AppsForceUpdateSchedule
description: Расписание принудительного обновления Windows 10 для приложений
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 9f902ef48caafa5f782c12d862e540bf7c482899
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48732525"
---
# <a name="windows10appsforceupdateschedule-resource-type"></a><span data-ttu-id="cb385-103">Тип ресурса windows10AppsForceUpdateSchedule</span><span class="sxs-lookup"><span data-stu-id="cb385-103">windows10AppsForceUpdateSchedule resource type</span></span>

<span data-ttu-id="cb385-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cb385-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cb385-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cb385-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cb385-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="cb385-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cb385-107">Расписание принудительного обновления Windows 10 для приложений</span><span class="sxs-lookup"><span data-stu-id="cb385-107">Windows 10 force update schedule for Apps</span></span>

## <a name="properties"></a><span data-ttu-id="cb385-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="cb385-108">Properties</span></span>
|<span data-ttu-id="cb385-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="cb385-109">Property</span></span>|<span data-ttu-id="cb385-110">Тип</span><span class="sxs-lookup"><span data-stu-id="cb385-110">Type</span></span>|<span data-ttu-id="cb385-111">Описание</span><span class="sxs-lookup"><span data-stu-id="cb385-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cb385-112">startDateTime</span><span class="sxs-lookup"><span data-stu-id="cb385-112">startDateTime</span></span>|<span data-ttu-id="cb385-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cb385-113">DateTimeOffset</span></span>|<span data-ttu-id="cb385-114">Время начала принудительного перезапуска.</span><span class="sxs-lookup"><span data-stu-id="cb385-114">The start time for the force restart.</span></span>|
|<span data-ttu-id="cb385-115">recurrence</span><span class="sxs-lookup"><span data-stu-id="cb385-115">recurrence</span></span>|[<span data-ttu-id="cb385-116">windows10AppsUpdateRecurrence</span><span class="sxs-lookup"><span data-stu-id="cb385-116">windows10AppsUpdateRecurrence</span></span>](../resources/intune-deviceconfig-windows10appsupdaterecurrence.md)|<span data-ttu-id="cb385-117">Расписание повторения.</span><span class="sxs-lookup"><span data-stu-id="cb385-117">Recurrence schedule.</span></span> <span data-ttu-id="cb385-118">Возможные значения: `none`, `daily`, `weekly`, `monthly`.</span><span class="sxs-lookup"><span data-stu-id="cb385-118">Possible values are: `none`, `daily`, `weekly`, `monthly`.</span></span>|
|<span data-ttu-id="cb385-119">руниммедиателифафтерстартдатетиме</span><span class="sxs-lookup"><span data-stu-id="cb385-119">runImmediatelyIfAfterStartDateTime</span></span>|<span data-ttu-id="cb385-120">Логический</span><span class="sxs-lookup"><span data-stu-id="cb385-120">Boolean</span></span>|<span data-ttu-id="cb385-121">Если этот параметр имеет значение true, задача выполняется немедленно, если StartDateTime находится в прошлое, иначе — выполняется при следующем повторении.</span><span class="sxs-lookup"><span data-stu-id="cb385-121">If true, runs the task immediately if StartDateTime is in the past, else, runs at the next recurrence.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cb385-122">Связи</span><span class="sxs-lookup"><span data-stu-id="cb385-122">Relationships</span></span>
<span data-ttu-id="cb385-123">Нет</span><span class="sxs-lookup"><span data-stu-id="cb385-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="cb385-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="cb385-124">JSON Representation</span></span>
<span data-ttu-id="cb385-125">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cb385-125">Here is a JSON representation of the resource.</span></span>
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






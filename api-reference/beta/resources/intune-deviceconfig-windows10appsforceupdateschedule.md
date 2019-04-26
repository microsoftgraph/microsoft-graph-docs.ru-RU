---
title: Тип ресурса windows10AppsForceUpdateSchedule
description: Расписание принудительного обновления Windows 10 для приложений
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3c8c76c08c434ab9c5e3506339e53cda41156e09
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32572264"
---
# <a name="windows10appsforceupdateschedule-resource-type"></a><span data-ttu-id="1d6cc-103">Тип ресурса windows10AppsForceUpdateSchedule</span><span class="sxs-lookup"><span data-stu-id="1d6cc-103">windows10AppsForceUpdateSchedule resource type</span></span>

> <span data-ttu-id="1d6cc-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1d6cc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1d6cc-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1d6cc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1d6cc-106">Расписание принудительного обновления Windows 10 для приложений</span><span class="sxs-lookup"><span data-stu-id="1d6cc-106">Windows 10 force update schedule for Apps</span></span>

## <a name="properties"></a><span data-ttu-id="1d6cc-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="1d6cc-107">Properties</span></span>
|<span data-ttu-id="1d6cc-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="1d6cc-108">Property</span></span>|<span data-ttu-id="1d6cc-109">Тип</span><span class="sxs-lookup"><span data-stu-id="1d6cc-109">Type</span></span>|<span data-ttu-id="1d6cc-110">Описание</span><span class="sxs-lookup"><span data-stu-id="1d6cc-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1d6cc-111">startDateTime</span><span class="sxs-lookup"><span data-stu-id="1d6cc-111">startDateTime</span></span>|<span data-ttu-id="1d6cc-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1d6cc-112">DateTimeOffset</span></span>|<span data-ttu-id="1d6cc-113">Время начала принудительного перезапуска.</span><span class="sxs-lookup"><span data-stu-id="1d6cc-113">The start time for the force restart.</span></span>|
|<span data-ttu-id="1d6cc-114">recurrence</span><span class="sxs-lookup"><span data-stu-id="1d6cc-114">recurrence</span></span>|[<span data-ttu-id="1d6cc-115">windows10AppsUpdateRecurrence</span><span class="sxs-lookup"><span data-stu-id="1d6cc-115">windows10AppsUpdateRecurrence</span></span>](../resources/intune-deviceconfig-windows10appsupdaterecurrence.md)|<span data-ttu-id="1d6cc-116">Расписание повторения.</span><span class="sxs-lookup"><span data-stu-id="1d6cc-116">Recurrence schedule.</span></span> <span data-ttu-id="1d6cc-117">Возможные значения: `none`, `daily`, `weekly`, `monthly`.</span><span class="sxs-lookup"><span data-stu-id="1d6cc-117">Possible values are: `none`, `daily`, `weekly`, `monthly`.</span></span>|
|<span data-ttu-id="1d6cc-118">Руниммедиателифафтерстартдатетиме</span><span class="sxs-lookup"><span data-stu-id="1d6cc-118">runImmediatelyIfAfterStartDateTime</span></span>|<span data-ttu-id="1d6cc-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="1d6cc-119">Boolean</span></span>|<span data-ttu-id="1d6cc-120">Если этот параметр имеет значение true, задача выполняется немедленно, если StartDateTime находится в прошлое, иначе — выполняется при следующем повторении.</span><span class="sxs-lookup"><span data-stu-id="1d6cc-120">If true, runs the task immediately if StartDateTime is in the past, else, runs at the next recurrence.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1d6cc-121">Отношения</span><span class="sxs-lookup"><span data-stu-id="1d6cc-121">Relationships</span></span>
<span data-ttu-id="1d6cc-122">Нет</span><span class="sxs-lookup"><span data-stu-id="1d6cc-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1d6cc-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1d6cc-123">JSON Representation</span></span>
<span data-ttu-id="1d6cc-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1d6cc-124">Here is a JSON representation of the resource.</span></span>
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






---
title: Тип ресурса windows10AppsForceUpdateSchedule
description: Расписание обновления force Windows 10 для приложения
author: tfitzmac
ms.openlocfilehash: 851f22e092f2669dfc44911783df6182cda1dc6d
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27323704"
---
# <a name="windows10appsforceupdateschedule-resource-type"></a><span data-ttu-id="de86b-103">Тип ресурса windows10AppsForceUpdateSchedule</span><span class="sxs-lookup"><span data-stu-id="de86b-103">windows10AppsForceUpdateSchedule resource type</span></span>

> <span data-ttu-id="de86b-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="de86b-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="de86b-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="de86b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="de86b-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="de86b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="de86b-107">Расписание обновления force Windows 10 для приложения</span><span class="sxs-lookup"><span data-stu-id="de86b-107">Windows 10 force update schedule for Apps</span></span>
## <a name="properties"></a><span data-ttu-id="de86b-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="de86b-108">Properties</span></span>
|<span data-ttu-id="de86b-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="de86b-109">Property</span></span>|<span data-ttu-id="de86b-110">Тип</span><span class="sxs-lookup"><span data-stu-id="de86b-110">Type</span></span>|<span data-ttu-id="de86b-111">Описание</span><span class="sxs-lookup"><span data-stu-id="de86b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="de86b-112">startDateTime</span><span class="sxs-lookup"><span data-stu-id="de86b-112">startDateTime</span></span>|<span data-ttu-id="de86b-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="de86b-113">DateTimeOffset</span></span>|<span data-ttu-id="de86b-114">Перезапустите время начала для сотрудников.</span><span class="sxs-lookup"><span data-stu-id="de86b-114">The start time for the force restart.</span></span>|
|<span data-ttu-id="de86b-115">recurrence</span><span class="sxs-lookup"><span data-stu-id="de86b-115">recurrence</span></span>|[<span data-ttu-id="de86b-116">windows10AppsUpdateRecurrence</span><span class="sxs-lookup"><span data-stu-id="de86b-116">windows10AppsUpdateRecurrence</span></span>](../resources/intune-deviceconfig-windows10appsupdaterecurrence.md)|<span data-ttu-id="de86b-117">Расписание повторения.</span><span class="sxs-lookup"><span data-stu-id="de86b-117">Recurrence schedule.</span></span> <span data-ttu-id="de86b-118">Возможные значения: `none`, `daily`, `weekly`, `monthly`.</span><span class="sxs-lookup"><span data-stu-id="de86b-118">Possible values are: `none`, `daily`, `weekly`, `monthly`.</span></span>|
|<span data-ttu-id="de86b-119">runImmediatelyIfAfterStartDateTime</span><span class="sxs-lookup"><span data-stu-id="de86b-119">runImmediatelyIfAfterStartDateTime</span></span>|<span data-ttu-id="de86b-120">Boolean.</span><span class="sxs-lookup"><span data-stu-id="de86b-120">Boolean</span></span>|<span data-ttu-id="de86b-121">Если значение true, если StartDateTime в прошлом else, будет выполняться в следующего повторения немедленно запускается задание.</span><span class="sxs-lookup"><span data-stu-id="de86b-121">If true, runs the task immediately if StartDateTime is in the past, else, runs at the next recurrence.</span></span>|

## <a name="relationships"></a><span data-ttu-id="de86b-122">Связи</span><span class="sxs-lookup"><span data-stu-id="de86b-122">Relationships</span></span>
<span data-ttu-id="de86b-123">Нет</span><span class="sxs-lookup"><span data-stu-id="de86b-123">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="de86b-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="de86b-124">JSON Representation</span></span>
<span data-ttu-id="de86b-125">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="de86b-125">Here is a JSON representation of the resource.</span></span>
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






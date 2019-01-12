---
title: Тип ресурса windows10AppsForceUpdateSchedule
description: Расписание обновления force Windows 10 для приложения
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 50793ee4ba26adc4b89cc8d36b3e8186debc402a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27981989"
---
# <a name="windows10appsforceupdateschedule-resource-type"></a><span data-ttu-id="9d241-103">Тип ресурса windows10AppsForceUpdateSchedule</span><span class="sxs-lookup"><span data-stu-id="9d241-103">windows10AppsForceUpdateSchedule resource type</span></span>

> <span data-ttu-id="9d241-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="9d241-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9d241-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9d241-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9d241-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="9d241-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9d241-107">Расписание обновления force Windows 10 для приложения</span><span class="sxs-lookup"><span data-stu-id="9d241-107">Windows 10 force update schedule for Apps</span></span>
## <a name="properties"></a><span data-ttu-id="9d241-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="9d241-108">Properties</span></span>
|<span data-ttu-id="9d241-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="9d241-109">Property</span></span>|<span data-ttu-id="9d241-110">Тип</span><span class="sxs-lookup"><span data-stu-id="9d241-110">Type</span></span>|<span data-ttu-id="9d241-111">Описание</span><span class="sxs-lookup"><span data-stu-id="9d241-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9d241-112">startDateTime</span><span class="sxs-lookup"><span data-stu-id="9d241-112">startDateTime</span></span>|<span data-ttu-id="9d241-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9d241-113">DateTimeOffset</span></span>|<span data-ttu-id="9d241-114">Перезапустите время начала для сотрудников.</span><span class="sxs-lookup"><span data-stu-id="9d241-114">The start time for the force restart.</span></span>|
|<span data-ttu-id="9d241-115">recurrence</span><span class="sxs-lookup"><span data-stu-id="9d241-115">recurrence</span></span>|[<span data-ttu-id="9d241-116">windows10AppsUpdateRecurrence</span><span class="sxs-lookup"><span data-stu-id="9d241-116">windows10AppsUpdateRecurrence</span></span>](../resources/intune-deviceconfig-windows10appsupdaterecurrence.md)|<span data-ttu-id="9d241-117">Расписание повторения.</span><span class="sxs-lookup"><span data-stu-id="9d241-117">Recurrence schedule.</span></span> <span data-ttu-id="9d241-118">Возможные значения: `none`, `daily`, `weekly`, `monthly`.</span><span class="sxs-lookup"><span data-stu-id="9d241-118">Possible values are: `none`, `daily`, `weekly`, `monthly`.</span></span>|
|<span data-ttu-id="9d241-119">runImmediatelyIfAfterStartDateTime</span><span class="sxs-lookup"><span data-stu-id="9d241-119">runImmediatelyIfAfterStartDateTime</span></span>|<span data-ttu-id="9d241-120">Логический</span><span class="sxs-lookup"><span data-stu-id="9d241-120">Boolean</span></span>|<span data-ttu-id="9d241-121">Если значение true, если StartDateTime в прошлом else, будет выполняться в следующего повторения немедленно запускается задание.</span><span class="sxs-lookup"><span data-stu-id="9d241-121">If true, runs the task immediately if StartDateTime is in the past, else, runs at the next recurrence.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9d241-122">Связи</span><span class="sxs-lookup"><span data-stu-id="9d241-122">Relationships</span></span>
<span data-ttu-id="9d241-123">Нет</span><span class="sxs-lookup"><span data-stu-id="9d241-123">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="9d241-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9d241-124">JSON Representation</span></span>
<span data-ttu-id="9d241-125">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9d241-125">Here is a JSON representation of the resource.</span></span>
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






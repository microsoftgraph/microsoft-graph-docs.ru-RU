---
title: Тип ресурса windows10AppsForceUpdateSchedule
description: Расписание обновления force Windows 10 для приложения
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 3e0bd9b0963f8547b03243aa7ef791a351dc2b08
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29418836"
---
# <a name="windows10appsforceupdateschedule-resource-type"></a><span data-ttu-id="d06ae-103">Тип ресурса windows10AppsForceUpdateSchedule</span><span class="sxs-lookup"><span data-stu-id="d06ae-103">windows10AppsForceUpdateSchedule resource type</span></span>

> <span data-ttu-id="d06ae-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="d06ae-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="d06ae-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d06ae-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d06ae-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d06ae-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d06ae-107">Расписание обновления force Windows 10 для приложения</span><span class="sxs-lookup"><span data-stu-id="d06ae-107">Windows 10 force update schedule for Apps</span></span>

## <a name="properties"></a><span data-ttu-id="d06ae-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="d06ae-108">Properties</span></span>
|<span data-ttu-id="d06ae-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="d06ae-109">Property</span></span>|<span data-ttu-id="d06ae-110">Тип</span><span class="sxs-lookup"><span data-stu-id="d06ae-110">Type</span></span>|<span data-ttu-id="d06ae-111">Описание</span><span class="sxs-lookup"><span data-stu-id="d06ae-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d06ae-112">startDateTime</span><span class="sxs-lookup"><span data-stu-id="d06ae-112">startDateTime</span></span>|<span data-ttu-id="d06ae-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d06ae-113">DateTimeOffset</span></span>|<span data-ttu-id="d06ae-114">Перезапустите время начала для сотрудников.</span><span class="sxs-lookup"><span data-stu-id="d06ae-114">The start time for the force restart.</span></span>|
|<span data-ttu-id="d06ae-115">recurrence</span><span class="sxs-lookup"><span data-stu-id="d06ae-115">recurrence</span></span>|[<span data-ttu-id="d06ae-116">windows10AppsUpdateRecurrence</span><span class="sxs-lookup"><span data-stu-id="d06ae-116">windows10AppsUpdateRecurrence</span></span>](../resources/intune-deviceconfig-windows10appsupdaterecurrence.md)|<span data-ttu-id="d06ae-117">Расписание повторения.</span><span class="sxs-lookup"><span data-stu-id="d06ae-117">Recurrence schedule.</span></span> <span data-ttu-id="d06ae-118">Возможные значения: `none`, `daily`, `weekly`, `monthly`.</span><span class="sxs-lookup"><span data-stu-id="d06ae-118">Possible values are: `none`, `daily`, `weekly`, `monthly`.</span></span>|
|<span data-ttu-id="d06ae-119">runImmediatelyIfAfterStartDateTime</span><span class="sxs-lookup"><span data-stu-id="d06ae-119">runImmediatelyIfAfterStartDateTime</span></span>|<span data-ttu-id="d06ae-120">Логический</span><span class="sxs-lookup"><span data-stu-id="d06ae-120">Boolean</span></span>|<span data-ttu-id="d06ae-121">Если значение true, если StartDateTime в прошлом else, будет выполняться в следующего повторения немедленно запускается задание.</span><span class="sxs-lookup"><span data-stu-id="d06ae-121">If true, runs the task immediately if StartDateTime is in the past, else, runs at the next recurrence.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d06ae-122">Отношения</span><span class="sxs-lookup"><span data-stu-id="d06ae-122">Relationships</span></span>
<span data-ttu-id="d06ae-123">Нет</span><span class="sxs-lookup"><span data-stu-id="d06ae-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d06ae-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d06ae-124">JSON Representation</span></span>
<span data-ttu-id="d06ae-125">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d06ae-125">Here is a JSON representation of the resource.</span></span>
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





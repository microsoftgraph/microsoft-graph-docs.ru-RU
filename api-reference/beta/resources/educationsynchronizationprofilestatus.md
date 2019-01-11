---
title: Тип ресурса educationSynchronizationProfileStatus
description: 'Представляет состояние синхронизации профилей синхронизации данных school. '
author: mmast-msft
localization_priority: Normal
ms.openlocfilehash: 4476ffc7c64fb5d9852c46e2b748587e79d427c1
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27858165"
---
# <a name="educationsynchronizationprofilestatus-resource-type"></a><span data-ttu-id="d850f-103">Тип ресурса educationSynchronizationProfileStatus</span><span class="sxs-lookup"><span data-stu-id="d850f-103">educationSynchronizationProfileStatus resource type</span></span>

> <span data-ttu-id="d850f-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="d850f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d850f-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d850f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d850f-106">Представляет состояния синхронизации данных school [синхронизации профилей](educationsynchronizationprofile.md).</span><span class="sxs-lookup"><span data-stu-id="d850f-106">Represents the synchronization status of a school data [synchronization profile](educationsynchronizationprofile.md).</span></span> 

> <span data-ttu-id="d850f-107">**Примечание:** Обновления для **educationSynchronizationProfileStatus** может отложить из-за асинхронной фоновой синхронизации обработки.</span><span class="sxs-lookup"><span data-stu-id="d850f-107">**Note:** Updates to the **educationSynchronizationProfileStatus** might be delayed due to the asynchronous nature of background sync processing.</span></span>

## <a name="methods"></a><span data-ttu-id="d850f-108">Методы</span><span class="sxs-lookup"><span data-stu-id="d850f-108">Methods</span></span>

| <span data-ttu-id="d850f-109">Метод</span><span class="sxs-lookup"><span data-stu-id="d850f-109">Method</span></span> | <span data-ttu-id="d850f-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="d850f-110">Return Type</span></span> | <span data-ttu-id="d850f-111">Описание</span><span class="sxs-lookup"><span data-stu-id="d850f-111">Description</span></span> |
|:-|:-|:-|
| [<span data-ttu-id="d850f-112">Получение состояния синхронизации</span><span class="sxs-lookup"><span data-stu-id="d850f-112">Get status of a sync</span></span>](../api/educationsynchronizationprofilestatus-get.md) | <span data-ttu-id="d850f-113">**educationSynchronizationProfileStatus**</span><span class="sxs-lookup"><span data-stu-id="d850f-113">**educationSynchronizationProfileStatus**</span></span> | <span data-ttu-id="d850f-114">Возвращает состояние определенного синхронизации профилей.</span><span class="sxs-lookup"><span data-stu-id="d850f-114">Return the status of a specific synchronization profile.</span></span> |

## <a name="properties"></a><span data-ttu-id="d850f-115">Свойства</span><span class="sxs-lookup"><span data-stu-id="d850f-115">Properties</span></span>

| <span data-ttu-id="d850f-116">Свойство</span><span class="sxs-lookup"><span data-stu-id="d850f-116">Property</span></span> | <span data-ttu-id="d850f-117">Тип</span><span class="sxs-lookup"><span data-stu-id="d850f-117">Type</span></span> | <span data-ttu-id="d850f-118">Описание</span><span class="sxs-lookup"><span data-stu-id="d850f-118">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="d850f-119">**status**</span><span class="sxs-lookup"><span data-stu-id="d850f-119">**status**</span></span> | <span data-ttu-id="d850f-120">string</span><span class="sxs-lookup"><span data-stu-id="d850f-120">string</span></span> | <span data-ttu-id="d850f-121">Состояние синхронизации. Возможные значения: `paused`, `inProgress`, `success`, `error`, `quarantined`, `validationError`.</span><span class="sxs-lookup"><span data-stu-id="d850f-121">The status of a sync. Possible values are: `paused`, `inProgress`, `success`, `error`, `quarantined`, `validationError`.</span></span> |
| <span data-ttu-id="d850f-122">**lastSynchronizationDateTime**</span><span class="sxs-lookup"><span data-stu-id="d850f-122">**lastSynchronizationDateTime**</span></span> | <span data-ttu-id="d850f-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d850f-123">DateTimeOffset</span></span> | <span data-ttu-id="d850f-124">Представляет время, когда наблюдались последних изменений в каталоге.</span><span class="sxs-lookup"><span data-stu-id="d850f-124">Represents the time when most recent changes have been observed in the directory.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="d850f-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d850f-125">JSON representation</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "#microsoft.graph.educationSynchronizationProfileStatus"
}-->

```json
{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#education/synchronizationProfiles('{id}')/profileStatus/$entity",
    "status": {"@odata.type":"microsoft.graph.educationSynchronizationStatus"},
    "lastSynchronizationDateTime": "DateTimeOffset"
}
```

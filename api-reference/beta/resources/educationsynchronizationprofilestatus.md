---
title: Тип ресурса educationSynchronizationProfileStatus
description: 'Представляет состояние синхронизации профилей синхронизации данных school. '
ms.openlocfilehash: 6d2c638e1f92a6c3e090cb2bf3bb55e8482bbc4c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27082615"
---
# <a name="educationsynchronizationprofilestatus-resource-type"></a><span data-ttu-id="14045-103">Тип ресурса educationSynchronizationProfileStatus</span><span class="sxs-lookup"><span data-stu-id="14045-103">educationSynchronizationProfileStatus resource type</span></span>

> <span data-ttu-id="14045-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="14045-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="14045-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="14045-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="14045-106">Представляет состояния синхронизации данных school [синхронизации профилей](educationsynchronizationprofile.md).</span><span class="sxs-lookup"><span data-stu-id="14045-106">Represents the synchronization status of a school data [synchronization profile](educationsynchronizationprofile.md).</span></span> 

> <span data-ttu-id="14045-107">**Примечание:** Обновления для **educationSynchronizationProfileStatus** может отложить из-за асинхронной фоновой синхронизации обработки.</span><span class="sxs-lookup"><span data-stu-id="14045-107">**Note:** Updates to the **educationSynchronizationProfileStatus** might be delayed due to the asynchronous nature of background sync processing.</span></span>

## <a name="methods"></a><span data-ttu-id="14045-108">Методы</span><span class="sxs-lookup"><span data-stu-id="14045-108">Methods</span></span>

| <span data-ttu-id="14045-109">Метод</span><span class="sxs-lookup"><span data-stu-id="14045-109">Method</span></span> | <span data-ttu-id="14045-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="14045-110">Return Type</span></span> | <span data-ttu-id="14045-111">Описание</span><span class="sxs-lookup"><span data-stu-id="14045-111">Description</span></span> |
|:-|:-|:-|
| [<span data-ttu-id="14045-112">Получение состояния синхронизации</span><span class="sxs-lookup"><span data-stu-id="14045-112">Get status of a sync</span></span>](../api/educationsynchronizationprofilestatus-get.md) | <span data-ttu-id="14045-113">**educationSynchronizationProfileStatus**</span><span class="sxs-lookup"><span data-stu-id="14045-113">**educationSynchronizationProfileStatus**</span></span> | <span data-ttu-id="14045-114">Возвращает состояние определенного синхронизации профилей.</span><span class="sxs-lookup"><span data-stu-id="14045-114">Return the status of a specific synchronization profile.</span></span> |

## <a name="properties"></a><span data-ttu-id="14045-115">Свойства</span><span class="sxs-lookup"><span data-stu-id="14045-115">Properties</span></span>

| <span data-ttu-id="14045-116">Свойство</span><span class="sxs-lookup"><span data-stu-id="14045-116">Property</span></span> | <span data-ttu-id="14045-117">Тип</span><span class="sxs-lookup"><span data-stu-id="14045-117">Type</span></span> | <span data-ttu-id="14045-118">Description</span><span class="sxs-lookup"><span data-stu-id="14045-118">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="14045-119">**status**</span><span class="sxs-lookup"><span data-stu-id="14045-119">**status**</span></span> | <span data-ttu-id="14045-120">string</span><span class="sxs-lookup"><span data-stu-id="14045-120">string</span></span> | <span data-ttu-id="14045-121">Состояние синхронизации. Возможные значения: `paused`, `inProgress`, `success`, `error`, `quarantined`, `validationError`.</span><span class="sxs-lookup"><span data-stu-id="14045-121">The status of a sync. Possible values are: `paused`, `inProgress`, `success`, `error`, `quarantined`, `validationError`.</span></span> |
| <span data-ttu-id="14045-122">**lastSynchronizationDateTime**</span><span class="sxs-lookup"><span data-stu-id="14045-122">**lastSynchronizationDateTime**</span></span> | <span data-ttu-id="14045-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="14045-123">DateTimeOffset</span></span> | <span data-ttu-id="14045-124">Представляет время, когда наблюдались последних изменений в каталоге.</span><span class="sxs-lookup"><span data-stu-id="14045-124">Represents the time when most recent changes have been observed in the directory.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="14045-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="14045-125">JSON representation</span></span>
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
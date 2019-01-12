---
title: Тип ресурса educationSynchronizationProfileStatus
description: 'Представляет состояние синхронизации профилей синхронизации данных school. '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: d16619b0cf1e2c09358cf585b896b0c7c7d4f318
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27928929"
---
# <a name="educationsynchronizationprofilestatus-resource-type"></a><span data-ttu-id="0e087-103">Тип ресурса educationSynchronizationProfileStatus</span><span class="sxs-lookup"><span data-stu-id="0e087-103">educationSynchronizationProfileStatus resource type</span></span>

> <span data-ttu-id="0e087-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="0e087-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0e087-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0e087-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0e087-106">Представляет состояния синхронизации данных school [синхронизации профилей](educationsynchronizationprofile.md).</span><span class="sxs-lookup"><span data-stu-id="0e087-106">Represents the synchronization status of a school data [synchronization profile](educationsynchronizationprofile.md).</span></span> 

> <span data-ttu-id="0e087-107">**Примечание:** Обновления для **educationSynchronizationProfileStatus** может отложить из-за асинхронной фоновой синхронизации обработки.</span><span class="sxs-lookup"><span data-stu-id="0e087-107">**Note:** Updates to the **educationSynchronizationProfileStatus** might be delayed due to the asynchronous nature of background sync processing.</span></span>

## <a name="methods"></a><span data-ttu-id="0e087-108">Методы</span><span class="sxs-lookup"><span data-stu-id="0e087-108">Methods</span></span>

| <span data-ttu-id="0e087-109">Метод</span><span class="sxs-lookup"><span data-stu-id="0e087-109">Method</span></span> | <span data-ttu-id="0e087-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="0e087-110">Return Type</span></span> | <span data-ttu-id="0e087-111">Описание</span><span class="sxs-lookup"><span data-stu-id="0e087-111">Description</span></span> |
|:-|:-|:-|
| [<span data-ttu-id="0e087-112">Получение состояния синхронизации</span><span class="sxs-lookup"><span data-stu-id="0e087-112">Get status of a sync</span></span>](../api/educationsynchronizationprofilestatus-get.md) | <span data-ttu-id="0e087-113">**educationSynchronizationProfileStatus**</span><span class="sxs-lookup"><span data-stu-id="0e087-113">**educationSynchronizationProfileStatus**</span></span> | <span data-ttu-id="0e087-114">Возвращает состояние определенного синхронизации профилей.</span><span class="sxs-lookup"><span data-stu-id="0e087-114">Return the status of a specific synchronization profile.</span></span> |

## <a name="properties"></a><span data-ttu-id="0e087-115">Свойства</span><span class="sxs-lookup"><span data-stu-id="0e087-115">Properties</span></span>

| <span data-ttu-id="0e087-116">Свойство</span><span class="sxs-lookup"><span data-stu-id="0e087-116">Property</span></span> | <span data-ttu-id="0e087-117">Тип</span><span class="sxs-lookup"><span data-stu-id="0e087-117">Type</span></span> | <span data-ttu-id="0e087-118">Описание</span><span class="sxs-lookup"><span data-stu-id="0e087-118">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="0e087-119">**status**</span><span class="sxs-lookup"><span data-stu-id="0e087-119">**status**</span></span> | <span data-ttu-id="0e087-120">string</span><span class="sxs-lookup"><span data-stu-id="0e087-120">string</span></span> | <span data-ttu-id="0e087-121">Состояние синхронизации. Возможные значения: `paused`, `inProgress`, `success`, `error`, `quarantined`, `validationError`.</span><span class="sxs-lookup"><span data-stu-id="0e087-121">The status of a sync. Possible values are: `paused`, `inProgress`, `success`, `error`, `quarantined`, `validationError`.</span></span> |
| <span data-ttu-id="0e087-122">**lastSynchronizationDateTime**</span><span class="sxs-lookup"><span data-stu-id="0e087-122">**lastSynchronizationDateTime**</span></span> | <span data-ttu-id="0e087-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0e087-123">DateTimeOffset</span></span> | <span data-ttu-id="0e087-124">Представляет время, когда наблюдались последних изменений в каталоге.</span><span class="sxs-lookup"><span data-stu-id="0e087-124">Represents the time when most recent changes have been observed in the directory.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="0e087-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0e087-125">JSON representation</span></span>
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

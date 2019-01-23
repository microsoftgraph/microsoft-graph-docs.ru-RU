---
title: Тип ресурса educationSynchronizationProfileStatus
description: 'Представляет состояние синхронизации профилей синхронизации данных school. '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 1fd77f48544e5e6bc0c582e4ce9fb2a5b1b6601a
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29396156"
---
# <a name="educationsynchronizationprofilestatus-resource-type"></a><span data-ttu-id="d20b4-103">Тип ресурса educationSynchronizationProfileStatus</span><span class="sxs-lookup"><span data-stu-id="d20b4-103">educationSynchronizationProfileStatus resource type</span></span>

> <span data-ttu-id="d20b4-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="d20b4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d20b4-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d20b4-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d20b4-106">Представляет состояния синхронизации данных school [синхронизации профилей](educationsynchronizationprofile.md).</span><span class="sxs-lookup"><span data-stu-id="d20b4-106">Represents the synchronization status of a school data [synchronization profile](educationsynchronizationprofile.md).</span></span> 

> <span data-ttu-id="d20b4-107">**Примечание:** Обновления для **educationSynchronizationProfileStatus** может отложить из-за асинхронной фоновой синхронизации обработки.</span><span class="sxs-lookup"><span data-stu-id="d20b4-107">**Note:** Updates to the **educationSynchronizationProfileStatus** might be delayed due to the asynchronous nature of background sync processing.</span></span>

## <a name="methods"></a><span data-ttu-id="d20b4-108">Методы</span><span class="sxs-lookup"><span data-stu-id="d20b4-108">Methods</span></span>

| <span data-ttu-id="d20b4-109">Метод</span><span class="sxs-lookup"><span data-stu-id="d20b4-109">Method</span></span> | <span data-ttu-id="d20b4-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="d20b4-110">Return Type</span></span> | <span data-ttu-id="d20b4-111">Описание</span><span class="sxs-lookup"><span data-stu-id="d20b4-111">Description</span></span> |
|:-|:-|:-|
| [<span data-ttu-id="d20b4-112">Получение состояния синхронизации</span><span class="sxs-lookup"><span data-stu-id="d20b4-112">Get status of a sync</span></span>](../api/educationsynchronizationprofilestatus-get.md) | <span data-ttu-id="d20b4-113">**educationSynchronizationProfileStatus**</span><span class="sxs-lookup"><span data-stu-id="d20b4-113">**educationSynchronizationProfileStatus**</span></span> | <span data-ttu-id="d20b4-114">Возвращает состояние определенного синхронизации профилей.</span><span class="sxs-lookup"><span data-stu-id="d20b4-114">Return the status of a specific synchronization profile.</span></span> |

## <a name="properties"></a><span data-ttu-id="d20b4-115">Свойства</span><span class="sxs-lookup"><span data-stu-id="d20b4-115">Properties</span></span>

| <span data-ttu-id="d20b4-116">Свойство</span><span class="sxs-lookup"><span data-stu-id="d20b4-116">Property</span></span> | <span data-ttu-id="d20b4-117">Тип</span><span class="sxs-lookup"><span data-stu-id="d20b4-117">Type</span></span> | <span data-ttu-id="d20b4-118">Описание</span><span class="sxs-lookup"><span data-stu-id="d20b4-118">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="d20b4-119">**status**</span><span class="sxs-lookup"><span data-stu-id="d20b4-119">**status**</span></span> | <span data-ttu-id="d20b4-120">educationSynchronizationStatus</span><span class="sxs-lookup"><span data-stu-id="d20b4-120">educationSynchronizationStatus</span></span> | <span data-ttu-id="d20b4-121">Состояние синхронизации. Возможные значения: `paused`, `inProgress`, `success`, `error`, `quarantined`, `validationError`.</span><span class="sxs-lookup"><span data-stu-id="d20b4-121">The status of a sync. Possible values are: `paused`, `inProgress`, `success`, `error`, `quarantined`, `validationError`.</span></span> |
| <span data-ttu-id="d20b4-122">**lastSynchronizationDateTime**</span><span class="sxs-lookup"><span data-stu-id="d20b4-122">**lastSynchronizationDateTime**</span></span> | <span data-ttu-id="d20b4-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d20b4-123">DateTimeOffset</span></span> | <span data-ttu-id="d20b4-124">Представляет время, когда наблюдались последних изменений в каталоге.</span><span class="sxs-lookup"><span data-stu-id="d20b4-124">Represents the time when most recent changes have been observed in the directory.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="d20b4-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d20b4-125">JSON representation</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationSynchronizationProfileStatus"
}-->

```json
{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#education/synchronizationProfiles('{id}')/profileStatus/$entity",
    "status": {"@odata.type":"microsoft.graph.educationSynchronizationStatus"},
    "lastSynchronizationDateTime": "DateTimeOffset"
}
```

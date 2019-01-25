---
title: Тип ресурса educationSynchronizationProfileStatus
description: 'Представляет состояние синхронизации профилей синхронизации данных school. '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 12908f6454cb27c673935f1e4c64c921b7ff0dcd
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523542"
---
# <a name="educationsynchronizationprofilestatus-resource-type"></a><span data-ttu-id="91386-103">Тип ресурса educationSynchronizationProfileStatus</span><span class="sxs-lookup"><span data-stu-id="91386-103">educationSynchronizationProfileStatus resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="91386-104">Представляет состояния синхронизации данных school [синхронизации профилей](educationsynchronizationprofile.md).</span><span class="sxs-lookup"><span data-stu-id="91386-104">Represents the synchronization status of a school data [synchronization profile](educationsynchronizationprofile.md).</span></span> 

> <span data-ttu-id="91386-105">**Примечание:** Обновления для **educationSynchronizationProfileStatus** может отложить из-за асинхронной фоновой синхронизации обработки.</span><span class="sxs-lookup"><span data-stu-id="91386-105">**Note:** Updates to the **educationSynchronizationProfileStatus** might be delayed due to the asynchronous nature of background sync processing.</span></span>

## <a name="methods"></a><span data-ttu-id="91386-106">Методы</span><span class="sxs-lookup"><span data-stu-id="91386-106">Methods</span></span>

| <span data-ttu-id="91386-107">Метод</span><span class="sxs-lookup"><span data-stu-id="91386-107">Method</span></span> | <span data-ttu-id="91386-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="91386-108">Return Type</span></span> | <span data-ttu-id="91386-109">Описание</span><span class="sxs-lookup"><span data-stu-id="91386-109">Description</span></span> |
|:-|:-|:-|
| [<span data-ttu-id="91386-110">Получение состояния синхронизации</span><span class="sxs-lookup"><span data-stu-id="91386-110">Get status of a sync</span></span>](../api/educationsynchronizationprofilestatus-get.md) | <span data-ttu-id="91386-111">**educationSynchronizationProfileStatus**</span><span class="sxs-lookup"><span data-stu-id="91386-111">**educationSynchronizationProfileStatus**</span></span> | <span data-ttu-id="91386-112">Возвращает состояние определенного синхронизации профилей.</span><span class="sxs-lookup"><span data-stu-id="91386-112">Return the status of a specific synchronization profile.</span></span> |

## <a name="properties"></a><span data-ttu-id="91386-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="91386-113">Properties</span></span>

| <span data-ttu-id="91386-114">Свойство</span><span class="sxs-lookup"><span data-stu-id="91386-114">Property</span></span> | <span data-ttu-id="91386-115">Тип</span><span class="sxs-lookup"><span data-stu-id="91386-115">Type</span></span> | <span data-ttu-id="91386-116">Описание</span><span class="sxs-lookup"><span data-stu-id="91386-116">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="91386-117">**status**</span><span class="sxs-lookup"><span data-stu-id="91386-117">**status**</span></span> | <span data-ttu-id="91386-118">educationSynchronizationStatus</span><span class="sxs-lookup"><span data-stu-id="91386-118">educationSynchronizationStatus</span></span> | <span data-ttu-id="91386-119">Состояние синхронизации. Возможные значения: `paused`, `inProgress`, `success`, `error`, `quarantined`, `validationError`.</span><span class="sxs-lookup"><span data-stu-id="91386-119">The status of a sync. Possible values are: `paused`, `inProgress`, `success`, `error`, `quarantined`, `validationError`.</span></span> |
| <span data-ttu-id="91386-120">**lastSynchronizationDateTime**</span><span class="sxs-lookup"><span data-stu-id="91386-120">**lastSynchronizationDateTime**</span></span> | <span data-ttu-id="91386-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="91386-121">DateTimeOffset</span></span> | <span data-ttu-id="91386-122">Представляет время, когда наблюдались последних изменений в каталоге.</span><span class="sxs-lookup"><span data-stu-id="91386-122">Represents the time when most recent changes have been observed in the directory.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="91386-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="91386-123">JSON representation</span></span>
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
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationsynchronizationprofilestatus.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

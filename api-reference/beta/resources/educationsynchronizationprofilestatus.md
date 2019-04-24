---
title: Тип ресурса Едукатионсинчронизатионпрофилестатус
description: 'Представляет состояние синхронизации профиля School Data Synchronization. '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 12908f6454cb27c673935f1e4c64c921b7ff0dcd
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32507095"
---
# <a name="educationsynchronizationprofilestatus-resource-type"></a><span data-ttu-id="43e5b-103">Тип ресурса Едукатионсинчронизатионпрофилестатус</span><span class="sxs-lookup"><span data-stu-id="43e5b-103">educationSynchronizationProfileStatus resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="43e5b-104">Представляет состояние синхронизации профиля School Data [Synchronization](educationsynchronizationprofile.md).</span><span class="sxs-lookup"><span data-stu-id="43e5b-104">Represents the synchronization status of a school data [synchronization profile](educationsynchronizationprofile.md).</span></span> 

> <span data-ttu-id="43e5b-105">**Примечание:** Обновление **едукатионсинчронизатионпрофилестатус** может быть отложено из-за асинхронной обработки фоновой синхронизации.</span><span class="sxs-lookup"><span data-stu-id="43e5b-105">**Note:** Updates to the **educationSynchronizationProfileStatus** might be delayed due to the asynchronous nature of background sync processing.</span></span>

## <a name="methods"></a><span data-ttu-id="43e5b-106">Методы</span><span class="sxs-lookup"><span data-stu-id="43e5b-106">Methods</span></span>

| <span data-ttu-id="43e5b-107">Метод</span><span class="sxs-lookup"><span data-stu-id="43e5b-107">Method</span></span> | <span data-ttu-id="43e5b-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="43e5b-108">Return Type</span></span> | <span data-ttu-id="43e5b-109">Описание</span><span class="sxs-lookup"><span data-stu-id="43e5b-109">Description</span></span> |
|:-|:-|:-|
| [<span data-ttu-id="43e5b-110">Получение состояния синхронизации</span><span class="sxs-lookup"><span data-stu-id="43e5b-110">Get status of a sync</span></span>](../api/educationsynchronizationprofilestatus-get.md) | <span data-ttu-id="43e5b-111">**Едукатионсинчронизатионпрофилестатус**</span><span class="sxs-lookup"><span data-stu-id="43e5b-111">**educationSynchronizationProfileStatus**</span></span> | <span data-ttu-id="43e5b-112">Возврат состояния определенного профиля синхронизации.</span><span class="sxs-lookup"><span data-stu-id="43e5b-112">Return the status of a specific synchronization profile.</span></span> |

## <a name="properties"></a><span data-ttu-id="43e5b-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="43e5b-113">Properties</span></span>

| <span data-ttu-id="43e5b-114">Свойство</span><span class="sxs-lookup"><span data-stu-id="43e5b-114">Property</span></span> | <span data-ttu-id="43e5b-115">Тип</span><span class="sxs-lookup"><span data-stu-id="43e5b-115">Type</span></span> | <span data-ttu-id="43e5b-116">Описание</span><span class="sxs-lookup"><span data-stu-id="43e5b-116">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="43e5b-117">**status**</span><span class="sxs-lookup"><span data-stu-id="43e5b-117">**status**</span></span> | <span data-ttu-id="43e5b-118">Едукатионсинчронизатионстатус</span><span class="sxs-lookup"><span data-stu-id="43e5b-118">educationSynchronizationStatus</span></span> | <span data-ttu-id="43e5b-119">Состояние синхронизации. Возможные `paused`значения:, `inProgress`, `success`, `error`, `quarantined`,. `validationError`</span><span class="sxs-lookup"><span data-stu-id="43e5b-119">The status of a sync. Possible values are: `paused`, `inProgress`, `success`, `error`, `quarantined`, `validationError`.</span></span> |
| <span data-ttu-id="43e5b-120">**Ластсинчронизатиондатетиме**</span><span class="sxs-lookup"><span data-stu-id="43e5b-120">**lastSynchronizationDateTime**</span></span> | <span data-ttu-id="43e5b-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="43e5b-121">DateTimeOffset</span></span> | <span data-ttu-id="43e5b-122">Представляет время, в течение которого последние изменения были просмотрены в каталоге.</span><span class="sxs-lookup"><span data-stu-id="43e5b-122">Represents the time when most recent changes have been observed in the directory.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="43e5b-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="43e5b-123">JSON representation</span></span>
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

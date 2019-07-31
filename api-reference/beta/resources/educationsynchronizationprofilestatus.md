---
title: Тип ресурса Едукатионсинчронизатионпрофилестатус
description: 'Представляет состояние синхронизации профиля School Data Synchronization. '
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 827d54fbedbf9c6f386063d82fd00e8eddfe7296
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972343"
---
# <a name="educationsynchronizationprofilestatus-resource-type"></a><span data-ttu-id="dee7e-103">Тип ресурса Едукатионсинчронизатионпрофилестатус</span><span class="sxs-lookup"><span data-stu-id="dee7e-103">educationSynchronizationProfileStatus resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dee7e-104">Представляет состояние синхронизации профиля School Data [Synchronization](educationsynchronizationprofile.md).</span><span class="sxs-lookup"><span data-stu-id="dee7e-104">Represents the synchronization status of a school data [synchronization profile](educationsynchronizationprofile.md).</span></span> 

> <span data-ttu-id="dee7e-105">**Примечание:** Обновление **едукатионсинчронизатионпрофилестатус** может быть отложено из-за асинхронной обработки фоновой синхронизации.</span><span class="sxs-lookup"><span data-stu-id="dee7e-105">**Note:** Updates to the **educationSynchronizationProfileStatus** might be delayed due to the asynchronous nature of background sync processing.</span></span>

## <a name="methods"></a><span data-ttu-id="dee7e-106">Методы</span><span class="sxs-lookup"><span data-stu-id="dee7e-106">Methods</span></span>

| <span data-ttu-id="dee7e-107">Метод</span><span class="sxs-lookup"><span data-stu-id="dee7e-107">Method</span></span> | <span data-ttu-id="dee7e-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="dee7e-108">Return Type</span></span> | <span data-ttu-id="dee7e-109">Описание</span><span class="sxs-lookup"><span data-stu-id="dee7e-109">Description</span></span> |
|:-|:-|:-|
| [<span data-ttu-id="dee7e-110">Получение состояния синхронизации</span><span class="sxs-lookup"><span data-stu-id="dee7e-110">Get status of a sync</span></span>](../api/educationsynchronizationprofilestatus-get.md) | <span data-ttu-id="dee7e-111">**Едукатионсинчронизатионпрофилестатус**</span><span class="sxs-lookup"><span data-stu-id="dee7e-111">**educationSynchronizationProfileStatus**</span></span> | <span data-ttu-id="dee7e-112">Возврат состояния определенного профиля синхронизации.</span><span class="sxs-lookup"><span data-stu-id="dee7e-112">Return the status of a specific synchronization profile.</span></span> |

## <a name="properties"></a><span data-ttu-id="dee7e-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="dee7e-113">Properties</span></span>

| <span data-ttu-id="dee7e-114">Свойство</span><span class="sxs-lookup"><span data-stu-id="dee7e-114">Property</span></span> | <span data-ttu-id="dee7e-115">Тип</span><span class="sxs-lookup"><span data-stu-id="dee7e-115">Type</span></span> | <span data-ttu-id="dee7e-116">Описание</span><span class="sxs-lookup"><span data-stu-id="dee7e-116">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="dee7e-117">**status**</span><span class="sxs-lookup"><span data-stu-id="dee7e-117">**status**</span></span> | <span data-ttu-id="dee7e-118">Едукатионсинчронизатионстатус</span><span class="sxs-lookup"><span data-stu-id="dee7e-118">educationSynchronizationStatus</span></span> | <span data-ttu-id="dee7e-119">Состояние синхронизации. Возможные `paused`значения:, `inProgress`, `success`, `error`, `quarantined`,. `validationError`</span><span class="sxs-lookup"><span data-stu-id="dee7e-119">The status of a sync. Possible values are: `paused`, `inProgress`, `success`, `error`, `quarantined`, `validationError`.</span></span> |
| <span data-ttu-id="dee7e-120">**Ластсинчронизатиондатетиме**</span><span class="sxs-lookup"><span data-stu-id="dee7e-120">**lastSynchronizationDateTime**</span></span> | <span data-ttu-id="dee7e-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dee7e-121">DateTimeOffset</span></span> | <span data-ttu-id="dee7e-122">Представляет время, в течение которого последние изменения были просмотрены в каталоге.</span><span class="sxs-lookup"><span data-stu-id="dee7e-122">Represents the time when most recent changes have been observed in the directory.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="dee7e-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="dee7e-123">JSON representation</span></span>
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

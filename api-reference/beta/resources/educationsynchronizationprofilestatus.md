---
title: Тип ресурса Едукатионсинчронизатионпрофилестатус
description: 'Представляет состояние синхронизации профиля School Data Synchronization. '
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 88e2f85cc4b24bd55cdfc1fbc5aeecd7bee8c461
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42500032"
---
# <a name="educationsynchronizationprofilestatus-resource-type"></a><span data-ttu-id="b84f2-103">Тип ресурса Едукатионсинчронизатионпрофилестатус</span><span class="sxs-lookup"><span data-stu-id="b84f2-103">educationSynchronizationProfileStatus resource type</span></span>

<span data-ttu-id="b84f2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b84f2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b84f2-105">Представляет состояние синхронизации профиля School Data [Synchronization](educationsynchronizationprofile.md).</span><span class="sxs-lookup"><span data-stu-id="b84f2-105">Represents the synchronization status of a school data [synchronization profile](educationsynchronizationprofile.md).</span></span> 

> <span data-ttu-id="b84f2-106">**Примечание:** Обновление **едукатионсинчронизатионпрофилестатус** может быть отложено из-за асинхронной обработки фоновой синхронизации.</span><span class="sxs-lookup"><span data-stu-id="b84f2-106">**Note:** Updates to the **educationSynchronizationProfileStatus** might be delayed due to the asynchronous nature of background sync processing.</span></span>

## <a name="methods"></a><span data-ttu-id="b84f2-107">Методы</span><span class="sxs-lookup"><span data-stu-id="b84f2-107">Methods</span></span>

| <span data-ttu-id="b84f2-108">Метод</span><span class="sxs-lookup"><span data-stu-id="b84f2-108">Method</span></span> | <span data-ttu-id="b84f2-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="b84f2-109">Return Type</span></span> | <span data-ttu-id="b84f2-110">Описание</span><span class="sxs-lookup"><span data-stu-id="b84f2-110">Description</span></span> |
|:-|:-|:-|
| [<span data-ttu-id="b84f2-111">Получение состояния синхронизации</span><span class="sxs-lookup"><span data-stu-id="b84f2-111">Get status of a sync</span></span>](../api/educationsynchronizationprofilestatus-get.md) | <span data-ttu-id="b84f2-112">**едукатионсинчронизатионпрофилестатус**</span><span class="sxs-lookup"><span data-stu-id="b84f2-112">**educationSynchronizationProfileStatus**</span></span> | <span data-ttu-id="b84f2-113">Возврат состояния определенного профиля синхронизации.</span><span class="sxs-lookup"><span data-stu-id="b84f2-113">Return the status of a specific synchronization profile.</span></span> |

## <a name="properties"></a><span data-ttu-id="b84f2-114">Свойства</span><span class="sxs-lookup"><span data-stu-id="b84f2-114">Properties</span></span>

| <span data-ttu-id="b84f2-115">Свойство</span><span class="sxs-lookup"><span data-stu-id="b84f2-115">Property</span></span> | <span data-ttu-id="b84f2-116">Тип</span><span class="sxs-lookup"><span data-stu-id="b84f2-116">Type</span></span> | <span data-ttu-id="b84f2-117">Описание</span><span class="sxs-lookup"><span data-stu-id="b84f2-117">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="b84f2-118">**status**</span><span class="sxs-lookup"><span data-stu-id="b84f2-118">**status**</span></span> | <span data-ttu-id="b84f2-119">едукатионсинчронизатионстатус</span><span class="sxs-lookup"><span data-stu-id="b84f2-119">educationSynchronizationStatus</span></span> | <span data-ttu-id="b84f2-120">Состояние синхронизации. Возможные `paused`значения:, `inProgress`, `success`, `error`, `quarantined`,. `validationError`</span><span class="sxs-lookup"><span data-stu-id="b84f2-120">The status of a sync. Possible values are: `paused`, `inProgress`, `success`, `error`, `quarantined`, `validationError`.</span></span> |
| <span data-ttu-id="b84f2-121">**ластсинчронизатиондатетиме**</span><span class="sxs-lookup"><span data-stu-id="b84f2-121">**lastSynchronizationDateTime**</span></span> | <span data-ttu-id="b84f2-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b84f2-122">DateTimeOffset</span></span> | <span data-ttu-id="b84f2-123">Представляет время, в течение которого последние изменения были просмотрены в каталоге.</span><span class="sxs-lookup"><span data-stu-id="b84f2-123">Represents the time when most recent changes have been observed in the directory.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="b84f2-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b84f2-124">JSON representation</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationSynchronizationProfileStatus"
}-->

```json
{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#education/synchronizationProfiles/{id}/profileStatus/$entity",
    "status": {"@odata.type":"microsoft.graph.educationSynchronizationStatus"},
    "lastSynchronizationDateTime": "DateTimeOffset"
}
```

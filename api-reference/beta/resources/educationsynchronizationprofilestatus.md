---
title: Тип ресурса Едукатионсинчронизатионпрофилестатус
description: 'Представляет состояние синхронизации профиля School Data Synchronization. '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: e54a80df832eba66dcdc5eb08b38feee6f4cd57a
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33340508"
---
# <a name="educationsynchronizationprofilestatus-resource-type"></a><span data-ttu-id="9f84f-103">Тип ресурса Едукатионсинчронизатионпрофилестатус</span><span class="sxs-lookup"><span data-stu-id="9f84f-103">educationSynchronizationProfileStatus resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9f84f-104">Представляет состояние синхронизации профиля School Data [Synchronization](educationsynchronizationprofile.md).</span><span class="sxs-lookup"><span data-stu-id="9f84f-104">Represents the synchronization status of a school data [synchronization profile](educationsynchronizationprofile.md).</span></span> 

> <span data-ttu-id="9f84f-105">**Примечание:** Обновление **едукатионсинчронизатионпрофилестатус** может быть отложено из-за асинхронной обработки фоновой синхронизации.</span><span class="sxs-lookup"><span data-stu-id="9f84f-105">**Note:** Updates to the **educationSynchronizationProfileStatus** might be delayed due to the asynchronous nature of background sync processing.</span></span>

## <a name="methods"></a><span data-ttu-id="9f84f-106">Методы</span><span class="sxs-lookup"><span data-stu-id="9f84f-106">Methods</span></span>

| <span data-ttu-id="9f84f-107">Метод</span><span class="sxs-lookup"><span data-stu-id="9f84f-107">Method</span></span> | <span data-ttu-id="9f84f-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="9f84f-108">Return Type</span></span> | <span data-ttu-id="9f84f-109">Описание</span><span class="sxs-lookup"><span data-stu-id="9f84f-109">Description</span></span> |
|:-|:-|:-|
| [<span data-ttu-id="9f84f-110">Получение состояния синхронизации</span><span class="sxs-lookup"><span data-stu-id="9f84f-110">Get status of a sync</span></span>](../api/educationsynchronizationprofilestatus-get.md) | <span data-ttu-id="9f84f-111">**Едукатионсинчронизатионпрофилестатус**</span><span class="sxs-lookup"><span data-stu-id="9f84f-111">**educationSynchronizationProfileStatus**</span></span> | <span data-ttu-id="9f84f-112">Возврат состояния определенного профиля синхронизации.</span><span class="sxs-lookup"><span data-stu-id="9f84f-112">Return the status of a specific synchronization profile.</span></span> |

## <a name="properties"></a><span data-ttu-id="9f84f-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="9f84f-113">Properties</span></span>

| <span data-ttu-id="9f84f-114">Свойство</span><span class="sxs-lookup"><span data-stu-id="9f84f-114">Property</span></span> | <span data-ttu-id="9f84f-115">Тип</span><span class="sxs-lookup"><span data-stu-id="9f84f-115">Type</span></span> | <span data-ttu-id="9f84f-116">Описание</span><span class="sxs-lookup"><span data-stu-id="9f84f-116">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="9f84f-117">**status**</span><span class="sxs-lookup"><span data-stu-id="9f84f-117">**status**</span></span> | <span data-ttu-id="9f84f-118">Едукатионсинчронизатионстатус</span><span class="sxs-lookup"><span data-stu-id="9f84f-118">educationSynchronizationStatus</span></span> | <span data-ttu-id="9f84f-119">Состояние синхронизации. Возможные `paused`значения:, `inProgress`, `success`, `error`, `quarantined`,. `validationError`</span><span class="sxs-lookup"><span data-stu-id="9f84f-119">The status of a sync. Possible values are: `paused`, `inProgress`, `success`, `error`, `quarantined`, `validationError`.</span></span> |
| <span data-ttu-id="9f84f-120">**Ластсинчронизатиондатетиме**</span><span class="sxs-lookup"><span data-stu-id="9f84f-120">**lastSynchronizationDateTime**</span></span> | <span data-ttu-id="9f84f-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9f84f-121">DateTimeOffset</span></span> | <span data-ttu-id="9f84f-122">Представляет время, в течение которого последние изменения были просмотрены в каталоге.</span><span class="sxs-lookup"><span data-stu-id="9f84f-122">Represents the time when most recent changes have been observed in the directory.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="9f84f-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9f84f-123">JSON representation</span></span>
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

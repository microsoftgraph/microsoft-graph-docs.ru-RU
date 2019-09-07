---
title: Тип ресурса Едукатионсинчронизатионпрофилестатус
description: 'Представляет состояние синхронизации профиля School Data Synchronization. '
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: e3cc519f30b571d6c69dce48b74cd70da7f58e6f
ms.sourcegitcommit: c68a83d28fa4bfca6e0618467934813a9ae17b12
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/07/2019
ms.locfileid: "36792816"
---
# <a name="educationsynchronizationprofilestatus-resource-type"></a><span data-ttu-id="f7092-103">Тип ресурса Едукатионсинчронизатионпрофилестатус</span><span class="sxs-lookup"><span data-stu-id="f7092-103">educationSynchronizationProfileStatus resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f7092-104">Представляет состояние синхронизации профиля School Data [Synchronization](educationsynchronizationprofile.md).</span><span class="sxs-lookup"><span data-stu-id="f7092-104">Represents the synchronization status of a school data [synchronization profile](educationsynchronizationprofile.md).</span></span> 

> <span data-ttu-id="f7092-105">**Примечание:** Обновление **едукатионсинчронизатионпрофилестатус** может быть отложено из-за асинхронной обработки фоновой синхронизации.</span><span class="sxs-lookup"><span data-stu-id="f7092-105">**Note:** Updates to the **educationSynchronizationProfileStatus** might be delayed due to the asynchronous nature of background sync processing.</span></span>

## <a name="methods"></a><span data-ttu-id="f7092-106">Методы</span><span class="sxs-lookup"><span data-stu-id="f7092-106">Methods</span></span>

| <span data-ttu-id="f7092-107">Метод</span><span class="sxs-lookup"><span data-stu-id="f7092-107">Method</span></span> | <span data-ttu-id="f7092-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="f7092-108">Return Type</span></span> | <span data-ttu-id="f7092-109">Описание</span><span class="sxs-lookup"><span data-stu-id="f7092-109">Description</span></span> |
|:-|:-|:-|
| [<span data-ttu-id="f7092-110">Получение состояния синхронизации</span><span class="sxs-lookup"><span data-stu-id="f7092-110">Get status of a sync</span></span>](../api/educationsynchronizationprofilestatus-get.md) | <span data-ttu-id="f7092-111">**едукатионсинчронизатионпрофилестатус**</span><span class="sxs-lookup"><span data-stu-id="f7092-111">**educationSynchronizationProfileStatus**</span></span> | <span data-ttu-id="f7092-112">Возврат состояния определенного профиля синхронизации.</span><span class="sxs-lookup"><span data-stu-id="f7092-112">Return the status of a specific synchronization profile.</span></span> |

## <a name="properties"></a><span data-ttu-id="f7092-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="f7092-113">Properties</span></span>

| <span data-ttu-id="f7092-114">Свойство</span><span class="sxs-lookup"><span data-stu-id="f7092-114">Property</span></span> | <span data-ttu-id="f7092-115">Тип</span><span class="sxs-lookup"><span data-stu-id="f7092-115">Type</span></span> | <span data-ttu-id="f7092-116">Описание</span><span class="sxs-lookup"><span data-stu-id="f7092-116">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="f7092-117">**status**</span><span class="sxs-lookup"><span data-stu-id="f7092-117">**status**</span></span> | <span data-ttu-id="f7092-118">едукатионсинчронизатионстатус</span><span class="sxs-lookup"><span data-stu-id="f7092-118">educationSynchronizationStatus</span></span> | <span data-ttu-id="f7092-119">Состояние синхронизации. Возможные `paused`значения:, `inProgress`, `success`, `error`, `quarantined`,. `validationError`</span><span class="sxs-lookup"><span data-stu-id="f7092-119">The status of a sync. Possible values are: `paused`, `inProgress`, `success`, `error`, `quarantined`, `validationError`.</span></span> |
| <span data-ttu-id="f7092-120">**ластсинчронизатиондатетиме**</span><span class="sxs-lookup"><span data-stu-id="f7092-120">**lastSynchronizationDateTime**</span></span> | <span data-ttu-id="f7092-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f7092-121">DateTimeOffset</span></span> | <span data-ttu-id="f7092-122">Представляет время, в течение которого последние изменения были просмотрены в каталоге.</span><span class="sxs-lookup"><span data-stu-id="f7092-122">Represents the time when most recent changes have been observed in the directory.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="f7092-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f7092-123">JSON representation</span></span>
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

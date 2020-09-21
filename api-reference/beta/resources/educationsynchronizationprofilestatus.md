---
title: Тип ресурса Едукатионсинчронизатионпрофилестатус
description: 'Представляет состояние синхронизации профиля School Data Synchronization. '
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 0e792b55cddaee3069eaaf53cc9dce68aae041e9
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47979555"
---
# <a name="educationsynchronizationprofilestatus-resource-type"></a><span data-ttu-id="83154-103">Тип ресурса Едукатионсинчронизатионпрофилестатус</span><span class="sxs-lookup"><span data-stu-id="83154-103">educationSynchronizationProfileStatus resource type</span></span>

<span data-ttu-id="83154-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="83154-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="83154-105">Представляет состояние синхронизации профиля School Data [Synchronization](educationsynchronizationprofile.md).</span><span class="sxs-lookup"><span data-stu-id="83154-105">Represents the synchronization status of a school data [synchronization profile](educationsynchronizationprofile.md).</span></span>

> <span data-ttu-id="83154-106">**Примечание:** Обновление **едукатионсинчронизатионпрофилестатус** может быть отложено из-за асинхронной обработки фоновой синхронизации.</span><span class="sxs-lookup"><span data-stu-id="83154-106">**Note:** Updates to the **educationSynchronizationProfileStatus** might be delayed due to the asynchronous nature of background sync processing.</span></span>

## <a name="methods"></a><span data-ttu-id="83154-107">Методы</span><span class="sxs-lookup"><span data-stu-id="83154-107">Methods</span></span>

| <span data-ttu-id="83154-108">Метод</span><span class="sxs-lookup"><span data-stu-id="83154-108">Method</span></span>                                                                      | <span data-ttu-id="83154-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="83154-109">Return Type</span></span>                               | <span data-ttu-id="83154-110">Описание</span><span class="sxs-lookup"><span data-stu-id="83154-110">Description</span></span>                                              |
| :-------------------------------------------------------------------------- | :---------------------------------------- | :------------------------------------------------------- |
| [<span data-ttu-id="83154-111">Получение состояния синхронизации</span><span class="sxs-lookup"><span data-stu-id="83154-111">Get status of a sync</span></span>](../api/educationsynchronizationprofilestatus-get.md) | <span data-ttu-id="83154-112">**едукатионсинчронизатионпрофилестатус**</span><span class="sxs-lookup"><span data-stu-id="83154-112">**educationSynchronizationProfileStatus**</span></span> | <span data-ttu-id="83154-113">Возврат состояния определенного профиля синхронизации.</span><span class="sxs-lookup"><span data-stu-id="83154-113">Return the status of a specific synchronization profile.</span></span> |

## <a name="properties"></a><span data-ttu-id="83154-114">Свойства</span><span class="sxs-lookup"><span data-stu-id="83154-114">Properties</span></span>

| <span data-ttu-id="83154-115">Свойство</span><span class="sxs-lookup"><span data-stu-id="83154-115">Property</span></span>                    | <span data-ttu-id="83154-116">Тип</span><span class="sxs-lookup"><span data-stu-id="83154-116">Type</span></span>                           | <span data-ttu-id="83154-117">Описание</span><span class="sxs-lookup"><span data-stu-id="83154-117">Description</span></span>                                                                                                              |
| :-------------------------- | :----------------------------- | :----------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="83154-118">id</span><span class="sxs-lookup"><span data-stu-id="83154-118">id</span></span>                          | <span data-ttu-id="83154-119">String</span><span class="sxs-lookup"><span data-stu-id="83154-119">String</span></span>                         | <span data-ttu-id="83154-120">Уникальный идентификатор ресурса.</span><span class="sxs-lookup"><span data-stu-id="83154-120">The unique identifier for the resource.</span></span> <span data-ttu-id="83154-121">(только для чтения)</span><span class="sxs-lookup"><span data-stu-id="83154-121">(read-only)</span></span>                                                                      |
| <span data-ttu-id="83154-122">status</span><span class="sxs-lookup"><span data-stu-id="83154-122">status</span></span>                      | <span data-ttu-id="83154-123">едукатионсинчронизатионстатус</span><span class="sxs-lookup"><span data-stu-id="83154-123">educationSynchronizationStatus</span></span> | <span data-ttu-id="83154-124">Состояние синхронизации. Возможные значения: `paused` ,, `inProgress` , `success` , `error` `quarantined` , `validationError` .</span><span class="sxs-lookup"><span data-stu-id="83154-124">The status of a sync. Possible values are: `paused`, `inProgress`, `success`, `error`, `quarantined`, `validationError`.</span></span> |
| <span data-ttu-id="83154-125">ластсинчронизатиондатетиме</span><span class="sxs-lookup"><span data-stu-id="83154-125">lastSynchronizationDateTime</span></span> | <span data-ttu-id="83154-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="83154-126">DateTimeOffset</span></span>                 | <span data-ttu-id="83154-127">Представляет время, в течение которого последние изменения были просмотрены в каталоге.</span><span class="sxs-lookup"><span data-stu-id="83154-127">Represents the time when most recent changes have been observed in the directory.</span></span>                                        |

## <a name="json-representation"></a><span data-ttu-id="83154-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="83154-128">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationSynchronizationProfileStatus"
}-->

```json
{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#education/synchronizationProfiles/{id}/profileStatus/$entity",
  "id": "String",
  "status": { "@odata.type": "microsoft.graph.educationSynchronizationStatus" },
  "lastSynchronizationDateTime": "DateTimeOffset"
}
```



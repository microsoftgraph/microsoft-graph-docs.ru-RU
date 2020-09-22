---
title: Тип ресурса Счедулеинформатион
description: 'Представляет доступность пользователя, списка рассылки или ресурса за указанный период времени. '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-teams
author: harini84
ms.openlocfilehash: d503ec6241bd73492a5790f3f0f7b76a44b6245e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47985820"
---
# <a name="scheduleinformation-resource-type"></a><span data-ttu-id="32d53-103">Тип ресурса Счедулеинформатион</span><span class="sxs-lookup"><span data-stu-id="32d53-103">scheduleInformation resource type</span></span>

<span data-ttu-id="32d53-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="32d53-104">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="32d53-105">Представляет доступность пользователя, списка рассылки или ресурса (помещения или оборудования) за указанный период времени.</span><span class="sxs-lookup"><span data-stu-id="32d53-105">Represents the availability of a user, distribution list, or resource (room or equipment) for a specified time period.</span></span>

## <a name="properties"></a><span data-ttu-id="32d53-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="32d53-106">Properties</span></span>
| <span data-ttu-id="32d53-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="32d53-107">Property</span></span>     | <span data-ttu-id="32d53-108">Тип</span><span class="sxs-lookup"><span data-stu-id="32d53-108">Type</span></span>   |<span data-ttu-id="32d53-109">Описание</span><span class="sxs-lookup"><span data-stu-id="32d53-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="32d53-110">аваилабилитивиев</span><span class="sxs-lookup"><span data-stu-id="32d53-110">availabilityView</span></span> |<span data-ttu-id="32d53-111">String</span><span class="sxs-lookup"><span data-stu-id="32d53-111">String</span></span> |<span data-ttu-id="32d53-112">Представляет объединенное представление доступности всех элементов в `scheduleItems` .</span><span class="sxs-lookup"><span data-stu-id="32d53-112">Represents a merged view of availability of all the items in `scheduleItems`.</span></span> <span data-ttu-id="32d53-113">Представление состоит из временных слотов.</span><span class="sxs-lookup"><span data-stu-id="32d53-113">The view consists of time slots.</span></span> <span data-ttu-id="32d53-114">Доступность во время каждого временного слота указывается следующим образом: `0` = Free, `1` = под вопросом, `2` = занят, `3` = нет на месте, `4` Рабочий процесс.</span><span class="sxs-lookup"><span data-stu-id="32d53-114">Availability during each time slot is indicated with: `0`= free, `1`= tentative, `2`= busy, `3`= out of office, `4`= working elsewhere.</span></span>|
|<span data-ttu-id="32d53-115">error</span><span class="sxs-lookup"><span data-stu-id="32d53-115">error</span></span> |[<span data-ttu-id="32d53-116">фрибусеррор</span><span class="sxs-lookup"><span data-stu-id="32d53-116">freeBusyError</span></span>](freebusyerror.md) |<span data-ttu-id="32d53-117">Сведения об ошибке при попытке получить сведения о доступности пользователя, списка рассылки или ресурса.</span><span class="sxs-lookup"><span data-stu-id="32d53-117">Error information from attempting to get the availability of the user, distribution list, or resource.</span></span> |
|<span data-ttu-id="32d53-118">счедулеид</span><span class="sxs-lookup"><span data-stu-id="32d53-118">scheduleId</span></span> |<span data-ttu-id="32d53-119">String</span><span class="sxs-lookup"><span data-stu-id="32d53-119">String</span></span> |<span data-ttu-id="32d53-120">SMTP-адрес пользователя, списка рассылки или ресурса, определяющего экземпляр **счедулеинформатион**.</span><span class="sxs-lookup"><span data-stu-id="32d53-120">An SMTP address of the user, distribution list, or resource, identifying an instance of **scheduleInformation**.</span></span> |
|<span data-ttu-id="32d53-121">счедулеитемс</span><span class="sxs-lookup"><span data-stu-id="32d53-121">scheduleItems</span></span> |<span data-ttu-id="32d53-122">Коллекция [счедулеитем](scheduleitem.md)</span><span class="sxs-lookup"><span data-stu-id="32d53-122">[scheduleItem](scheduleitem.md) collection</span></span> |<span data-ttu-id="32d53-123">Содержит элементы, описывающие доступность пользователя или ресурса.</span><span class="sxs-lookup"><span data-stu-id="32d53-123">Contains the items that describe the availability of the user or resource.</span></span> |
|<span data-ttu-id="32d53-124">workingHours</span><span class="sxs-lookup"><span data-stu-id="32d53-124">workingHours</span></span> |[<span data-ttu-id="32d53-125">workingHours</span><span class="sxs-lookup"><span data-stu-id="32d53-125">workingHours</span></span>](workinghours.md) |<span data-ttu-id="32d53-126">Дни недели и часы работы пользователя в определенном часовом поясе.</span><span class="sxs-lookup"><span data-stu-id="32d53-126">The days of the week and hours in a specific time zone that the user works.</span></span> <span data-ttu-id="32d53-127">Они задаются как часть [mailboxSettings](mailboxsettings.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="32d53-127">These are set as part of the user's [mailboxSettings](mailboxsettings.md).</span></span>|


## <a name="json-representation"></a><span data-ttu-id="32d53-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="32d53-128">JSON representation</span></span>

<span data-ttu-id="32d53-129">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="32d53-129">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.scheduleInformation"
}-->

```json
{
  "availabilityView": "String",
  "error": {"@odata.type": "microsoft.graph.freeBusyError"},
  "scheduleId": "String",
  "scheduleItems": [{"@odata.type": "microsoft.graph.scheduleItem"}],
  "workingHours": {"@odata.type": "microsoft.graph.workingHours"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "scheduleInformation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->



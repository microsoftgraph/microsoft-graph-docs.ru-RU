---
title: Тип ресурса Счедулеинформатион
description: 'Представляет доступность пользователя, списка рассылки или ресурса за указанный период времени. '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-teams
author: ''
ms.openlocfilehash: e43bd0fc88cd8b7cdcb793deca8940ccaae9461f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520979"
---
# <a name="scheduleinformation-resource-type"></a><span data-ttu-id="53ba3-103">Тип ресурса Счедулеинформатион</span><span class="sxs-lookup"><span data-stu-id="53ba3-103">scheduleInformation resource type</span></span>

<span data-ttu-id="53ba3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="53ba3-104">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="53ba3-105">Представляет доступность пользователя, списка рассылки или ресурса (помещения или оборудования) за указанный период времени.</span><span class="sxs-lookup"><span data-stu-id="53ba3-105">Represents the availability of a user, distribution list, or resource (room or equipment) for a specified time period.</span></span>

## <a name="properties"></a><span data-ttu-id="53ba3-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="53ba3-106">Properties</span></span>
| <span data-ttu-id="53ba3-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="53ba3-107">Property</span></span>     | <span data-ttu-id="53ba3-108">Тип</span><span class="sxs-lookup"><span data-stu-id="53ba3-108">Type</span></span>   |<span data-ttu-id="53ba3-109">Описание</span><span class="sxs-lookup"><span data-stu-id="53ba3-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="53ba3-110">аваилабилитивиев</span><span class="sxs-lookup"><span data-stu-id="53ba3-110">availabilityView</span></span> |<span data-ttu-id="53ba3-111">String</span><span class="sxs-lookup"><span data-stu-id="53ba3-111">String</span></span> |<span data-ttu-id="53ba3-112">Представляет объединенное представление доступности всех элементов в `scheduleItems`.</span><span class="sxs-lookup"><span data-stu-id="53ba3-112">Represents a merged view of availability of all the items in `scheduleItems`.</span></span> <span data-ttu-id="53ba3-113">Представление состоит из временных слотов.</span><span class="sxs-lookup"><span data-stu-id="53ba3-113">The view consists of time slots.</span></span> <span data-ttu-id="53ba3-114">Доступность во время каждого временного слота указывается следующим `0`образом: = `1`Free, = `2`под вопросом, `3`= занят, = нет `4`на месте, Рабочий процесс.</span><span class="sxs-lookup"><span data-stu-id="53ba3-114">Availability during each time slot is indicated with: `0`= free, `1`= tentative, `2`= busy, `3`= out of office, `4`= working elsewhere.</span></span>|
|<span data-ttu-id="53ba3-115">error</span><span class="sxs-lookup"><span data-stu-id="53ba3-115">error</span></span> |[<span data-ttu-id="53ba3-116">фрибусеррор</span><span class="sxs-lookup"><span data-stu-id="53ba3-116">freeBusyError</span></span>](freebusyerror.md) |<span data-ttu-id="53ba3-117">Сведения об ошибке при попытке получить сведения о доступности пользователя, списка рассылки или ресурса.</span><span class="sxs-lookup"><span data-stu-id="53ba3-117">Error information from attempting to get the availability of the user, distribution list, or resource.</span></span> |
|<span data-ttu-id="53ba3-118">счедулеид</span><span class="sxs-lookup"><span data-stu-id="53ba3-118">scheduleId</span></span> |<span data-ttu-id="53ba3-119">String</span><span class="sxs-lookup"><span data-stu-id="53ba3-119">String</span></span> |<span data-ttu-id="53ba3-120">SMTP-адрес пользователя, списка рассылки или ресурса, определяющего экземпляр **счедулеинформатион**.</span><span class="sxs-lookup"><span data-stu-id="53ba3-120">An SMTP address of the user, distribution list, or resource, identifying an instance of **scheduleInformation**.</span></span> |
|<span data-ttu-id="53ba3-121">счедулеитемс</span><span class="sxs-lookup"><span data-stu-id="53ba3-121">scheduleItems</span></span> |<span data-ttu-id="53ba3-122">Коллекция [счедулеитем](scheduleitem.md)</span><span class="sxs-lookup"><span data-stu-id="53ba3-122">[scheduleItem](scheduleitem.md) collection</span></span> |<span data-ttu-id="53ba3-123">Содержит элементы, описывающие доступность пользователя или ресурса.</span><span class="sxs-lookup"><span data-stu-id="53ba3-123">Contains the items that describe the availability of the user or resource.</span></span> |
|<span data-ttu-id="53ba3-124">workingHours</span><span class="sxs-lookup"><span data-stu-id="53ba3-124">workingHours</span></span> |[<span data-ttu-id="53ba3-125">workingHours</span><span class="sxs-lookup"><span data-stu-id="53ba3-125">workingHours</span></span>](workinghours.md) |<span data-ttu-id="53ba3-126">Дни недели и часы работы пользователя в определенном часовом поясе.</span><span class="sxs-lookup"><span data-stu-id="53ba3-126">The days of the week and hours in a specific time zone that the user works.</span></span> <span data-ttu-id="53ba3-127">Они задаются как часть [mailboxSettings](mailboxsettings.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="53ba3-127">These are set as part of the user's [mailboxSettings](mailboxsettings.md).</span></span>|


## <a name="json-representation"></a><span data-ttu-id="53ba3-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="53ba3-128">JSON representation</span></span>

<span data-ttu-id="53ba3-129">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="53ba3-129">The following is a JSON representation of the resource.</span></span>

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

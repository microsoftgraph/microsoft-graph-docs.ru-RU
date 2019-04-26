---
title: Тип ресурса Счедулеинформатион
description: 'Представляет доступность пользователя, списка рассылки или ресурса за указанный период времени. '
localization_priority: Normal
ms.openlocfilehash: b15d492477368d47fd3ebc9fc00bd3dcfc3e6688
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33343516"
---
# <a name="scheduleinformation-resource-type"></a><span data-ttu-id="07d4e-103">Тип ресурса Счедулеинформатион</span><span class="sxs-lookup"><span data-stu-id="07d4e-103">scheduleInformation resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="07d4e-104">Представляет доступность пользователя, списка рассылки или ресурса (помещения или оборудования) за указанный период времени.</span><span class="sxs-lookup"><span data-stu-id="07d4e-104">Represents the availability of a user, distribution list, or resource (room or equipment) for a specified time period.</span></span>

## <a name="properties"></a><span data-ttu-id="07d4e-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="07d4e-105">Properties</span></span>
| <span data-ttu-id="07d4e-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="07d4e-106">Property</span></span>     | <span data-ttu-id="07d4e-107">Тип</span><span class="sxs-lookup"><span data-stu-id="07d4e-107">Type</span></span>   |<span data-ttu-id="07d4e-108">Описание</span><span class="sxs-lookup"><span data-stu-id="07d4e-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="07d4e-109">Аваилабилитивиев</span><span class="sxs-lookup"><span data-stu-id="07d4e-109">availabilityView</span></span> |<span data-ttu-id="07d4e-110">String</span><span class="sxs-lookup"><span data-stu-id="07d4e-110">String</span></span> |<span data-ttu-id="07d4e-111">Представляет объединенное представление доступности всех элементов в `scheduleItems`.</span><span class="sxs-lookup"><span data-stu-id="07d4e-111">Represents a merged view of availability of all the items in `scheduleItems`.</span></span> <span data-ttu-id="07d4e-112">Представление состоит из временных слотов.</span><span class="sxs-lookup"><span data-stu-id="07d4e-112">The view consists of time slots.</span></span> <span data-ttu-id="07d4e-113">Доступность во время каждого временного слота указывается следующим `0`образом: = `1`Free, = `2`под вопросом, `3`= занят, = нет `4`на месте, Рабочий процесс.</span><span class="sxs-lookup"><span data-stu-id="07d4e-113">Availability during each time slot is indicated with: `0`= free, `1`= tentative, `2`= busy, `3`= out of office, `4`= working elsewhere.</span></span>|
|<span data-ttu-id="07d4e-114">error</span><span class="sxs-lookup"><span data-stu-id="07d4e-114">error</span></span> |[<span data-ttu-id="07d4e-115">Фрибусеррор</span><span class="sxs-lookup"><span data-stu-id="07d4e-115">freeBusyError</span></span>](freebusyerror.md) |<span data-ttu-id="07d4e-116">Сведения об ошибке при попытке получить сведения о доступности пользователя, списка рассылки или ресурса.</span><span class="sxs-lookup"><span data-stu-id="07d4e-116">Error information from attempting to get the availability of the user, distribution list, or resource.</span></span> |
|<span data-ttu-id="07d4e-117">Счедулеид</span><span class="sxs-lookup"><span data-stu-id="07d4e-117">scheduleId</span></span> |<span data-ttu-id="07d4e-118">String</span><span class="sxs-lookup"><span data-stu-id="07d4e-118">String</span></span> |<span data-ttu-id="07d4e-119">SMTP-адрес пользователя, списка рассылки или ресурса, определяющего экземпляр **счедулеинформатион**.</span><span class="sxs-lookup"><span data-stu-id="07d4e-119">An SMTP address of the user, distribution list, or resource, identifying an instance of **scheduleInformation**.</span></span> |
|<span data-ttu-id="07d4e-120">Счедулеитемс</span><span class="sxs-lookup"><span data-stu-id="07d4e-120">scheduleItems</span></span> |<span data-ttu-id="07d4e-121">Коллекция [счедулеитем](scheduleitem.md)</span><span class="sxs-lookup"><span data-stu-id="07d4e-121">[scheduleItem](scheduleitem.md) collection</span></span> |<span data-ttu-id="07d4e-122">Содержит элементы, описывающие доступность пользователя или ресурса.</span><span class="sxs-lookup"><span data-stu-id="07d4e-122">Contains the items that describe the availability of the user or resource.</span></span> |
|<span data-ttu-id="07d4e-123">workingHours</span><span class="sxs-lookup"><span data-stu-id="07d4e-123">workingHours</span></span> |[<span data-ttu-id="07d4e-124">workingHours</span><span class="sxs-lookup"><span data-stu-id="07d4e-124">workingHours</span></span>](workinghours.md) |<span data-ttu-id="07d4e-125">Дни недели и часы работы пользователя в определенном часовом поясе.</span><span class="sxs-lookup"><span data-stu-id="07d4e-125">The days of the week and hours in a specific time zone that the user works.</span></span> <span data-ttu-id="07d4e-126">Они задаются как часть [mailboxSettings](mailboxsettings.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="07d4e-126">These are set as part of the user's [mailboxSettings](mailboxsettings.md).</span></span>|


## <a name="json-representation"></a><span data-ttu-id="07d4e-127">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="07d4e-127">JSON representation</span></span>

<span data-ttu-id="07d4e-128">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="07d4e-128">The following is a JSON representation of the resource.</span></span>

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

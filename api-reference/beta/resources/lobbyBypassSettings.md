---
title: Тип ресурса Лоббибипасссеттингс
description: Указывает, какие участники могут обходить зал собрания.
author: frankpeng7
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 3723f6593547b75c60a82b8436995c931d64e436
ms.sourcegitcommit: 7dcae492d8b4707d068adca3a74732e25a8198e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/10/2020
ms.locfileid: "47423688"
---
# <a name="lobbybypasssettings-resource-type"></a><span data-ttu-id="3bb12-103">Тип ресурса Лоббибипасссеттингс</span><span class="sxs-lookup"><span data-stu-id="3bb12-103">lobbyBypassSettings resource type</span></span>

<span data-ttu-id="3bb12-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3bb12-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3bb12-105">Указывает, какие участники могут обходить зал собрания.</span><span class="sxs-lookup"><span data-stu-id="3bb12-105">Specifies which participants can bypass the meeting lobby.</span></span>

## <a name="properties"></a><span data-ttu-id="3bb12-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="3bb12-106">Properties</span></span>

| <span data-ttu-id="3bb12-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="3bb12-107">Property</span></span>              | <span data-ttu-id="3bb12-108">Тип</span><span class="sxs-lookup"><span data-stu-id="3bb12-108">Type</span></span>    | <span data-ttu-id="3bb12-109">Описание</span><span class="sxs-lookup"><span data-stu-id="3bb12-109">Description</span></span>                                                         | 
| --------------------- | ------- | ------------------------------------------------------------------- | 
| <span data-ttu-id="3bb12-110">scope</span><span class="sxs-lookup"><span data-stu-id="3bb12-110">scope</span></span>                 | <span data-ttu-id="3bb12-111">лоббибипассскопе</span><span class="sxs-lookup"><span data-stu-id="3bb12-111">lobbyBypassScope</span></span>  | <span data-ttu-id="3bb12-112">Указывает тип участников, которые автоматически отправляются на собрание, минуя "зал ожидания".</span><span class="sxs-lookup"><span data-stu-id="3bb12-112">Specifies the type of participants that are automatically admitted into a meeting, bypassing the lobby.</span></span> <span data-ttu-id="3bb12-113">Возможные значения перечислены в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="3bb12-113">Possible values are listed in the following table.</span></span> <span data-ttu-id="3bb12-114">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="3bb12-114">Optional.</span></span>|
| <span data-ttu-id="3bb12-115">исдиалинбипассенаблед</span><span class="sxs-lookup"><span data-stu-id="3bb12-115">isDialInBypassEnabled</span></span> | <span data-ttu-id="3bb12-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="3bb12-116">Boolean</span></span> | <span data-ttu-id="3bb12-117">Указывает, следует ли всегда разрешать абонентам с телефонным подключением обходить "зал ожидания".</span><span class="sxs-lookup"><span data-stu-id="3bb12-117">Specifies whether or not to always let dial-in callers bypass the lobby.</span></span> <span data-ttu-id="3bb12-118">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="3bb12-118">Optional.</span></span> | 

### <a name="lobbybypassscope-values"></a><span data-ttu-id="3bb12-119">значения Лоббибипассскопе</span><span class="sxs-lookup"><span data-stu-id="3bb12-119">lobbyBypassScope values</span></span>

| <span data-ttu-id="3bb12-120">Значение</span><span class="sxs-lookup"><span data-stu-id="3bb12-120">Value</span></span>                    | <span data-ttu-id="3bb12-121">Описание</span><span class="sxs-lookup"><span data-stu-id="3bb12-121">Description</span></span>                                                                                                                                              |
| ------------------------ | -------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="3bb12-122">organizer</span><span class="sxs-lookup"><span data-stu-id="3bb12-122">organizer</span></span>                | <span data-ttu-id="3bb12-123">Только организатор дойдет на собрание, минуя "зал ожидания".</span><span class="sxs-lookup"><span data-stu-id="3bb12-123">Only the organizer is admitted into the meeting, bypassing the lobby.</span></span> <span data-ttu-id="3bb12-124">Все остальные участники помещаются в зал собрания.</span><span class="sxs-lookup"><span data-stu-id="3bb12-124">All other participants are placed in the meeting lobby.</span></span>                                                                                                         |
| <span data-ttu-id="3bb12-125">organization;</span><span class="sxs-lookup"><span data-stu-id="3bb12-125">organization</span></span>             | <span data-ttu-id="3bb12-126">Только участники одной компании могут присутствовать на собрании, минуя "зал ожидания".</span><span class="sxs-lookup"><span data-stu-id="3bb12-126">Only the participants from the same company are admitted into the meeting, bypassing the lobby.</span></span> <span data-ttu-id="3bb12-127">Все остальные участники помещаются в зал собрания.</span><span class="sxs-lookup"><span data-stu-id="3bb12-127">All other participants are placed in the meeting lobby.</span></span>                                                                              |
| <span data-ttu-id="3bb12-128">организатионандфедератед</span><span class="sxs-lookup"><span data-stu-id="3bb12-128">organizationAndFederated</span></span> | <span data-ttu-id="3bb12-129">Только участники одной компании или доверенной Организации доходят на собрание, минуя "зал ожидания".</span><span class="sxs-lookup"><span data-stu-id="3bb12-129">Only the participants from the same company or trusted organization are admitted into the meeting, bypassing the lobby.</span></span> <span data-ttu-id="3bb12-130">Все остальные участники помещаются в зал собрания.</span><span class="sxs-lookup"><span data-stu-id="3bb12-130">All other participants are placed in the meeting lobby.</span></span> |
| <span data-ttu-id="3bb12-131">просматривающи</span><span class="sxs-lookup"><span data-stu-id="3bb12-131">everyone</span></span>                 | <span data-ttu-id="3bb12-132">Все пользователи размещаются на собрании.</span><span class="sxs-lookup"><span data-stu-id="3bb12-132">Everyone is admitted into the meeting.</span></span> <span data-ttu-id="3bb12-133">В зал собрания не помещаются участники.</span><span class="sxs-lookup"><span data-stu-id="3bb12-133">No participants are placed in the meeting lobby.</span></span>                                                                                                                   |
| <span data-ttu-id="3bb12-134">unknownFutureValue</span><span class="sxs-lookup"><span data-stu-id="3bb12-134">unknownFutureValue</span></span>       | <span data-ttu-id="3bb12-135">Неизвестное будущее значение.</span><span class="sxs-lookup"><span data-stu-id="3bb12-135">Unknow future value.</span></span>                                                                                                                                     |

## <a name="json-representation"></a><span data-ttu-id="3bb12-136">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3bb12-136">JSON representation</span></span>

<span data-ttu-id="3bb12-137">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3bb12-137">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.lobbyBypassSettings"
}-->
```json
{
  "scope": "organizer | organization | organizationAndFederated | everyone | unknownFutureValue",
  "isDialInBypassEnabled": "Boolean",
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "lobbyBypassSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

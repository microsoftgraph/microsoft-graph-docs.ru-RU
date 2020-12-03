---
title: Тип ресурса Лоббибипасссеттингс
description: Указывает, какие участники могут обходить зал собрания.
author: frankpeng7
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 761a45ce5c4e29d06287edb18aa8d79256c08923
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/01/2020
ms.locfileid: "49523163"
---
# <a name="lobbybypasssettings-resource-type"></a><span data-ttu-id="ecbf6-103">Тип ресурса Лоббибипасссеттингс</span><span class="sxs-lookup"><span data-stu-id="ecbf6-103">lobbyBypassSettings resource type</span></span>

<span data-ttu-id="ecbf6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ecbf6-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ecbf6-105">Указывает, какие участники могут обходить зал собрания.</span><span class="sxs-lookup"><span data-stu-id="ecbf6-105">Specifies which participants can bypass the meeting lobby.</span></span>

## <a name="properties"></a><span data-ttu-id="ecbf6-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="ecbf6-106">Properties</span></span>

| <span data-ttu-id="ecbf6-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="ecbf6-107">Property</span></span>              | <span data-ttu-id="ecbf6-108">Тип</span><span class="sxs-lookup"><span data-stu-id="ecbf6-108">Type</span></span>             | <span data-ttu-id="ecbf6-109">Описание</span><span class="sxs-lookup"><span data-stu-id="ecbf6-109">Description</span></span>                                                                                                                                                          |
| --------------------- | ---------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="ecbf6-110">scope</span><span class="sxs-lookup"><span data-stu-id="ecbf6-110">scope</span></span>                 | <span data-ttu-id="ecbf6-111">лоббибипассскопе</span><span class="sxs-lookup"><span data-stu-id="ecbf6-111">lobbyBypassScope</span></span> | <span data-ttu-id="ecbf6-112">Указывает тип участников, которые автоматически отправляются на собрание, минуя "зал ожидания".</span><span class="sxs-lookup"><span data-stu-id="ecbf6-112">Specifies the type of participants that are automatically admitted into a meeting, bypassing the lobby.</span></span> <span data-ttu-id="ecbf6-113">Возможные значения перечислены в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="ecbf6-113">Possible values are listed in the following table.</span></span> <span data-ttu-id="ecbf6-114">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="ecbf6-114">Optional.</span></span> |
| <span data-ttu-id="ecbf6-115">исдиалинбипассенаблед</span><span class="sxs-lookup"><span data-stu-id="ecbf6-115">isDialInBypassEnabled</span></span> | <span data-ttu-id="ecbf6-116">Логический</span><span class="sxs-lookup"><span data-stu-id="ecbf6-116">Boolean</span></span>          | <span data-ttu-id="ecbf6-117">Указывает, следует ли всегда разрешать абонентам с телефонным подключением обходить "зал ожидания".</span><span class="sxs-lookup"><span data-stu-id="ecbf6-117">Specifies whether or not to always let dial-in callers bypass the lobby.</span></span> <span data-ttu-id="ecbf6-118">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="ecbf6-118">Optional.</span></span>                                                                                   |

### <a name="lobbybypassscope-values"></a><span data-ttu-id="ecbf6-119">значения Лоббибипассскопе</span><span class="sxs-lookup"><span data-stu-id="ecbf6-119">lobbyBypassScope values</span></span>

| <span data-ttu-id="ecbf6-120">Значение</span><span class="sxs-lookup"><span data-stu-id="ecbf6-120">Value</span></span>                    | <span data-ttu-id="ecbf6-121">Описание</span><span class="sxs-lookup"><span data-stu-id="ecbf6-121">Description</span></span>                                                                                                                                                                     |
| ------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="ecbf6-122">organizer</span><span class="sxs-lookup"><span data-stu-id="ecbf6-122">organizer</span></span>                | <span data-ttu-id="ecbf6-123">Только организатор дойдет на собрание, минуя "зал ожидания".</span><span class="sxs-lookup"><span data-stu-id="ecbf6-123">Only the organizer is admitted into the meeting, bypassing the lobby.</span></span> <span data-ttu-id="ecbf6-124">Все остальные участники помещаются в зал собрания.</span><span class="sxs-lookup"><span data-stu-id="ecbf6-124">All other participants are placed in the meeting lobby.</span></span>                                                   |
| <span data-ttu-id="ecbf6-125">organization;</span><span class="sxs-lookup"><span data-stu-id="ecbf6-125">organization</span></span>             | <span data-ttu-id="ecbf6-126">Только участники одной компании могут присутствовать на собрании, минуя "зал ожидания".</span><span class="sxs-lookup"><span data-stu-id="ecbf6-126">Only the participants from the same company are admitted into the meeting, bypassing the lobby.</span></span> <span data-ttu-id="ecbf6-127">Все остальные участники помещаются в зал собрания.</span><span class="sxs-lookup"><span data-stu-id="ecbf6-127">All other participants are placed in the meeting lobby.</span></span>                         |
| <span data-ttu-id="ecbf6-128">организатионандфедератед</span><span class="sxs-lookup"><span data-stu-id="ecbf6-128">organizationAndFederated</span></span> | <span data-ttu-id="ecbf6-129">Только участники одной компании или доверенной Организации доходят на собрание, минуя "зал ожидания".</span><span class="sxs-lookup"><span data-stu-id="ecbf6-129">Only the participants from the same company or trusted organization are admitted into the meeting, bypassing the lobby.</span></span> <span data-ttu-id="ecbf6-130">Все остальные участники помещаются в зал собрания.</span><span class="sxs-lookup"><span data-stu-id="ecbf6-130">All other participants are placed in the meeting lobby.</span></span> |
| <span data-ttu-id="ecbf6-131">просматривающи</span><span class="sxs-lookup"><span data-stu-id="ecbf6-131">everyone</span></span>                 | <span data-ttu-id="ecbf6-132">Все пользователи размещаются на собрании.</span><span class="sxs-lookup"><span data-stu-id="ecbf6-132">Everyone is admitted into the meeting.</span></span> <span data-ttu-id="ecbf6-133">В зал собрания не помещаются участники.</span><span class="sxs-lookup"><span data-stu-id="ecbf6-133">No participants are placed in the meeting lobby.</span></span>                                                                                         |
| <span data-ttu-id="ecbf6-134">unknownFutureValue</span><span class="sxs-lookup"><span data-stu-id="ecbf6-134">unknownFutureValue</span></span>       | <span data-ttu-id="ecbf6-135">Неизвестное будущее значение.</span><span class="sxs-lookup"><span data-stu-id="ecbf6-135">Unknow future value.</span></span>                                                                                                                                                            |

## <a name="json-representation"></a><span data-ttu-id="ecbf6-136">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ecbf6-136">JSON representation</span></span>

<span data-ttu-id="ecbf6-137">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ecbf6-137">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.lobbyBypassSettings"
}-->
```json
{
  "scope": "String",
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

---
title: тип ресурса lobbyBypassSettings
description: Указывает, какие участники могут обойти вестибюль собрания.
author: mkhribech
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: c6d530765e1bc356486f0b8893c69c445c07181f
ms.sourcegitcommit: 7abb0672a38a6d9b11a2e0d2cc221222cb8358bb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2021
ms.locfileid: "52896685"
---
# <a name="lobbybypasssettings-resource-type"></a><span data-ttu-id="4a656-103">тип ресурса lobbyBypassSettings</span><span class="sxs-lookup"><span data-stu-id="4a656-103">lobbyBypassSettings resource type</span></span>

<span data-ttu-id="4a656-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4a656-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4a656-105">Указывает, какие участники могут обойти вестибюль собрания.</span><span class="sxs-lookup"><span data-stu-id="4a656-105">Specifies which participants can bypass the meeting lobby.</span></span>

## <a name="properties"></a><span data-ttu-id="4a656-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="4a656-106">Properties</span></span>

| <span data-ttu-id="4a656-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="4a656-107">Property</span></span>              | <span data-ttu-id="4a656-108">Тип</span><span class="sxs-lookup"><span data-stu-id="4a656-108">Type</span></span>    | <span data-ttu-id="4a656-109">Описание</span><span class="sxs-lookup"><span data-stu-id="4a656-109">Description</span></span>                                                         | 
| --------------------- | ------- | ------------------------------------------------------------------- | 
| <span data-ttu-id="4a656-110">scope</span><span class="sxs-lookup"><span data-stu-id="4a656-110">scope</span></span>                 | [<span data-ttu-id="4a656-111">lobbyBypassScope</span><span class="sxs-lookup"><span data-stu-id="4a656-111">lobbyBypassScope</span></span>](#lobbybypassscope-values)  | <span data-ttu-id="4a656-112">Указывает тип участников, которые автоматически впускаются на собрание, минуя вестибюль.</span><span class="sxs-lookup"><span data-stu-id="4a656-112">Specifies the type of participants that are automatically admitted into a meeting, bypassing the lobby.</span></span> <span data-ttu-id="4a656-113">Возможные значения перечислены в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="4a656-113">Possible values are listed in the following table.</span></span> <span data-ttu-id="4a656-114">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="4a656-114">Optional.</span></span>|
| <span data-ttu-id="4a656-115">isDialInBypassEnabled</span><span class="sxs-lookup"><span data-stu-id="4a656-115">isDialInBypassEnabled</span></span> | <span data-ttu-id="4a656-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="4a656-116">Boolean</span></span> | <span data-ttu-id="4a656-117">Указывает, следует ли всегда позволять звонителям в обход вестибюля.</span><span class="sxs-lookup"><span data-stu-id="4a656-117">Specifies whether or not to always let dial-in callers bypass the lobby.</span></span> <span data-ttu-id="4a656-118">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="4a656-118">Optional.</span></span> | 

### <a name="lobbybypassscope-values"></a><span data-ttu-id="4a656-119">значения lobbyBypassScope</span><span class="sxs-lookup"><span data-stu-id="4a656-119">lobbyBypassScope values</span></span>

| <span data-ttu-id="4a656-120">Значение</span><span class="sxs-lookup"><span data-stu-id="4a656-120">Value</span></span>                    | <span data-ttu-id="4a656-121">Описание</span><span class="sxs-lookup"><span data-stu-id="4a656-121">Description</span></span>                                                                                                                                              |
| ------------------------ | -------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="4a656-122">organizer</span><span class="sxs-lookup"><span data-stu-id="4a656-122">organizer</span></span>                | <span data-ttu-id="4a656-123">На собрание впускается только организатор, минуя вестибюль.</span><span class="sxs-lookup"><span data-stu-id="4a656-123">Only the organizer is admitted into the meeting, bypassing the lobby.</span></span> <span data-ttu-id="4a656-124">Все остальные участники размещены в вестибюле собрания.</span><span class="sxs-lookup"><span data-stu-id="4a656-124">All other participants are placed in the meeting lobby.</span></span>                                                                                                         |
| <span data-ttu-id="4a656-125">organization;</span><span class="sxs-lookup"><span data-stu-id="4a656-125">organization</span></span>             | <span data-ttu-id="4a656-126">Только участники из одной компании допущены на собрание, минуя вестибюль.</span><span class="sxs-lookup"><span data-stu-id="4a656-126">Only the participants from the same company are admitted into the meeting, bypassing the lobby.</span></span> <span data-ttu-id="4a656-127">Все остальные участники размещены в вестибюле собрания.</span><span class="sxs-lookup"><span data-stu-id="4a656-127">All other participants are placed in the meeting lobby.</span></span>                                                                              |
| <span data-ttu-id="4a656-128">organizationAndFederated</span><span class="sxs-lookup"><span data-stu-id="4a656-128">organizationAndFederated</span></span> | <span data-ttu-id="4a656-129">Только участники из одной компании или доверяемой организации впускаются в собрание, минуя лобби.</span><span class="sxs-lookup"><span data-stu-id="4a656-129">Only the participants from the same company or trusted organization are admitted into the meeting, bypassing the lobby.</span></span> <span data-ttu-id="4a656-130">Все остальные участники размещены в вестибюле собрания.</span><span class="sxs-lookup"><span data-stu-id="4a656-130">All other participants are placed in the meeting lobby.</span></span> |
| <span data-ttu-id="4a656-131">все</span><span class="sxs-lookup"><span data-stu-id="4a656-131">everyone</span></span>                 | <span data-ttu-id="4a656-132">Все допущены к собранию.</span><span class="sxs-lookup"><span data-stu-id="4a656-132">Everyone is admitted into the meeting.</span></span> <span data-ttu-id="4a656-133">Участники не размещаются в вестибюле собрания.</span><span class="sxs-lookup"><span data-stu-id="4a656-133">No participants are placed in the meeting lobby.</span></span>                                                                                                                   |
| <span data-ttu-id="4a656-134">unknownFutureValue</span><span class="sxs-lookup"><span data-stu-id="4a656-134">unknownFutureValue</span></span>       | <span data-ttu-id="4a656-135">Unknow future value.</span><span class="sxs-lookup"><span data-stu-id="4a656-135">Unknow future value.</span></span>                                                                                                                                     |

## <a name="json-representation"></a><span data-ttu-id="4a656-136">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4a656-136">JSON representation</span></span>

<span data-ttu-id="4a656-137">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4a656-137">The following is a JSON representation of the resource.</span></span>

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

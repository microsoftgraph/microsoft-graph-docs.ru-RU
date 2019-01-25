---
title: Тип ресурса audioRoutingGroup
description: Аудио группы маршрутизации хранит закрытый звука маршрута между участниками в многосторонней беседе. Источник — это участник самого и приемники являются подмножеством других участников в многосторонней беседе.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: e7fc7de5b5caaa2f4079c453f9cd855a42577cb8
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29509625"
---
# <a name="audioroutinggroup-resource-type"></a><span data-ttu-id="cbfe0-104">Тип ресурса audioRoutingGroup</span><span class="sxs-lookup"><span data-stu-id="cbfe0-104">audioRoutingGroup resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cbfe0-105">Аудио группы маршрутизации хранит закрытый звука маршрута между участниками в многосторонней беседе.</span><span class="sxs-lookup"><span data-stu-id="cbfe0-105">The audio routing group stores a private audio route between participants in a multiparty conversation.</span></span> <span data-ttu-id="cbfe0-106">Источник — это участник самого и приемники являются подмножеством других участников в многосторонней беседе.</span><span class="sxs-lookup"><span data-stu-id="cbfe0-106">Source is the participant itself and the receivers are a subset of other participants in the multiparty conversation.</span></span>

> <span data-ttu-id="cbfe0-107">**Примечание:** [ConfigureMixer](../api/participant-configuremixer.md) не затрагивает все маршруты, для всей продолжительности вызова для настройки громкость сочетания приемника источника.</span><span class="sxs-lookup"><span data-stu-id="cbfe0-107">**Note:** [ConfigureMixer](../api/participant-configuremixer.md) does not involve any routes, it is for the entire call for setting the volume levels for source-receiver combinations.</span></span>

## <a name="methods"></a><span data-ttu-id="cbfe0-108">Методы</span><span class="sxs-lookup"><span data-stu-id="cbfe0-108">Methods</span></span>

| <span data-ttu-id="cbfe0-109">Метод</span><span class="sxs-lookup"><span data-stu-id="cbfe0-109">Method</span></span>                                                  | <span data-ttu-id="cbfe0-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="cbfe0-110">Return Type</span></span>                               | <span data-ttu-id="cbfe0-111">Описание</span><span class="sxs-lookup"><span data-stu-id="cbfe0-111">Description</span></span>                                  |
|:--------------------------------------------------------|:------------------------------------------|:---------------------------------------------|
| [<span data-ttu-id="cbfe0-112">Получение audioRoutingGroup</span><span class="sxs-lookup"><span data-stu-id="cbfe0-112">Get audioRoutingGroup</span></span>](../api/audioroutinggroup-get.md)| [<span data-ttu-id="cbfe0-113">audioRoutingGroup</span><span class="sxs-lookup"><span data-stu-id="cbfe0-113">audioRoutingGroup</span></span>](audioroutinggroup.md) | <span data-ttu-id="cbfe0-114">Чтение свойства и связи объекта audioRoutingGroup.</span><span class="sxs-lookup"><span data-stu-id="cbfe0-114">Read properties and relationships of audioRoutingGroup object.</span></span>|
| [<span data-ttu-id="cbfe0-115">Update</span><span class="sxs-lookup"><span data-stu-id="cbfe0-115">Update</span></span>](../api/audioroutinggroup-update.md)            | [<span data-ttu-id="cbfe0-116">audioRoutingGroup</span><span class="sxs-lookup"><span data-stu-id="cbfe0-116">audioRoutingGroup</span></span>](audioroutinggroup.md) | <span data-ttu-id="cbfe0-117">Обновление списка получателей.</span><span class="sxs-lookup"><span data-stu-id="cbfe0-117">Update receivers list.</span></span>                       |
| [<span data-ttu-id="cbfe0-118">Delete</span><span class="sxs-lookup"><span data-stu-id="cbfe0-118">Delete</span></span>](../api/audioroutinggroup-delete.md)            | <span data-ttu-id="cbfe0-119">Нет</span><span class="sxs-lookup"><span data-stu-id="cbfe0-119">None</span></span>                                      | <span data-ttu-id="cbfe0-120">Удаление звука группы маршрутизации.</span><span class="sxs-lookup"><span data-stu-id="cbfe0-120">Delete the audio routing group.</span></span>              |

## <a name="properties"></a><span data-ttu-id="cbfe0-121">Свойства</span><span class="sxs-lookup"><span data-stu-id="cbfe0-121">Properties</span></span>

| <span data-ttu-id="cbfe0-122">Свойство</span><span class="sxs-lookup"><span data-stu-id="cbfe0-122">Property</span></span>      | <span data-ttu-id="cbfe0-123">Тип</span><span class="sxs-lookup"><span data-stu-id="cbfe0-123">Type</span></span>              | <span data-ttu-id="cbfe0-124">Описание</span><span class="sxs-lookup"><span data-stu-id="cbfe0-124">Description</span></span>                                                          |
| :----------   | :---------------- | :--------------------------------------------------------------------|
| <span data-ttu-id="cbfe0-125">id</span><span class="sxs-lookup"><span data-stu-id="cbfe0-125">id</span></span>            | <span data-ttu-id="cbfe0-126">String</span><span class="sxs-lookup"><span data-stu-id="cbfe0-126">String</span></span>            | <span data-ttu-id="cbfe0-127">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="cbfe0-127">Read-only.</span></span> <span data-ttu-id="cbfe0-128">Сервер, созданный.</span><span class="sxs-lookup"><span data-stu-id="cbfe0-128">Server generated.</span></span>                                         |
| <span data-ttu-id="cbfe0-129">Приемники</span><span class="sxs-lookup"><span data-stu-id="cbfe0-129">receivers</span></span>     | <span data-ttu-id="cbfe0-130">string collection</span><span class="sxs-lookup"><span data-stu-id="cbfe0-130">String Collection</span></span> | <span data-ttu-id="cbfe0-131">Список получения участников идентификаторы.</span><span class="sxs-lookup"><span data-stu-id="cbfe0-131">List of receiving participant ids.</span></span>                                   |
| <span data-ttu-id="cbfe0-132">routingMode</span><span class="sxs-lookup"><span data-stu-id="cbfe0-132">routingMode</span></span>   | <span data-ttu-id="cbfe0-133">String</span><span class="sxs-lookup"><span data-stu-id="cbfe0-133">String</span></span>            | <span data-ttu-id="cbfe0-134">Режим группы маршрутизации.</span><span class="sxs-lookup"><span data-stu-id="cbfe0-134">Routing group mode.</span></span>  <span data-ttu-id="cbfe0-135">Возможные значения: `oneToOne`, `multicast`.</span><span class="sxs-lookup"><span data-stu-id="cbfe0-135">Possible values are: `oneToOne`, `multicast`.</span></span>   |
| <span data-ttu-id="cbfe0-136">sources</span><span class="sxs-lookup"><span data-stu-id="cbfe0-136">sources</span></span>       | <span data-ttu-id="cbfe0-137">string collection</span><span class="sxs-lookup"><span data-stu-id="cbfe0-137">String Collection</span></span> | <span data-ttu-id="cbfe0-138">Список идентификаторов участников источника.</span><span class="sxs-lookup"><span data-stu-id="cbfe0-138">List of source participant ids.</span></span>                                      |

> <span data-ttu-id="cbfe0-139">**Примечание:** Режим маршрутизации определяет ограничения на доступ к источникам и приемников.</span><span class="sxs-lookup"><span data-stu-id="cbfe0-139">**Note:** Routing mode determines the restrictions on the sources and receivers.</span></span> <span data-ttu-id="cbfe0-140">Поддерживаются только следующие группы маршрутизации.</span><span class="sxs-lookup"><span data-stu-id="cbfe0-140">Only the following routing groups are supported.</span></span>
> - <span data-ttu-id="cbfe0-141">`oneToOne`-источники и приемники имеют только одному участнику.</span><span class="sxs-lookup"><span data-stu-id="cbfe0-141">`oneToOne` - sources and receivers have only one participant each.</span></span>
> - <span data-ttu-id="cbfe0-142">`multicast`-источник имеет один участник, но имеется несколько приемников.</span><span class="sxs-lookup"><span data-stu-id="cbfe0-142">`multicast` - source has one participant but there are multiple receivers.</span></span> <span data-ttu-id="cbfe0-143">Список приемники могут быть обновлены.</span><span class="sxs-lookup"><span data-stu-id="cbfe0-143">Receivers list may be updated.</span></span>

> <span data-ttu-id="cbfe0-144">**Примечание:** При создании количество аудио маршрутизации групп (например робот каждого участника), пересылается только звук верхней 4 доминирующий динамики.</span><span class="sxs-lookup"><span data-stu-id="cbfe0-144">**Note:** If you create many audio routing groups (e.g. a bot per participant), only the audio of the top 4 dominant speakers is forwarded.</span></span> <span data-ttu-id="cbfe0-145">Это означает даже при использовании настраиваемого звука группу маршрутизации, если динамик не громкость, в главном Микшер, он/она не удается Херд с робот, даже при наличии закрытый звука группы для этого динамика и робот.</span><span class="sxs-lookup"><span data-stu-id="cbfe0-145">It means even with customized audio routing group, if the speaker is not loud enough in the main mixer, he/she cannot be heard by the bot even if there is a private audio group just for this speaker and the bot.</span></span>

## <a name="relationships"></a><span data-ttu-id="cbfe0-146">Отношения</span><span class="sxs-lookup"><span data-stu-id="cbfe0-146">Relationships</span></span>
<span data-ttu-id="cbfe0-147">Нет</span><span class="sxs-lookup"><span data-stu-id="cbfe0-147">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="cbfe0-148">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="cbfe0-148">JSON representation</span></span>

<span data-ttu-id="cbfe0-149">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cbfe0-149">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.audioRoutingGroup"
}-->
```json
{
  "id": "String (identifier)",
  "receivers": [ "String" ],
  "routingMode": "oneToOne | multicast",
  "sources": [ "String" ]
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "audioRoutingGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/audioroutinggroup.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

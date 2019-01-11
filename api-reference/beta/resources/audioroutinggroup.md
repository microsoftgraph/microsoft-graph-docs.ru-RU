---
title: Тип ресурса audioRoutingGroup
description: Аудио группы маршрутизации хранит закрытый звука маршрута между участниками в многосторонней беседе. Источник — это участник самого и приемники являются подмножеством других участников в многосторонней беседе.
author: VinodRavichandran
localization_priority: Normal
ms.openlocfilehash: cb1b8b67404ef6a3c8f397a6b5debe9acc252b5f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27860650"
---
# <a name="audioroutinggroup-resource-type"></a><span data-ttu-id="9e035-104">Тип ресурса audioRoutingGroup</span><span class="sxs-lookup"><span data-stu-id="9e035-104">audioRoutingGroup resource type</span></span>

> <span data-ttu-id="9e035-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="9e035-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9e035-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9e035-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9e035-107">Аудио группы маршрутизации хранит закрытый звука маршрута между участниками в многосторонней беседе.</span><span class="sxs-lookup"><span data-stu-id="9e035-107">The audio routing group stores a private audio route between participants in a multiparty conversation.</span></span> <span data-ttu-id="9e035-108">Источник — это участник самого и приемники являются подмножеством других участников в многосторонней беседе.</span><span class="sxs-lookup"><span data-stu-id="9e035-108">Source is the participant itself and the receivers are a subset of other participants in the multiparty conversation.</span></span>

> <span data-ttu-id="9e035-109">**Примечание:** [ConfigureMixer](../api/participant-configuremixer.md) не затрагивает все маршруты, для всей продолжительности вызова для настройки громкость сочетания приемника источника.</span><span class="sxs-lookup"><span data-stu-id="9e035-109">**Note:** [ConfigureMixer](../api/participant-configuremixer.md) does not involve any routes, it is for the entire call for setting the volume levels for source-receiver combinations.</span></span>

## <a name="methods"></a><span data-ttu-id="9e035-110">Методы</span><span class="sxs-lookup"><span data-stu-id="9e035-110">Methods</span></span>

| <span data-ttu-id="9e035-111">Метод</span><span class="sxs-lookup"><span data-stu-id="9e035-111">Method</span></span>                                                  | <span data-ttu-id="9e035-112">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="9e035-112">Return Type</span></span>                               | <span data-ttu-id="9e035-113">Описание</span><span class="sxs-lookup"><span data-stu-id="9e035-113">Description</span></span>                                  |
|:--------------------------------------------------------|:------------------------------------------|:---------------------------------------------|
| [<span data-ttu-id="9e035-114">Получение audioRoutingGroup</span><span class="sxs-lookup"><span data-stu-id="9e035-114">Get audioRoutingGroup</span></span>](../api/audioroutinggroup-get.md)| [<span data-ttu-id="9e035-115">audioRoutingGroup</span><span class="sxs-lookup"><span data-stu-id="9e035-115">audioRoutingGroup</span></span>](audioroutinggroup.md) | <span data-ttu-id="9e035-116">Чтение свойства и связи объекта audioRoutingGroup.</span><span class="sxs-lookup"><span data-stu-id="9e035-116">Read properties and relationships of audioRoutingGroup object.</span></span>|
| <span data-ttu-id="9e035-117">[обновление](../api/audioroutinggroup-update.md).</span><span class="sxs-lookup"><span data-stu-id="9e035-117">[Update](../api/audioroutinggroup-update.md)</span></span>            | [<span data-ttu-id="9e035-118">audioRoutingGroup</span><span class="sxs-lookup"><span data-stu-id="9e035-118">audioRoutingGroup</span></span>](audioroutinggroup.md) | <span data-ttu-id="9e035-119">Обновление списка получателей.</span><span class="sxs-lookup"><span data-stu-id="9e035-119">Update receivers list.</span></span>                       |
| [<span data-ttu-id="9e035-120">Delete</span><span class="sxs-lookup"><span data-stu-id="9e035-120">Delete</span></span>](../api/audioroutinggroup-delete.md)            | <span data-ttu-id="9e035-121">Нет</span><span class="sxs-lookup"><span data-stu-id="9e035-121">None</span></span>                                      | <span data-ttu-id="9e035-122">Удаление звука группы маршрутизации.</span><span class="sxs-lookup"><span data-stu-id="9e035-122">Delete the audio routing group.</span></span>              |

## <a name="properties"></a><span data-ttu-id="9e035-123">Свойства</span><span class="sxs-lookup"><span data-stu-id="9e035-123">Properties</span></span>

| <span data-ttu-id="9e035-124">Свойство</span><span class="sxs-lookup"><span data-stu-id="9e035-124">Property</span></span>      | <span data-ttu-id="9e035-125">Тип</span><span class="sxs-lookup"><span data-stu-id="9e035-125">Type</span></span>              | <span data-ttu-id="9e035-126">Описание</span><span class="sxs-lookup"><span data-stu-id="9e035-126">Description</span></span>                                                          |
| :----------   | :---------------- | :--------------------------------------------------------------------|
| <span data-ttu-id="9e035-127">id</span><span class="sxs-lookup"><span data-stu-id="9e035-127">id</span></span>            | <span data-ttu-id="9e035-128">Строка</span><span class="sxs-lookup"><span data-stu-id="9e035-128">String</span></span>            | <span data-ttu-id="9e035-129">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9e035-129">Read-only.</span></span> <span data-ttu-id="9e035-130">Сервер, созданный.</span><span class="sxs-lookup"><span data-stu-id="9e035-130">Server generated.</span></span>                                         |
| <span data-ttu-id="9e035-131">Приемники</span><span class="sxs-lookup"><span data-stu-id="9e035-131">receivers</span></span>     | <span data-ttu-id="9e035-132">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="9e035-132">String Collection</span></span> | <span data-ttu-id="9e035-133">Список получения участников идентификаторы.</span><span class="sxs-lookup"><span data-stu-id="9e035-133">List of receiving participant ids.</span></span>                                   |
| <span data-ttu-id="9e035-134">routingMode</span><span class="sxs-lookup"><span data-stu-id="9e035-134">routingMode</span></span>   | <span data-ttu-id="9e035-135">Строка</span><span class="sxs-lookup"><span data-stu-id="9e035-135">String</span></span>            | <span data-ttu-id="9e035-136">Режим группы маршрутизации.</span><span class="sxs-lookup"><span data-stu-id="9e035-136">Routing group mode.</span></span>  <span data-ttu-id="9e035-137">Возможные значения: `oneToOne`, `multicast`.</span><span class="sxs-lookup"><span data-stu-id="9e035-137">Possible values are: `oneToOne`, `multicast`.</span></span>   |
| <span data-ttu-id="9e035-138">sources</span><span class="sxs-lookup"><span data-stu-id="9e035-138">sources</span></span>       | <span data-ttu-id="9e035-139">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="9e035-139">String Collection</span></span> | <span data-ttu-id="9e035-140">Список идентификаторов участников источника.</span><span class="sxs-lookup"><span data-stu-id="9e035-140">List of source participant ids.</span></span>                                      |

> <span data-ttu-id="9e035-141">**Примечание:** Режим маршрутизации определяет ограничения на доступ к источникам и приемников.</span><span class="sxs-lookup"><span data-stu-id="9e035-141">**Note:** Routing mode determines the restrictions on the sources and receivers.</span></span> <span data-ttu-id="9e035-142">Поддерживаются только следующие группы маршрутизации.</span><span class="sxs-lookup"><span data-stu-id="9e035-142">Only the following routing groups are supported.</span></span>
> - <span data-ttu-id="9e035-143">`oneToOne`-источники и приемники имеют только одному участнику.</span><span class="sxs-lookup"><span data-stu-id="9e035-143">`oneToOne` - sources and receivers have only one participant each.</span></span>
> - <span data-ttu-id="9e035-144">`multicast`-источник имеет один участник, но имеется несколько приемников.</span><span class="sxs-lookup"><span data-stu-id="9e035-144">`multicast` - source has one participant but there are multiple receivers.</span></span> <span data-ttu-id="9e035-145">Список приемники могут быть обновлены.</span><span class="sxs-lookup"><span data-stu-id="9e035-145">Receivers list may be updated.</span></span>

> <span data-ttu-id="9e035-146">**Примечание:** При создании количество аудио маршрутизации групп (например робот каждого участника), пересылается только звук верхней 4 доминирующий динамики.</span><span class="sxs-lookup"><span data-stu-id="9e035-146">**Note:** If you create many audio routing groups (e.g. a bot per participant), only the audio of the top 4 dominant speakers is forwarded.</span></span> <span data-ttu-id="9e035-147">Это означает даже при использовании настраиваемого звука группу маршрутизации, если динамик не громкость, в главном Микшер, он/она не удается Херд с робот, даже при наличии закрытый звука группы для этого динамика и робот.</span><span class="sxs-lookup"><span data-stu-id="9e035-147">It means even with customized audio routing group, if the speaker is not loud enough in the main mixer, he/she cannot be heard by the bot even if there is a private audio group just for this speaker and the bot.</span></span>

## <a name="relationships"></a><span data-ttu-id="9e035-148">Связи</span><span class="sxs-lookup"><span data-stu-id="9e035-148">Relationships</span></span>
<span data-ttu-id="9e035-149">Нет</span><span class="sxs-lookup"><span data-stu-id="9e035-149">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9e035-150">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9e035-150">JSON representation</span></span>

<span data-ttu-id="9e035-151">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9e035-151">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "audioRoutingGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

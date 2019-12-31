---
title: Тип ресурса Аудиораутингграуп
description: В группе маршрутизации звука хранится частный звуковой маршрут между участниками в составе многоадресной беседы. Источник — сам участник, а приемники являются подмножеством других участников многочастой беседы.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: cb96e83f6c80a3b3c50b37612731272ca329e3cc
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/31/2019
ms.locfileid: "40913753"
---
# <a name="audioroutinggroup-resource-type"></a><span data-ttu-id="c85da-104">Тип ресурса Аудиораутингграуп</span><span class="sxs-lookup"><span data-stu-id="c85da-104">audioRoutingGroup resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c85da-105">В группе маршрутизации звука хранится частный звуковой маршрут между участниками в составе многоадресной беседы.</span><span class="sxs-lookup"><span data-stu-id="c85da-105">The audio routing group stores a private audio route between participants in a multiparty conversation.</span></span> <span data-ttu-id="c85da-106">Источник — сам участник, а приемники являются подмножеством других участников многочастой беседы.</span><span class="sxs-lookup"><span data-stu-id="c85da-106">Source is the participant itself and the receivers are a subset of other participants in the multiparty conversation.</span></span>

> <span data-ttu-id="c85da-107">**Note:** [конфигуремиксер](../api/participant-configuremixer.md) не включает ни одного маршрута, он предназначен для всего вызова для настройки уровней громкости для комбинаций исходного приемника.</span><span class="sxs-lookup"><span data-stu-id="c85da-107">**Note:** [ConfigureMixer](../api/participant-configuremixer.md) does not involve any routes, it is for the entire call for setting the volume levels for source-receiver combinations.</span></span>

## <a name="methods"></a><span data-ttu-id="c85da-108">Методы</span><span class="sxs-lookup"><span data-stu-id="c85da-108">Methods</span></span>

| <span data-ttu-id="c85da-109">Метод</span><span class="sxs-lookup"><span data-stu-id="c85da-109">Method</span></span>                                                  | <span data-ttu-id="c85da-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="c85da-110">Return Type</span></span>                               | <span data-ttu-id="c85da-111">Описание</span><span class="sxs-lookup"><span data-stu-id="c85da-111">Description</span></span>                                  |
|:--------------------------------------------------------|:------------------------------------------|:---------------------------------------------|
| [<span data-ttu-id="c85da-112">Получение Аудиораутингграуп</span><span class="sxs-lookup"><span data-stu-id="c85da-112">Get audioRoutingGroup</span></span>](../api/audioroutinggroup-get.md)| [<span data-ttu-id="c85da-113">audioRoutingGroup</span><span class="sxs-lookup"><span data-stu-id="c85da-113">audioRoutingGroup</span></span>](audioroutinggroup.md) | <span data-ttu-id="c85da-114">Чтение свойств и связей объекта Аудиораутингграуп.</span><span class="sxs-lookup"><span data-stu-id="c85da-114">Read properties and relationships of audioRoutingGroup object.</span></span>|
| <span data-ttu-id="c85da-115">[обновление](../api/audioroutinggroup-update.md).</span><span class="sxs-lookup"><span data-stu-id="c85da-115">[Update](../api/audioroutinggroup-update.md)</span></span>            | [<span data-ttu-id="c85da-116">audioRoutingGroup</span><span class="sxs-lookup"><span data-stu-id="c85da-116">audioRoutingGroup</span></span>](audioroutinggroup.md) | <span data-ttu-id="c85da-117">Обновление списка получателей.</span><span class="sxs-lookup"><span data-stu-id="c85da-117">Update receivers list.</span></span>                       |
| <span data-ttu-id="c85da-118">[удаление](../api/audioroutinggroup-delete.md);</span><span class="sxs-lookup"><span data-stu-id="c85da-118">[Delete](../api/audioroutinggroup-delete.md)</span></span>            | <span data-ttu-id="c85da-119">Нет</span><span class="sxs-lookup"><span data-stu-id="c85da-119">None</span></span>                                      | <span data-ttu-id="c85da-120">Удаление группы маршрутизации звука.</span><span class="sxs-lookup"><span data-stu-id="c85da-120">Delete the audio routing group.</span></span>              |

## <a name="properties"></a><span data-ttu-id="c85da-121">Свойства</span><span class="sxs-lookup"><span data-stu-id="c85da-121">Properties</span></span>

| <span data-ttu-id="c85da-122">Свойство</span><span class="sxs-lookup"><span data-stu-id="c85da-122">Property</span></span>      | <span data-ttu-id="c85da-123">Тип</span><span class="sxs-lookup"><span data-stu-id="c85da-123">Type</span></span>              | <span data-ttu-id="c85da-124">Описание</span><span class="sxs-lookup"><span data-stu-id="c85da-124">Description</span></span>                                                          |
| :----------   | :---------------- | :--------------------------------------------------------------------|
| <span data-ttu-id="c85da-125">id</span><span class="sxs-lookup"><span data-stu-id="c85da-125">id</span></span>            | <span data-ttu-id="c85da-126">string</span><span class="sxs-lookup"><span data-stu-id="c85da-126">string</span></span>            | <span data-ttu-id="c85da-127">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c85da-127">Read-only.</span></span>                                                           |
| <span data-ttu-id="c85da-128">приемники</span><span class="sxs-lookup"><span data-stu-id="c85da-128">receivers</span></span>     | <span data-ttu-id="c85da-129">Коллекция (string)</span><span class="sxs-lookup"><span data-stu-id="c85da-129">collection(string)</span></span> | <span data-ttu-id="c85da-130">Список идентификаторов участников.</span><span class="sxs-lookup"><span data-stu-id="c85da-130">List of receiving participant ids.</span></span>                                   |
| <span data-ttu-id="c85da-131">раутингмоде</span><span class="sxs-lookup"><span data-stu-id="c85da-131">routingMode</span></span>   | <span data-ttu-id="c85da-132">string</span><span class="sxs-lookup"><span data-stu-id="c85da-132">string</span></span>            | <span data-ttu-id="c85da-133">Режим группы маршрутизации.</span><span class="sxs-lookup"><span data-stu-id="c85da-133">Routing group mode.</span></span>  <span data-ttu-id="c85da-134">Возможные значения: `oneToOne`, `multicast`.</span><span class="sxs-lookup"><span data-stu-id="c85da-134">Possible values are: `oneToOne`, `multicast`.</span></span>   |
| <span data-ttu-id="c85da-135">sources</span><span class="sxs-lookup"><span data-stu-id="c85da-135">sources</span></span>       | <span data-ttu-id="c85da-136">Коллекция (string)</span><span class="sxs-lookup"><span data-stu-id="c85da-136">collection(string)</span></span> | <span data-ttu-id="c85da-137">Список идентификаторов участников исходного участника.</span><span class="sxs-lookup"><span data-stu-id="c85da-137">List of source participant ids.</span></span>                                      |

> <span data-ttu-id="c85da-138">**Примечание:** Режим маршрутизации определяет ограничения для источников и получателей.</span><span class="sxs-lookup"><span data-stu-id="c85da-138">**Note:** Routing mode determines the restrictions on the sources and receivers.</span></span> <span data-ttu-id="c85da-139">Поддерживаются только следующие группы маршрутизации.</span><span class="sxs-lookup"><span data-stu-id="c85da-139">Only the following routing groups are supported.</span></span>
> - <span data-ttu-id="c85da-140">`oneToOne`— у источников и приемников есть только один участник.</span><span class="sxs-lookup"><span data-stu-id="c85da-140">`oneToOne` - sources and receivers have only one participant each.</span></span>
> - <span data-ttu-id="c85da-141">`multicast`Источник имеет одного участника, но существует несколько получателей.</span><span class="sxs-lookup"><span data-stu-id="c85da-141">`multicast` - source has one participant but there are multiple receivers.</span></span> <span data-ttu-id="c85da-142">Список получателей можно обновить.</span><span class="sxs-lookup"><span data-stu-id="c85da-142">Receivers list may be updated.</span></span>

> <span data-ttu-id="c85da-143">**Примечание:** Если вы создаете множество групп маршрутизации звука (например, Bot для каждого участника), пересылается только звук главных 4 главных динамиков.</span><span class="sxs-lookup"><span data-stu-id="c85da-143">**Note:** If you create many audio routing groups (e.g. a bot per participant), only the audio of the top 4 dominant speakers is forwarded.</span></span> <span data-ttu-id="c85da-144">Это означает, что даже если пользователь настроил группу маршрутизации аудио, если динамики не хватает громкости в основном микшере, то он/она не может быть слышна с помощью Bot, даже если для этого динамика и для этого динамика достаточно частной группы звука.</span><span class="sxs-lookup"><span data-stu-id="c85da-144">It means even with customized audio routing group, if the speaker is not loud enough in the main mixer, he/she cannot be heard by the bot even if there is a private audio group just for this speaker and the bot.</span></span>

## <a name="relationships"></a><span data-ttu-id="c85da-145">Отношения</span><span class="sxs-lookup"><span data-stu-id="c85da-145">Relationships</span></span>
<span data-ttu-id="c85da-146">Нет</span><span class="sxs-lookup"><span data-stu-id="c85da-146">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c85da-147">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c85da-147">JSON representation</span></span>

<span data-ttu-id="c85da-148">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c85da-148">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.audioRoutingGroup"
}-->
```json
{
  "id": "string (identifier)",
  "receivers": [ "string" ],
  "routingMode": "oneToOne | multicast",
  "sources": [ "string" ]
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
  "suppressions": []
}
-->

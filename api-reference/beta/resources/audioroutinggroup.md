---
title: Тип ресурса Аудиораутингграуп
description: В группе маршрутизации звука хранится частный звуковой маршрут между участниками в составе многоадресной беседы. Источник — сам участник, а приемники являются подмножеством других участников многочастой беседы.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 36ea9fccc107dd88008fcb7bb6c88a4134607e2f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47998987"
---
# <a name="audioroutinggroup-resource-type"></a><span data-ttu-id="19fb2-104">Тип ресурса Аудиораутингграуп</span><span class="sxs-lookup"><span data-stu-id="19fb2-104">audioRoutingGroup resource type</span></span>

<span data-ttu-id="19fb2-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="19fb2-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="19fb2-106">В группе маршрутизации звука хранится частный звуковой маршрут между участниками в составе многоадресной беседы.</span><span class="sxs-lookup"><span data-stu-id="19fb2-106">The audio routing group stores a private audio route between participants in a multiparty conversation.</span></span> <span data-ttu-id="19fb2-107">Источник — сам участник, а приемники являются подмножеством других участников многочастой беседы.</span><span class="sxs-lookup"><span data-stu-id="19fb2-107">Source is the participant itself and the receivers are a subset of other participants in the multiparty conversation.</span></span>

> <span data-ttu-id="19fb2-108">**Note:** [конфигуремиксер](../api/participant-configuremixer.md) не включает ни одного маршрута, он предназначен для всего вызова для настройки уровней громкости для комбинаций исходного приемника.</span><span class="sxs-lookup"><span data-stu-id="19fb2-108">**Note:** [ConfigureMixer](../api/participant-configuremixer.md) does not involve any routes, it is for the entire call for setting the volume levels for source-receiver combinations.</span></span>

## <a name="methods"></a><span data-ttu-id="19fb2-109">Методы</span><span class="sxs-lookup"><span data-stu-id="19fb2-109">Methods</span></span>

| <span data-ttu-id="19fb2-110">Метод</span><span class="sxs-lookup"><span data-stu-id="19fb2-110">Method</span></span>                                                  | <span data-ttu-id="19fb2-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="19fb2-111">Return Type</span></span>                               | <span data-ttu-id="19fb2-112">Описание</span><span class="sxs-lookup"><span data-stu-id="19fb2-112">Description</span></span>                                  |
|:--------------------------------------------------------|:------------------------------------------|:---------------------------------------------|
| [<span data-ttu-id="19fb2-113">Получение Аудиораутингграуп</span><span class="sxs-lookup"><span data-stu-id="19fb2-113">Get audioRoutingGroup</span></span>](../api/audioroutinggroup-get.md)| [<span data-ttu-id="19fb2-114">audioRoutingGroup</span><span class="sxs-lookup"><span data-stu-id="19fb2-114">audioRoutingGroup</span></span>](audioroutinggroup.md) | <span data-ttu-id="19fb2-115">Чтение свойств и связей объекта Аудиораутингграуп.</span><span class="sxs-lookup"><span data-stu-id="19fb2-115">Read properties and relationships of audioRoutingGroup object.</span></span>|
| <span data-ttu-id="19fb2-116">[обновление](../api/audioroutinggroup-update.md).</span><span class="sxs-lookup"><span data-stu-id="19fb2-116">[Update](../api/audioroutinggroup-update.md)</span></span>            | [<span data-ttu-id="19fb2-117">audioRoutingGroup</span><span class="sxs-lookup"><span data-stu-id="19fb2-117">audioRoutingGroup</span></span>](audioroutinggroup.md) | <span data-ttu-id="19fb2-118">Обновление списка получателей.</span><span class="sxs-lookup"><span data-stu-id="19fb2-118">Update receivers list.</span></span>                       |
| <span data-ttu-id="19fb2-119">[удаление](../api/audioroutinggroup-delete.md);</span><span class="sxs-lookup"><span data-stu-id="19fb2-119">[Delete](../api/audioroutinggroup-delete.md)</span></span>            | <span data-ttu-id="19fb2-120">Нет</span><span class="sxs-lookup"><span data-stu-id="19fb2-120">None</span></span>                                      | <span data-ttu-id="19fb2-121">Удаление группы маршрутизации звука.</span><span class="sxs-lookup"><span data-stu-id="19fb2-121">Delete the audio routing group.</span></span>              |

## <a name="properties"></a><span data-ttu-id="19fb2-122">Свойства</span><span class="sxs-lookup"><span data-stu-id="19fb2-122">Properties</span></span>

| <span data-ttu-id="19fb2-123">Свойство</span><span class="sxs-lookup"><span data-stu-id="19fb2-123">Property</span></span>      | <span data-ttu-id="19fb2-124">Тип</span><span class="sxs-lookup"><span data-stu-id="19fb2-124">Type</span></span>              | <span data-ttu-id="19fb2-125">Описание</span><span class="sxs-lookup"><span data-stu-id="19fb2-125">Description</span></span>                                                          |
| :----------   | :---------------- | :--------------------------------------------------------------------|
| <span data-ttu-id="19fb2-126">id</span><span class="sxs-lookup"><span data-stu-id="19fb2-126">id</span></span>            | <span data-ttu-id="19fb2-127">string</span><span class="sxs-lookup"><span data-stu-id="19fb2-127">string</span></span>            | <span data-ttu-id="19fb2-128">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="19fb2-128">Read-only.</span></span>                                                           |
| <span data-ttu-id="19fb2-129">приемники</span><span class="sxs-lookup"><span data-stu-id="19fb2-129">receivers</span></span>     | <span data-ttu-id="19fb2-130">Коллекция (string)</span><span class="sxs-lookup"><span data-stu-id="19fb2-130">collection(string)</span></span> | <span data-ttu-id="19fb2-131">Список идентификаторов участников.</span><span class="sxs-lookup"><span data-stu-id="19fb2-131">List of receiving participant ids.</span></span>                                   |
| <span data-ttu-id="19fb2-132">раутингмоде</span><span class="sxs-lookup"><span data-stu-id="19fb2-132">routingMode</span></span>   | <span data-ttu-id="19fb2-133">string</span><span class="sxs-lookup"><span data-stu-id="19fb2-133">string</span></span>            | <span data-ttu-id="19fb2-134">Режим группы маршрутизации.</span><span class="sxs-lookup"><span data-stu-id="19fb2-134">Routing group mode.</span></span>  <span data-ttu-id="19fb2-135">Возможные значения: `oneToOne`, `multicast`.</span><span class="sxs-lookup"><span data-stu-id="19fb2-135">Possible values are: `oneToOne`, `multicast`.</span></span>   |
| <span data-ttu-id="19fb2-136">sources</span><span class="sxs-lookup"><span data-stu-id="19fb2-136">sources</span></span>       | <span data-ttu-id="19fb2-137">Коллекция (string)</span><span class="sxs-lookup"><span data-stu-id="19fb2-137">collection(string)</span></span> | <span data-ttu-id="19fb2-138">Список идентификаторов участников исходного участника.</span><span class="sxs-lookup"><span data-stu-id="19fb2-138">List of source participant ids.</span></span>                                      |

> <span data-ttu-id="19fb2-139">**Примечание:** Режим маршрутизации определяет ограничения для источников и получателей.</span><span class="sxs-lookup"><span data-stu-id="19fb2-139">**Note:** Routing mode determines the restrictions on the sources and receivers.</span></span> <span data-ttu-id="19fb2-140">Поддерживаются только следующие группы маршрутизации.</span><span class="sxs-lookup"><span data-stu-id="19fb2-140">Only the following routing groups are supported.</span></span>
> - <span data-ttu-id="19fb2-141">`oneToOne` — у источников и приемников есть только один участник.</span><span class="sxs-lookup"><span data-stu-id="19fb2-141">`oneToOne` - sources and receivers have only one participant each.</span></span>
> - <span data-ttu-id="19fb2-142">`multicast` Источник имеет одного участника, но существует несколько получателей.</span><span class="sxs-lookup"><span data-stu-id="19fb2-142">`multicast` - source has one participant but there are multiple receivers.</span></span> <span data-ttu-id="19fb2-143">Список получателей можно обновить.</span><span class="sxs-lookup"><span data-stu-id="19fb2-143">Receivers list may be updated.</span></span>

> <span data-ttu-id="19fb2-144">**Примечание:** Если вы создаете множество групп маршрутизации звука (например, Bot для каждого участника), пересылается только звук главных 4 главных динамиков.</span><span class="sxs-lookup"><span data-stu-id="19fb2-144">**Note:** If you create many audio routing groups (e.g. a bot per participant), only the audio of the top 4 dominant speakers is forwarded.</span></span> <span data-ttu-id="19fb2-145">Это означает, что даже если пользователь настроил группу маршрутизации аудио, если динамики не хватает громкости в основном микшере, то он/она не может быть слышна с помощью Bot, даже если для этого динамика и для этого динамика достаточно частной группы звука.</span><span class="sxs-lookup"><span data-stu-id="19fb2-145">It means even with customized audio routing group, if the speaker is not loud enough in the main mixer, he/she cannot be heard by the bot even if there is a private audio group just for this speaker and the bot.</span></span>

## <a name="relationships"></a><span data-ttu-id="19fb2-146">Связи</span><span class="sxs-lookup"><span data-stu-id="19fb2-146">Relationships</span></span>
<span data-ttu-id="19fb2-147">Нет</span><span class="sxs-lookup"><span data-stu-id="19fb2-147">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="19fb2-148">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="19fb2-148">JSON representation</span></span>

<span data-ttu-id="19fb2-149">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="19fb2-149">The following is a JSON representation of the resource.</span></span>

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



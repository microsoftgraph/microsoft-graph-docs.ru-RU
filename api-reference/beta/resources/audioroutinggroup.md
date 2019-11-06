---
title: Тип ресурса Аудиораутингграуп
description: В группе маршрутизации звука хранится частный звуковой маршрут между участниками в составе многоадресной беседы. Источник — сам участник, а приемники являются подмножеством других участников многочастой беседы.
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 827f67239be572bbc2b20b8900ea33b9b0294412
ms.sourcegitcommit: 9bddc0b7746383e8d05ce50d163af3f4196f12a6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/06/2019
ms.locfileid: "38006763"
---
# <a name="audioroutinggroup-resource-type"></a><span data-ttu-id="53ffc-104">Тип ресурса Аудиораутингграуп</span><span class="sxs-lookup"><span data-stu-id="53ffc-104">audioRoutingGroup resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="53ffc-105">В группе маршрутизации звука хранится частный звуковой маршрут между участниками в составе многоадресной беседы.</span><span class="sxs-lookup"><span data-stu-id="53ffc-105">The audio routing group stores a private audio route between participants in a multiparty conversation.</span></span> <span data-ttu-id="53ffc-106">Источник — сам участник, а приемники являются подмножеством других участников многочастой беседы.</span><span class="sxs-lookup"><span data-stu-id="53ffc-106">Source is the participant itself and the receivers are a subset of other participants in the multiparty conversation.</span></span>

> <span data-ttu-id="53ffc-107">**Note:** [конфигуремиксер](../api/participant-configuremixer.md) не включает ни одного маршрута, он предназначен для всего вызова для настройки уровней громкости для комбинаций исходного приемника.</span><span class="sxs-lookup"><span data-stu-id="53ffc-107">**Note:** [ConfigureMixer](../api/participant-configuremixer.md) does not involve any routes, it is for the entire call for setting the volume levels for source-receiver combinations.</span></span>

## <a name="methods"></a><span data-ttu-id="53ffc-108">Методы</span><span class="sxs-lookup"><span data-stu-id="53ffc-108">Methods</span></span>

| <span data-ttu-id="53ffc-109">Метод</span><span class="sxs-lookup"><span data-stu-id="53ffc-109">Method</span></span>                                                  | <span data-ttu-id="53ffc-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="53ffc-110">Return Type</span></span>                               | <span data-ttu-id="53ffc-111">Описание</span><span class="sxs-lookup"><span data-stu-id="53ffc-111">Description</span></span>                                  |
|:--------------------------------------------------------|:------------------------------------------|:---------------------------------------------|
| [<span data-ttu-id="53ffc-112">Получение Аудиораутингграуп</span><span class="sxs-lookup"><span data-stu-id="53ffc-112">Get audioRoutingGroup</span></span>](../api/audioroutinggroup-get.md)| [<span data-ttu-id="53ffc-113">audioRoutingGroup</span><span class="sxs-lookup"><span data-stu-id="53ffc-113">audioRoutingGroup</span></span>](audioroutinggroup.md) | <span data-ttu-id="53ffc-114">Чтение свойств и связей объекта Аудиораутингграуп.</span><span class="sxs-lookup"><span data-stu-id="53ffc-114">Read properties and relationships of audioRoutingGroup object.</span></span>|
| [<span data-ttu-id="53ffc-115">Update</span><span class="sxs-lookup"><span data-stu-id="53ffc-115">Update</span></span>](../api/audioroutinggroup-update.md)            | [<span data-ttu-id="53ffc-116">audioRoutingGroup</span><span class="sxs-lookup"><span data-stu-id="53ffc-116">audioRoutingGroup</span></span>](audioroutinggroup.md) | <span data-ttu-id="53ffc-117">Обновление списка получателей.</span><span class="sxs-lookup"><span data-stu-id="53ffc-117">Update receivers list.</span></span>                       |
| [<span data-ttu-id="53ffc-118">Delete</span><span class="sxs-lookup"><span data-stu-id="53ffc-118">Delete</span></span>](../api/audioroutinggroup-delete.md)            | <span data-ttu-id="53ffc-119">Нет</span><span class="sxs-lookup"><span data-stu-id="53ffc-119">None</span></span>                                      | <span data-ttu-id="53ffc-120">Удаление группы маршрутизации звука.</span><span class="sxs-lookup"><span data-stu-id="53ffc-120">Delete the audio routing group.</span></span>              |

## <a name="properties"></a><span data-ttu-id="53ffc-121">Свойства</span><span class="sxs-lookup"><span data-stu-id="53ffc-121">Properties</span></span>

| <span data-ttu-id="53ffc-122">Свойство</span><span class="sxs-lookup"><span data-stu-id="53ffc-122">Property</span></span>      | <span data-ttu-id="53ffc-123">Тип</span><span class="sxs-lookup"><span data-stu-id="53ffc-123">Type</span></span>              | <span data-ttu-id="53ffc-124">Описание</span><span class="sxs-lookup"><span data-stu-id="53ffc-124">Description</span></span>                                                          |
| :----------   | :---------------- | :--------------------------------------------------------------------|
| <span data-ttu-id="53ffc-125">id</span><span class="sxs-lookup"><span data-stu-id="53ffc-125">id</span></span>            | <span data-ttu-id="53ffc-126">string</span><span class="sxs-lookup"><span data-stu-id="53ffc-126">string</span></span>            | <span data-ttu-id="53ffc-127">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="53ffc-127">Read-only.</span></span>                                                           |
| <span data-ttu-id="53ffc-128">приемники</span><span class="sxs-lookup"><span data-stu-id="53ffc-128">receivers</span></span>     | <span data-ttu-id="53ffc-129">Коллекция (string)</span><span class="sxs-lookup"><span data-stu-id="53ffc-129">collection(string)</span></span> | <span data-ttu-id="53ffc-130">Список идентификаторов участников.</span><span class="sxs-lookup"><span data-stu-id="53ffc-130">List of receiving participant ids.</span></span>                                   |
| <span data-ttu-id="53ffc-131">раутингмоде</span><span class="sxs-lookup"><span data-stu-id="53ffc-131">routingMode</span></span>   | <span data-ttu-id="53ffc-132">string</span><span class="sxs-lookup"><span data-stu-id="53ffc-132">string</span></span>            | <span data-ttu-id="53ffc-133">Режим группы маршрутизации.</span><span class="sxs-lookup"><span data-stu-id="53ffc-133">Routing group mode.</span></span>  <span data-ttu-id="53ffc-134">Возможные значения: `oneToOne`, `multicast`.</span><span class="sxs-lookup"><span data-stu-id="53ffc-134">Possible values are: `oneToOne`, `multicast`.</span></span>   |
| <span data-ttu-id="53ffc-135">sources</span><span class="sxs-lookup"><span data-stu-id="53ffc-135">sources</span></span>       | <span data-ttu-id="53ffc-136">Коллекция (string)</span><span class="sxs-lookup"><span data-stu-id="53ffc-136">collection(string)</span></span> | <span data-ttu-id="53ffc-137">Список идентификаторов участников исходного участника.</span><span class="sxs-lookup"><span data-stu-id="53ffc-137">List of source participant ids.</span></span>                                      |

> <span data-ttu-id="53ffc-138">**Примечание:** Режим маршрутизации определяет ограничения для источников и получателей.</span><span class="sxs-lookup"><span data-stu-id="53ffc-138">**Note:** Routing mode determines the restrictions on the sources and receivers.</span></span> <span data-ttu-id="53ffc-139">Поддерживаются только следующие группы маршрутизации.</span><span class="sxs-lookup"><span data-stu-id="53ffc-139">Only the following routing groups are supported.</span></span>
> - <span data-ttu-id="53ffc-140">`oneToOne`— у источников и приемников есть только один участник.</span><span class="sxs-lookup"><span data-stu-id="53ffc-140">`oneToOne` - sources and receivers have only one participant each.</span></span>
> - <span data-ttu-id="53ffc-141">`multicast`Источник имеет одного участника, но существует несколько получателей.</span><span class="sxs-lookup"><span data-stu-id="53ffc-141">`multicast` - source has one participant but there are multiple receivers.</span></span> <span data-ttu-id="53ffc-142">Список получателей можно обновить.</span><span class="sxs-lookup"><span data-stu-id="53ffc-142">Receivers list may be updated.</span></span>

> <span data-ttu-id="53ffc-143">**Примечание:** Если вы создаете множество групп маршрутизации звука (например, Bot для каждого участника), пересылается только звук главных 4 главных динамиков.</span><span class="sxs-lookup"><span data-stu-id="53ffc-143">**Note:** If you create many audio routing groups (e.g. a bot per participant), only the audio of the top 4 dominant speakers is forwarded.</span></span> <span data-ttu-id="53ffc-144">Это означает, что даже если пользователь настроил группу маршрутизации аудио, если динамики не хватает громкости в основном микшере, то он/она не может быть слышна с помощью Bot, даже если для этого динамика и для этого динамика достаточно частной группы звука.</span><span class="sxs-lookup"><span data-stu-id="53ffc-144">It means even with customized audio routing group, if the speaker is not loud enough in the main mixer, he/she cannot be heard by the bot even if there is a private audio group just for this speaker and the bot.</span></span>

## <a name="relationships"></a><span data-ttu-id="53ffc-145">Связи</span><span class="sxs-lookup"><span data-stu-id="53ffc-145">Relationships</span></span>
<span data-ttu-id="53ffc-146">Нет</span><span class="sxs-lookup"><span data-stu-id="53ffc-146">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="53ffc-147">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="53ffc-147">JSON representation</span></span>

<span data-ttu-id="53ffc-148">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="53ffc-148">The following is a JSON representation of the resource.</span></span>

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

---
title: Тип ресурса Аудиораутингграуп
description: В группе маршрутизации звука хранится частный звуковой маршрут между участниками в составе многоадресной беседы. Источник — сам участник, а приемники являются подмножеством других участников многочастой беседы.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: e7fc7de5b5caaa2f4079c453f9cd855a42577cb8
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32544003"
---
# <a name="audioroutinggroup-resource-type"></a><span data-ttu-id="1f94a-104">Тип ресурса Аудиораутингграуп</span><span class="sxs-lookup"><span data-stu-id="1f94a-104">audioRoutingGroup resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1f94a-105">В группе маршрутизации звука хранится частный звуковой маршрут между участниками в составе многоадресной беседы.</span><span class="sxs-lookup"><span data-stu-id="1f94a-105">The audio routing group stores a private audio route between participants in a multiparty conversation.</span></span> <span data-ttu-id="1f94a-106">Источник — сам участник, а приемники являются подмножеством других участников многочастой беседы.</span><span class="sxs-lookup"><span data-stu-id="1f94a-106">Source is the participant itself and the receivers are a subset of other participants in the multiparty conversation.</span></span>

> <span data-ttu-id="1f94a-107">**Примечание:** [Конфигуремиксер](../api/participant-configuremixer.md) не включает ни одного маршрута, он предназначен для всего вызова для настройки уровней громкости для комбинаций исходного приемника.</span><span class="sxs-lookup"><span data-stu-id="1f94a-107">**Note:** [ConfigureMixer](../api/participant-configuremixer.md) does not involve any routes, it is for the entire call for setting the volume levels for source-receiver combinations.</span></span>

## <a name="methods"></a><span data-ttu-id="1f94a-108">Методы</span><span class="sxs-lookup"><span data-stu-id="1f94a-108">Methods</span></span>

| <span data-ttu-id="1f94a-109">Метод</span><span class="sxs-lookup"><span data-stu-id="1f94a-109">Method</span></span>                                                  | <span data-ttu-id="1f94a-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="1f94a-110">Return Type</span></span>                               | <span data-ttu-id="1f94a-111">Описание</span><span class="sxs-lookup"><span data-stu-id="1f94a-111">Description</span></span>                                  |
|:--------------------------------------------------------|:------------------------------------------|:---------------------------------------------|
| [<span data-ttu-id="1f94a-112">Получение Аудиораутингграуп</span><span class="sxs-lookup"><span data-stu-id="1f94a-112">Get audioRoutingGroup</span></span>](../api/audioroutinggroup-get.md)| [<span data-ttu-id="1f94a-113">audioRoutingGroup</span><span class="sxs-lookup"><span data-stu-id="1f94a-113">audioRoutingGroup</span></span>](audioroutinggroup.md) | <span data-ttu-id="1f94a-114">Чтение свойств и связей объекта Аудиораутингграуп.</span><span class="sxs-lookup"><span data-stu-id="1f94a-114">Read properties and relationships of audioRoutingGroup object.</span></span>|
| [<span data-ttu-id="1f94a-115">Обновление</span><span class="sxs-lookup"><span data-stu-id="1f94a-115">Update</span></span>](../api/audioroutinggroup-update.md)            | [<span data-ttu-id="1f94a-116">audioRoutingGroup</span><span class="sxs-lookup"><span data-stu-id="1f94a-116">audioRoutingGroup</span></span>](audioroutinggroup.md) | <span data-ttu-id="1f94a-117">Обновление списка получателей.</span><span class="sxs-lookup"><span data-stu-id="1f94a-117">Update receivers list.</span></span>                       |
| [<span data-ttu-id="1f94a-118">Удаление</span><span class="sxs-lookup"><span data-stu-id="1f94a-118">Delete</span></span>](../api/audioroutinggroup-delete.md)            | <span data-ttu-id="1f94a-119">Нет</span><span class="sxs-lookup"><span data-stu-id="1f94a-119">None</span></span>                                      | <span data-ttu-id="1f94a-120">Удаление группы маршрутизации звука.</span><span class="sxs-lookup"><span data-stu-id="1f94a-120">Delete the audio routing group.</span></span>              |

## <a name="properties"></a><span data-ttu-id="1f94a-121">Свойства</span><span class="sxs-lookup"><span data-stu-id="1f94a-121">Properties</span></span>

| <span data-ttu-id="1f94a-122">Свойство</span><span class="sxs-lookup"><span data-stu-id="1f94a-122">Property</span></span>      | <span data-ttu-id="1f94a-123">Тип</span><span class="sxs-lookup"><span data-stu-id="1f94a-123">Type</span></span>              | <span data-ttu-id="1f94a-124">Описание</span><span class="sxs-lookup"><span data-stu-id="1f94a-124">Description</span></span>                                                          |
| :----------   | :---------------- | :--------------------------------------------------------------------|
| <span data-ttu-id="1f94a-125">id</span><span class="sxs-lookup"><span data-stu-id="1f94a-125">id</span></span>            | <span data-ttu-id="1f94a-126">String</span><span class="sxs-lookup"><span data-stu-id="1f94a-126">String</span></span>            | <span data-ttu-id="1f94a-127">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1f94a-127">Read-only.</span></span> <span data-ttu-id="1f94a-128">Создается сервером.</span><span class="sxs-lookup"><span data-stu-id="1f94a-128">Server generated.</span></span>                                         |
| <span data-ttu-id="1f94a-129">приемники</span><span class="sxs-lookup"><span data-stu-id="1f94a-129">receivers</span></span>     | <span data-ttu-id="1f94a-130">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="1f94a-130">String Collection</span></span> | <span data-ttu-id="1f94a-131">Список идентификаторов участников.</span><span class="sxs-lookup"><span data-stu-id="1f94a-131">List of receiving participant ids.</span></span>                                   |
| <span data-ttu-id="1f94a-132">Раутингмоде</span><span class="sxs-lookup"><span data-stu-id="1f94a-132">routingMode</span></span>   | <span data-ttu-id="1f94a-133">String</span><span class="sxs-lookup"><span data-stu-id="1f94a-133">String</span></span>            | <span data-ttu-id="1f94a-134">Режим группы маршрутизации.</span><span class="sxs-lookup"><span data-stu-id="1f94a-134">Routing group mode.</span></span>  <span data-ttu-id="1f94a-135">Возможные значения: `oneToOne`, `multicast`.</span><span class="sxs-lookup"><span data-stu-id="1f94a-135">Possible values are: `oneToOne`, `multicast`.</span></span>   |
| <span data-ttu-id="1f94a-136">sources</span><span class="sxs-lookup"><span data-stu-id="1f94a-136">sources</span></span>       | <span data-ttu-id="1f94a-137">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="1f94a-137">String Collection</span></span> | <span data-ttu-id="1f94a-138">Список идентификаторов участников исходного участника.</span><span class="sxs-lookup"><span data-stu-id="1f94a-138">List of source participant ids.</span></span>                                      |

> <span data-ttu-id="1f94a-139">**Примечание:** Режим маршрутизации определяет ограничения для источников и получателей.</span><span class="sxs-lookup"><span data-stu-id="1f94a-139">**Note:** Routing mode determines the restrictions on the sources and receivers.</span></span> <span data-ttu-id="1f94a-140">Поддерживаются только следующие группы маршрутизации.</span><span class="sxs-lookup"><span data-stu-id="1f94a-140">Only the following routing groups are supported.</span></span>
> - <span data-ttu-id="1f94a-141">`oneToOne`— у источников и приемников есть только один участник.</span><span class="sxs-lookup"><span data-stu-id="1f94a-141">`oneToOne` - sources and receivers have only one participant each.</span></span>
> - <span data-ttu-id="1f94a-142">`multicast`Источник имеет одного участника, но существует несколько получателей.</span><span class="sxs-lookup"><span data-stu-id="1f94a-142">`multicast` - source has one participant but there are multiple receivers.</span></span> <span data-ttu-id="1f94a-143">Список получателей можно обновить.</span><span class="sxs-lookup"><span data-stu-id="1f94a-143">Receivers list may be updated.</span></span>

> <span data-ttu-id="1f94a-144">**Примечание:** Если вы создаете множество групп маршрутизации звука (например, Bot для каждого участника), пересылается только звук главных 4 главных динамиков.</span><span class="sxs-lookup"><span data-stu-id="1f94a-144">**Note:** If you create many audio routing groups (e.g. a bot per participant), only the audio of the top 4 dominant speakers is forwarded.</span></span> <span data-ttu-id="1f94a-145">Это означает, что даже если пользователь настроил группу маршрутизации аудио, если динамики не хватает громкости в основном микшере, то он/она не может быть слышна с помощью Bot, даже если для этого динамика и для этого динамика достаточно частной группы звука.</span><span class="sxs-lookup"><span data-stu-id="1f94a-145">It means even with customized audio routing group, if the speaker is not loud enough in the main mixer, he/she cannot be heard by the bot even if there is a private audio group just for this speaker and the bot.</span></span>

## <a name="relationships"></a><span data-ttu-id="1f94a-146">Отношения</span><span class="sxs-lookup"><span data-stu-id="1f94a-146">Relationships</span></span>
<span data-ttu-id="1f94a-147">Нет</span><span class="sxs-lookup"><span data-stu-id="1f94a-147">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1f94a-148">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="1f94a-148">JSON representation</span></span>

<span data-ttu-id="1f94a-149">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1f94a-149">The following is a JSON representation of the resource.</span></span>

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

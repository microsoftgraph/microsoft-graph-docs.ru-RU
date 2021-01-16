---
title: Тип ресурса plannerTaskCreation
description: Содержит сведения об источнике plannerTask.
author: TarkanSevilmis
localization_priority: Normal
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: e8a2a4bf3aae5f23a04c7ecb8ad043631f946b20
ms.sourcegitcommit: 1d2adc4062c8e83d23768682cf66a731bccd313c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/16/2021
ms.locfileid: "49883262"
---
# <a name="plannertaskcreation-resource-type"></a><span data-ttu-id="f6c25-103">Тип ресурса plannerTaskCreation</span><span class="sxs-lookup"><span data-stu-id="f6c25-103">plannerTaskCreation resource type</span></span>

<span data-ttu-id="f6c25-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f6c25-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f6c25-105">Содержит сведения об источнике [plannerTask.](plannerTask.md)</span><span class="sxs-lookup"><span data-stu-id="f6c25-105">Contains information about the origin of the [plannerTask](plannerTask.md).</span></span> <span data-ttu-id="f6c25-106">У этого ресурса будут либо все его свойства, либо только одно свойство будет иметь значение, которое указывает, что задача была создана процессом, `null` описанным этим свойством.</span><span class="sxs-lookup"><span data-stu-id="f6c25-106">This resource will either have all its properties set to `null`, or exactly one property will have a value that indicates that the task was created by the process described by that property.</span></span> <span data-ttu-id="f6c25-107">Все свойства `null` указывают, что эта задача не была создана специализированным процессом.</span><span class="sxs-lookup"><span data-stu-id="f6c25-107">All properties `null` indicates this task was not created by any specialized process.</span></span> <span data-ttu-id="f6c25-108">Приложениям не нужно знать источник задачи, чтобы иметь возможность работать с ней; Однако некоторые приложения могут использовать дополнительные сведения для предоставления определенных функций, которые могут быть доступны для выполнения этих задач.</span><span class="sxs-lookup"><span data-stu-id="f6c25-108">Apps do not need to know the origin of the task to be able to work with it; however, some apps can use the additional information to provide specific experiences around these tasks.</span></span> <span data-ttu-id="f6c25-109">Дополнительные дополнительные ресурсы см. в документации.</span><span class="sxs-lookup"><span data-stu-id="f6c25-109">See the documentation for specific resources to learn more.</span></span>

## <a name="properties"></a><span data-ttu-id="f6c25-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="f6c25-110">Properties</span></span>
|<span data-ttu-id="f6c25-111">Свойство</span><span class="sxs-lookup"><span data-stu-id="f6c25-111">Property</span></span>|<span data-ttu-id="f6c25-112">Тип</span><span class="sxs-lookup"><span data-stu-id="f6c25-112">Type</span></span>|<span data-ttu-id="f6c25-113">Описание</span><span class="sxs-lookup"><span data-stu-id="f6c25-113">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f6c25-114">teamsPublicationInfo</span><span class="sxs-lookup"><span data-stu-id="f6c25-114">teamsPublicationInfo</span></span>|[<span data-ttu-id="f6c25-115">plannerTeamsPublicationInfo</span><span class="sxs-lookup"><span data-stu-id="f6c25-115">plannerTeamsPublicationInfo</span></span>](../resources/plannerteamspublicationinfo.md)|<span data-ttu-id="f6c25-116">Сведения о процессе публикации, который создал эту задачу.</span><span class="sxs-lookup"><span data-stu-id="f6c25-116">Information about the publication process that created this task.</span></span> <span data-ttu-id="f6c25-117">`null` указывает, что задача не была создана процессом публикации.</span><span class="sxs-lookup"><span data-stu-id="f6c25-117">`null` value indicates that the task was not created by a publication process.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f6c25-118">Связи</span><span class="sxs-lookup"><span data-stu-id="f6c25-118">Relationships</span></span>
<span data-ttu-id="f6c25-119">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="f6c25-119">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f6c25-120">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="f6c25-120">JSON representation</span></span>
<span data-ttu-id="f6c25-121">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f6c25-121">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.plannerTaskCreation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.plannerTaskCreation",
  "teamsPublicationInfo": {
    "@odata.type": "microsoft.graph.plannerTeamsPublicationInfo"
  }
}
```


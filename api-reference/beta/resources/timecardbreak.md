---
title: тип ресурса timeCardBreak
description: Представляет определенный разрыв химкарта.
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 509667ec1fad41f956ee5ee6d6a4371b8d17fc2e
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/06/2021
ms.locfileid: "52786394"
---
# <a name="timecardbreak-resource-type"></a><span data-ttu-id="f6a94-103">тип ресурса timeCardBreak</span><span class="sxs-lookup"><span data-stu-id="f6a94-103">timeCardBreak resource type</span></span>

<span data-ttu-id="f6a94-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f6a94-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f6a94-105">Представляет определенный [разрыв timeCard.](timecard.md)</span><span class="sxs-lookup"><span data-stu-id="f6a94-105">Represents a specific [timeCard](timecard.md) break.</span></span>

## <a name="properties"></a><span data-ttu-id="f6a94-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="f6a94-106">Properties</span></span>
|<span data-ttu-id="f6a94-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="f6a94-107">Property</span></span>               |<span data-ttu-id="f6a94-108">Тип</span><span class="sxs-lookup"><span data-stu-id="f6a94-108">Type</span></span>           |<span data-ttu-id="f6a94-109">Описание</span><span class="sxs-lookup"><span data-stu-id="f6a94-109">Description</span></span>                                                                |
|-----------------------|---------------|---------------------------------------------------------------------------|
| <span data-ttu-id="f6a94-110">breakId</span><span class="sxs-lookup"><span data-stu-id="f6a94-110">breakId</span></span>                   |`Edm.string`  |<span data-ttu-id="f6a94-111">ID **timeCardBreak**.</span><span class="sxs-lookup"><span data-stu-id="f6a94-111">ID of the **timeCardBreak**.</span></span>|
| <span data-ttu-id="f6a94-112">начать</span><span class="sxs-lookup"><span data-stu-id="f6a94-112">start</span></span>                 |[<span data-ttu-id="f6a94-113">timeCardEvent</span><span class="sxs-lookup"><span data-stu-id="f6a94-113">timeCardEvent</span></span>](timecardevent.md)    | <span data-ttu-id="f6a94-114">Событие начала **timeCardBreak**.</span><span class="sxs-lookup"><span data-stu-id="f6a94-114">The start event of the **timeCardBreak**.</span></span>|
| <span data-ttu-id="f6a94-115">end</span><span class="sxs-lookup"><span data-stu-id="f6a94-115">end</span></span>                   |[<span data-ttu-id="f6a94-116">timeCardEvent</span><span class="sxs-lookup"><span data-stu-id="f6a94-116">timeCardEvent</span></span>](timecardevent.md)    | <span data-ttu-id="f6a94-117">Событие начала **timeCardBreak**.</span><span class="sxs-lookup"><span data-stu-id="f6a94-117">The start event of the **timeCardBreak**.</span></span>|
| <span data-ttu-id="f6a94-118">notes</span><span class="sxs-lookup"><span data-stu-id="f6a94-118">notes</span></span>                 |[<span data-ttu-id="f6a94-119">itemBody</span><span class="sxs-lookup"><span data-stu-id="f6a94-119">itemBody</span></span>](itembody.md)  | <span data-ttu-id="f6a94-120">Заметки о **timeCardBreak**.</span><span class="sxs-lookup"><span data-stu-id="f6a94-120">Notes about the **timeCardBreak**.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="f6a94-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f6a94-121">JSON representation</span></span>

<span data-ttu-id="f6a94-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f6a94-122">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.timeCardBreak"
}-->
```json
{
    "breakId":"string",
    "notes":{
        "content": "string",
        "contentType": "string"
    },
    "start":{
        "dateTime":"String (timestamp)",
        "atApprovedLocation":true,
        "notes":{
            "content": "string",
            "contentType": "text"
        },
    },
    "end":null
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "timeCardBreak resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

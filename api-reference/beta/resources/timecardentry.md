---
title: тип ресурса timeCardEntry
description: Представляет определенную запись с химкаром.
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: d09b324b4d43765f05de789129021e2eb1f24789
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/06/2021
ms.locfileid: "52786411"
---
# <a name="timecardentry-resource-type"></a><span data-ttu-id="fbdf4-103">тип ресурса timeCardEntry</span><span class="sxs-lookup"><span data-stu-id="fbdf4-103">timeCardEntry resource type</span></span>

<span data-ttu-id="fbdf4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fbdf4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fbdf4-105">Представляет определенную [запись timeCard.](timecard.md)</span><span class="sxs-lookup"><span data-stu-id="fbdf4-105">Represents a specific [timeCard](timecard.md) entry.</span></span>

## <a name="properties"></a><span data-ttu-id="fbdf4-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="fbdf4-106">Properties</span></span>
|<span data-ttu-id="fbdf4-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="fbdf4-107">Property</span></span>               |<span data-ttu-id="fbdf4-108">Тип</span><span class="sxs-lookup"><span data-stu-id="fbdf4-108">Type</span></span>           |<span data-ttu-id="fbdf4-109">Описание</span><span class="sxs-lookup"><span data-stu-id="fbdf4-109">Description</span></span>                                                                |
|-----------------------|---------------|---------------------------------------------------------------------------|
| <span data-ttu-id="fbdf4-110">clockInEvent</span><span class="sxs-lookup"><span data-stu-id="fbdf4-110">clockInEvent</span></span>       |[<span data-ttu-id="fbdf4-111">timeCardEvent</span><span class="sxs-lookup"><span data-stu-id="fbdf4-111">timeCardEvent</span></span>](timecardevent.md)    | <span data-ttu-id="fbdf4-112">Событие с часовой стрелкой **timeCard**.</span><span class="sxs-lookup"><span data-stu-id="fbdf4-112">The clock-in event of the **timeCard**.</span></span>|
| <span data-ttu-id="fbdf4-113">clockOutEvent</span><span class="sxs-lookup"><span data-stu-id="fbdf4-113">clockOutEvent</span></span>                 |[<span data-ttu-id="fbdf4-114">timeCardEvent</span><span class="sxs-lookup"><span data-stu-id="fbdf4-114">timeCardEvent</span></span>](timecardevent.md)  |<span data-ttu-id="fbdf4-115">Событие clock-out **timeCard**.</span><span class="sxs-lookup"><span data-stu-id="fbdf4-115">The clock-out event of the **timeCard**.</span></span> |
| <span data-ttu-id="fbdf4-116">перерывы</span><span class="sxs-lookup"><span data-stu-id="fbdf4-116">breaks</span></span>    |<span data-ttu-id="fbdf4-117">[коллекция timeCardBreak](timecardbreak.md)</span><span class="sxs-lookup"><span data-stu-id="fbdf4-117">[timeCardBreak](timecardbreak.md) collection</span></span>    |<span data-ttu-id="fbdf4-118">Список перерывов, связанных с **timeCard**.</span><span class="sxs-lookup"><span data-stu-id="fbdf4-118">The list of breaks associated with the **timeCard**.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="fbdf4-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="fbdf4-119">JSON representation</span></span>

<span data-ttu-id="fbdf4-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fbdf4-120">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.timeCardEntry"
}-->
```json
{
   "clockInEvent": { "@odata.type":"microsoft.graph.timeCardEvent" },
   "clockOutEvent": { "@odata.type":"microsoft.graph.timeCardEvent" },
   "breaks":[
      {
         "breakId":"string",
         "notes":{
             "content": "string",
             "contentType": "text"
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
   ]
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "timecardentry resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

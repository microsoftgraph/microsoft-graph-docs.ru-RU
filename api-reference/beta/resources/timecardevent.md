---
title: тип ресурса timeCardEvent
description: Представляет определенное событие с хет-листом.
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: a8be7d000b3d55368f7378e9b993b5015b7ef632
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/06/2021
ms.locfileid: "52786399"
---
# <a name="timecardevent-resource-type"></a><span data-ttu-id="b549d-103">тип ресурса timeCardEvent</span><span class="sxs-lookup"><span data-stu-id="b549d-103">timeCardEvent resource type</span></span>

<span data-ttu-id="b549d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b549d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b549d-105">Представляет определенное [событие timeCard.](timecard.md)</span><span class="sxs-lookup"><span data-stu-id="b549d-105">Represents a specific [timeCard](timecard.md) event.</span></span>

## <a name="properties"></a><span data-ttu-id="b549d-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="b549d-106">Properties</span></span>
|<span data-ttu-id="b549d-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="b549d-107">Property</span></span>               |<span data-ttu-id="b549d-108">Тип</span><span class="sxs-lookup"><span data-stu-id="b549d-108">Type</span></span>           |<span data-ttu-id="b549d-109">Описание</span><span class="sxs-lookup"><span data-stu-id="b549d-109">Description</span></span>                                                                |
|-----------------------|---------------|---------------------------------------------------------------------------|
| <span data-ttu-id="b549d-110">dateTime</span><span class="sxs-lookup"><span data-stu-id="b549d-110">dateTime</span></span>                  |`Edm.dateTimeOffset`  |<span data-ttu-id="b549d-111">Время записи.</span><span class="sxs-lookup"><span data-stu-id="b549d-111">The time the entry is recorded.</span></span> |
| <span data-ttu-id="b549d-112">atApprovedLocation</span><span class="sxs-lookup"><span data-stu-id="b549d-112">atApprovedLocation</span></span> |`Edm.boolean `  |<span data-ttu-id="b549d-113">Указывает, была ли запись записана в утвержденное расположение.</span><span class="sxs-lookup"><span data-stu-id="b549d-113">Indicates whether the entry was recorded at the approved location.</span></span> |
| <span data-ttu-id="b549d-114">notes</span><span class="sxs-lookup"><span data-stu-id="b549d-114">notes</span></span>                 |[<span data-ttu-id="b549d-115">itemBody</span><span class="sxs-lookup"><span data-stu-id="b549d-115">itemBody</span></span>](itembody.md)  | <span data-ttu-id="b549d-116">Заметки о **timeCardEvent**.</span><span class="sxs-lookup"><span data-stu-id="b549d-116">Notes about the **timeCardEvent**.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="b549d-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b549d-117">JSON representation</span></span>

<span data-ttu-id="b549d-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b549d-118">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.timeCardEvent"
}-->
```json
{
   "atApprovedLocation":true,
   "notes":{ "@odata.type":"microsoft.graph.itemBody" }
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "timeCardEvent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

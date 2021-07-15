---
title: тип ресурса rejectJoinResponse
description: Содержит ответ на отклонение участника, который пытается присоединиться к собранию.
author: yizhenww
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: c917b2c5ba0ed273af1c8e89c78b07a80d6c45fc
ms.sourcegitcommit: 6d247f44a6ee4d8515c3863ee8a2683163c9f829
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/14/2021
ms.locfileid: "53428869"
---
# <a name="rejectjoinresponse-resource-type"></a><span data-ttu-id="51974-103">тип ресурса rejectJoinResponse</span><span class="sxs-lookup"><span data-stu-id="51974-103">rejectJoinResponse resource type</span></span>

<span data-ttu-id="51974-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="51974-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="51974-105">Содержит ответ на отклонение участника, который пытается присоединиться к собранию.</span><span class="sxs-lookup"><span data-stu-id="51974-105">Contains a response to reject a participant who tries to join the meeting.</span></span>

<span data-ttu-id="51974-106">Это имеет тот же эффект, что и отклонение уведомления о входящих вызовах политики с помощью метода [отклонить вызов.](../api/call-reject.md)</span><span class="sxs-lookup"><span data-stu-id="51974-106">This has the same effect as rejecting a policy recording incoming call notification using the [reject-call](../api/call-reject.md) method.</span></span> <span data-ttu-id="51974-107">Бот будет по-прежнему получать уведомление о присоединении участника к новому пользователю до тех пор, пока его емкость не будет достигнута.</span><span class="sxs-lookup"><span data-stu-id="51974-107">The bot will continue to receive a participant joining notification for a new user joining until its capacity has been reached.</span></span>

## <a name="properties"></a><span data-ttu-id="51974-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="51974-108">Properties</span></span>

| <span data-ttu-id="51974-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="51974-109">Property</span></span>         | <span data-ttu-id="51974-110">Тип</span><span class="sxs-lookup"><span data-stu-id="51974-110">Type</span></span>                            | <span data-ttu-id="51974-111">Описание</span><span class="sxs-lookup"><span data-stu-id="51974-111">Description</span></span>                                                                                                                                                  |
| :--------------- | :------------------------------ | :----------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="51974-112">reason</span><span class="sxs-lookup"><span data-stu-id="51974-112">reason</span></span>           | <span data-ttu-id="51974-113">String</span><span class="sxs-lookup"><span data-stu-id="51974-113">String</span></span>                          | <span data-ttu-id="51974-114">Причина отказа.</span><span class="sxs-lookup"><span data-stu-id="51974-114">The rejection reason.</span></span> <span data-ttu-id="51974-115">Возможные значения: `None`, `Busy` и `Forbidden`.</span><span class="sxs-lookup"><span data-stu-id="51974-115">Possible values are `None`, `Busy`, and `Forbidden`.</span></span>                                                                                     |

## <a name="json-representation"></a><span data-ttu-id="51974-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="51974-116">JSON representation</span></span>

<span data-ttu-id="51974-117">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="51974-117">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.rejectJoinResponse"
}-->
```json
{
  "reason": "None | Busy | Forbidden" 
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "rejectJoinResponse resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

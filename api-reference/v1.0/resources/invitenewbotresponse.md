---
title: тип ресурса inviteNewBotResponse
description: Содержит ответ на запрос о повторном отправлении уведомления о присоединении участника в качестве входящих вызовов в нужное расположение.
author: yizhenww
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 675b7cd1df35b25e3414f36a4dd04e389e05b192
ms.sourcegitcommit: 6d247f44a6ee4d8515c3863ee8a2683163c9f829
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/14/2021
ms.locfileid: "53430188"
---
# <a name="invitenewbotresponse-resource-type"></a><span data-ttu-id="16bfb-103">тип ресурса inviteNewBotResponse</span><span class="sxs-lookup"><span data-stu-id="16bfb-103">inviteNewBotResponse resource type</span></span>

<span data-ttu-id="16bfb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="16bfb-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="16bfb-105">Содержит ответ на запрос о повторном отправлении уведомления о присоединении участника в качестве входящих вызовов в нужное расположение.</span><span class="sxs-lookup"><span data-stu-id="16bfb-105">Contains a response to a request to have a participant joining notification sent out again as a incoming call notification to the desired location.</span></span>

## <a name="properties"></a><span data-ttu-id="16bfb-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="16bfb-106">Properties</span></span>

| <span data-ttu-id="16bfb-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="16bfb-107">Property</span></span>         | <span data-ttu-id="16bfb-108">Тип</span><span class="sxs-lookup"><span data-stu-id="16bfb-108">Type</span></span>                            | <span data-ttu-id="16bfb-109">Описание</span><span class="sxs-lookup"><span data-stu-id="16bfb-109">Description</span></span>                                                                                                                                                  |
| :--------------- | :------------------------------ | :----------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="16bfb-110">inviteUri</span><span class="sxs-lookup"><span data-stu-id="16bfb-110">inviteUri</span></span>        | <span data-ttu-id="16bfb-111">String</span><span class="sxs-lookup"><span data-stu-id="16bfb-111">String</span></span>                          | <span data-ttu-id="16bfb-112">URI для получения нового уведомления о входящих вызовах.</span><span class="sxs-lookup"><span data-stu-id="16bfb-112">URI to receive new incoming call notification.</span></span>                                                                                                                |

## <a name="json-representation"></a><span data-ttu-id="16bfb-113">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="16bfb-113">JSON representation</span></span>

<span data-ttu-id="16bfb-114">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="16bfb-114">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.inviteNewBotResponse"
}-->
```json
{
  "inviteUri": "uri" 
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "inviteNewBotResponse resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

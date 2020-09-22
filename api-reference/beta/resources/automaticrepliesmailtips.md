---
title: Тип ресурса Аутоматикреплиесмаилтипс
description: Подсказки о любых автоматических ответах, настроенных в почтовом ящике.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: svpsiva
ms.openlocfilehash: 2191f715d3763707f132c4907e34189941436c59
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48034084"
---
# <a name="automaticrepliesmailtips-resource-type"></a><span data-ttu-id="c348a-103">Тип ресурса Аутоматикреплиесмаилтипс</span><span class="sxs-lookup"><span data-stu-id="c348a-103">automaticRepliesMailTips resource type</span></span>

<span data-ttu-id="c348a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c348a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c348a-105">[Подсказки](../resources/mailtips.md) о любых автоматических ответах, настроенных в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="c348a-105">[MailTips](../resources/mailtips.md) about any automatic replies that have been set up on a mailbox.</span></span>

## <a name="properties"></a><span data-ttu-id="c348a-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="c348a-106">Properties</span></span>
| <span data-ttu-id="c348a-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="c348a-107">Property</span></span>     | <span data-ttu-id="c348a-108">Тип</span><span class="sxs-lookup"><span data-stu-id="c348a-108">Type</span></span>   |<span data-ttu-id="c348a-109">Описание</span><span class="sxs-lookup"><span data-stu-id="c348a-109">Description</span></span>|
|:-----|:-----|:-----|
| <span data-ttu-id="c348a-110">message</span><span class="sxs-lookup"><span data-stu-id="c348a-110">message</span></span> | <span data-ttu-id="c348a-111">String</span><span class="sxs-lookup"><span data-stu-id="c348a-111">String</span></span> | <span data-ttu-id="c348a-112">Сообщение автоматического ответа.</span><span class="sxs-lookup"><span data-stu-id="c348a-112">The automatic reply message.</span></span> |
| <span data-ttu-id="c348a-113">мессажелангуаже</span><span class="sxs-lookup"><span data-stu-id="c348a-113">messageLanguage</span></span> | [<span data-ttu-id="c348a-114">localeInfo</span><span class="sxs-lookup"><span data-stu-id="c348a-114">localeInfo</span></span>](../resources/localeinfo.md) | <span data-ttu-id="c348a-115">Язык, на котором находится сообщение с автоматическим ответом.</span><span class="sxs-lookup"><span data-stu-id="c348a-115">The language that the automatic reply message is in.</span></span> |
| <span data-ttu-id="c348a-116">счедуледендтиме</span><span class="sxs-lookup"><span data-stu-id="c348a-116">scheduledEndTime</span></span> | [<span data-ttu-id="c348a-117">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="c348a-117">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md) | <span data-ttu-id="c348a-118">Дата и время завершения установки автоматических ответов.</span><span class="sxs-lookup"><span data-stu-id="c348a-118">The date and time that automatic replies are set to end.</span></span> |
| <span data-ttu-id="c348a-119">счедуледстарттиме</span><span class="sxs-lookup"><span data-stu-id="c348a-119">scheduledStartTime</span></span> | [<span data-ttu-id="c348a-120">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="c348a-120">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md) | <span data-ttu-id="c348a-121">Дата и время начала набора автоматических ответов.</span><span class="sxs-lookup"><span data-stu-id="c348a-121">The date and time that automatic replies are set to begin.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="c348a-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c348a-122">JSON representation</span></span>

<span data-ttu-id="c348a-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c348a-123">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "messageLanguage",
    "scheduledEndTime",
    "scheduledStartTime"
  ],
  "@odata.type": "microsoft.graph.automaticRepliesMailTips"
}-->

```json
{
  "message": "string",
  "messageLanguage": {"@odata.type": "microsoft.graph.localeInfo"},
  "scheduledEndTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "scheduledStartTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "automaticRepliesMailTips resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->



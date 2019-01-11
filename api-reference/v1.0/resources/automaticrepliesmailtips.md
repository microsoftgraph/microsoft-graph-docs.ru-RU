---
title: Тип ресурса automaticRepliesMailTips
description: Почтовые подсказки о автоматические ответы, которые были настроены для почтового ящика.
localization_priority: Normal
ms.openlocfilehash: bb477979b975996f70e4b8ac624befab7f254f46
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27816277"
---
# <a name="automaticrepliesmailtips-resource-type"></a><span data-ttu-id="51cac-103">Тип ресурса automaticRepliesMailTips</span><span class="sxs-lookup"><span data-stu-id="51cac-103">automaticRepliesMailTips resource type</span></span>


<span data-ttu-id="51cac-104">[Почтовые подсказки](../resources/mailtips.md) о автоматические ответы, которые были настроены для почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="51cac-104">[MailTips](../resources/mailtips.md) about any automatic replies that have been set up on a mailbox.</span></span>

## <a name="properties"></a><span data-ttu-id="51cac-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="51cac-105">Properties</span></span>
| <span data-ttu-id="51cac-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="51cac-106">Property</span></span>     | <span data-ttu-id="51cac-107">Тип</span><span class="sxs-lookup"><span data-stu-id="51cac-107">Type</span></span>   |<span data-ttu-id="51cac-108">Описание</span><span class="sxs-lookup"><span data-stu-id="51cac-108">Description</span></span>|
|:-----|:-----|:-----|
| <span data-ttu-id="51cac-109">message</span><span class="sxs-lookup"><span data-stu-id="51cac-109">message</span></span> | <span data-ttu-id="51cac-110">String</span><span class="sxs-lookup"><span data-stu-id="51cac-110">String</span></span> | <span data-ttu-id="51cac-111">Сообщение автоматического ответа.</span><span class="sxs-lookup"><span data-stu-id="51cac-111">The automatic reply message.</span></span> |
| <span data-ttu-id="51cac-112">messageLanguage</span><span class="sxs-lookup"><span data-stu-id="51cac-112">messageLanguage</span></span> | [<span data-ttu-id="51cac-113">localeInfo</span><span class="sxs-lookup"><span data-stu-id="51cac-113">localeInfo</span></span>](../resources/localeinfo.md) | <span data-ttu-id="51cac-114">Язык, сообщение автоматического ответа.</span><span class="sxs-lookup"><span data-stu-id="51cac-114">The language that the automatic reply message is in.</span></span> |
| <span data-ttu-id="51cac-115">scheduledEndTime</span><span class="sxs-lookup"><span data-stu-id="51cac-115">scheduledEndTime</span></span> | [<span data-ttu-id="51cac-116">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="51cac-116">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md) | <span data-ttu-id="51cac-117">Дата и время окончания устанавливаются автоматические ответы.</span><span class="sxs-lookup"><span data-stu-id="51cac-117">The date and time that automatic replies are set to end.</span></span> |
| <span data-ttu-id="51cac-118">scheduledStartTime</span><span class="sxs-lookup"><span data-stu-id="51cac-118">scheduledStartTime</span></span> | [<span data-ttu-id="51cac-119">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="51cac-119">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md) | <span data-ttu-id="51cac-120">Дата и время автоматические ответы чтобы начать.</span><span class="sxs-lookup"><span data-stu-id="51cac-120">The date and time that automatic replies are set to begin.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="51cac-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="51cac-121">JSON representation</span></span>

<span data-ttu-id="51cac-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="51cac-122">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "automaticRepliesMailTips resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

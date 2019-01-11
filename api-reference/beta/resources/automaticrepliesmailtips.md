---
title: Тип ресурса automaticRepliesMailTips
description: Почтовые подсказки о автоматические ответы, которые были настроены для почтового ящика.
localization_priority: Normal
ms.openlocfilehash: 80ecaaa9fced0bcb00494b0414a86f0a11fd8996
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27833231"
---
# <a name="automaticrepliesmailtips-resource-type"></a><span data-ttu-id="46c2e-103">Тип ресурса automaticRepliesMailTips</span><span class="sxs-lookup"><span data-stu-id="46c2e-103">automaticRepliesMailTips resource type</span></span>

> <span data-ttu-id="46c2e-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="46c2e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="46c2e-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="46c2e-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="46c2e-106">[Почтовые подсказки](../resources/mailtips.md) о автоматические ответы, которые были настроены для почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="46c2e-106">[MailTips](../resources/mailtips.md) about any automatic replies that have been set up on a mailbox.</span></span>

## <a name="properties"></a><span data-ttu-id="46c2e-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="46c2e-107">Properties</span></span>
| <span data-ttu-id="46c2e-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="46c2e-108">Property</span></span>     | <span data-ttu-id="46c2e-109">Тип</span><span class="sxs-lookup"><span data-stu-id="46c2e-109">Type</span></span>   |<span data-ttu-id="46c2e-110">Описание</span><span class="sxs-lookup"><span data-stu-id="46c2e-110">Description</span></span>|
|:-----|:-----|:-----|
| <span data-ttu-id="46c2e-111">message</span><span class="sxs-lookup"><span data-stu-id="46c2e-111">message</span></span> | <span data-ttu-id="46c2e-112">String</span><span class="sxs-lookup"><span data-stu-id="46c2e-112">String</span></span> | <span data-ttu-id="46c2e-113">Сообщение автоматического ответа.</span><span class="sxs-lookup"><span data-stu-id="46c2e-113">The automatic reply message.</span></span> |
| <span data-ttu-id="46c2e-114">messageLanguage</span><span class="sxs-lookup"><span data-stu-id="46c2e-114">messageLanguage</span></span> | [<span data-ttu-id="46c2e-115">localeInfo</span><span class="sxs-lookup"><span data-stu-id="46c2e-115">localeInfo</span></span>](../resources/localeinfo.md) | <span data-ttu-id="46c2e-116">Язык, сообщение автоматического ответа.</span><span class="sxs-lookup"><span data-stu-id="46c2e-116">The language that the automatic reply message is in.</span></span> |
| <span data-ttu-id="46c2e-117">scheduledEndTime</span><span class="sxs-lookup"><span data-stu-id="46c2e-117">scheduledEndTime</span></span> | [<span data-ttu-id="46c2e-118">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="46c2e-118">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md) | <span data-ttu-id="46c2e-119">Дата и время окончания устанавливаются автоматические ответы.</span><span class="sxs-lookup"><span data-stu-id="46c2e-119">The date and time that automatic replies are set to end.</span></span> |
| <span data-ttu-id="46c2e-120">scheduledStartTime</span><span class="sxs-lookup"><span data-stu-id="46c2e-120">scheduledStartTime</span></span> | [<span data-ttu-id="46c2e-121">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="46c2e-121">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md) | <span data-ttu-id="46c2e-122">Дата и время автоматические ответы чтобы начать.</span><span class="sxs-lookup"><span data-stu-id="46c2e-122">The date and time that automatic replies are set to begin.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="46c2e-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="46c2e-123">JSON representation</span></span>

<span data-ttu-id="46c2e-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="46c2e-124">Here is a JSON representation of the resource.</span></span>

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

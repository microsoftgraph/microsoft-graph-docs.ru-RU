---
title: Тип ресурса automaticRepliesMailTips
description: Сообщения об автоматических ответах, которые были настроены для почтового ящика.
localization_priority: Normal
author: abheek-das
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 1cc7f65a526d4550182f1e6dc0c5ea25a12ee182
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50135753"
---
# <a name="automaticrepliesmailtips-resource-type"></a><span data-ttu-id="d23b8-103">Тип ресурса automaticRepliesMailTips</span><span class="sxs-lookup"><span data-stu-id="d23b8-103">automaticRepliesMailTips resource type</span></span>

<span data-ttu-id="d23b8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d23b8-104">Namespace: microsoft.graph</span></span>


<span data-ttu-id="d23b8-105">[Сообщения об автоматических](../resources/mailtips.md) ответах, которые были настроены для почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="d23b8-105">[MailTips](../resources/mailtips.md) about any automatic replies that have been set up on a mailbox.</span></span>

## <a name="properties"></a><span data-ttu-id="d23b8-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="d23b8-106">Properties</span></span>
| <span data-ttu-id="d23b8-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="d23b8-107">Property</span></span>     | <span data-ttu-id="d23b8-108">Тип</span><span class="sxs-lookup"><span data-stu-id="d23b8-108">Type</span></span>   |<span data-ttu-id="d23b8-109">Описание</span><span class="sxs-lookup"><span data-stu-id="d23b8-109">Description</span></span>|
|:-----|:-----|:-----|
| <span data-ttu-id="d23b8-110">message</span><span class="sxs-lookup"><span data-stu-id="d23b8-110">message</span></span> | <span data-ttu-id="d23b8-111">String</span><span class="sxs-lookup"><span data-stu-id="d23b8-111">String</span></span> | <span data-ttu-id="d23b8-112">Автоматическое ответное сообщение.</span><span class="sxs-lookup"><span data-stu-id="d23b8-112">The automatic reply message.</span></span> |
| <span data-ttu-id="d23b8-113">messageLanguage</span><span class="sxs-lookup"><span data-stu-id="d23b8-113">messageLanguage</span></span> | [<span data-ttu-id="d23b8-114">localeInfo</span><span class="sxs-lookup"><span data-stu-id="d23b8-114">localeInfo</span></span>](../resources/localeinfo.md) | <span data-ttu-id="d23b8-115">Язык, на который находится автоматическое ответное сообщение.</span><span class="sxs-lookup"><span data-stu-id="d23b8-115">The language that the automatic reply message is in.</span></span> |
| <span data-ttu-id="d23b8-116">scheduledEndTime</span><span class="sxs-lookup"><span data-stu-id="d23b8-116">scheduledEndTime</span></span> | [<span data-ttu-id="d23b8-117">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="d23b8-117">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md) | <span data-ttu-id="d23b8-118">Дата и время окончания автоматических ответов.</span><span class="sxs-lookup"><span data-stu-id="d23b8-118">The date and time that automatic replies are set to end.</span></span> |
| <span data-ttu-id="d23b8-119">scheduledStartTime</span><span class="sxs-lookup"><span data-stu-id="d23b8-119">scheduledStartTime</span></span> | [<span data-ttu-id="d23b8-120">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="d23b8-120">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md) | <span data-ttu-id="d23b8-121">Дата и время начала автоматических ответов.</span><span class="sxs-lookup"><span data-stu-id="d23b8-121">The date and time that automatic replies are set to begin.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="d23b8-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d23b8-122">JSON representation</span></span>

<span data-ttu-id="d23b8-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d23b8-123">Here is a JSON representation of the resource.</span></span>

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


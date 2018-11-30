---
title: Тип ресурса automaticRepliesMailTips
description: Почтовые подсказки о автоматические ответы, которые были настроены для почтового ящика.
ms.openlocfilehash: 943a465671c777305e5623104c82f377ff9496dd
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27026393"
---
# <a name="automaticrepliesmailtips-resource-type"></a><span data-ttu-id="bc192-103">Тип ресурса automaticRepliesMailTips</span><span class="sxs-lookup"><span data-stu-id="bc192-103">automaticRepliesMailTips resource type</span></span>


<span data-ttu-id="bc192-104">[Почтовые подсказки](../resources/mailtips.md) о автоматические ответы, которые были настроены для почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="bc192-104">[MailTips](../resources/mailtips.md) about any automatic replies that have been set up on a mailbox.</span></span>

## <a name="properties"></a><span data-ttu-id="bc192-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="bc192-105">Properties</span></span>
| <span data-ttu-id="bc192-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="bc192-106">Property</span></span>     | <span data-ttu-id="bc192-107">Тип</span><span class="sxs-lookup"><span data-stu-id="bc192-107">Type</span></span>   |<span data-ttu-id="bc192-108">Описание</span><span class="sxs-lookup"><span data-stu-id="bc192-108">Description</span></span>|
|:-----|:-----|:-----|
| <span data-ttu-id="bc192-109">message</span><span class="sxs-lookup"><span data-stu-id="bc192-109">message</span></span> | <span data-ttu-id="bc192-110">String</span><span class="sxs-lookup"><span data-stu-id="bc192-110">String</span></span> | <span data-ttu-id="bc192-111">Сообщение автоматического ответа.</span><span class="sxs-lookup"><span data-stu-id="bc192-111">The automatic reply message.</span></span> |
| <span data-ttu-id="bc192-112">messageLanguage</span><span class="sxs-lookup"><span data-stu-id="bc192-112">messageLanguage</span></span> | [<span data-ttu-id="bc192-113">localeInfo</span><span class="sxs-lookup"><span data-stu-id="bc192-113">localeInfo</span></span>](../resources/localeinfo.md) | <span data-ttu-id="bc192-114">Язык, сообщение автоматического ответа.</span><span class="sxs-lookup"><span data-stu-id="bc192-114">The language that the automatic reply message is in.</span></span> |
| <span data-ttu-id="bc192-115">scheduledEndTime</span><span class="sxs-lookup"><span data-stu-id="bc192-115">scheduledEndTime</span></span> | [<span data-ttu-id="bc192-116">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="bc192-116">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md) | <span data-ttu-id="bc192-117">Дата и время окончания устанавливаются автоматические ответы.</span><span class="sxs-lookup"><span data-stu-id="bc192-117">The date and time that automatic replies are set to end.</span></span> |
| <span data-ttu-id="bc192-118">scheduledStartTime</span><span class="sxs-lookup"><span data-stu-id="bc192-118">scheduledStartTime</span></span> | [<span data-ttu-id="bc192-119">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="bc192-119">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md) | <span data-ttu-id="bc192-120">Дата и время автоматические ответы чтобы начать.</span><span class="sxs-lookup"><span data-stu-id="bc192-120">The date and time that automatic replies are set to begin.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="bc192-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bc192-121">JSON representation</span></span>

<span data-ttu-id="bc192-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bc192-122">Here is a JSON representation of the resource.</span></span>

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
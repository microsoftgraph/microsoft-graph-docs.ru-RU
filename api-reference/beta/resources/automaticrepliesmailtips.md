---
title: Тип ресурса Аутоматикреплиесмаилтипс
description: Подсказки о любых автоматических ответах, настроенных в почтовом ящике.
localization_priority: Normal
ms.openlocfilehash: 7eb9d57da427090c554e111ae6ba1eeb369437ca
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32535586"
---
# <a name="automaticrepliesmailtips-resource-type"></a><span data-ttu-id="59539-103">Тип ресурса Аутоматикреплиесмаилтипс</span><span class="sxs-lookup"><span data-stu-id="59539-103">automaticRepliesMailTips resource type</span></span>


<span data-ttu-id="59539-104">[Подсказки](../resources/mailtips.md) о любых автоматических ответах, настроенных в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="59539-104">[MailTips](../resources/mailtips.md) about any automatic replies that have been set up on a mailbox.</span></span>

## <a name="properties"></a><span data-ttu-id="59539-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="59539-105">Properties</span></span>
| <span data-ttu-id="59539-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="59539-106">Property</span></span>     | <span data-ttu-id="59539-107">Тип</span><span class="sxs-lookup"><span data-stu-id="59539-107">Type</span></span>   |<span data-ttu-id="59539-108">Описание</span><span class="sxs-lookup"><span data-stu-id="59539-108">Description</span></span>|
|:-----|:-----|:-----|
| <span data-ttu-id="59539-109">message</span><span class="sxs-lookup"><span data-stu-id="59539-109">message</span></span> | <span data-ttu-id="59539-110">String</span><span class="sxs-lookup"><span data-stu-id="59539-110">String</span></span> | <span data-ttu-id="59539-111">Сообщение автоматического ответа.</span><span class="sxs-lookup"><span data-stu-id="59539-111">The automatic reply message.</span></span> |
| <span data-ttu-id="59539-112">Мессажелангуаже</span><span class="sxs-lookup"><span data-stu-id="59539-112">messageLanguage</span></span> | [<span data-ttu-id="59539-113">localeInfo</span><span class="sxs-lookup"><span data-stu-id="59539-113">localeInfo</span></span>](../resources/localeinfo.md) | <span data-ttu-id="59539-114">Язык, на котором находится сообщение с автоматическим ответом.</span><span class="sxs-lookup"><span data-stu-id="59539-114">The language that the automatic reply message is in.</span></span> |
| <span data-ttu-id="59539-115">Счедуледендтиме</span><span class="sxs-lookup"><span data-stu-id="59539-115">scheduledEndTime</span></span> | [<span data-ttu-id="59539-116">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="59539-116">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md) | <span data-ttu-id="59539-117">Дата и время завершения установки автоматических ответов.</span><span class="sxs-lookup"><span data-stu-id="59539-117">The date and time that automatic replies are set to end.</span></span> |
| <span data-ttu-id="59539-118">Счедуледстарттиме</span><span class="sxs-lookup"><span data-stu-id="59539-118">scheduledStartTime</span></span> | [<span data-ttu-id="59539-119">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="59539-119">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md) | <span data-ttu-id="59539-120">Дата и время начала набора автоматических ответов.</span><span class="sxs-lookup"><span data-stu-id="59539-120">The date and time that automatic replies are set to begin.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="59539-121">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="59539-121">JSON representation</span></span>

<span data-ttu-id="59539-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="59539-122">Here is a JSON representation of the resource.</span></span>

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

---
title: Тип ресурса Аутоматикреплиесмаилтипс
description: Подсказки о любых автоматических ответах, настроенных в почтовом ящике.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 74fda9db7de1a97ce2b7e44ca9d56020b87ab6f9
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35974252"
---
# <a name="automaticrepliesmailtips-resource-type"></a><span data-ttu-id="9714a-103">Тип ресурса Аутоматикреплиесмаилтипс</span><span class="sxs-lookup"><span data-stu-id="9714a-103">automaticRepliesMailTips resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9714a-104">[Подсказки](../resources/mailtips.md) о любых автоматических ответах, настроенных в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="9714a-104">[MailTips](../resources/mailtips.md) about any automatic replies that have been set up on a mailbox.</span></span>

## <a name="properties"></a><span data-ttu-id="9714a-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="9714a-105">Properties</span></span>
| <span data-ttu-id="9714a-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="9714a-106">Property</span></span>     | <span data-ttu-id="9714a-107">Тип</span><span class="sxs-lookup"><span data-stu-id="9714a-107">Type</span></span>   |<span data-ttu-id="9714a-108">Описание</span><span class="sxs-lookup"><span data-stu-id="9714a-108">Description</span></span>|
|:-----|:-----|:-----|
| <span data-ttu-id="9714a-109">message</span><span class="sxs-lookup"><span data-stu-id="9714a-109">message</span></span> | <span data-ttu-id="9714a-110">String</span><span class="sxs-lookup"><span data-stu-id="9714a-110">String</span></span> | <span data-ttu-id="9714a-111">Сообщение автоматического ответа.</span><span class="sxs-lookup"><span data-stu-id="9714a-111">The automatic reply message.</span></span> |
| <span data-ttu-id="9714a-112">Мессажелангуаже</span><span class="sxs-lookup"><span data-stu-id="9714a-112">messageLanguage</span></span> | [<span data-ttu-id="9714a-113">localeInfo</span><span class="sxs-lookup"><span data-stu-id="9714a-113">localeInfo</span></span>](../resources/localeinfo.md) | <span data-ttu-id="9714a-114">Язык, на котором находится сообщение с автоматическим ответом.</span><span class="sxs-lookup"><span data-stu-id="9714a-114">The language that the automatic reply message is in.</span></span> |
| <span data-ttu-id="9714a-115">Счедуледендтиме</span><span class="sxs-lookup"><span data-stu-id="9714a-115">scheduledEndTime</span></span> | [<span data-ttu-id="9714a-116">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="9714a-116">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md) | <span data-ttu-id="9714a-117">Дата и время завершения установки автоматических ответов.</span><span class="sxs-lookup"><span data-stu-id="9714a-117">The date and time that automatic replies are set to end.</span></span> |
| <span data-ttu-id="9714a-118">Счедуледстарттиме</span><span class="sxs-lookup"><span data-stu-id="9714a-118">scheduledStartTime</span></span> | [<span data-ttu-id="9714a-119">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="9714a-119">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md) | <span data-ttu-id="9714a-120">Дата и время начала набора автоматических ответов.</span><span class="sxs-lookup"><span data-stu-id="9714a-120">The date and time that automatic replies are set to begin.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="9714a-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9714a-121">JSON representation</span></span>

<span data-ttu-id="9714a-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9714a-122">Here is a JSON representation of the resource.</span></span>

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

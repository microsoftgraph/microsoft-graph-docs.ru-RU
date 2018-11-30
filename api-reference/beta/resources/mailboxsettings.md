---
title: Тип ресурса mailboxSettings
description: Параметры основного параметра вошедшего пользователя.
ms.openlocfilehash: 79a01c59ec0a891c13107095a950a7cc8ae0b547
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27074877"
---
# <a name="mailboxsettings-resource-type"></a><span data-ttu-id="f8fb9-103">Тип ресурса mailboxSettings</span><span class="sxs-lookup"><span data-stu-id="f8fb9-103">mailboxSettings resource type</span></span>

> <span data-ttu-id="f8fb9-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="f8fb9-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f8fb9-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f8fb9-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f8fb9-106">Параметры основного параметра вошедшего пользователя.</span><span class="sxs-lookup"><span data-stu-id="f8fb9-106">Settings for the primary mailbox of the signed-in user.</span></span>


## <a name="properties"></a><span data-ttu-id="f8fb9-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="f8fb9-107">Properties</span></span>
| <span data-ttu-id="f8fb9-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="f8fb9-108">Property</span></span>     | <span data-ttu-id="f8fb9-109">Тип</span><span class="sxs-lookup"><span data-stu-id="f8fb9-109">Type</span></span>   |<span data-ttu-id="f8fb9-110">Описание</span><span class="sxs-lookup"><span data-stu-id="f8fb9-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f8fb9-111">archiveFolder</span><span class="sxs-lookup"><span data-stu-id="f8fb9-111">archiveFolder</span></span>|<span data-ttu-id="f8fb9-112">string</span><span class="sxs-lookup"><span data-stu-id="f8fb9-112">string</span></span>|<span data-ttu-id="f8fb9-113">Идентификатор архивной папки пользователя.</span><span class="sxs-lookup"><span data-stu-id="f8fb9-113">Folder ID of an archive folder for the user.</span></span>|
|<span data-ttu-id="f8fb9-114">automaticRepliesSetting</span><span class="sxs-lookup"><span data-stu-id="f8fb9-114">automaticRepliesSetting</span></span>|[<span data-ttu-id="f8fb9-115">automaticRepliesSetting</span><span class="sxs-lookup"><span data-stu-id="f8fb9-115">automaticRepliesSetting</span></span>](automaticrepliessetting.md)|<span data-ttu-id="f8fb9-116">Параметры конфигурации для автоматического уведомления отправителя о входящем письме с помощью сообщения от пользователя, вошедшего в систему.</span><span class="sxs-lookup"><span data-stu-id="f8fb9-116">Configuration settings to automatically notify the sender of an incoming email with a message from the signed-in user.</span></span>|
|<span data-ttu-id="f8fb9-117">language</span><span class="sxs-lookup"><span data-stu-id="f8fb9-117">language</span></span>|[<span data-ttu-id="f8fb9-118">localeInfo</span><span class="sxs-lookup"><span data-stu-id="f8fb9-118">localeInfo</span></span>](localeinfo.md)|<span data-ttu-id="f8fb9-119">Сведения о языковом стандарте пользователя, в том числе о предпочитаемом языке и стране или регионе.</span><span class="sxs-lookup"><span data-stu-id="f8fb9-119">The locale information for the user, including the preferred language and country/region.</span></span>|
|<span data-ttu-id="f8fb9-120">timeZone</span><span class="sxs-lookup"><span data-stu-id="f8fb9-120">timeZone</span></span>|<span data-ttu-id="f8fb9-121">string</span><span class="sxs-lookup"><span data-stu-id="f8fb9-121">string</span></span>|<span data-ttu-id="f8fb9-122">Часовой пояс почтового ящика пользователя по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="f8fb9-122">The default time zone for the user's mailbox.</span></span>|
|<span data-ttu-id="f8fb9-123">workingHours</span><span class="sxs-lookup"><span data-stu-id="f8fb9-123">workingHours</span></span>|[<span data-ttu-id="f8fb9-124">workingHours</span><span class="sxs-lookup"><span data-stu-id="f8fb9-124">workingHours</span></span>](workinghours.md)|<span data-ttu-id="f8fb9-125">Дни недели и часы работы пользователя в определенном часовом поясе.</span><span class="sxs-lookup"><span data-stu-id="f8fb9-125">The days of the week and hours in a specific time zone that the user works.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f8fb9-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f8fb9-126">JSON representation</span></span>

<span data-ttu-id="f8fb9-127">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f8fb9-127">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "archiveFolder"
  ],
  "@odata.type": "microsoft.graph.mailboxSettings"
}-->

```json
{
  "archiveFolder": "string",
  "automaticRepliesSetting": {"@odata.type": "microsoft.graph.automaticRepliesSetting"},
  "language": {"@odata.type": "microsoft.graph.localeInfo"},
  "timeZone": "string",
  "workingHours": {"@odata.type": "microsoft.graph.workingHours"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "mailboxSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
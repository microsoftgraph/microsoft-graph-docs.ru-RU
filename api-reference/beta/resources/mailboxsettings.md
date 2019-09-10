---
title: Тип ресурса mailboxSettings
description: Параметры основного параметра вошедшего пользователя.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 63340e1edd86ad61c48d707ef0bff685a57c3ef8
ms.sourcegitcommit: 3e7769ad097e9c34233fa5fea83afa23c34e14a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/10/2019
ms.locfileid: "36822734"
---
# <a name="mailboxsettings-resource-type"></a><span data-ttu-id="cce08-103">Тип ресурса mailboxSettings</span><span class="sxs-lookup"><span data-stu-id="cce08-103">mailboxSettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cce08-104">Параметры основного почтового ящика [пользователя](user.md).</span><span class="sxs-lookup"><span data-stu-id="cce08-104">Settings for the primary mailbox of a [user](user.md).</span></span>

<span data-ttu-id="cce08-105">Вы можете [получить](../api/user-get-mailboxsettings.md) или [Обновить](../api/user-update-mailboxsettings.md) параметры почтового ящика пользователя, запросите свойство **mailboxSettings** пользователя.</span><span class="sxs-lookup"><span data-stu-id="cce08-105">You can [get](../api/user-get-mailboxsettings.md) or [update](../api/user-update-mailboxsettings.md) a user's mailbox settings by querying the user's **mailboxSettings** property.</span></span>


## <a name="properties"></a><span data-ttu-id="cce08-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="cce08-106">Properties</span></span>
| <span data-ttu-id="cce08-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="cce08-107">Property</span></span>     | <span data-ttu-id="cce08-108">Тип</span><span class="sxs-lookup"><span data-stu-id="cce08-108">Type</span></span>   |<span data-ttu-id="cce08-109">Описание</span><span class="sxs-lookup"><span data-stu-id="cce08-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cce08-110">archiveFolder</span><span class="sxs-lookup"><span data-stu-id="cce08-110">archiveFolder</span></span>|<span data-ttu-id="cce08-111">string</span><span class="sxs-lookup"><span data-stu-id="cce08-111">string</span></span>|<span data-ttu-id="cce08-112">Идентификатор архивной папки пользователя.</span><span class="sxs-lookup"><span data-stu-id="cce08-112">Folder ID of an archive folder for the user.</span></span>|
|<span data-ttu-id="cce08-113">automaticRepliesSetting</span><span class="sxs-lookup"><span data-stu-id="cce08-113">automaticRepliesSetting</span></span>|[<span data-ttu-id="cce08-114">automaticRepliesSetting</span><span class="sxs-lookup"><span data-stu-id="cce08-114">automaticRepliesSetting</span></span>](automaticrepliessetting.md)|<span data-ttu-id="cce08-115">Параметры конфигурации для автоматического уведомления отправителя о входящем письме с помощью сообщения от пользователя, вошедшего в систему.</span><span class="sxs-lookup"><span data-stu-id="cce08-115">Configuration settings to automatically notify the sender of an incoming email with a message from the signed-in user.</span></span>|
|<span data-ttu-id="cce08-116">dateFormat</span><span class="sxs-lookup"><span data-stu-id="cce08-116">dateFormat</span></span>|<span data-ttu-id="cce08-117">string</span><span class="sxs-lookup"><span data-stu-id="cce08-117">string</span></span>|<span data-ttu-id="cce08-118">Формат даты для почтового ящика пользователя.</span><span class="sxs-lookup"><span data-stu-id="cce08-118">The date format for the user's mailbox.</span></span>|
|<span data-ttu-id="cce08-119">language</span><span class="sxs-lookup"><span data-stu-id="cce08-119">language</span></span>|[<span data-ttu-id="cce08-120">localeInfo</span><span class="sxs-lookup"><span data-stu-id="cce08-120">localeInfo</span></span>](localeinfo.md)|<span data-ttu-id="cce08-121">Сведения о языковом стандарте пользователя, в том числе о предпочитаемом языке и стране или регионе.</span><span class="sxs-lookup"><span data-stu-id="cce08-121">The locale information for the user, including the preferred language and country/region.</span></span>|
|<span data-ttu-id="cce08-122">тимеформат</span><span class="sxs-lookup"><span data-stu-id="cce08-122">timeFormat</span></span>|<span data-ttu-id="cce08-123">string</span><span class="sxs-lookup"><span data-stu-id="cce08-123">string</span></span>|<span data-ttu-id="cce08-124">Формат времени для почтового ящика пользователя.</span><span class="sxs-lookup"><span data-stu-id="cce08-124">The time format for the user's mailbox.</span></span>|
|<span data-ttu-id="cce08-125">timeZone</span><span class="sxs-lookup"><span data-stu-id="cce08-125">timeZone</span></span>|<span data-ttu-id="cce08-126">string</span><span class="sxs-lookup"><span data-stu-id="cce08-126">string</span></span>|<span data-ttu-id="cce08-127">Часовой пояс, используемый по умолчанию, для почтового ящика пользователя.</span><span class="sxs-lookup"><span data-stu-id="cce08-127">The default time zone for the user's mailbox.</span></span>|
|<span data-ttu-id="cce08-128">workingHours</span><span class="sxs-lookup"><span data-stu-id="cce08-128">workingHours</span></span>|[<span data-ttu-id="cce08-129">workingHours</span><span class="sxs-lookup"><span data-stu-id="cce08-129">workingHours</span></span>](workinghours.md)|<span data-ttu-id="cce08-130">Дни недели и часы работы пользователя в определенном часовом поясе.</span><span class="sxs-lookup"><span data-stu-id="cce08-130">The days of the week and hours in a specific time zone that the user works.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="cce08-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="cce08-131">JSON representation</span></span>

<span data-ttu-id="cce08-132">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cce08-132">Here is a JSON representation of the resource.</span></span>

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
  "dateFormat": "string",
  "language": {"@odata.type": "microsoft.graph.localeInfo"},
  "timeFormat": "string",
  "timeZone": "string",
  "workingHours": {"@odata.type": "microsoft.graph.workingHours"}
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "mailboxSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

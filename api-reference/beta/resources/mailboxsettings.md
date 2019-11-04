---
title: Тип ресурса mailboxSettings
description: Параметры основного параметра вошедшего пользователя.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 0df39f5fb94f648e8d5c5a8b0ff9a10c7a9a7efa
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939287"
---
# <a name="mailboxsettings-resource-type"></a><span data-ttu-id="9d5fd-103">Тип ресурса mailboxSettings</span><span class="sxs-lookup"><span data-stu-id="9d5fd-103">mailboxSettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9d5fd-104">Параметры основного почтового ящика [пользователя](user.md).</span><span class="sxs-lookup"><span data-stu-id="9d5fd-104">Settings for the primary mailbox of a [user](user.md).</span></span>

<span data-ttu-id="9d5fd-105">Вы можете [получить](../api/user-get-mailboxsettings.md) или [Обновить](../api/user-update-mailboxsettings.md) параметры почтового ящика пользователя, запросите свойство **mailboxSettings** пользователя.</span><span class="sxs-lookup"><span data-stu-id="9d5fd-105">You can [get](../api/user-get-mailboxsettings.md) or [update](../api/user-update-mailboxsettings.md) a user's mailbox settings by querying the user's **mailboxSettings** property.</span></span>


## <a name="properties"></a><span data-ttu-id="9d5fd-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="9d5fd-106">Properties</span></span>
| <span data-ttu-id="9d5fd-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="9d5fd-107">Property</span></span>     | <span data-ttu-id="9d5fd-108">Тип</span><span class="sxs-lookup"><span data-stu-id="9d5fd-108">Type</span></span>   |<span data-ttu-id="9d5fd-109">Описание</span><span class="sxs-lookup"><span data-stu-id="9d5fd-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9d5fd-110">archiveFolder</span><span class="sxs-lookup"><span data-stu-id="9d5fd-110">archiveFolder</span></span>|<span data-ttu-id="9d5fd-111">string</span><span class="sxs-lookup"><span data-stu-id="9d5fd-111">string</span></span>|<span data-ttu-id="9d5fd-112">Идентификатор архивной папки пользователя.</span><span class="sxs-lookup"><span data-stu-id="9d5fd-112">Folder ID of an archive folder for the user.</span></span>|
|<span data-ttu-id="9d5fd-113">automaticRepliesSetting</span><span class="sxs-lookup"><span data-stu-id="9d5fd-113">automaticRepliesSetting</span></span>|[<span data-ttu-id="9d5fd-114">automaticRepliesSetting</span><span class="sxs-lookup"><span data-stu-id="9d5fd-114">automaticRepliesSetting</span></span>](automaticrepliessetting.md)|<span data-ttu-id="9d5fd-115">Параметры конфигурации для автоматического уведомления отправителя о входящем письме с помощью сообщения от пользователя, вошедшего в систему.</span><span class="sxs-lookup"><span data-stu-id="9d5fd-115">Configuration settings to automatically notify the sender of an incoming email with a message from the signed-in user.</span></span>|
|<span data-ttu-id="9d5fd-116">dateFormat</span><span class="sxs-lookup"><span data-stu-id="9d5fd-116">dateFormat</span></span>|<span data-ttu-id="9d5fd-117">string</span><span class="sxs-lookup"><span data-stu-id="9d5fd-117">string</span></span>|<span data-ttu-id="9d5fd-118">Формат даты для почтового ящика пользователя.</span><span class="sxs-lookup"><span data-stu-id="9d5fd-118">The date format for the user's mailbox.</span></span>|
|<span data-ttu-id="9d5fd-119">делегатемитингмессажеделиверйоптионс</span><span class="sxs-lookup"><span data-stu-id="9d5fd-119">delegateMeetingMessageDeliveryOptions</span></span>|<span data-ttu-id="9d5fd-120">делегатемитингмессажеделиверйоптионс</span><span class="sxs-lookup"><span data-stu-id="9d5fd-120">delegateMeetingMessageDeliveryOptions</span></span>| <span data-ttu-id="9d5fd-121">Если у пользователя есть представитель календаря, этот параметр указывает, будут ли представитель, владелец почтового ящика или и то, и другое, получать сообщения о собраниях и ответы на приглашения.</span><span class="sxs-lookup"><span data-stu-id="9d5fd-121">If the user has a calendar delegate, this specifies whether the delegate, mailbox owner, or both receive meeting messages and meeting responses.</span></span> <span data-ttu-id="9d5fd-122">Возможные значения: `sendToDelegateAndInformationToPrincipal`, `sendToDelegateAndPrincipal`, `sendToDelegateOnly`.</span><span class="sxs-lookup"><span data-stu-id="9d5fd-122">Possible values are: `sendToDelegateAndInformationToPrincipal`, `sendToDelegateAndPrincipal`, `sendToDelegateOnly`.</span></span>|
|<span data-ttu-id="9d5fd-123">language</span><span class="sxs-lookup"><span data-stu-id="9d5fd-123">language</span></span>|[<span data-ttu-id="9d5fd-124">localeInfo</span><span class="sxs-lookup"><span data-stu-id="9d5fd-124">localeInfo</span></span>](localeinfo.md)|<span data-ttu-id="9d5fd-125">Сведения о языковом стандарте пользователя, в том числе о предпочитаемом языке и стране или регионе.</span><span class="sxs-lookup"><span data-stu-id="9d5fd-125">The locale information for the user, including the preferred language and country/region.</span></span>|
|<span data-ttu-id="9d5fd-126">тимеформат</span><span class="sxs-lookup"><span data-stu-id="9d5fd-126">timeFormat</span></span>|<span data-ttu-id="9d5fd-127">string</span><span class="sxs-lookup"><span data-stu-id="9d5fd-127">string</span></span>|<span data-ttu-id="9d5fd-128">Формат времени для почтового ящика пользователя.</span><span class="sxs-lookup"><span data-stu-id="9d5fd-128">The time format for the user's mailbox.</span></span>|
|<span data-ttu-id="9d5fd-129">timeZone</span><span class="sxs-lookup"><span data-stu-id="9d5fd-129">timeZone</span></span>|<span data-ttu-id="9d5fd-130">string</span><span class="sxs-lookup"><span data-stu-id="9d5fd-130">string</span></span>|<span data-ttu-id="9d5fd-131">Часовой пояс, используемый по умолчанию, для почтового ящика пользователя.</span><span class="sxs-lookup"><span data-stu-id="9d5fd-131">The default time zone for the user's mailbox.</span></span>|
|<span data-ttu-id="9d5fd-132">workingHours</span><span class="sxs-lookup"><span data-stu-id="9d5fd-132">workingHours</span></span>|[<span data-ttu-id="9d5fd-133">workingHours</span><span class="sxs-lookup"><span data-stu-id="9d5fd-133">workingHours</span></span>](workinghours.md)|<span data-ttu-id="9d5fd-134">Дни недели и часы работы пользователя в определенном часовом поясе.</span><span class="sxs-lookup"><span data-stu-id="9d5fd-134">The days of the week and hours in a specific time zone that the user works.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9d5fd-135">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9d5fd-135">JSON representation</span></span>

<span data-ttu-id="9d5fd-136">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9d5fd-136">Here is a JSON representation of the resource.</span></span>

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
  "delegateMeetingMessageDeliveryOptions": "String",
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

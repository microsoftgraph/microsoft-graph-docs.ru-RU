---
title: Тип ресурса mailboxSettings
description: Параметры основного параметра вошедшего пользователя.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: f6dbb44810c9469eb6ddb4dc8fd3299bb2b71e71
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522871"
---
# <a name="mailboxsettings-resource-type"></a><span data-ttu-id="59393-103">Тип ресурса mailboxSettings</span><span class="sxs-lookup"><span data-stu-id="59393-103">mailboxSettings resource type</span></span>

<span data-ttu-id="59393-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="59393-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="59393-105">Параметры основного почтового ящика [пользователя](user.md).</span><span class="sxs-lookup"><span data-stu-id="59393-105">Settings for the primary mailbox of a [user](user.md).</span></span>

<span data-ttu-id="59393-106">Вы можете [получить](../api/user-get-mailboxsettings.md) или [Обновить](../api/user-update-mailboxsettings.md) параметры почтового ящика пользователя, запросите свойство **mailboxSettings** пользователя.</span><span class="sxs-lookup"><span data-stu-id="59393-106">You can [get](../api/user-get-mailboxsettings.md) or [update](../api/user-update-mailboxsettings.md) a user's mailbox settings by querying the user's **mailboxSettings** property.</span></span>


## <a name="properties"></a><span data-ttu-id="59393-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="59393-107">Properties</span></span>
| <span data-ttu-id="59393-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="59393-108">Property</span></span>     | <span data-ttu-id="59393-109">Тип</span><span class="sxs-lookup"><span data-stu-id="59393-109">Type</span></span>   |<span data-ttu-id="59393-110">Описание</span><span class="sxs-lookup"><span data-stu-id="59393-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="59393-111">archiveFolder</span><span class="sxs-lookup"><span data-stu-id="59393-111">archiveFolder</span></span>|<span data-ttu-id="59393-112">строка</span><span class="sxs-lookup"><span data-stu-id="59393-112">string</span></span>|<span data-ttu-id="59393-113">Идентификатор архивной папки пользователя.</span><span class="sxs-lookup"><span data-stu-id="59393-113">Folder ID of an archive folder for the user.</span></span>|
|<span data-ttu-id="59393-114">automaticRepliesSetting</span><span class="sxs-lookup"><span data-stu-id="59393-114">automaticRepliesSetting</span></span>|[<span data-ttu-id="59393-115">automaticRepliesSetting</span><span class="sxs-lookup"><span data-stu-id="59393-115">automaticRepliesSetting</span></span>](automaticrepliessetting.md)|<span data-ttu-id="59393-116">Параметры конфигурации для автоматического уведомления отправителя о входящем письме с помощью сообщения от пользователя, вошедшего в систему.</span><span class="sxs-lookup"><span data-stu-id="59393-116">Configuration settings to automatically notify the sender of an incoming email with a message from the signed-in user.</span></span>|
|<span data-ttu-id="59393-117">dateFormat</span><span class="sxs-lookup"><span data-stu-id="59393-117">dateFormat</span></span>|<span data-ttu-id="59393-118">строка</span><span class="sxs-lookup"><span data-stu-id="59393-118">string</span></span>|<span data-ttu-id="59393-119">Формат даты для почтового ящика пользователя.</span><span class="sxs-lookup"><span data-stu-id="59393-119">The date format for the user's mailbox.</span></span>|
|<span data-ttu-id="59393-120">делегатемитингмессажеделиверйоптионс</span><span class="sxs-lookup"><span data-stu-id="59393-120">delegateMeetingMessageDeliveryOptions</span></span>|<span data-ttu-id="59393-121">делегатемитингмессажеделиверйоптионс</span><span class="sxs-lookup"><span data-stu-id="59393-121">delegateMeetingMessageDeliveryOptions</span></span>| <span data-ttu-id="59393-122">Если у пользователя есть представитель календаря, этот параметр указывает, будут ли представитель, владелец почтового ящика или и то, и другое, получать сообщения о собраниях и ответы на приглашения.</span><span class="sxs-lookup"><span data-stu-id="59393-122">If the user has a calendar delegate, this specifies whether the delegate, mailbox owner, or both receive meeting messages and meeting responses.</span></span> <span data-ttu-id="59393-123">Возможные значения: `sendToDelegateAndInformationToPrincipal`, `sendToDelegateAndPrincipal`, `sendToDelegateOnly`.</span><span class="sxs-lookup"><span data-stu-id="59393-123">Possible values are: `sendToDelegateAndInformationToPrincipal`, `sendToDelegateAndPrincipal`, `sendToDelegateOnly`.</span></span> <span data-ttu-id="59393-124">Значение по умолчанию: `sendToDelegateOnly`.</span><span class="sxs-lookup"><span data-stu-id="59393-124">The default is `sendToDelegateOnly`.</span></span>|
|<span data-ttu-id="59393-125">language</span><span class="sxs-lookup"><span data-stu-id="59393-125">language</span></span>|[<span data-ttu-id="59393-126">localeInfo</span><span class="sxs-lookup"><span data-stu-id="59393-126">localeInfo</span></span>](localeinfo.md)|<span data-ttu-id="59393-127">Сведения о языковом стандарте пользователя, в том числе о предпочитаемом языке и стране или регионе.</span><span class="sxs-lookup"><span data-stu-id="59393-127">The locale information for the user, including the preferred language and country/region.</span></span>|
|<span data-ttu-id="59393-128">тимеформат</span><span class="sxs-lookup"><span data-stu-id="59393-128">timeFormat</span></span>|<span data-ttu-id="59393-129">строка</span><span class="sxs-lookup"><span data-stu-id="59393-129">string</span></span>|<span data-ttu-id="59393-130">Формат времени для почтового ящика пользователя.</span><span class="sxs-lookup"><span data-stu-id="59393-130">The time format for the user's mailbox.</span></span>|
|<span data-ttu-id="59393-131">timeZone</span><span class="sxs-lookup"><span data-stu-id="59393-131">timeZone</span></span>|<span data-ttu-id="59393-132">string</span><span class="sxs-lookup"><span data-stu-id="59393-132">string</span></span>|<span data-ttu-id="59393-133">Часовой пояс, используемый по умолчанию, для почтового ящика пользователя.</span><span class="sxs-lookup"><span data-stu-id="59393-133">The default time zone for the user's mailbox.</span></span>|
|<span data-ttu-id="59393-134">workingHours</span><span class="sxs-lookup"><span data-stu-id="59393-134">workingHours</span></span>|[<span data-ttu-id="59393-135">workingHours</span><span class="sxs-lookup"><span data-stu-id="59393-135">workingHours</span></span>](workinghours.md)|<span data-ttu-id="59393-136">Дни недели и часы работы пользователя в определенном часовом поясе.</span><span class="sxs-lookup"><span data-stu-id="59393-136">The days of the week and hours in a specific time zone that the user works.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="59393-137">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="59393-137">JSON representation</span></span>

<span data-ttu-id="59393-138">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="59393-138">Here is a JSON representation of the resource.</span></span>

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

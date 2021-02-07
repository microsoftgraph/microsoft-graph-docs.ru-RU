---
title: Тип ресурса mailboxSettings
description: Параметры основного параметра вошедшего пользователя.
localization_priority: Normal
author: abheek-das
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 8f233906cb17869acabd06cee8f83739e194d7a5
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50128362"
---
# <a name="mailboxsettings-resource-type"></a><span data-ttu-id="cc283-103">Тип ресурса mailboxSettings</span><span class="sxs-lookup"><span data-stu-id="cc283-103">mailboxSettings resource type</span></span>

<span data-ttu-id="cc283-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cc283-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="cc283-105">Параметры основного почтового ящика [пользователя.](user.md)</span><span class="sxs-lookup"><span data-stu-id="cc283-105">Settings for the primary mailbox of a [user](user.md).</span></span>

<span data-ttu-id="cc283-106">Вы можете [получить](../api/user-get-mailboxsettings.md) или [обновить](../api/user-update-mailboxsettings.md) параметры почтового ящика пользователя, запросив свойство **mailboxSettings** пользователя.</span><span class="sxs-lookup"><span data-stu-id="cc283-106">You can [get](../api/user-get-mailboxsettings.md) or [update](../api/user-update-mailboxsettings.md) a user's mailbox settings by querying the user's **mailboxSettings** property.</span></span>


## <a name="properties"></a><span data-ttu-id="cc283-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="cc283-107">Properties</span></span>
| <span data-ttu-id="cc283-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="cc283-108">Property</span></span>     | <span data-ttu-id="cc283-109">Тип</span><span class="sxs-lookup"><span data-stu-id="cc283-109">Type</span></span>   |<span data-ttu-id="cc283-110">Описание</span><span class="sxs-lookup"><span data-stu-id="cc283-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cc283-111">archiveFolder</span><span class="sxs-lookup"><span data-stu-id="cc283-111">archiveFolder</span></span>|<span data-ttu-id="cc283-112">string</span><span class="sxs-lookup"><span data-stu-id="cc283-112">string</span></span>|<span data-ttu-id="cc283-113">Идентификатор архивной папки пользователя.</span><span class="sxs-lookup"><span data-stu-id="cc283-113">Folder ID of an archive folder for the user.</span></span>|
|<span data-ttu-id="cc283-114">automaticRepliesSetting</span><span class="sxs-lookup"><span data-stu-id="cc283-114">automaticRepliesSetting</span></span>|[<span data-ttu-id="cc283-115">automaticRepliesSetting</span><span class="sxs-lookup"><span data-stu-id="cc283-115">automaticRepliesSetting</span></span>](automaticrepliessetting.md)|<span data-ttu-id="cc283-116">Параметры конфигурации для автоматического уведомления отправителя о входящем письме с помощью сообщения от пользователя, вошедшего в систему.</span><span class="sxs-lookup"><span data-stu-id="cc283-116">Configuration settings to automatically notify the sender of an incoming email with a message from the signed-in user.</span></span>|
|<span data-ttu-id="cc283-117">dateFormat</span><span class="sxs-lookup"><span data-stu-id="cc283-117">dateFormat</span></span>|<span data-ttu-id="cc283-118">string</span><span class="sxs-lookup"><span data-stu-id="cc283-118">string</span></span>|<span data-ttu-id="cc283-119">Формат даты для почтового ящика пользователя.</span><span class="sxs-lookup"><span data-stu-id="cc283-119">The date format for the user's mailbox.</span></span>|
|<span data-ttu-id="cc283-120">delegateMeetingMessageDeliveryOptions</span><span class="sxs-lookup"><span data-stu-id="cc283-120">delegateMeetingMessageDeliveryOptions</span></span>|<span data-ttu-id="cc283-121">delegateMeetingMessageDeliveryOptions</span><span class="sxs-lookup"><span data-stu-id="cc283-121">delegateMeetingMessageDeliveryOptions</span></span>| <span data-ttu-id="cc283-122">Если у пользователя есть делегат календаря, это указывает, будет ли делегат, владелец почтового ящика или оба получать сообщения о собрании и ответы на них.</span><span class="sxs-lookup"><span data-stu-id="cc283-122">If the user has a calendar delegate, this specifies whether the delegate, mailbox owner, or both receive meeting messages and meeting responses.</span></span> <span data-ttu-id="cc283-123">Возможные значения: `sendToDelegateAndInformationToPrincipal`, `sendToDelegateAndPrincipal`, `sendToDelegateOnly`.</span><span class="sxs-lookup"><span data-stu-id="cc283-123">Possible values are: `sendToDelegateAndInformationToPrincipal`, `sendToDelegateAndPrincipal`, `sendToDelegateOnly`.</span></span>|
|<span data-ttu-id="cc283-124">language</span><span class="sxs-lookup"><span data-stu-id="cc283-124">language</span></span>|[<span data-ttu-id="cc283-125">localeInfo</span><span class="sxs-lookup"><span data-stu-id="cc283-125">localeInfo</span></span>](localeinfo.md)|<span data-ttu-id="cc283-126">Сведения о языковом стандарте пользователя, в том числе о предпочитаемом языке и стране или регионе.</span><span class="sxs-lookup"><span data-stu-id="cc283-126">The locale information for the user, including the preferred language and country/region.</span></span>|
|<span data-ttu-id="cc283-127">timeFormat</span><span class="sxs-lookup"><span data-stu-id="cc283-127">timeFormat</span></span>|<span data-ttu-id="cc283-128">string</span><span class="sxs-lookup"><span data-stu-id="cc283-128">string</span></span>|<span data-ttu-id="cc283-129">Формат времени для почтового ящика пользователя.</span><span class="sxs-lookup"><span data-stu-id="cc283-129">The time format for the user's mailbox.</span></span>|
|<span data-ttu-id="cc283-130">timeZone</span><span class="sxs-lookup"><span data-stu-id="cc283-130">timeZone</span></span>|<span data-ttu-id="cc283-131">string</span><span class="sxs-lookup"><span data-stu-id="cc283-131">string</span></span>|<span data-ttu-id="cc283-132">Часовой пояс, используемый по умолчанию, для почтового ящика пользователя.</span><span class="sxs-lookup"><span data-stu-id="cc283-132">The default time zone for the user's mailbox.</span></span>|
|<span data-ttu-id="cc283-133">workingHours</span><span class="sxs-lookup"><span data-stu-id="cc283-133">workingHours</span></span>|[<span data-ttu-id="cc283-134">workingHours</span><span class="sxs-lookup"><span data-stu-id="cc283-134">workingHours</span></span>](workinghours.md)|<span data-ttu-id="cc283-135">Дни недели и часы работы пользователя в определенном часовом поясе.</span><span class="sxs-lookup"><span data-stu-id="cc283-135">The days of the week and hours in a specific time zone that the user works.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="cc283-136">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="cc283-136">JSON representation</span></span>

<span data-ttu-id="cc283-137">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cc283-137">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "mailboxSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


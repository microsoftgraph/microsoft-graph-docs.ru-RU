---
title: Тип ресурса mailboxSettings
description: Параметры основного параметра вошедшего пользователя.
localization_priority: Normal
author: svpsiva
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: b8acb5e7b6fe3327121124d0a5f604a7690cb180
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43461885"
---
# <a name="mailboxsettings-resource-type"></a><span data-ttu-id="6f4cc-103">Тип ресурса mailboxSettings</span><span class="sxs-lookup"><span data-stu-id="6f4cc-103">mailboxSettings resource type</span></span>

<span data-ttu-id="6f4cc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6f4cc-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6f4cc-105">Параметры основного почтового ящика [пользователя](user.md).</span><span class="sxs-lookup"><span data-stu-id="6f4cc-105">Settings for the primary mailbox of a [user](user.md).</span></span>

<span data-ttu-id="6f4cc-106">Вы можете [получить](../api/user-get-mailboxsettings.md) или [Обновить](../api/user-update-mailboxsettings.md) параметры почтового ящика пользователя, запросите свойство **mailboxSettings** пользователя.</span><span class="sxs-lookup"><span data-stu-id="6f4cc-106">You can [get](../api/user-get-mailboxsettings.md) or [update](../api/user-update-mailboxsettings.md) a user's mailbox settings by querying the user's **mailboxSettings** property.</span></span>


## <a name="properties"></a><span data-ttu-id="6f4cc-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="6f4cc-107">Properties</span></span>
| <span data-ttu-id="6f4cc-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="6f4cc-108">Property</span></span>     | <span data-ttu-id="6f4cc-109">Тип</span><span class="sxs-lookup"><span data-stu-id="6f4cc-109">Type</span></span>   |<span data-ttu-id="6f4cc-110">Описание</span><span class="sxs-lookup"><span data-stu-id="6f4cc-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6f4cc-111">archiveFolder</span><span class="sxs-lookup"><span data-stu-id="6f4cc-111">archiveFolder</span></span>|<span data-ttu-id="6f4cc-112">string</span><span class="sxs-lookup"><span data-stu-id="6f4cc-112">string</span></span>|<span data-ttu-id="6f4cc-113">Идентификатор архивной папки пользователя.</span><span class="sxs-lookup"><span data-stu-id="6f4cc-113">Folder ID of an archive folder for the user.</span></span>|
|<span data-ttu-id="6f4cc-114">automaticRepliesSetting</span><span class="sxs-lookup"><span data-stu-id="6f4cc-114">automaticRepliesSetting</span></span>|[<span data-ttu-id="6f4cc-115">automaticRepliesSetting</span><span class="sxs-lookup"><span data-stu-id="6f4cc-115">automaticRepliesSetting</span></span>](automaticrepliessetting.md)|<span data-ttu-id="6f4cc-116">Параметры конфигурации для автоматического уведомления отправителя о входящем письме с помощью сообщения от пользователя, вошедшего в систему.</span><span class="sxs-lookup"><span data-stu-id="6f4cc-116">Configuration settings to automatically notify the sender of an incoming email with a message from the signed-in user.</span></span>|
|<span data-ttu-id="6f4cc-117">dateFormat</span><span class="sxs-lookup"><span data-stu-id="6f4cc-117">dateFormat</span></span>|<span data-ttu-id="6f4cc-118">string</span><span class="sxs-lookup"><span data-stu-id="6f4cc-118">string</span></span>|<span data-ttu-id="6f4cc-119">Формат даты для почтового ящика пользователя.</span><span class="sxs-lookup"><span data-stu-id="6f4cc-119">The date format for the user's mailbox.</span></span>|
|<span data-ttu-id="6f4cc-120">делегатемитингмессажеделиверйоптионс</span><span class="sxs-lookup"><span data-stu-id="6f4cc-120">delegateMeetingMessageDeliveryOptions</span></span>|<span data-ttu-id="6f4cc-121">делегатемитингмессажеделиверйоптионс</span><span class="sxs-lookup"><span data-stu-id="6f4cc-121">delegateMeetingMessageDeliveryOptions</span></span>| <span data-ttu-id="6f4cc-122">Если у пользователя есть представитель календаря, этот параметр указывает, будут ли представитель, владелец почтового ящика или и то, и другое, получать сообщения о собраниях и ответы на приглашения.</span><span class="sxs-lookup"><span data-stu-id="6f4cc-122">If the user has a calendar delegate, this specifies whether the delegate, mailbox owner, or both receive meeting messages and meeting responses.</span></span> <span data-ttu-id="6f4cc-123">Возможные значения: `sendToDelegateAndInformationToPrincipal`, `sendToDelegateAndPrincipal`, `sendToDelegateOnly`.</span><span class="sxs-lookup"><span data-stu-id="6f4cc-123">Possible values are: `sendToDelegateAndInformationToPrincipal`, `sendToDelegateAndPrincipal`, `sendToDelegateOnly`.</span></span>|
|<span data-ttu-id="6f4cc-124">language</span><span class="sxs-lookup"><span data-stu-id="6f4cc-124">language</span></span>|[<span data-ttu-id="6f4cc-125">localeInfo</span><span class="sxs-lookup"><span data-stu-id="6f4cc-125">localeInfo</span></span>](localeinfo.md)|<span data-ttu-id="6f4cc-126">Сведения о языковом стандарте пользователя, в том числе о предпочитаемом языке и стране или регионе.</span><span class="sxs-lookup"><span data-stu-id="6f4cc-126">The locale information for the user, including the preferred language and country/region.</span></span>|
|<span data-ttu-id="6f4cc-127">тимеформат</span><span class="sxs-lookup"><span data-stu-id="6f4cc-127">timeFormat</span></span>|<span data-ttu-id="6f4cc-128">string</span><span class="sxs-lookup"><span data-stu-id="6f4cc-128">string</span></span>|<span data-ttu-id="6f4cc-129">Формат времени для почтового ящика пользователя.</span><span class="sxs-lookup"><span data-stu-id="6f4cc-129">The time format for the user's mailbox.</span></span>|
|<span data-ttu-id="6f4cc-130">timeZone</span><span class="sxs-lookup"><span data-stu-id="6f4cc-130">timeZone</span></span>|<span data-ttu-id="6f4cc-131">string</span><span class="sxs-lookup"><span data-stu-id="6f4cc-131">string</span></span>|<span data-ttu-id="6f4cc-132">Часовой пояс, используемый по умолчанию, для почтового ящика пользователя.</span><span class="sxs-lookup"><span data-stu-id="6f4cc-132">The default time zone for the user's mailbox.</span></span>|
|<span data-ttu-id="6f4cc-133">workingHours</span><span class="sxs-lookup"><span data-stu-id="6f4cc-133">workingHours</span></span>|[<span data-ttu-id="6f4cc-134">workingHours</span><span class="sxs-lookup"><span data-stu-id="6f4cc-134">workingHours</span></span>](workinghours.md)|<span data-ttu-id="6f4cc-135">Дни недели и часы работы пользователя в определенном часовом поясе.</span><span class="sxs-lookup"><span data-stu-id="6f4cc-135">The days of the week and hours in a specific time zone that the user works.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6f4cc-136">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6f4cc-136">JSON representation</span></span>

<span data-ttu-id="6f4cc-137">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6f4cc-137">Here is a JSON representation of the resource.</span></span>

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

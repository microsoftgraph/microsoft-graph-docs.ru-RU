---
title: Тип ресурса mailboxSettings
description: Параметры основного параметра вошедшего пользователя.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 6d966ecb599d98c92bf1e70eca1f61fb665e359d
ms.sourcegitcommit: 7c017000888a910a0ad85404946f4fc50742c8d1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/01/2020
ms.locfileid: "41652046"
---
# <a name="mailboxsettings-resource-type"></a><span data-ttu-id="8b511-103">Тип ресурса mailboxSettings</span><span class="sxs-lookup"><span data-stu-id="8b511-103">mailboxSettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8b511-104">Параметры основного почтового ящика [пользователя](user.md).</span><span class="sxs-lookup"><span data-stu-id="8b511-104">Settings for the primary mailbox of a [user](user.md).</span></span>

<span data-ttu-id="8b511-105">Вы можете [получить](../api/user-get-mailboxsettings.md) или [Обновить](../api/user-update-mailboxsettings.md) параметры почтового ящика пользователя, запросите свойство **mailboxSettings** пользователя.</span><span class="sxs-lookup"><span data-stu-id="8b511-105">You can [get](../api/user-get-mailboxsettings.md) or [update](../api/user-update-mailboxsettings.md) a user's mailbox settings by querying the user's **mailboxSettings** property.</span></span>


## <a name="properties"></a><span data-ttu-id="8b511-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="8b511-106">Properties</span></span>
| <span data-ttu-id="8b511-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="8b511-107">Property</span></span>     | <span data-ttu-id="8b511-108">Тип</span><span class="sxs-lookup"><span data-stu-id="8b511-108">Type</span></span>   |<span data-ttu-id="8b511-109">Описание</span><span class="sxs-lookup"><span data-stu-id="8b511-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8b511-110">archiveFolder</span><span class="sxs-lookup"><span data-stu-id="8b511-110">archiveFolder</span></span>|<span data-ttu-id="8b511-111">string</span><span class="sxs-lookup"><span data-stu-id="8b511-111">string</span></span>|<span data-ttu-id="8b511-112">Идентификатор архивной папки пользователя.</span><span class="sxs-lookup"><span data-stu-id="8b511-112">Folder ID of an archive folder for the user.</span></span>|
|<span data-ttu-id="8b511-113">automaticRepliesSetting</span><span class="sxs-lookup"><span data-stu-id="8b511-113">automaticRepliesSetting</span></span>|[<span data-ttu-id="8b511-114">automaticRepliesSetting</span><span class="sxs-lookup"><span data-stu-id="8b511-114">automaticRepliesSetting</span></span>](automaticrepliessetting.md)|<span data-ttu-id="8b511-115">Параметры конфигурации для автоматического уведомления отправителя о входящем письме с помощью сообщения от пользователя, вошедшего в систему.</span><span class="sxs-lookup"><span data-stu-id="8b511-115">Configuration settings to automatically notify the sender of an incoming email with a message from the signed-in user.</span></span>|
|<span data-ttu-id="8b511-116">dateFormat</span><span class="sxs-lookup"><span data-stu-id="8b511-116">dateFormat</span></span>|<span data-ttu-id="8b511-117">string</span><span class="sxs-lookup"><span data-stu-id="8b511-117">string</span></span>|<span data-ttu-id="8b511-118">Формат даты для почтового ящика пользователя.</span><span class="sxs-lookup"><span data-stu-id="8b511-118">The date format for the user's mailbox.</span></span>|
|<span data-ttu-id="8b511-119">делегатемитингмессажеделиверйоптионс</span><span class="sxs-lookup"><span data-stu-id="8b511-119">delegateMeetingMessageDeliveryOptions</span></span>|<span data-ttu-id="8b511-120">делегатемитингмессажеделиверйоптионс</span><span class="sxs-lookup"><span data-stu-id="8b511-120">delegateMeetingMessageDeliveryOptions</span></span>| <span data-ttu-id="8b511-121">Если у пользователя есть представитель календаря, этот параметр указывает, будут ли представитель, владелец почтового ящика или и то, и другое, получать сообщения о собраниях и ответы на приглашения.</span><span class="sxs-lookup"><span data-stu-id="8b511-121">If the user has a calendar delegate, this specifies whether the delegate, mailbox owner, or both receive meeting messages and meeting responses.</span></span> <span data-ttu-id="8b511-122">Возможные значения: `sendToDelegateAndInformationToPrincipal`, `sendToDelegateAndPrincipal`, `sendToDelegateOnly`.</span><span class="sxs-lookup"><span data-stu-id="8b511-122">Possible values are: `sendToDelegateAndInformationToPrincipal`, `sendToDelegateAndPrincipal`, `sendToDelegateOnly`.</span></span> <span data-ttu-id="8b511-123">Значение по умолчанию: `sendToDelegateOnly`.</span><span class="sxs-lookup"><span data-stu-id="8b511-123">The default is `sendToDelegateOnly`.</span></span>|
|<span data-ttu-id="8b511-124">language</span><span class="sxs-lookup"><span data-stu-id="8b511-124">language</span></span>|[<span data-ttu-id="8b511-125">localeInfo</span><span class="sxs-lookup"><span data-stu-id="8b511-125">localeInfo</span></span>](localeinfo.md)|<span data-ttu-id="8b511-126">Сведения о языковом стандарте пользователя, в том числе о предпочитаемом языке и стране или регионе.</span><span class="sxs-lookup"><span data-stu-id="8b511-126">The locale information for the user, including the preferred language and country/region.</span></span>|
|<span data-ttu-id="8b511-127">тимеформат</span><span class="sxs-lookup"><span data-stu-id="8b511-127">timeFormat</span></span>|<span data-ttu-id="8b511-128">string</span><span class="sxs-lookup"><span data-stu-id="8b511-128">string</span></span>|<span data-ttu-id="8b511-129">Формат времени для почтового ящика пользователя.</span><span class="sxs-lookup"><span data-stu-id="8b511-129">The time format for the user's mailbox.</span></span>|
|<span data-ttu-id="8b511-130">timeZone</span><span class="sxs-lookup"><span data-stu-id="8b511-130">timeZone</span></span>|<span data-ttu-id="8b511-131">string</span><span class="sxs-lookup"><span data-stu-id="8b511-131">string</span></span>|<span data-ttu-id="8b511-132">Часовой пояс, используемый по умолчанию, для почтового ящика пользователя.</span><span class="sxs-lookup"><span data-stu-id="8b511-132">The default time zone for the user's mailbox.</span></span>|
|<span data-ttu-id="8b511-133">workingHours</span><span class="sxs-lookup"><span data-stu-id="8b511-133">workingHours</span></span>|[<span data-ttu-id="8b511-134">workingHours</span><span class="sxs-lookup"><span data-stu-id="8b511-134">workingHours</span></span>](workinghours.md)|<span data-ttu-id="8b511-135">Дни недели и часы работы пользователя в определенном часовом поясе.</span><span class="sxs-lookup"><span data-stu-id="8b511-135">The days of the week and hours in a specific time zone that the user works.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8b511-136">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8b511-136">JSON representation</span></span>

<span data-ttu-id="8b511-137">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8b511-137">Here is a JSON representation of the resource.</span></span>

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

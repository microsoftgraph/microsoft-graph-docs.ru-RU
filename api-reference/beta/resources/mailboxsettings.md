---
title: Тип ресурса mailboxSettings
description: Параметры основного параметра вошедшего пользователя.
localization_priority: Normal
author: svpsiva
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 36cc855b76b7d87d951f733fd0f84739f04aa138
ms.sourcegitcommit: b083a570375252eff8054f9fe70e1e5e2becc06d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/23/2020
ms.locfileid: "44846172"
---
# <a name="mailboxsettings-resource-type"></a><span data-ttu-id="f4945-103">Тип ресурса mailboxSettings</span><span class="sxs-lookup"><span data-stu-id="f4945-103">mailboxSettings resource type</span></span>

<span data-ttu-id="f4945-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f4945-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f4945-105">Параметры основного почтового ящика [пользователя](user.md).</span><span class="sxs-lookup"><span data-stu-id="f4945-105">Settings for the primary mailbox of a [user](user.md).</span></span>

<span data-ttu-id="f4945-106">Вы можете [получить](../api/user-get-mailboxsettings.md) или [Обновить](../api/user-update-mailboxsettings.md) параметры почтового ящика пользователя, запросите свойство **mailboxSettings** пользователя.</span><span class="sxs-lookup"><span data-stu-id="f4945-106">You can [get](../api/user-get-mailboxsettings.md) or [update](../api/user-update-mailboxsettings.md) a user's mailbox settings by querying the user's **mailboxSettings** property.</span></span>


## <a name="properties"></a><span data-ttu-id="f4945-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="f4945-107">Properties</span></span>
| <span data-ttu-id="f4945-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="f4945-108">Property</span></span>     | <span data-ttu-id="f4945-109">Тип</span><span class="sxs-lookup"><span data-stu-id="f4945-109">Type</span></span>   |<span data-ttu-id="f4945-110">Описание</span><span class="sxs-lookup"><span data-stu-id="f4945-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f4945-111">archiveFolder</span><span class="sxs-lookup"><span data-stu-id="f4945-111">archiveFolder</span></span>|<span data-ttu-id="f4945-112">string</span><span class="sxs-lookup"><span data-stu-id="f4945-112">string</span></span>|<span data-ttu-id="f4945-113">Идентификатор архивной папки пользователя.</span><span class="sxs-lookup"><span data-stu-id="f4945-113">Folder ID of an archive folder for the user.</span></span> <span data-ttu-id="f4945-114">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f4945-114">Read only.</span></span>|
|<span data-ttu-id="f4945-115">automaticRepliesSetting</span><span class="sxs-lookup"><span data-stu-id="f4945-115">automaticRepliesSetting</span></span>|[<span data-ttu-id="f4945-116">automaticRepliesSetting</span><span class="sxs-lookup"><span data-stu-id="f4945-116">automaticRepliesSetting</span></span>](automaticrepliessetting.md)|<span data-ttu-id="f4945-117">Параметры конфигурации для автоматического уведомления отправителя о входящем письме с помощью сообщения от пользователя, вошедшего в систему.</span><span class="sxs-lookup"><span data-stu-id="f4945-117">Configuration settings to automatically notify the sender of an incoming email with a message from the signed-in user.</span></span>|
|<span data-ttu-id="f4945-118">dateFormat</span><span class="sxs-lookup"><span data-stu-id="f4945-118">dateFormat</span></span>|<span data-ttu-id="f4945-119">string</span><span class="sxs-lookup"><span data-stu-id="f4945-119">string</span></span>|<span data-ttu-id="f4945-120">Формат даты для почтового ящика пользователя.</span><span class="sxs-lookup"><span data-stu-id="f4945-120">The date format for the user's mailbox.</span></span>|
|<span data-ttu-id="f4945-121">делегатемитингмессажеделиверйоптионс</span><span class="sxs-lookup"><span data-stu-id="f4945-121">delegateMeetingMessageDeliveryOptions</span></span>|<span data-ttu-id="f4945-122">делегатемитингмессажеделиверйоптионс</span><span class="sxs-lookup"><span data-stu-id="f4945-122">delegateMeetingMessageDeliveryOptions</span></span>| <span data-ttu-id="f4945-123">Если у пользователя есть представитель календаря, этот параметр указывает, будут ли представитель, владелец почтового ящика или и то, и другое, получать сообщения о собраниях и ответы на приглашения.</span><span class="sxs-lookup"><span data-stu-id="f4945-123">If the user has a calendar delegate, this specifies whether the delegate, mailbox owner, or both receive meeting messages and meeting responses.</span></span> <span data-ttu-id="f4945-124">Возможные значения: `sendToDelegateAndInformationToPrincipal`, `sendToDelegateAndPrincipal`, `sendToDelegateOnly`.</span><span class="sxs-lookup"><span data-stu-id="f4945-124">Possible values are: `sendToDelegateAndInformationToPrincipal`, `sendToDelegateAndPrincipal`, `sendToDelegateOnly`.</span></span> <span data-ttu-id="f4945-125">Значение по умолчанию: `sendToDelegateOnly` .</span><span class="sxs-lookup"><span data-stu-id="f4945-125">The default is `sendToDelegateOnly`.</span></span>|
|<span data-ttu-id="f4945-126">language</span><span class="sxs-lookup"><span data-stu-id="f4945-126">language</span></span>|[<span data-ttu-id="f4945-127">localeInfo</span><span class="sxs-lookup"><span data-stu-id="f4945-127">localeInfo</span></span>](localeinfo.md)|<span data-ttu-id="f4945-128">Сведения о языковом стандарте пользователя, в том числе о предпочитаемом языке и стране или регионе.</span><span class="sxs-lookup"><span data-stu-id="f4945-128">The locale information for the user, including the preferred language and country/region.</span></span>|
|<span data-ttu-id="f4945-129">тимеформат</span><span class="sxs-lookup"><span data-stu-id="f4945-129">timeFormat</span></span>|<span data-ttu-id="f4945-130">string</span><span class="sxs-lookup"><span data-stu-id="f4945-130">string</span></span>|<span data-ttu-id="f4945-131">Формат времени для почтового ящика пользователя.</span><span class="sxs-lookup"><span data-stu-id="f4945-131">The time format for the user's mailbox.</span></span>|
|<span data-ttu-id="f4945-132">timeZone</span><span class="sxs-lookup"><span data-stu-id="f4945-132">timeZone</span></span>|<span data-ttu-id="f4945-133">string</span><span class="sxs-lookup"><span data-stu-id="f4945-133">string</span></span>|<span data-ttu-id="f4945-134">Часовой пояс, используемый по умолчанию, для почтового ящика пользователя.</span><span class="sxs-lookup"><span data-stu-id="f4945-134">The default time zone for the user's mailbox.</span></span>|
|<span data-ttu-id="f4945-135">workingHours</span><span class="sxs-lookup"><span data-stu-id="f4945-135">workingHours</span></span>|[<span data-ttu-id="f4945-136">workingHours</span><span class="sxs-lookup"><span data-stu-id="f4945-136">workingHours</span></span>](workinghours.md)|<span data-ttu-id="f4945-137">Дни недели и часы работы пользователя в определенном часовом поясе.</span><span class="sxs-lookup"><span data-stu-id="f4945-137">The days of the week and hours in a specific time zone that the user works.</span></span>|
|<span data-ttu-id="f4945-138">усерпурпосе</span><span class="sxs-lookup"><span data-stu-id="f4945-138">userPurpose</span></span>|[<span data-ttu-id="f4945-139">усерпурпосе</span><span class="sxs-lookup"><span data-stu-id="f4945-139">userPurpose</span></span>](userpurpose.md)|<span data-ttu-id="f4945-140">Назначение почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="f4945-140">The purpose of the mailbox.</span></span> <span data-ttu-id="f4945-141">Используется для различения почтового ящика одного пользователя из общего почтового ящика и почтового ящика оборудования в Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="f4945-141">Used to differentiate a mailbox for a single user from a shared mailbox and equipment mailbox in Exchange Online.</span></span> <span data-ttu-id="f4945-142">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f4945-142">Read only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f4945-143">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f4945-143">JSON representation</span></span>

<span data-ttu-id="f4945-144">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f4945-144">Here is a JSON representation of the resource.</span></span>

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
  "workingHours": {"@odata.type": "microsoft.graph.workingHours"},
  "userPurpose": {"@odata.type": "microsoft.graph.userPurpose"}
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

---
title: Тип ресурса mailboxSettings
description: Параметры основного параметра вошедшего пользователя.
localization_priority: Normal
author: abheek-das
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 5da5e2294845fdf0aba2029acd410a59a7c0806c
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50135232"
---
# <a name="mailboxsettings-resource-type"></a><span data-ttu-id="55231-103">Тип ресурса mailboxSettings</span><span class="sxs-lookup"><span data-stu-id="55231-103">mailboxSettings resource type</span></span>

<span data-ttu-id="55231-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="55231-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="55231-105">Параметры основного почтового ящика [пользователя.](user.md)</span><span class="sxs-lookup"><span data-stu-id="55231-105">Settings for the primary mailbox of a [user](user.md).</span></span>

<span data-ttu-id="55231-106">Вы можете [получить](../api/user-get-mailboxsettings.md) или [обновить](../api/user-update-mailboxsettings.md) параметры почтового ящика пользователя, запросив свойство **mailboxSettings пользователя.**</span><span class="sxs-lookup"><span data-stu-id="55231-106">You can [get](../api/user-get-mailboxsettings.md) or [update](../api/user-update-mailboxsettings.md) a user's mailbox settings by querying the user's **mailboxSettings** property.</span></span>


## <a name="properties"></a><span data-ttu-id="55231-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="55231-107">Properties</span></span>
| <span data-ttu-id="55231-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="55231-108">Property</span></span>     | <span data-ttu-id="55231-109">Тип</span><span class="sxs-lookup"><span data-stu-id="55231-109">Type</span></span>   |<span data-ttu-id="55231-110">Описание</span><span class="sxs-lookup"><span data-stu-id="55231-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="55231-111">archiveFolder</span><span class="sxs-lookup"><span data-stu-id="55231-111">archiveFolder</span></span>|<span data-ttu-id="55231-112">string</span><span class="sxs-lookup"><span data-stu-id="55231-112">string</span></span>|<span data-ttu-id="55231-113">Идентификатор архивной папки пользователя.</span><span class="sxs-lookup"><span data-stu-id="55231-113">Folder ID of an archive folder for the user.</span></span> <span data-ttu-id="55231-114">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="55231-114">Read only.</span></span>|
|<span data-ttu-id="55231-115">automaticRepliesSetting</span><span class="sxs-lookup"><span data-stu-id="55231-115">automaticRepliesSetting</span></span>|[<span data-ttu-id="55231-116">automaticRepliesSetting</span><span class="sxs-lookup"><span data-stu-id="55231-116">automaticRepliesSetting</span></span>](automaticrepliessetting.md)|<span data-ttu-id="55231-117">Параметры конфигурации для автоматического уведомления отправителя о входящем письме с помощью сообщения от пользователя, вошедшего в систему.</span><span class="sxs-lookup"><span data-stu-id="55231-117">Configuration settings to automatically notify the sender of an incoming email with a message from the signed-in user.</span></span>|
|<span data-ttu-id="55231-118">dateFormat</span><span class="sxs-lookup"><span data-stu-id="55231-118">dateFormat</span></span>|<span data-ttu-id="55231-119">string</span><span class="sxs-lookup"><span data-stu-id="55231-119">string</span></span>|<span data-ttu-id="55231-120">Формат даты для почтового ящика пользователя.</span><span class="sxs-lookup"><span data-stu-id="55231-120">The date format for the user's mailbox.</span></span>|
|<span data-ttu-id="55231-121">delegateMeetingMessageDeliveryOptions</span><span class="sxs-lookup"><span data-stu-id="55231-121">delegateMeetingMessageDeliveryOptions</span></span>|<span data-ttu-id="55231-122">delegateMeetingMessageDeliveryOptions</span><span class="sxs-lookup"><span data-stu-id="55231-122">delegateMeetingMessageDeliveryOptions</span></span>| <span data-ttu-id="55231-123">Если у пользователя есть делегат календаря, это указывает, будет ли делегат, владелец почтового ящика или оба получать сообщения о собрании и ответы на них.</span><span class="sxs-lookup"><span data-stu-id="55231-123">If the user has a calendar delegate, this specifies whether the delegate, mailbox owner, or both receive meeting messages and meeting responses.</span></span> <span data-ttu-id="55231-124">Возможные значения: `sendToDelegateAndInformationToPrincipal`, `sendToDelegateAndPrincipal`, `sendToDelegateOnly`.</span><span class="sxs-lookup"><span data-stu-id="55231-124">Possible values are: `sendToDelegateAndInformationToPrincipal`, `sendToDelegateAndPrincipal`, `sendToDelegateOnly`.</span></span> <span data-ttu-id="55231-125">Значение по `sendToDelegateOnly` умолчанию: .</span><span class="sxs-lookup"><span data-stu-id="55231-125">The default is `sendToDelegateOnly`.</span></span>|
|<span data-ttu-id="55231-126">language</span><span class="sxs-lookup"><span data-stu-id="55231-126">language</span></span>|[<span data-ttu-id="55231-127">localeInfo</span><span class="sxs-lookup"><span data-stu-id="55231-127">localeInfo</span></span>](localeinfo.md)|<span data-ttu-id="55231-128">Сведения о языковом стандарте пользователя, в том числе о предпочитаемом языке и стране или регионе.</span><span class="sxs-lookup"><span data-stu-id="55231-128">The locale information for the user, including the preferred language and country/region.</span></span>|
|<span data-ttu-id="55231-129">timeFormat</span><span class="sxs-lookup"><span data-stu-id="55231-129">timeFormat</span></span>|<span data-ttu-id="55231-130">string</span><span class="sxs-lookup"><span data-stu-id="55231-130">string</span></span>|<span data-ttu-id="55231-131">Формат времени для почтового ящика пользователя.</span><span class="sxs-lookup"><span data-stu-id="55231-131">The time format for the user's mailbox.</span></span>|
|<span data-ttu-id="55231-132">timeZone</span><span class="sxs-lookup"><span data-stu-id="55231-132">timeZone</span></span>|<span data-ttu-id="55231-133">string</span><span class="sxs-lookup"><span data-stu-id="55231-133">string</span></span>|<span data-ttu-id="55231-134">Часовой пояс, используемый по умолчанию, для почтового ящика пользователя.</span><span class="sxs-lookup"><span data-stu-id="55231-134">The default time zone for the user's mailbox.</span></span>|
|<span data-ttu-id="55231-135">workingHours</span><span class="sxs-lookup"><span data-stu-id="55231-135">workingHours</span></span>|[<span data-ttu-id="55231-136">workingHours</span><span class="sxs-lookup"><span data-stu-id="55231-136">workingHours</span></span>](workinghours.md)|<span data-ttu-id="55231-137">Дни недели и часы работы пользователя в определенном часовом поясе.</span><span class="sxs-lookup"><span data-stu-id="55231-137">The days of the week and hours in a specific time zone that the user works.</span></span>|
|<span data-ttu-id="55231-138">userPurpose</span><span class="sxs-lookup"><span data-stu-id="55231-138">userPurpose</span></span>|[<span data-ttu-id="55231-139">userPurpose</span><span class="sxs-lookup"><span data-stu-id="55231-139">userPurpose</span></span>](userpurpose.md)|<span data-ttu-id="55231-140">Назначение почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="55231-140">The purpose of the mailbox.</span></span> <span data-ttu-id="55231-141">Используется для различения почтового ящика отдельного пользователя от общего почтового ящика и почтового ящика оборудования в Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="55231-141">Used to differentiate a mailbox for a single user from a shared mailbox and equipment mailbox in Exchange Online.</span></span> <span data-ttu-id="55231-142">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="55231-142">Read only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="55231-143">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="55231-143">JSON representation</span></span>

<span data-ttu-id="55231-144">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="55231-144">Here is a JSON representation of the resource.</span></span>

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



---
title: Тип ресурса mailboxSettings
description: Параметры основного параметра вошедшего пользователя.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 12dc1a5992146c23ac6f2858fd7ee0b3508e455a
ms.sourcegitcommit: f23cc661a0e30d01a6b59cfdae90768c55b80ae2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/08/2019
ms.locfileid: "37418302"
---
# <a name="mailboxsettings-resource-type"></a><span data-ttu-id="5d8ff-103">Тип ресурса mailboxSettings</span><span class="sxs-lookup"><span data-stu-id="5d8ff-103">mailboxSettings resource type</span></span>

<span data-ttu-id="5d8ff-104">Параметры основного почтового ящика [пользователя](user.md).</span><span class="sxs-lookup"><span data-stu-id="5d8ff-104">Settings for the primary mailbox of a [user](user.md).</span></span>

<span data-ttu-id="5d8ff-105">Вы можете [получить](../api/user-get-mailboxsettings.md) или [Обновить](../api/user-update-mailboxsettings.md) параметры почтового ящика пользователя, запросите свойство **mailboxSettings** пользователя.</span><span class="sxs-lookup"><span data-stu-id="5d8ff-105">You can [get](../api/user-get-mailboxsettings.md) or [update](../api/user-update-mailboxsettings.md) a user's mailbox settings by querying the user's **mailboxSettings** property.</span></span>


## <a name="properties"></a><span data-ttu-id="5d8ff-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="5d8ff-106">Properties</span></span>
| <span data-ttu-id="5d8ff-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="5d8ff-107">Property</span></span>     | <span data-ttu-id="5d8ff-108">Тип</span><span class="sxs-lookup"><span data-stu-id="5d8ff-108">Type</span></span>   |<span data-ttu-id="5d8ff-109">Описание</span><span class="sxs-lookup"><span data-stu-id="5d8ff-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5d8ff-110">archiveFolder</span><span class="sxs-lookup"><span data-stu-id="5d8ff-110">archiveFolder</span></span>|<span data-ttu-id="5d8ff-111">string</span><span class="sxs-lookup"><span data-stu-id="5d8ff-111">string</span></span>|<span data-ttu-id="5d8ff-112">Идентификатор архивной папки пользователя.</span><span class="sxs-lookup"><span data-stu-id="5d8ff-112">Folder ID of an archive folder for the user.</span></span>|
|<span data-ttu-id="5d8ff-113">automaticRepliesSetting</span><span class="sxs-lookup"><span data-stu-id="5d8ff-113">automaticRepliesSetting</span></span>|[<span data-ttu-id="5d8ff-114">automaticRepliesSetting</span><span class="sxs-lookup"><span data-stu-id="5d8ff-114">automaticRepliesSetting</span></span>](automaticrepliessetting.md)|<span data-ttu-id="5d8ff-115">Параметры конфигурации для автоматического уведомления отправителя о входящем письме с помощью сообщения от пользователя, вошедшего в систему.</span><span class="sxs-lookup"><span data-stu-id="5d8ff-115">Configuration settings to automatically notify the sender of an incoming email with a message from the signed-in user.</span></span>|
|<span data-ttu-id="5d8ff-116">dateFormat</span><span class="sxs-lookup"><span data-stu-id="5d8ff-116">dateFormat</span></span>|<span data-ttu-id="5d8ff-117">string</span><span class="sxs-lookup"><span data-stu-id="5d8ff-117">string</span></span>|<span data-ttu-id="5d8ff-118">Формат даты для почтового ящика пользователя.</span><span class="sxs-lookup"><span data-stu-id="5d8ff-118">The date format for the user's mailbox.</span></span>|
|<span data-ttu-id="5d8ff-119">language</span><span class="sxs-lookup"><span data-stu-id="5d8ff-119">language</span></span>|[<span data-ttu-id="5d8ff-120">localeInfo</span><span class="sxs-lookup"><span data-stu-id="5d8ff-120">localeInfo</span></span>](localeinfo.md)|<span data-ttu-id="5d8ff-121">Сведения о языковом стандарте пользователя, в том числе о предпочитаемом языке и стране или регионе.</span><span class="sxs-lookup"><span data-stu-id="5d8ff-121">The locale information for the user, including the preferred language and country/region.</span></span>|
|<span data-ttu-id="5d8ff-122">тимеформат</span><span class="sxs-lookup"><span data-stu-id="5d8ff-122">timeFormat</span></span>|<span data-ttu-id="5d8ff-123">string</span><span class="sxs-lookup"><span data-stu-id="5d8ff-123">string</span></span>|<span data-ttu-id="5d8ff-124">Формат времени для почтового ящика пользователя.</span><span class="sxs-lookup"><span data-stu-id="5d8ff-124">The time format for the user's mailbox.</span></span>|
|<span data-ttu-id="5d8ff-125">timeZone</span><span class="sxs-lookup"><span data-stu-id="5d8ff-125">timeZone</span></span>|<span data-ttu-id="5d8ff-126">string</span><span class="sxs-lookup"><span data-stu-id="5d8ff-126">string</span></span>|<span data-ttu-id="5d8ff-127">Часовой пояс, используемый по умолчанию, для почтового ящика пользователя.</span><span class="sxs-lookup"><span data-stu-id="5d8ff-127">The default time zone for the user's mailbox.</span></span>|
|<span data-ttu-id="5d8ff-128">workingHours</span><span class="sxs-lookup"><span data-stu-id="5d8ff-128">workingHours</span></span>|[<span data-ttu-id="5d8ff-129">workingHours</span><span class="sxs-lookup"><span data-stu-id="5d8ff-129">workingHours</span></span>](workinghours.md)|<span data-ttu-id="5d8ff-130">Дни недели и часы работы пользователя в определенном часовом поясе.</span><span class="sxs-lookup"><span data-stu-id="5d8ff-130">The days of the week and hours in a specific time zone that the user works.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5d8ff-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5d8ff-131">JSON representation</span></span>

<span data-ttu-id="5d8ff-132">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5d8ff-132">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "mailboxSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

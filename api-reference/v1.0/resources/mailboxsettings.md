---
title: Тип ресурса mailboxSettings
description: Параметры основного параметра вошедшего пользователя.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: a9fb455d2a67835ff1a3a10f89ee188a21e9956b
ms.sourcegitcommit: 3e7769ad097e9c34233fa5fea83afa23c34e14a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/10/2019
ms.locfileid: "36822783"
---
# <a name="mailboxsettings-resource-type"></a><span data-ttu-id="b2e3d-103">Тип ресурса mailboxSettings</span><span class="sxs-lookup"><span data-stu-id="b2e3d-103">mailboxSettings resource type</span></span>

<span data-ttu-id="b2e3d-104">Параметры основного почтового ящика [пользователя](user.md).</span><span class="sxs-lookup"><span data-stu-id="b2e3d-104">Settings for the primary mailbox of a [user](user.md).</span></span>

<span data-ttu-id="b2e3d-105">Вы можете [получить](../api/user-get-mailboxsettings.md) или [Обновить](../api/user-update-mailboxsettings.md) параметры почтового ящика пользователя, запросите свойство **mailboxSettings** пользователя.</span><span class="sxs-lookup"><span data-stu-id="b2e3d-105">You can [get](../api/user-get-mailboxsettings.md) or [update](../api/user-update-mailboxsettings.md) a user's mailbox settings by querying the user's **mailboxSettings** property.</span></span>


## <a name="properties"></a><span data-ttu-id="b2e3d-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="b2e3d-106">Properties</span></span>
| <span data-ttu-id="b2e3d-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="b2e3d-107">Property</span></span>     | <span data-ttu-id="b2e3d-108">Тип</span><span class="sxs-lookup"><span data-stu-id="b2e3d-108">Type</span></span>   |<span data-ttu-id="b2e3d-109">Описание</span><span class="sxs-lookup"><span data-stu-id="b2e3d-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b2e3d-110">archiveFolder</span><span class="sxs-lookup"><span data-stu-id="b2e3d-110">archiveFolder</span></span>|<span data-ttu-id="b2e3d-111">string</span><span class="sxs-lookup"><span data-stu-id="b2e3d-111">string</span></span>|<span data-ttu-id="b2e3d-112">Идентификатор архивной папки пользователя.</span><span class="sxs-lookup"><span data-stu-id="b2e3d-112">Folder ID of an archive folder for the user.</span></span>|
|<span data-ttu-id="b2e3d-113">automaticRepliesSetting</span><span class="sxs-lookup"><span data-stu-id="b2e3d-113">automaticRepliesSetting</span></span>|[<span data-ttu-id="b2e3d-114">automaticRepliesSetting</span><span class="sxs-lookup"><span data-stu-id="b2e3d-114">automaticRepliesSetting</span></span>](automaticrepliessetting.md)|<span data-ttu-id="b2e3d-115">Параметры конфигурации для автоматического уведомления отправителя о входящем письме с помощью сообщения от пользователя, вошедшего в систему.</span><span class="sxs-lookup"><span data-stu-id="b2e3d-115">Configuration settings to automatically notify the sender of an incoming email with a message from the signed-in user.</span></span>|
|<span data-ttu-id="b2e3d-116">language</span><span class="sxs-lookup"><span data-stu-id="b2e3d-116">language</span></span>|[<span data-ttu-id="b2e3d-117">localeInfo</span><span class="sxs-lookup"><span data-stu-id="b2e3d-117">localeInfo</span></span>](localeinfo.md)|<span data-ttu-id="b2e3d-118">Сведения о языковом стандарте пользователя, в том числе о предпочитаемом языке и стране или регионе.</span><span class="sxs-lookup"><span data-stu-id="b2e3d-118">The locale information for the user, including the preferred language and country/region.</span></span>|
|<span data-ttu-id="b2e3d-119">timeZone</span><span class="sxs-lookup"><span data-stu-id="b2e3d-119">timeZone</span></span>|<span data-ttu-id="b2e3d-120">string</span><span class="sxs-lookup"><span data-stu-id="b2e3d-120">string</span></span>|<span data-ttu-id="b2e3d-121">Часовой пояс, используемый по умолчанию, для почтового ящика пользователя.</span><span class="sxs-lookup"><span data-stu-id="b2e3d-121">The default time zone for the user's mailbox.</span></span>|
|<span data-ttu-id="b2e3d-122">workingHours</span><span class="sxs-lookup"><span data-stu-id="b2e3d-122">workingHours</span></span>|[<span data-ttu-id="b2e3d-123">workingHours</span><span class="sxs-lookup"><span data-stu-id="b2e3d-123">workingHours</span></span>](workinghours.md)|<span data-ttu-id="b2e3d-124">Дни недели и часы работы пользователя в определенном часовом поясе.</span><span class="sxs-lookup"><span data-stu-id="b2e3d-124">The days of the week and hours in a specific time zone that the user works.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b2e3d-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b2e3d-125">JSON representation</span></span>

<span data-ttu-id="b2e3d-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b2e3d-126">Here is a JSON representation of the resource.</span></span>

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

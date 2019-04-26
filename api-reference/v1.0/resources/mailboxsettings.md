---
title: Тип ресурса mailboxSettings
description: Параметры основного параметра вошедшего пользователя.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 53ded2d60161d833f70a3b747e0ec35953d5bd39
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32574000"
---
# <a name="mailboxsettings-resource-type"></a><span data-ttu-id="4bc08-103">Тип ресурса mailboxSettings</span><span class="sxs-lookup"><span data-stu-id="4bc08-103">mailboxSettings resource type</span></span>

<span data-ttu-id="4bc08-104">Параметры основного параметра вошедшего пользователя.</span><span class="sxs-lookup"><span data-stu-id="4bc08-104">Settings for the primary mailbox of the signed-in user.</span></span>


## <a name="properties"></a><span data-ttu-id="4bc08-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="4bc08-105">Properties</span></span>
| <span data-ttu-id="4bc08-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="4bc08-106">Property</span></span>     | <span data-ttu-id="4bc08-107">Тип</span><span class="sxs-lookup"><span data-stu-id="4bc08-107">Type</span></span>   |<span data-ttu-id="4bc08-108">Описание</span><span class="sxs-lookup"><span data-stu-id="4bc08-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4bc08-109">archiveFolder</span><span class="sxs-lookup"><span data-stu-id="4bc08-109">archiveFolder</span></span>|<span data-ttu-id="4bc08-110">string</span><span class="sxs-lookup"><span data-stu-id="4bc08-110">string</span></span>|<span data-ttu-id="4bc08-111">Идентификатор архивной папки пользователя.</span><span class="sxs-lookup"><span data-stu-id="4bc08-111">Folder ID of an archive folder for the user.</span></span>|
|<span data-ttu-id="4bc08-112">automaticRepliesSetting</span><span class="sxs-lookup"><span data-stu-id="4bc08-112">automaticRepliesSetting</span></span>|[<span data-ttu-id="4bc08-113">automaticRepliesSetting</span><span class="sxs-lookup"><span data-stu-id="4bc08-113">automaticRepliesSetting</span></span>](automaticrepliessetting.md)|<span data-ttu-id="4bc08-114">Параметры конфигурации для автоматического уведомления отправителя о входящем письме с помощью сообщения от пользователя, вошедшего в систему.</span><span class="sxs-lookup"><span data-stu-id="4bc08-114">Configuration settings to automatically notify the sender of an incoming email with a message from the signed-in user.</span></span>|
|<span data-ttu-id="4bc08-115">language</span><span class="sxs-lookup"><span data-stu-id="4bc08-115">language</span></span>|[<span data-ttu-id="4bc08-116">localeInfo</span><span class="sxs-lookup"><span data-stu-id="4bc08-116">localeInfo</span></span>](localeinfo.md)|<span data-ttu-id="4bc08-117">Сведения о языковом стандарте пользователя, в том числе о предпочитаемом языке и стране или регионе.</span><span class="sxs-lookup"><span data-stu-id="4bc08-117">The locale information for the user, including the preferred language and country/region.</span></span>|
|<span data-ttu-id="4bc08-118">timeZone</span><span class="sxs-lookup"><span data-stu-id="4bc08-118">timeZone</span></span>|<span data-ttu-id="4bc08-119">string</span><span class="sxs-lookup"><span data-stu-id="4bc08-119">string</span></span>|<span data-ttu-id="4bc08-120">Часовой пояс, используемый по умолчанию, для почтового ящика пользователя.</span><span class="sxs-lookup"><span data-stu-id="4bc08-120">The default time zone for the user's mailbox.</span></span>|
|<span data-ttu-id="4bc08-121">workingHours</span><span class="sxs-lookup"><span data-stu-id="4bc08-121">workingHours</span></span>|[<span data-ttu-id="4bc08-122">workingHours</span><span class="sxs-lookup"><span data-stu-id="4bc08-122">workingHours</span></span>](workinghours.md)|<span data-ttu-id="4bc08-123">Дни недели и часы работы пользователя в определенном часовом поясе.</span><span class="sxs-lookup"><span data-stu-id="4bc08-123">The days of the week and hours in a specific time zone that the user works.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4bc08-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4bc08-124">JSON representation</span></span>

<span data-ttu-id="4bc08-125">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4bc08-125">Here is a JSON representation of the resource.</span></span>

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

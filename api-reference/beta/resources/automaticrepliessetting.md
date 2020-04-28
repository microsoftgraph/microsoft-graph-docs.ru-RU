---
title: Тип ресурса automaticRepliesSetting
description: 'Параметры конфигурации для автоматического уведомления отправителя о входящих сообщениях электронной почты с сообщением из '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 5058f734eb2f477b1a9cdd917d00429a2b551deb
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508068"
---
# <a name="automaticrepliessetting-resource-type"></a><span data-ttu-id="d71ab-103">Тип ресурса automaticRepliesSetting</span><span class="sxs-lookup"><span data-stu-id="d71ab-103">automaticRepliesSetting resource type</span></span>

<span data-ttu-id="d71ab-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d71ab-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d71ab-p101">Параметры для настройки автоматического уведомления отправителя письма с помощью сообщения от пользователя, выполнившего вход. Например, для отправки автоматического ответа с уведомлением о том, что пользователь, выполнивший вход, не может отвечать на электронные сообщения.</span><span class="sxs-lookup"><span data-stu-id="d71ab-p101">Configuration settings to automatically notify the sender of an incoming email with a message from the signed-in user. For example, an automatic reply to notify that the signed-in user is unavailable to respond to emails.</span></span> 


## <a name="properties"></a><span data-ttu-id="d71ab-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="d71ab-107">Properties</span></span>
| <span data-ttu-id="d71ab-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="d71ab-108">Property</span></span>     | <span data-ttu-id="d71ab-109">Тип</span><span class="sxs-lookup"><span data-stu-id="d71ab-109">Type</span></span>   |<span data-ttu-id="d71ab-110">Описание</span><span class="sxs-lookup"><span data-stu-id="d71ab-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d71ab-111">екстерналаудиенце</span><span class="sxs-lookup"><span data-stu-id="d71ab-111">externalAudience</span></span>|<span data-ttu-id="d71ab-112">String</span><span class="sxs-lookup"><span data-stu-id="d71ab-112">String</span></span>| <span data-ttu-id="d71ab-p102">Внешняя аудитория по отношению к организации пользователя, выполнившего вход, которая получит сообщение **ExternalReplyMessage**, если для параметра **Status** задано значение `AlwaysEnabled` или `Scheduled`. Возможные значения: `none`, `contactsOnly`, `all`.</span><span class="sxs-lookup"><span data-stu-id="d71ab-p102">The set of audience external to the signed-in user's organization who will receive the **ExternalReplyMessage**, if **Status** is `AlwaysEnabled` or `Scheduled`. Possible values are: `none`, `contactsOnly`, `all`.</span></span>|
|<span data-ttu-id="d71ab-115">екстерналреплимессаже</span><span class="sxs-lookup"><span data-stu-id="d71ab-115">externalReplyMessage</span></span>|<span data-ttu-id="d71ab-116">string</span><span class="sxs-lookup"><span data-stu-id="d71ab-116">string</span></span>|<span data-ttu-id="d71ab-117">Автоматический ответ, который нужно отправить указанной внешней аудитории, если для параметра **Status** задано значение `AlwaysEnabled` или `Scheduled`.</span><span class="sxs-lookup"><span data-stu-id="d71ab-117">The automatic reply to send to the specified external audience, if **Status** is `AlwaysEnabled` or `Scheduled`.</span></span>|
|<span data-ttu-id="d71ab-118">интерналреплимессаже</span><span class="sxs-lookup"><span data-stu-id="d71ab-118">internalReplyMessage</span></span>|<span data-ttu-id="d71ab-119">string</span><span class="sxs-lookup"><span data-stu-id="d71ab-119">string</span></span>|<span data-ttu-id="d71ab-120">Автоматический ответ, который нужно отправить сотрудникам организации пользователя, выполнившего вход, если для параметра **Status** задано значение `AlwaysEnabled` или `Scheduled`.</span><span class="sxs-lookup"><span data-stu-id="d71ab-120">The automatic reply to send to the audience internal to the signed-in user's organization, if **Status** is `AlwaysEnabled` or `Scheduled`.</span></span> |
|<span data-ttu-id="d71ab-121">scheduledEndDateTime</span><span class="sxs-lookup"><span data-stu-id="d71ab-121">scheduledEndDateTime</span></span>|[<span data-ttu-id="d71ab-122">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="d71ab-122">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="d71ab-123">Дата и время завершения отправки автоматических ответов, если для параметра **Status** установлено значение `Scheduled`.</span><span class="sxs-lookup"><span data-stu-id="d71ab-123">The date and time that automatic replies are set to end, if **Status** is set to `Scheduled`.</span></span> |
|<span data-ttu-id="d71ab-124">scheduledStartDateTime</span><span class="sxs-lookup"><span data-stu-id="d71ab-124">scheduledStartDateTime</span></span>|[<span data-ttu-id="d71ab-125">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="d71ab-125">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="d71ab-126">Дата и время начала отправки автоматических ответов, если для параметра **Status** установлено значение `Scheduled`.</span><span class="sxs-lookup"><span data-stu-id="d71ab-126">The date and time that automatic replies are set to begin, if **Status** is set to `Scheduled`.</span></span>|
|<span data-ttu-id="d71ab-127">status</span><span class="sxs-lookup"><span data-stu-id="d71ab-127">status</span></span>|<span data-ttu-id="d71ab-128">String</span><span class="sxs-lookup"><span data-stu-id="d71ab-128">String</span></span>|<span data-ttu-id="d71ab-p103">Состояние настройки автоматических ответов. Возможные значения: `disabled`, `alwaysEnabled`, `scheduled`.</span><span class="sxs-lookup"><span data-stu-id="d71ab-p103">Configurations status for automatic replies. Possible values are: `disabled`, `alwaysEnabled`, `scheduled`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d71ab-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d71ab-131">JSON representation</span></span>

<span data-ttu-id="d71ab-132">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d71ab-132">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.automaticRepliesSetting"
}-->

```json
{
  "externalAudience": "String",
  "externalReplyMessage": "string",
  "internalReplyMessage": "string",
  "scheduledEndDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "scheduledStartDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "status": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "automaticRepliesSetting resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

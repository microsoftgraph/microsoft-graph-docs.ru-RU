---
title: Тип ресурса automaticRepliesSetting
description: 'Параметры конфигурации для автоматического уведомления отправитель входящего сообщения электронной почты с сообщением от '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: abheek-das
ms.openlocfilehash: 0d030549c242e0d6932c1f7a19a76ef515ef2956
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50136957"
---
# <a name="automaticrepliessetting-resource-type"></a><span data-ttu-id="7b62f-103">Тип ресурса automaticRepliesSetting</span><span class="sxs-lookup"><span data-stu-id="7b62f-103">automaticRepliesSetting resource type</span></span>

<span data-ttu-id="7b62f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7b62f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7b62f-p101">Параметры для настройки автоматического уведомления отправителя письма с помощью сообщения от пользователя, выполнившего вход. Например, для отправки автоматического ответа с уведомлением о том, что пользователь, выполнивший вход, не может отвечать на электронные сообщения.</span><span class="sxs-lookup"><span data-stu-id="7b62f-p101">Configuration settings to automatically notify the sender of an incoming email with a message from the signed-in user. For example, an automatic reply to notify that the signed-in user is unavailable to respond to emails.</span></span>


## <a name="properties"></a><span data-ttu-id="7b62f-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="7b62f-107">Properties</span></span>
| <span data-ttu-id="7b62f-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="7b62f-108">Property</span></span>     | <span data-ttu-id="7b62f-109">Тип</span><span class="sxs-lookup"><span data-stu-id="7b62f-109">Type</span></span>   |<span data-ttu-id="7b62f-110">Описание</span><span class="sxs-lookup"><span data-stu-id="7b62f-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7b62f-111">externalAudience</span><span class="sxs-lookup"><span data-stu-id="7b62f-111">externalAudience</span></span>|<span data-ttu-id="7b62f-112">String</span><span class="sxs-lookup"><span data-stu-id="7b62f-112">String</span></span>| <span data-ttu-id="7b62f-p102">Внешняя аудитория по отношению к организации пользователя, выполнившего вход, которая получит сообщение **ExternalReplyMessage**, если для параметра **Status** задано значение `AlwaysEnabled` или `Scheduled`. Возможные значения: `none`, `contactsOnly`, `all`.</span><span class="sxs-lookup"><span data-stu-id="7b62f-p102">The set of audience external to the signed-in user's organization who will receive the **ExternalReplyMessage**, if **Status** is `AlwaysEnabled` or `Scheduled`. Possible values are: `none`, `contactsOnly`, `all`.</span></span>|
|<span data-ttu-id="7b62f-115">externalReplyMessage</span><span class="sxs-lookup"><span data-stu-id="7b62f-115">externalReplyMessage</span></span>|<span data-ttu-id="7b62f-116">string</span><span class="sxs-lookup"><span data-stu-id="7b62f-116">string</span></span>|<span data-ttu-id="7b62f-117">Автоматический ответ, который нужно отправить указанной внешней аудитории, если для параметра **Status** задано значение `AlwaysEnabled` или `Scheduled`.</span><span class="sxs-lookup"><span data-stu-id="7b62f-117">The automatic reply to send to the specified external audience, if **Status** is `AlwaysEnabled` or `Scheduled`.</span></span>|
|<span data-ttu-id="7b62f-118">internalReplyMessage</span><span class="sxs-lookup"><span data-stu-id="7b62f-118">internalReplyMessage</span></span>|<span data-ttu-id="7b62f-119">string</span><span class="sxs-lookup"><span data-stu-id="7b62f-119">string</span></span>|<span data-ttu-id="7b62f-120">Автоматический ответ, который нужно отправить сотрудникам организации пользователя, выполнившего вход, если для параметра **Status** задано значение `AlwaysEnabled` или `Scheduled`.</span><span class="sxs-lookup"><span data-stu-id="7b62f-120">The automatic reply to send to the audience internal to the signed-in user's organization, if **Status** is `AlwaysEnabled` or `Scheduled`.</span></span> |
|<span data-ttu-id="7b62f-121">scheduledEndDateTime</span><span class="sxs-lookup"><span data-stu-id="7b62f-121">scheduledEndDateTime</span></span>|[<span data-ttu-id="7b62f-122">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="7b62f-122">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="7b62f-123">Дата и время завершения отправки автоматических ответов, если для параметра **Status** установлено значение `Scheduled`.</span><span class="sxs-lookup"><span data-stu-id="7b62f-123">The date and time that automatic replies are set to end, if **Status** is set to `Scheduled`.</span></span> |
|<span data-ttu-id="7b62f-124">scheduledStartDateTime</span><span class="sxs-lookup"><span data-stu-id="7b62f-124">scheduledStartDateTime</span></span>|[<span data-ttu-id="7b62f-125">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="7b62f-125">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="7b62f-126">Дата и время начала отправки автоматических ответов, если для параметра **Status** установлено значение `Scheduled`.</span><span class="sxs-lookup"><span data-stu-id="7b62f-126">The date and time that automatic replies are set to begin, if **Status** is set to `Scheduled`.</span></span>|
|<span data-ttu-id="7b62f-127">status</span><span class="sxs-lookup"><span data-stu-id="7b62f-127">status</span></span>|<span data-ttu-id="7b62f-128">String</span><span class="sxs-lookup"><span data-stu-id="7b62f-128">String</span></span>|<span data-ttu-id="7b62f-p103">Состояние настройки автоматических ответов. Возможные значения: `disabled`, `alwaysEnabled`, `scheduled`.</span><span class="sxs-lookup"><span data-stu-id="7b62f-p103">Configurations status for automatic replies. Possible values are: `disabled`, `alwaysEnabled`, `scheduled`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7b62f-131">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="7b62f-131">JSON representation</span></span>

<span data-ttu-id="7b62f-132">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7b62f-132">Here is a JSON representation of the resource.</span></span>

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



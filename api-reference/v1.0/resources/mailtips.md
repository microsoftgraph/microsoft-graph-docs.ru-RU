---
title: Тип ресурса подсказок
description: 'Информационные сообщения о получателе, отображаемых для пользователей, хотя они составлять сообщение. Например сообщение об отсутствии '
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: d1ee1af2ae5b62d085942615ae0bd3ec320b19b3
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27951805"
---
# <a name="mailtips-resource-type"></a><span data-ttu-id="696c7-104">Тип ресурса подсказок</span><span class="sxs-lookup"><span data-stu-id="696c7-104">mailTips resource type</span></span>

<span data-ttu-id="696c7-105">Информационные сообщения о получателе, отображаемых для пользователей, хотя они составлять сообщение.</span><span class="sxs-lookup"><span data-stu-id="696c7-105">Informative messages about a recipient, that are displayed to users while they are composing a message.</span></span> <span data-ttu-id="696c7-106">Например отсутствии сообщение как автоматического ответа для получателя сообщения.</span><span class="sxs-lookup"><span data-stu-id="696c7-106">For example, an out-of-office message as an automatic reply for a message recipient.</span></span>


## <a name="properties"></a><span data-ttu-id="696c7-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="696c7-107">Properties</span></span>
| <span data-ttu-id="696c7-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="696c7-108">Property</span></span>     | <span data-ttu-id="696c7-109">Тип</span><span class="sxs-lookup"><span data-stu-id="696c7-109">Type</span></span>   |<span data-ttu-id="696c7-110">Описание</span><span class="sxs-lookup"><span data-stu-id="696c7-110">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="696c7-111">automaticReplies</span><span class="sxs-lookup"><span data-stu-id="696c7-111">automaticReplies</span></span> | [<span data-ttu-id="696c7-112">automaticRepliesMailTips</span><span class="sxs-lookup"><span data-stu-id="696c7-112">automaticRepliesMailTips</span></span>](../resources/automaticrepliesmailtips.md) | <span data-ttu-id="696c7-113">Почтовые подсказки для автоматического ответа, если она была настроена для получателя.</span><span class="sxs-lookup"><span data-stu-id="696c7-113">Mail tips for automatic reply if it has been set up by the recipient.</span></span> |
| <span data-ttu-id="696c7-114">customMailTip</span><span class="sxs-lookup"><span data-stu-id="696c7-114">customMailTip</span></span> | <span data-ttu-id="696c7-115">Строка</span><span class="sxs-lookup"><span data-stu-id="696c7-115">String</span></span> | <span data-ttu-id="696c7-116">Совет настраиваемых почты, который может устанавливаться на почтовый ящик получателя.</span><span class="sxs-lookup"><span data-stu-id="696c7-116">A custom mail tip that can be set on the recipient's mailbox.</span></span> |
| <span data-ttu-id="696c7-117">deliveryRestricted</span><span class="sxs-lookup"><span data-stu-id="696c7-117">deliveryRestricted</span></span>| <span data-ttu-id="696c7-118">Логический</span><span class="sxs-lookup"><span data-stu-id="696c7-118">Boolean</span></span> | <span data-ttu-id="696c7-119">Ли почтовый ящик получателя restricted, например, прием сообщений только в стандартном списке отправителей, отклонение сообщения из предварительно заданных списка отправителей или принимать сообщения от только проверенных.</span><span class="sxs-lookup"><span data-stu-id="696c7-119">Whether the recipient's mailbox is restricted, for example, accepting messages from only a predefined list of senders, rejecting messages from a predefined list of senders, or accepting messages from only authenticated senders.</span></span> |
| <span data-ttu-id="696c7-120">emailAddress</span><span class="sxs-lookup"><span data-stu-id="696c7-120">emailAddress</span></span> | [<span data-ttu-id="696c7-121">emailAddress</span><span class="sxs-lookup"><span data-stu-id="696c7-121">emailAddress</span></span>](../resources/emailaddress.md) | <span data-ttu-id="696c7-122">Адрес электронной почты для получения подсказки для получателя.</span><span class="sxs-lookup"><span data-stu-id="696c7-122">The email address of the recipient to get mailtips for.</span></span> |
| <span data-ttu-id="696c7-123">error</span><span class="sxs-lookup"><span data-stu-id="696c7-123">error</span></span> | [<span data-ttu-id="696c7-124">mailTipsError</span><span class="sxs-lookup"><span data-stu-id="696c7-124">mailTipsError</span></span>](../resources/mailtipserror.md) | <span data-ttu-id="696c7-125">Ошибки, возникающие во время действия [getMailTips](../api/user-getmailtips.md) .</span><span class="sxs-lookup"><span data-stu-id="696c7-125">Errors that occur during the [getMailTips](../api/user-getmailtips.md) action.</span></span> |
| <span data-ttu-id="696c7-126">externalMemberCount</span><span class="sxs-lookup"><span data-stu-id="696c7-126">externalMemberCount</span></span> | <span data-ttu-id="696c7-127">Int32</span><span class="sxs-lookup"><span data-stu-id="696c7-127">Int32</span></span> | <span data-ttu-id="696c7-128">Число внешних участников, если получатель является списком рассылки.</span><span class="sxs-lookup"><span data-stu-id="696c7-128">The number of external members if the recipient is a distribution list.</span></span> |
| <span data-ttu-id="696c7-129">isModerated</span><span class="sxs-lookup"><span data-stu-id="696c7-129">isModerated</span></span> |<span data-ttu-id="696c7-130">Логический</span><span class="sxs-lookup"><span data-stu-id="696c7-130">Boolean</span></span>  | <span data-ttu-id="696c7-131">Отправка сообщений получателю, требуется ли утверждение.</span><span class="sxs-lookup"><span data-stu-id="696c7-131">Whether sending messages to the recipient requires approval.</span></span> <span data-ttu-id="696c7-132">Например если получатель является большой список рассылки и модератор установлен до утверждать сообщений, отправленных в этот список рассылки, или если отправка сообщений получателя требует утверждения руководителем получателя.</span><span class="sxs-lookup"><span data-stu-id="696c7-132">For example, if the recipient is a large distribution list and a moderator has been set up to approve messages sent to that distribution list, or if sending messages to a recipient requires approval of the recipient's manager.</span></span> |
| <span data-ttu-id="696c7-133">mailboxFull</span><span class="sxs-lookup"><span data-stu-id="696c7-133">mailboxFull</span></span> | <span data-ttu-id="696c7-134">Логический</span><span class="sxs-lookup"><span data-stu-id="696c7-134">Boolean</span></span> | <span data-ttu-id="696c7-135">Состояние полный почтовый ящик получателя.</span><span class="sxs-lookup"><span data-stu-id="696c7-135">The mailbox full status of the recipient.</span></span> |
| <span data-ttu-id="696c7-136">maxMessageSize</span><span class="sxs-lookup"><span data-stu-id="696c7-136">maxMessageSize</span></span> | <span data-ttu-id="696c7-137">Int32</span><span class="sxs-lookup"><span data-stu-id="696c7-137">Int32</span></span> | <span data-ttu-id="696c7-138">Максимальный размер сообщения, настроенного для организации или почтовый ящик получателя.</span><span class="sxs-lookup"><span data-stu-id="696c7-138">The maximum message size that has been configured for the recipient's organization or mailbox.</span></span> |
| <span data-ttu-id="696c7-139">recipientScope</span><span class="sxs-lookup"><span data-stu-id="696c7-139">recipientScope</span></span> | <span data-ttu-id="696c7-140">recipientScopeType</span><span class="sxs-lookup"><span data-stu-id="696c7-140">recipientScopeType</span></span> | <span data-ttu-id="696c7-141">Область получателя.</span><span class="sxs-lookup"><span data-stu-id="696c7-141">The scope of the recipient.</span></span> <span data-ttu-id="696c7-142">Возможные значения: `none`, `internal`, `external`, `externalPartner`, `externalNonParther`.</span><span class="sxs-lookup"><span data-stu-id="696c7-142">Possible values are: `none`, `internal`, `external`, `externalPartner`, `externalNonParther`.</span></span> <span data-ttu-id="696c7-143">Например администратор может установить другой организации, чтобы быть «партнер».</span><span class="sxs-lookup"><span data-stu-id="696c7-143">For example, an administrator can set another organization to be its "partner".</span></span> <span data-ttu-id="696c7-144">Область полезен в том случае, если администратор хочет определенных подсказки необходимо сделать доступным для определенных областей.</span><span class="sxs-lookup"><span data-stu-id="696c7-144">The scope is useful if an administrator wants certain mailtips to be accessible to certain scopes.</span></span> <span data-ttu-id="696c7-145">Также полезно для отправителей, информирующее о том, что сообщение может привести к организации, помогая им подкорректировать формулировки, тонового сигнала и контент.</span><span class="sxs-lookup"><span data-stu-id="696c7-145">It's also useful to senders to inform them that their message may leave the organization, helping them make the correct decisions about wording, tone and content.</span></span>|
| <span data-ttu-id="696c7-146">recipientSuggestions</span><span class="sxs-lookup"><span data-stu-id="696c7-146">recipientSuggestions</span></span> | <span data-ttu-id="696c7-147">Коллекция [recipient](../resources/recipient.md)</span><span class="sxs-lookup"><span data-stu-id="696c7-147">[recipient](../resources/recipient.md) collection</span></span> | <span data-ttu-id="696c7-148">Получатели предложенных на основе предыдущих контекстах, где они отображаются в то же сообщение.</span><span class="sxs-lookup"><span data-stu-id="696c7-148">Recipients suggested based on previous contexts where they appear in the same message.</span></span> |
| <span data-ttu-id="696c7-149">totalMemberCount</span><span class="sxs-lookup"><span data-stu-id="696c7-149">totalMemberCount</span></span> | <span data-ttu-id="696c7-150">Int32</span><span class="sxs-lookup"><span data-stu-id="696c7-150">Int32</span></span> | <span data-ttu-id="696c7-151">Число участников, если получатель является списком рассылки.</span><span class="sxs-lookup"><span data-stu-id="696c7-151">The number of members if the recipient is a distribution list.</span></span> |

### <a name="recipientscopetype-values"></a><span data-ttu-id="696c7-152">recipientScopeType значения</span><span class="sxs-lookup"><span data-stu-id="696c7-152">recipientScopeType values</span></span>

| <span data-ttu-id="696c7-153">Значение</span><span class="sxs-lookup"><span data-stu-id="696c7-153">Value</span></span>
|:-------------------------
| <span data-ttu-id="696c7-154">Нет</span><span class="sxs-lookup"><span data-stu-id="696c7-154">none</span></span>
| <span data-ttu-id="696c7-155">Внутренний</span><span class="sxs-lookup"><span data-stu-id="696c7-155">internal</span></span>
| <span data-ttu-id="696c7-156">внешние</span><span class="sxs-lookup"><span data-stu-id="696c7-156">external</span></span>
| <span data-ttu-id="696c7-157">externalPartner</span><span class="sxs-lookup"><span data-stu-id="696c7-157">externalPartner</span></span>
| <span data-ttu-id="696c7-158">externalnonpartner по отношению</span><span class="sxs-lookup"><span data-stu-id="696c7-158">externalNonPartner</span></span>


## <a name="json-representation"></a><span data-ttu-id="696c7-159">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="696c7-159">JSON representation</span></span>

<span data-ttu-id="696c7-160">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="696c7-160">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "automaticReplies",
    "customMailTip",
    "deliveryRestricted",
    "emailAddress",
    "error",
    "externalMemberCount",
    "isModerated",
    "mailboxFull",
    "maxMessageSize",
    "recipientScope",
    "recipientSuggestions",
    "totalMemberCount"
  ],
  "@odata.type": "microsoft.graph.mailTips"
}-->

```json
{
  "automaticReplies": {"@odata.type": "microsoft.graph.automaticRepliesMailTips"},
  "customMailTip": "string",
  "deliveryRestricted": "boolean",
  "emailAddress": {"@odata.type": "microsoft.graph.emailAddress"},
  "error": {"@odata.type": "microsoft.graph.mailTipsError"},
  "externalMemberCount": 1024,
  "isModerated": "boolean",
  "mailboxFull": "boolean",
  "maxMessageSize": 1024,
  "recipientScope": "string",
  "recipientSuggestions": [{"@odata.type": "microsoft.graph.recipient"}],
  "totalMemberCount": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "mailtips resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

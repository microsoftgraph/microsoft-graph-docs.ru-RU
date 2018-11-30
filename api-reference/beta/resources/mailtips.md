---
title: Тип ресурса подсказок
description: 'Информационные сообщения о получателе, отображаемых для пользователей, хотя они составлять сообщение. Например сообщение об отсутствии '
ms.openlocfilehash: a8686f256301317af5b02388052c6ccb02e81f69
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27081364"
---
# <a name="mailtips-resource-type"></a><span data-ttu-id="97b0f-104">Тип ресурса подсказок</span><span class="sxs-lookup"><span data-stu-id="97b0f-104">mailTips resource type</span></span>

> <span data-ttu-id="97b0f-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="97b0f-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="97b0f-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="97b0f-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="97b0f-107">Информационные сообщения о получателе, отображаемых для пользователей, хотя они составлять сообщение.</span><span class="sxs-lookup"><span data-stu-id="97b0f-107">Informative messages about a recipient, that are displayed to users while they are composing a message.</span></span> <span data-ttu-id="97b0f-108">Например отсутствии сообщение как автоматического ответа для получателя сообщения.</span><span class="sxs-lookup"><span data-stu-id="97b0f-108">For example, an out-of-office message as an automatic reply for a message recipient.</span></span>


## <a name="properties"></a><span data-ttu-id="97b0f-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="97b0f-109">Properties</span></span>
| <span data-ttu-id="97b0f-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="97b0f-110">Property</span></span>     | <span data-ttu-id="97b0f-111">Тип</span><span class="sxs-lookup"><span data-stu-id="97b0f-111">Type</span></span>   |<span data-ttu-id="97b0f-112">Description</span><span class="sxs-lookup"><span data-stu-id="97b0f-112">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="97b0f-113">automaticReplies</span><span class="sxs-lookup"><span data-stu-id="97b0f-113">automaticReplies</span></span> | [<span data-ttu-id="97b0f-114">automaticRepliesMailTips</span><span class="sxs-lookup"><span data-stu-id="97b0f-114">automaticRepliesMailTips</span></span>](../resources/automaticrepliesmailtips.md) | <span data-ttu-id="97b0f-115">Почтовые подсказки для автоматического ответа, если она была настроена для получателя.</span><span class="sxs-lookup"><span data-stu-id="97b0f-115">Mail tips for automatic reply if it has been set up by the recipient.</span></span> |
| <span data-ttu-id="97b0f-116">customMailTip</span><span class="sxs-lookup"><span data-stu-id="97b0f-116">customMailTip</span></span> | <span data-ttu-id="97b0f-117">String</span><span class="sxs-lookup"><span data-stu-id="97b0f-117">String</span></span> | <span data-ttu-id="97b0f-118">Совет настраиваемых почты, который может устанавливаться на почтовый ящик получателя.</span><span class="sxs-lookup"><span data-stu-id="97b0f-118">A custom mail tip that can be set on the recipient's mailbox.</span></span> |
| <span data-ttu-id="97b0f-119">deliveryRestricted</span><span class="sxs-lookup"><span data-stu-id="97b0f-119">deliveryRestricted</span></span>| <span data-ttu-id="97b0f-120">Логический</span><span class="sxs-lookup"><span data-stu-id="97b0f-120">Boolean</span></span> | <span data-ttu-id="97b0f-121">Ли почтовый ящик получателя restricted, например, прием сообщений только в стандартном списке отправителей, отклонение сообщения из предварительно заданных списка отправителей или принимать сообщения от только проверенных.</span><span class="sxs-lookup"><span data-stu-id="97b0f-121">Whether the recipient's mailbox is restricted, for example, accepting messages from only a predefined list of senders, rejecting messages from a predefined list of senders, or accepting messages from only authenticated senders.</span></span> |
| <span data-ttu-id="97b0f-122">emailAddress</span><span class="sxs-lookup"><span data-stu-id="97b0f-122">emailAddress</span></span> | [<span data-ttu-id="97b0f-123">emailAddress</span><span class="sxs-lookup"><span data-stu-id="97b0f-123">emailAddress</span></span>](../resources/emailaddress.md) | <span data-ttu-id="97b0f-124">Адрес электронной почты для получения подсказки для получателя.</span><span class="sxs-lookup"><span data-stu-id="97b0f-124">The email address of the recipient to get mailtips for.</span></span> |
| <span data-ttu-id="97b0f-125">error</span><span class="sxs-lookup"><span data-stu-id="97b0f-125">error</span></span> | [<span data-ttu-id="97b0f-126">mailTipsError</span><span class="sxs-lookup"><span data-stu-id="97b0f-126">mailTipsError</span></span>](../resources/mailtipserror.md) | <span data-ttu-id="97b0f-127">Ошибки, возникающие во время действия [getMailTips](../api/user-getmailtips.md) .</span><span class="sxs-lookup"><span data-stu-id="97b0f-127">Errors that occur during the [getMailTips](../api/user-getmailtips.md) action.</span></span> |
| <span data-ttu-id="97b0f-128">externalMemberCount</span><span class="sxs-lookup"><span data-stu-id="97b0f-128">externalMemberCount</span></span> | <span data-ttu-id="97b0f-129">Int32</span><span class="sxs-lookup"><span data-stu-id="97b0f-129">Int32</span></span> | <span data-ttu-id="97b0f-130">Число внешних участников, если получатель является списком рассылки.</span><span class="sxs-lookup"><span data-stu-id="97b0f-130">The number of external members if the recipient is a distribution list.</span></span> |
| <span data-ttu-id="97b0f-131">isModerated</span><span class="sxs-lookup"><span data-stu-id="97b0f-131">isModerated</span></span> |<span data-ttu-id="97b0f-132">Логический</span><span class="sxs-lookup"><span data-stu-id="97b0f-132">Boolean</span></span>  | <span data-ttu-id="97b0f-133">Отправка сообщений получателю, требуется ли утверждение.</span><span class="sxs-lookup"><span data-stu-id="97b0f-133">Whether sending messages to the recipient requires approval.</span></span> <span data-ttu-id="97b0f-134">Например если получатель является большой список рассылки и модератор установлен до утверждать сообщений, отправленных в этот список рассылки, или если отправка сообщений получателя требует утверждения руководителем получателя.</span><span class="sxs-lookup"><span data-stu-id="97b0f-134">For example, if the recipient is a large distribution list and a moderator has been set up to approve messages sent to that distribution list, or if sending messages to a recipient requires approval of the recipient's manager.</span></span> |
| <span data-ttu-id="97b0f-135">mailboxFull</span><span class="sxs-lookup"><span data-stu-id="97b0f-135">mailboxFull</span></span> | <span data-ttu-id="97b0f-136">Логический</span><span class="sxs-lookup"><span data-stu-id="97b0f-136">Boolean</span></span> | <span data-ttu-id="97b0f-137">Состояние полный почтовый ящик получателя.</span><span class="sxs-lookup"><span data-stu-id="97b0f-137">The mailbox full status of the recipient.</span></span> |
| <span data-ttu-id="97b0f-138">maxMessageSize</span><span class="sxs-lookup"><span data-stu-id="97b0f-138">maxMessageSize</span></span> | <span data-ttu-id="97b0f-139">Int32</span><span class="sxs-lookup"><span data-stu-id="97b0f-139">Int32</span></span> | <span data-ttu-id="97b0f-140">Максимальный размер сообщения, настроенного для организации или почтовый ящик получателя.</span><span class="sxs-lookup"><span data-stu-id="97b0f-140">The maximum message size that has been configured for the recipient's organization or mailbox.</span></span> |
| <span data-ttu-id="97b0f-141">recipientScope</span><span class="sxs-lookup"><span data-stu-id="97b0f-141">recipientScope</span></span> | <span data-ttu-id="97b0f-142">String</span><span class="sxs-lookup"><span data-stu-id="97b0f-142">String</span></span> | <span data-ttu-id="97b0f-143">Область получателя.</span><span class="sxs-lookup"><span data-stu-id="97b0f-143">The scope of the recipient.</span></span> <span data-ttu-id="97b0f-144">Возможные значения: `none`, `internal`, `external`, `externalPartner`, `externalNonParther`.</span><span class="sxs-lookup"><span data-stu-id="97b0f-144">Possible values are: `none`, `internal`, `external`, `externalPartner`, `externalNonParther`.</span></span> <span data-ttu-id="97b0f-145">Например администратор может установить другой организации, чтобы быть «партнер».</span><span class="sxs-lookup"><span data-stu-id="97b0f-145">For example, an administrator can set another organization to be its "partner".</span></span> <span data-ttu-id="97b0f-146">Область полезен в том случае, если администратор хочет определенных подсказки необходимо сделать доступным для определенных областей.</span><span class="sxs-lookup"><span data-stu-id="97b0f-146">The scope is useful if an administrator wants certain mailtips to be accessible to certain scopes.</span></span> <span data-ttu-id="97b0f-147">Также полезно для отправителей, информирующее о том, что сообщение может привести к организации, помогая им подкорректировать формулировки, тонового сигнала и контент.</span><span class="sxs-lookup"><span data-stu-id="97b0f-147">It's also useful to senders to inform them that their message may leave the organization, helping them make the correct decisions about wording, tone and content.</span></span>|
| <span data-ttu-id="97b0f-148">recipientSuggestions</span><span class="sxs-lookup"><span data-stu-id="97b0f-148">recipientSuggestions</span></span> | <span data-ttu-id="97b0f-149">Коллекция [recipient](../resources/recipient.md)</span><span class="sxs-lookup"><span data-stu-id="97b0f-149">[recipient](../resources/recipient.md) collection</span></span> | <span data-ttu-id="97b0f-150">Получатели предложенных на основе предыдущих контекстах, где они отображаются в то же сообщение.</span><span class="sxs-lookup"><span data-stu-id="97b0f-150">Recipients suggested based on previous contexts where they appear in the same message.</span></span> |
| <span data-ttu-id="97b0f-151">totalMemberCount</span><span class="sxs-lookup"><span data-stu-id="97b0f-151">totalMemberCount</span></span> | <span data-ttu-id="97b0f-152">Int32</span><span class="sxs-lookup"><span data-stu-id="97b0f-152">Int32</span></span> | <span data-ttu-id="97b0f-153">Число участников, если получатель является списком рассылки.</span><span class="sxs-lookup"><span data-stu-id="97b0f-153">The number of members if the recipient is a distribution list.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="97b0f-154">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="97b0f-154">JSON representation</span></span>

<span data-ttu-id="97b0f-155">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="97b0f-155">Here is a JSON representation of the resource.</span></span>

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
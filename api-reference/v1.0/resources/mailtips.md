---
title: тип ресурса mailTips
description: 'Информативные сообщения о получателе, отображаемые пользователям во время их составления сообщения. Например, неавтное сообщение '
localization_priority: Normal
author: abheek-das
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 0a2dfe421c19b49c8c7f489bef55890a058e2c40
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50941374"
---
# <a name="mailtips-resource-type"></a><span data-ttu-id="602f4-104">тип ресурса mailTips</span><span class="sxs-lookup"><span data-stu-id="602f4-104">mailTips resource type</span></span>

<span data-ttu-id="602f4-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="602f4-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="602f4-106">Информативные сообщения о получателе, отображаемые пользователям во время их составления сообщения.</span><span class="sxs-lookup"><span data-stu-id="602f4-106">Informative messages about a recipient, that are displayed to users while they are composing a message.</span></span> <span data-ttu-id="602f4-107">Например, неавтоматическое сообщение в качестве автоматического ответа для получателя сообщения.</span><span class="sxs-lookup"><span data-stu-id="602f4-107">For example, an out-of-office message as an automatic reply for a message recipient.</span></span>


## <a name="properties"></a><span data-ttu-id="602f4-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="602f4-108">Properties</span></span>
| <span data-ttu-id="602f4-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="602f4-109">Property</span></span>     | <span data-ttu-id="602f4-110">Тип</span><span class="sxs-lookup"><span data-stu-id="602f4-110">Type</span></span>   |<span data-ttu-id="602f4-111">Описание</span><span class="sxs-lookup"><span data-stu-id="602f4-111">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="602f4-112">automaticReplies</span><span class="sxs-lookup"><span data-stu-id="602f4-112">automaticReplies</span></span> | [<span data-ttu-id="602f4-113">automaticRepliesMailTips</span><span class="sxs-lookup"><span data-stu-id="602f4-113">automaticRepliesMailTips</span></span>](../resources/automaticrepliesmailtips.md) | <span data-ttu-id="602f4-114">Советы по электронной почте для автоматического ответа, если оно было настроено получателем.</span><span class="sxs-lookup"><span data-stu-id="602f4-114">Mail tips for automatic reply if it has been set up by the recipient.</span></span> |
| <span data-ttu-id="602f4-115">customMailTip</span><span class="sxs-lookup"><span data-stu-id="602f4-115">customMailTip</span></span> | <span data-ttu-id="602f4-116">Строка</span><span class="sxs-lookup"><span data-stu-id="602f4-116">String</span></span> | <span data-ttu-id="602f4-117">Пользовательский совет по почте, который можно установить на почтовом ящике получателя.</span><span class="sxs-lookup"><span data-stu-id="602f4-117">A custom mail tip that can be set on the recipient's mailbox.</span></span> |
| <span data-ttu-id="602f4-118">deliveryRestricted</span><span class="sxs-lookup"><span data-stu-id="602f4-118">deliveryRestricted</span></span>| <span data-ttu-id="602f4-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="602f4-119">Boolean</span></span> | <span data-ttu-id="602f4-120">Ограничен ли почтовый ящик получателя, например, прием сообщений только из предварительного списка отправителей, отклонение сообщений из предварительного списка отправителей или прием сообщений только от авторов проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="602f4-120">Whether the recipient's mailbox is restricted, for example, accepting messages from only a predefined list of senders, rejecting messages from a predefined list of senders, or accepting messages from only authenticated senders.</span></span> |
| <span data-ttu-id="602f4-121">emailAddress</span><span class="sxs-lookup"><span data-stu-id="602f4-121">emailAddress</span></span> | [<span data-ttu-id="602f4-122">emailAddress</span><span class="sxs-lookup"><span data-stu-id="602f4-122">emailAddress</span></span>](../resources/emailaddress.md) | <span data-ttu-id="602f4-123">Адрес электронной почты получателя для получения почтовых отправлений.</span><span class="sxs-lookup"><span data-stu-id="602f4-123">The email address of the recipient to get mailtips for.</span></span> |
| <span data-ttu-id="602f4-124">error</span><span class="sxs-lookup"><span data-stu-id="602f4-124">error</span></span> | [<span data-ttu-id="602f4-125">mailTipsError</span><span class="sxs-lookup"><span data-stu-id="602f4-125">mailTipsError</span></span>](../resources/mailtipserror.md) | <span data-ttu-id="602f4-126">Ошибки, которые возникают во время [действия getMailTips.](../api/user-getmailtips.md)</span><span class="sxs-lookup"><span data-stu-id="602f4-126">Errors that occur during the [getMailTips](../api/user-getmailtips.md) action.</span></span> |
| <span data-ttu-id="602f4-127">externalMemberCount</span><span class="sxs-lookup"><span data-stu-id="602f4-127">externalMemberCount</span></span> | <span data-ttu-id="602f4-128">Int32</span><span class="sxs-lookup"><span data-stu-id="602f4-128">Int32</span></span> | <span data-ttu-id="602f4-129">Количество внешних участников, если получатель — это список рассылки.</span><span class="sxs-lookup"><span data-stu-id="602f4-129">The number of external members if the recipient is a distribution list.</span></span> |
| <span data-ttu-id="602f4-130">isModerated</span><span class="sxs-lookup"><span data-stu-id="602f4-130">isModerated</span></span> |<span data-ttu-id="602f4-131">Boolean</span><span class="sxs-lookup"><span data-stu-id="602f4-131">Boolean</span></span>  | <span data-ttu-id="602f4-132">Требуется ли для отправки сообщений получателю утверждение.</span><span class="sxs-lookup"><span data-stu-id="602f4-132">Whether sending messages to the recipient requires approval.</span></span> <span data-ttu-id="602f4-133">Например, если получатель — это большой список рассылки и модератор настроен для утверждения сообщений, отправленных в этот список рассылки, или если отправка сообщений получателю требует утверждения руководителя получателя.</span><span class="sxs-lookup"><span data-stu-id="602f4-133">For example, if the recipient is a large distribution list and a moderator has been set up to approve messages sent to that distribution list, or if sending messages to a recipient requires approval of the recipient's manager.</span></span> |
| <span data-ttu-id="602f4-134">mailboxFull</span><span class="sxs-lookup"><span data-stu-id="602f4-134">mailboxFull</span></span> | <span data-ttu-id="602f4-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="602f4-135">Boolean</span></span> | <span data-ttu-id="602f4-136">Полный статус почтового ящика получателя.</span><span class="sxs-lookup"><span data-stu-id="602f4-136">The mailbox full status of the recipient.</span></span> |
| <span data-ttu-id="602f4-137">maxMessageSize</span><span class="sxs-lookup"><span data-stu-id="602f4-137">maxMessageSize</span></span> | <span data-ttu-id="602f4-138">Int32</span><span class="sxs-lookup"><span data-stu-id="602f4-138">Int32</span></span> | <span data-ttu-id="602f4-139">Максимальный размер сообщения, настроенный для организации или почтового ящика получателя.</span><span class="sxs-lookup"><span data-stu-id="602f4-139">The maximum message size that has been configured for the recipient's organization or mailbox.</span></span> |
| <span data-ttu-id="602f4-140">recipientScope</span><span class="sxs-lookup"><span data-stu-id="602f4-140">recipientScope</span></span> | <span data-ttu-id="602f4-141">recipientScopeType</span><span class="sxs-lookup"><span data-stu-id="602f4-141">recipientScopeType</span></span> | <span data-ttu-id="602f4-142">Область получателя.</span><span class="sxs-lookup"><span data-stu-id="602f4-142">The scope of the recipient.</span></span> <span data-ttu-id="602f4-143">Возможные значения: `none`, `internal`, `external`, `externalPartner`, `externalNonParther`.</span><span class="sxs-lookup"><span data-stu-id="602f4-143">Possible values are: `none`, `internal`, `external`, `externalPartner`, `externalNonParther`.</span></span> <span data-ttu-id="602f4-144">Например, администратор может установить, что другая организация является ее "партнером".</span><span class="sxs-lookup"><span data-stu-id="602f4-144">For example, an administrator can set another organization to be its "partner".</span></span> <span data-ttu-id="602f4-145">Область полезна, если администратор хочет, чтобы определенные почтовые ящики были доступны для определенных областей.</span><span class="sxs-lookup"><span data-stu-id="602f4-145">The scope is useful if an administrator wants certain mailtips to be accessible to certain scopes.</span></span> <span data-ttu-id="602f4-146">Кроме того, отправителям полезно информировать их о том, что их сообщение может покинуть организацию, помогая им принимать правильные решения о формулировках, тоне и контенте.</span><span class="sxs-lookup"><span data-stu-id="602f4-146">It's also useful to senders to inform them that their message may leave the organization, helping them make the correct decisions about wording, tone and content.</span></span>|
| <span data-ttu-id="602f4-147">recipientSuggestions</span><span class="sxs-lookup"><span data-stu-id="602f4-147">recipientSuggestions</span></span> | <span data-ttu-id="602f4-148">Коллекция [recipient](../resources/recipient.md)</span><span class="sxs-lookup"><span data-stu-id="602f4-148">[recipient](../resources/recipient.md) collection</span></span> | <span data-ttu-id="602f4-149">Получатели предлагаются на основе предыдущих контекстов, в которых они отображаются в одном сообщении.</span><span class="sxs-lookup"><span data-stu-id="602f4-149">Recipients suggested based on previous contexts where they appear in the same message.</span></span> |
| <span data-ttu-id="602f4-150">totalMemberCount</span><span class="sxs-lookup"><span data-stu-id="602f4-150">totalMemberCount</span></span> | <span data-ttu-id="602f4-151">Int32</span><span class="sxs-lookup"><span data-stu-id="602f4-151">Int32</span></span> | <span data-ttu-id="602f4-152">Количество участников, если получатель — это список рассылки.</span><span class="sxs-lookup"><span data-stu-id="602f4-152">The number of members if the recipient is a distribution list.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="602f4-153">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="602f4-153">JSON representation</span></span>

<span data-ttu-id="602f4-154">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="602f4-154">Here is a JSON representation of the resource.</span></span>

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


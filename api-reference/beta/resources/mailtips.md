---
title: Тип ресурса mailTips
description: 'Информационные сообщения о получателе, которые отображаются пользователям во время их составления сообщения. Например, сообщение об простое '
localization_priority: Normal
author: abheek-das
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 53c17a270903d69f19ee513f5d3bcbec848171af
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50129844"
---
# <a name="mailtips-resource-type"></a><span data-ttu-id="79434-104">Тип ресурса mailTips</span><span class="sxs-lookup"><span data-stu-id="79434-104">mailTips resource type</span></span>

<span data-ttu-id="79434-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="79434-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="79434-106">Информационные сообщения о получателе, которые отображаются пользователям во время их составления сообщения.</span><span class="sxs-lookup"><span data-stu-id="79434-106">Informative messages about a recipient, that are displayed to users while they are composing a message.</span></span> <span data-ttu-id="79434-107">Например, сообщение об неавтоматической службе в качестве автоматического ответа для получателя сообщения.</span><span class="sxs-lookup"><span data-stu-id="79434-107">For example, an out-of-office message as an automatic reply for a message recipient.</span></span>


## <a name="properties"></a><span data-ttu-id="79434-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="79434-108">Properties</span></span>
| <span data-ttu-id="79434-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="79434-109">Property</span></span>     | <span data-ttu-id="79434-110">Тип</span><span class="sxs-lookup"><span data-stu-id="79434-110">Type</span></span>   |<span data-ttu-id="79434-111">Описание</span><span class="sxs-lookup"><span data-stu-id="79434-111">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="79434-112">automaticReplies</span><span class="sxs-lookup"><span data-stu-id="79434-112">automaticReplies</span></span> | [<span data-ttu-id="79434-113">automaticRepliesMailTips</span><span class="sxs-lookup"><span data-stu-id="79434-113">automaticRepliesMailTips</span></span>](../resources/automaticrepliesmailtips.md) | <span data-ttu-id="79434-114">Подсказки электронной почты для автоматического ответа, если он был настроен получателем.</span><span class="sxs-lookup"><span data-stu-id="79434-114">Mail tips for automatic reply if it has been set up by the recipient.</span></span> |
| <span data-ttu-id="79434-115">customMailTip</span><span class="sxs-lookup"><span data-stu-id="79434-115">customMailTip</span></span> | <span data-ttu-id="79434-116">Строка</span><span class="sxs-lookup"><span data-stu-id="79434-116">String</span></span> | <span data-ttu-id="79434-117">Пользовательская подсказка, которую можно настроить в почтовом ящике получателя.</span><span class="sxs-lookup"><span data-stu-id="79434-117">A custom mail tip that can be set on the recipient's mailbox.</span></span> |
| <span data-ttu-id="79434-118">deliveryRestricted</span><span class="sxs-lookup"><span data-stu-id="79434-118">deliveryRestricted</span></span>| <span data-ttu-id="79434-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="79434-119">Boolean</span></span> | <span data-ttu-id="79434-120">Ограничен ли почтовый ящик получателя, например принимать сообщения только из предварительно заранее задав их или принимать сообщения только от отправителей, подлинность и т. д.</span><span class="sxs-lookup"><span data-stu-id="79434-120">Whether the recipient's mailbox is restricted, for example, accepting messages from only a predefined list of senders, rejecting messages from a predefined list of senders, or accepting messages from only authenticated senders.</span></span> |
| <span data-ttu-id="79434-121">emailAddress</span><span class="sxs-lookup"><span data-stu-id="79434-121">emailAddress</span></span> | [<span data-ttu-id="79434-122">emailAddress</span><span class="sxs-lookup"><span data-stu-id="79434-122">emailAddress</span></span>](../resources/emailaddress.md) | <span data-ttu-id="79434-123">Адрес электронной почты получателя, для который необходимо получить электронные сообщения.</span><span class="sxs-lookup"><span data-stu-id="79434-123">The email address of the recipient to get mailtips for.</span></span> |
| <span data-ttu-id="79434-124">error</span><span class="sxs-lookup"><span data-stu-id="79434-124">error</span></span> | [<span data-ttu-id="79434-125">mailTipsError</span><span class="sxs-lookup"><span data-stu-id="79434-125">mailTipsError</span></span>](../resources/mailtipserror.md) | <span data-ttu-id="79434-126">Ошибки, которые возникают во время [действия getMailTips.](../api/user-getmailtips.md)</span><span class="sxs-lookup"><span data-stu-id="79434-126">Errors that occur during the [getMailTips](../api/user-getmailtips.md) action.</span></span> |
| <span data-ttu-id="79434-127">externalMemberCount</span><span class="sxs-lookup"><span data-stu-id="79434-127">externalMemberCount</span></span> | <span data-ttu-id="79434-128">Int32</span><span class="sxs-lookup"><span data-stu-id="79434-128">Int32</span></span> | <span data-ttu-id="79434-129">Количество внешних членов, если получатель является списком рассылки.</span><span class="sxs-lookup"><span data-stu-id="79434-129">The number of external members if the recipient is a distribution list.</span></span> |
| <span data-ttu-id="79434-130">isModerated</span><span class="sxs-lookup"><span data-stu-id="79434-130">isModerated</span></span> |<span data-ttu-id="79434-131">Boolean</span><span class="sxs-lookup"><span data-stu-id="79434-131">Boolean</span></span>  | <span data-ttu-id="79434-132">Требуется ли утверждение при отправке сообщений получателю.</span><span class="sxs-lookup"><span data-stu-id="79434-132">Whether sending messages to the recipient requires approval.</span></span> <span data-ttu-id="79434-133">Например, если получатель является большим списком рассылки и модератор настроен на утверждение сообщений, отправляемых в этот список рассылки, или если для отправки сообщений получателю требуется утверждение руководителя получателя.</span><span class="sxs-lookup"><span data-stu-id="79434-133">For example, if the recipient is a large distribution list and a moderator has been set up to approve messages sent to that distribution list, or if sending messages to a recipient requires approval of the recipient's manager.</span></span> |
| <span data-ttu-id="79434-134">mailboxFull</span><span class="sxs-lookup"><span data-stu-id="79434-134">mailboxFull</span></span> | <span data-ttu-id="79434-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="79434-135">Boolean</span></span> | <span data-ttu-id="79434-136">Полное состояние почтового ящика получателя.</span><span class="sxs-lookup"><span data-stu-id="79434-136">The mailbox full status of the recipient.</span></span> |
| <span data-ttu-id="79434-137">maxMessageSize</span><span class="sxs-lookup"><span data-stu-id="79434-137">maxMessageSize</span></span> | <span data-ttu-id="79434-138">Int32</span><span class="sxs-lookup"><span data-stu-id="79434-138">Int32</span></span> | <span data-ttu-id="79434-139">Максимальный размер сообщения, настроенный для организации или почтового ящика получателя.</span><span class="sxs-lookup"><span data-stu-id="79434-139">The maximum message size that has been configured for the recipient's organization or mailbox.</span></span> |
| <span data-ttu-id="79434-140">recipientScope</span><span class="sxs-lookup"><span data-stu-id="79434-140">recipientScope</span></span> | <span data-ttu-id="79434-141">Строка</span><span class="sxs-lookup"><span data-stu-id="79434-141">String</span></span> | <span data-ttu-id="79434-142">Область получателя.</span><span class="sxs-lookup"><span data-stu-id="79434-142">The scope of the recipient.</span></span> <span data-ttu-id="79434-143">Возможные значения: `none`, `internal`, `external`, `externalPartner`, `externalNonParther`.</span><span class="sxs-lookup"><span data-stu-id="79434-143">Possible values are: `none`, `internal`, `external`, `externalPartner`, `externalNonParther`.</span></span> <span data-ttu-id="79434-144">Например, администратор может сделать другую организацию ее "партнером".</span><span class="sxs-lookup"><span data-stu-id="79434-144">For example, an administrator can set another organization to be its "partner".</span></span> <span data-ttu-id="79434-145">Область полезна, если администратор хочет, чтобы определенные почтовые советы были доступны для определенных областей.</span><span class="sxs-lookup"><span data-stu-id="79434-145">The scope is useful if an administrator wants certain mailtips to be accessible to certain scopes.</span></span> <span data-ttu-id="79434-146">Кроме того, отправителям полезно сообщить им, что их сообщение может покинуть организацию, помогая принимать правильные решения о формулировках, тонах и содержимом.</span><span class="sxs-lookup"><span data-stu-id="79434-146">It's also useful to senders to inform them that their message may leave the organization, helping them make the correct decisions about wording, tone and content.</span></span>|
| <span data-ttu-id="79434-147">recipientSuggestions</span><span class="sxs-lookup"><span data-stu-id="79434-147">recipientSuggestions</span></span> | <span data-ttu-id="79434-148">Коллекция [recipient](../resources/recipient.md)</span><span class="sxs-lookup"><span data-stu-id="79434-148">[recipient](../resources/recipient.md) collection</span></span> | <span data-ttu-id="79434-149">Получатели, предлагаемые на основе предыдущих контекстов, в которых они отображаются в одном сообщении.</span><span class="sxs-lookup"><span data-stu-id="79434-149">Recipients suggested based on previous contexts where they appear in the same message.</span></span> |
| <span data-ttu-id="79434-150">totalMemberCount</span><span class="sxs-lookup"><span data-stu-id="79434-150">totalMemberCount</span></span> | <span data-ttu-id="79434-151">Int32</span><span class="sxs-lookup"><span data-stu-id="79434-151">Int32</span></span> | <span data-ttu-id="79434-152">Количество членов, если получатель является списком рассылки.</span><span class="sxs-lookup"><span data-stu-id="79434-152">The number of members if the recipient is a distribution list.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="79434-153">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="79434-153">JSON representation</span></span>

<span data-ttu-id="79434-154">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="79434-154">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "mailtips resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->



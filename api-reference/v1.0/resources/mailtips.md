---
title: Тип ресурса подсказки
description: 'Информативные сообщения о получателе, которые отображаются для пользователей во время составления сообщения. Например, сообщение об отсутствии на работе '
localization_priority: Normal
author: svpsiva
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 926f2c48981da637083e747245ecdee1b94351cb
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43461840"
---
# <a name="mailtips-resource-type"></a><span data-ttu-id="6bbf8-104">Тип ресурса подсказки</span><span class="sxs-lookup"><span data-stu-id="6bbf8-104">mailTips resource type</span></span>

<span data-ttu-id="6bbf8-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6bbf8-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6bbf8-106">Информативные сообщения о получателе, которые отображаются для пользователей во время составления сообщения.</span><span class="sxs-lookup"><span data-stu-id="6bbf8-106">Informative messages about a recipient, that are displayed to users while they are composing a message.</span></span> <span data-ttu-id="6bbf8-107">Например, сообщение об отсутствии на работе в качестве автоматического ответа для получателя сообщения.</span><span class="sxs-lookup"><span data-stu-id="6bbf8-107">For example, an out-of-office message as an automatic reply for a message recipient.</span></span>


## <a name="properties"></a><span data-ttu-id="6bbf8-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="6bbf8-108">Properties</span></span>
| <span data-ttu-id="6bbf8-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="6bbf8-109">Property</span></span>     | <span data-ttu-id="6bbf8-110">Тип</span><span class="sxs-lookup"><span data-stu-id="6bbf8-110">Type</span></span>   |<span data-ttu-id="6bbf8-111">Описание</span><span class="sxs-lookup"><span data-stu-id="6bbf8-111">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="6bbf8-112">аутоматикреплиес</span><span class="sxs-lookup"><span data-stu-id="6bbf8-112">automaticReplies</span></span> | [<span data-ttu-id="6bbf8-113">аутоматикреплиесмаилтипс</span><span class="sxs-lookup"><span data-stu-id="6bbf8-113">automaticRepliesMailTips</span></span>](../resources/automaticrepliesmailtips.md) | <span data-ttu-id="6bbf8-114">Советы по использованию электронной почты для автоматического ответа, если он настроен получателем.</span><span class="sxs-lookup"><span data-stu-id="6bbf8-114">Mail tips for automatic reply if it has been set up by the recipient.</span></span> |
| <span data-ttu-id="6bbf8-115">кустоммаилтип</span><span class="sxs-lookup"><span data-stu-id="6bbf8-115">customMailTip</span></span> | <span data-ttu-id="6bbf8-116">String</span><span class="sxs-lookup"><span data-stu-id="6bbf8-116">String</span></span> | <span data-ttu-id="6bbf8-117">Настраиваемая подсказка почты, которую можно настроить для почтового ящика получателя.</span><span class="sxs-lookup"><span data-stu-id="6bbf8-117">A custom mail tip that can be set on the recipient's mailbox.</span></span> |
| <span data-ttu-id="6bbf8-118">деливерирестриктед</span><span class="sxs-lookup"><span data-stu-id="6bbf8-118">deliveryRestricted</span></span>| <span data-ttu-id="6bbf8-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="6bbf8-119">Boolean</span></span> | <span data-ttu-id="6bbf8-120">Является ли почтовый ящик получателя ограниченным, например принимать сообщения только от предопределенного списка отправителей, отклонять сообщения из предопределенного списка отправителей или принимать сообщения только от отправителей, прошедших проверку подлинности.</span><span class="sxs-lookup"><span data-stu-id="6bbf8-120">Whether the recipient's mailbox is restricted, for example, accepting messages from only a predefined list of senders, rejecting messages from a predefined list of senders, or accepting messages from only authenticated senders.</span></span> |
| <span data-ttu-id="6bbf8-121">emailAddress</span><span class="sxs-lookup"><span data-stu-id="6bbf8-121">emailAddress</span></span> | [<span data-ttu-id="6bbf8-122">emailAddress</span><span class="sxs-lookup"><span data-stu-id="6bbf8-122">emailAddress</span></span>](../resources/emailaddress.md) | <span data-ttu-id="6bbf8-123">Адрес электронной почты получателя, для которого необходимо получить подсказки.</span><span class="sxs-lookup"><span data-stu-id="6bbf8-123">The email address of the recipient to get mailtips for.</span></span> |
| <span data-ttu-id="6bbf8-124">error</span><span class="sxs-lookup"><span data-stu-id="6bbf8-124">error</span></span> | [<span data-ttu-id="6bbf8-125">маилтипсеррор</span><span class="sxs-lookup"><span data-stu-id="6bbf8-125">mailTipsError</span></span>](../resources/mailtipserror.md) | <span data-ttu-id="6bbf8-126">Ошибки, возникающие при выполнении действия [подсказки](../api/user-getmailtips.md) .</span><span class="sxs-lookup"><span data-stu-id="6bbf8-126">Errors that occur during the [getMailTips](../api/user-getmailtips.md) action.</span></span> |
| <span data-ttu-id="6bbf8-127">екстерналмемберкаунт</span><span class="sxs-lookup"><span data-stu-id="6bbf8-127">externalMemberCount</span></span> | <span data-ttu-id="6bbf8-128">Int32</span><span class="sxs-lookup"><span data-stu-id="6bbf8-128">Int32</span></span> | <span data-ttu-id="6bbf8-129">Количество внешних участников, если получатель является списком рассылки.</span><span class="sxs-lookup"><span data-stu-id="6bbf8-129">The number of external members if the recipient is a distribution list.</span></span> |
| <span data-ttu-id="6bbf8-130">Модератор</span><span class="sxs-lookup"><span data-stu-id="6bbf8-130">isModerated</span></span> |<span data-ttu-id="6bbf8-131">Boolean</span><span class="sxs-lookup"><span data-stu-id="6bbf8-131">Boolean</span></span>  | <span data-ttu-id="6bbf8-132">Требуется ли утверждение для отправки сообщений получателю.</span><span class="sxs-lookup"><span data-stu-id="6bbf8-132">Whether sending messages to the recipient requires approval.</span></span> <span data-ttu-id="6bbf8-133">Например, если получатель является большим списком рассылки, а Модератор настроен на утверждение сообщений, отправленных в этот список рассылки, или если отправка сообщений получателю требует утверждения руководителя получателя.</span><span class="sxs-lookup"><span data-stu-id="6bbf8-133">For example, if the recipient is a large distribution list and a moderator has been set up to approve messages sent to that distribution list, or if sending messages to a recipient requires approval of the recipient's manager.</span></span> |
| <span data-ttu-id="6bbf8-134">маилбоксфулл</span><span class="sxs-lookup"><span data-stu-id="6bbf8-134">mailboxFull</span></span> | <span data-ttu-id="6bbf8-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="6bbf8-135">Boolean</span></span> | <span data-ttu-id="6bbf8-136">Полный статус почтового ящика получателя.</span><span class="sxs-lookup"><span data-stu-id="6bbf8-136">The mailbox full status of the recipient.</span></span> |
| <span data-ttu-id="6bbf8-137">maxMessageSize</span><span class="sxs-lookup"><span data-stu-id="6bbf8-137">maxMessageSize</span></span> | <span data-ttu-id="6bbf8-138">Int32</span><span class="sxs-lookup"><span data-stu-id="6bbf8-138">Int32</span></span> | <span data-ttu-id="6bbf8-139">Максимальный размер сообщения, настроенный для организации или почтового ящика получателя.</span><span class="sxs-lookup"><span data-stu-id="6bbf8-139">The maximum message size that has been configured for the recipient's organization or mailbox.</span></span> |
| <span data-ttu-id="6bbf8-140">реЦипиентскопе</span><span class="sxs-lookup"><span data-stu-id="6bbf8-140">recipientScope</span></span> | <span data-ttu-id="6bbf8-141">реЦипиентскопетипе</span><span class="sxs-lookup"><span data-stu-id="6bbf8-141">recipientScopeType</span></span> | <span data-ttu-id="6bbf8-142">Область получателя.</span><span class="sxs-lookup"><span data-stu-id="6bbf8-142">The scope of the recipient.</span></span> <span data-ttu-id="6bbf8-143">Возможные значения: `none`, `internal`, `external`, `externalPartner`, `externalNonParther`.</span><span class="sxs-lookup"><span data-stu-id="6bbf8-143">Possible values are: `none`, `internal`, `external`, `externalPartner`, `externalNonParther`.</span></span> <span data-ttu-id="6bbf8-144">Например, администратор может назначить другую организацию "партнером".</span><span class="sxs-lookup"><span data-stu-id="6bbf8-144">For example, an administrator can set another organization to be its "partner".</span></span> <span data-ttu-id="6bbf8-145">Область действия полезна, если администратору требуется, чтобы некоторые подсказки были доступны для определенных областей.</span><span class="sxs-lookup"><span data-stu-id="6bbf8-145">The scope is useful if an administrator wants certain mailtips to be accessible to certain scopes.</span></span> <span data-ttu-id="6bbf8-146">Кроме того, отправители могут уведомить пользователей о том, что их сообщения могут отказаться от Организации, помогая им принять правильные решения по работе со словами, тонами и содержимым.</span><span class="sxs-lookup"><span data-stu-id="6bbf8-146">It's also useful to senders to inform them that their message may leave the organization, helping them make the correct decisions about wording, tone and content.</span></span>|
| <span data-ttu-id="6bbf8-147">реЦипиентсугжестионс</span><span class="sxs-lookup"><span data-stu-id="6bbf8-147">recipientSuggestions</span></span> | <span data-ttu-id="6bbf8-148">Коллекция [recipient](../resources/recipient.md)</span><span class="sxs-lookup"><span data-stu-id="6bbf8-148">[recipient](../resources/recipient.md) collection</span></span> | <span data-ttu-id="6bbf8-149">Получатели, предлагаемые в соответствии с предыдущими контекстами, в которых они отображаются в одном сообщении.</span><span class="sxs-lookup"><span data-stu-id="6bbf8-149">Recipients suggested based on previous contexts where they appear in the same message.</span></span> |
| <span data-ttu-id="6bbf8-150">тоталмемберкаунт</span><span class="sxs-lookup"><span data-stu-id="6bbf8-150">totalMemberCount</span></span> | <span data-ttu-id="6bbf8-151">Int32</span><span class="sxs-lookup"><span data-stu-id="6bbf8-151">Int32</span></span> | <span data-ttu-id="6bbf8-152">Число участников, если получатель является списком рассылки.</span><span class="sxs-lookup"><span data-stu-id="6bbf8-152">The number of members if the recipient is a distribution list.</span></span> |

### <a name="recipientscopetype-values"></a><span data-ttu-id="6bbf8-153">значения РеЦипиентскопетипе</span><span class="sxs-lookup"><span data-stu-id="6bbf8-153">recipientScopeType values</span></span>

| <span data-ttu-id="6bbf8-154">Значение</span><span class="sxs-lookup"><span data-stu-id="6bbf8-154">Value</span></span>
|:-------------------------
| <span data-ttu-id="6bbf8-155">Нет</span><span class="sxs-lookup"><span data-stu-id="6bbf8-155">none</span></span>
| <span data-ttu-id="6bbf8-156">образом</span><span class="sxs-lookup"><span data-stu-id="6bbf8-156">internal</span></span>
| <span data-ttu-id="6bbf8-157">внешних</span><span class="sxs-lookup"><span data-stu-id="6bbf8-157">external</span></span>
| <span data-ttu-id="6bbf8-158">ExternalPartner.</span><span class="sxs-lookup"><span data-stu-id="6bbf8-158">externalPartner</span></span>
| <span data-ttu-id="6bbf8-159">externalNonPartner</span><span class="sxs-lookup"><span data-stu-id="6bbf8-159">externalNonPartner</span></span>


## <a name="json-representation"></a><span data-ttu-id="6bbf8-160">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6bbf8-160">JSON representation</span></span>

<span data-ttu-id="6bbf8-161">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6bbf8-161">Here is a JSON representation of the resource.</span></span>

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

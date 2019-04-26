---
title: Тип ресурса подсказки
description: 'Информативные сообщения о получателе, которые отображаются для пользователей во время составления сообщения. Например, сообщение об отсутствии на работе '
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 15f026fd5a6485e5a0549d5987f53e26f0929b75
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33342780"
---
# <a name="mailtips-resource-type"></a><span data-ttu-id="70bb0-104">Тип ресурса подсказки</span><span class="sxs-lookup"><span data-stu-id="70bb0-104">mailTips resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="70bb0-105">Информативные сообщения о получателе, которые отображаются для пользователей во время составления сообщения.</span><span class="sxs-lookup"><span data-stu-id="70bb0-105">Informative messages about a recipient, that are displayed to users while they are composing a message.</span></span> <span data-ttu-id="70bb0-106">Например, сообщение об отсутствии на работе в качестве автоматического ответа для получателя сообщения.</span><span class="sxs-lookup"><span data-stu-id="70bb0-106">For example, an out-of-office message as an automatic reply for a message recipient.</span></span>


## <a name="properties"></a><span data-ttu-id="70bb0-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="70bb0-107">Properties</span></span>
| <span data-ttu-id="70bb0-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="70bb0-108">Property</span></span>     | <span data-ttu-id="70bb0-109">Тип</span><span class="sxs-lookup"><span data-stu-id="70bb0-109">Type</span></span>   |<span data-ttu-id="70bb0-110">Описание</span><span class="sxs-lookup"><span data-stu-id="70bb0-110">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="70bb0-111">Аутоматикреплиес</span><span class="sxs-lookup"><span data-stu-id="70bb0-111">automaticReplies</span></span> | [<span data-ttu-id="70bb0-112">Аутоматикреплиесмаилтипс</span><span class="sxs-lookup"><span data-stu-id="70bb0-112">automaticRepliesMailTips</span></span>](../resources/automaticrepliesmailtips.md) | <span data-ttu-id="70bb0-113">Советы по использованию электронной почты для автоматического ответа, если он настроен получателем.</span><span class="sxs-lookup"><span data-stu-id="70bb0-113">Mail tips for automatic reply if it has been set up by the recipient.</span></span> |
| <span data-ttu-id="70bb0-114">Кустоммаилтип</span><span class="sxs-lookup"><span data-stu-id="70bb0-114">customMailTip</span></span> | <span data-ttu-id="70bb0-115">String</span><span class="sxs-lookup"><span data-stu-id="70bb0-115">String</span></span> | <span data-ttu-id="70bb0-116">Настраиваемая подсказка почты, которую можно настроить для почтового ящика получателя.</span><span class="sxs-lookup"><span data-stu-id="70bb0-116">A custom mail tip that can be set on the recipient's mailbox.</span></span> |
| <span data-ttu-id="70bb0-117">Деливерирестриктед</span><span class="sxs-lookup"><span data-stu-id="70bb0-117">deliveryRestricted</span></span>| <span data-ttu-id="70bb0-118">Логический</span><span class="sxs-lookup"><span data-stu-id="70bb0-118">Boolean</span></span> | <span data-ttu-id="70bb0-119">Является ли почтовый ящик получателя ограниченным, например принимать сообщения только от предопределенного списка отправителей, отклонять сообщения из предопределенного списка отправителей или принимать сообщения только от отправителей, прошедших проверку подлинности.</span><span class="sxs-lookup"><span data-stu-id="70bb0-119">Whether the recipient's mailbox is restricted, for example, accepting messages from only a predefined list of senders, rejecting messages from a predefined list of senders, or accepting messages from only authenticated senders.</span></span> |
| <span data-ttu-id="70bb0-120">emailAddress</span><span class="sxs-lookup"><span data-stu-id="70bb0-120">emailAddress</span></span> | [<span data-ttu-id="70bb0-121">emailAddress</span><span class="sxs-lookup"><span data-stu-id="70bb0-121">emailAddress</span></span>](../resources/emailaddress.md) | <span data-ttu-id="70bb0-122">Адрес электронной почты получателя, для которого необходимо получить подсказки.</span><span class="sxs-lookup"><span data-stu-id="70bb0-122">The email address of the recipient to get mailtips for.</span></span> |
| <span data-ttu-id="70bb0-123">error</span><span class="sxs-lookup"><span data-stu-id="70bb0-123">error</span></span> | [<span data-ttu-id="70bb0-124">Маилтипсеррор</span><span class="sxs-lookup"><span data-stu-id="70bb0-124">mailTipsError</span></span>](../resources/mailtipserror.md) | <span data-ttu-id="70bb0-125">Ошибки, возникающие при выполнении действия [подсказки](../api/user-getmailtips.md) .</span><span class="sxs-lookup"><span data-stu-id="70bb0-125">Errors that occur during the [getMailTips](../api/user-getmailtips.md) action.</span></span> |
| <span data-ttu-id="70bb0-126">Екстерналмемберкаунт</span><span class="sxs-lookup"><span data-stu-id="70bb0-126">externalMemberCount</span></span> | <span data-ttu-id="70bb0-127">Int32</span><span class="sxs-lookup"><span data-stu-id="70bb0-127">Int32</span></span> | <span data-ttu-id="70bb0-128">Количество внешних участников, если получатель является списком рассылки.</span><span class="sxs-lookup"><span data-stu-id="70bb0-128">The number of external members if the recipient is a distribution list.</span></span> |
| <span data-ttu-id="70bb0-129">Модератор</span><span class="sxs-lookup"><span data-stu-id="70bb0-129">isModerated</span></span> |<span data-ttu-id="70bb0-130">Логический</span><span class="sxs-lookup"><span data-stu-id="70bb0-130">Boolean</span></span>  | <span data-ttu-id="70bb0-131">Требуется ли утверждение для отправки сообщений получателю.</span><span class="sxs-lookup"><span data-stu-id="70bb0-131">Whether sending messages to the recipient requires approval.</span></span> <span data-ttu-id="70bb0-132">Например, если получатель является большим списком рассылки, а Модератор настроен на утверждение сообщений, отправленных в этот список рассылки, или если отправка сообщений получателю требует утверждения руководителя получателя.</span><span class="sxs-lookup"><span data-stu-id="70bb0-132">For example, if the recipient is a large distribution list and a moderator has been set up to approve messages sent to that distribution list, or if sending messages to a recipient requires approval of the recipient's manager.</span></span> |
| <span data-ttu-id="70bb0-133">Маилбоксфулл</span><span class="sxs-lookup"><span data-stu-id="70bb0-133">mailboxFull</span></span> | <span data-ttu-id="70bb0-134">Логический</span><span class="sxs-lookup"><span data-stu-id="70bb0-134">Boolean</span></span> | <span data-ttu-id="70bb0-135">Полный статус почтового ящика получателя.</span><span class="sxs-lookup"><span data-stu-id="70bb0-135">The mailbox full status of the recipient.</span></span> |
| <span data-ttu-id="70bb0-136">maxMessageSize</span><span class="sxs-lookup"><span data-stu-id="70bb0-136">maxMessageSize</span></span> | <span data-ttu-id="70bb0-137">Int32</span><span class="sxs-lookup"><span data-stu-id="70bb0-137">Int32</span></span> | <span data-ttu-id="70bb0-138">Максимальный размер сообщения, настроенный для организации или почтового ящика получателя.</span><span class="sxs-lookup"><span data-stu-id="70bb0-138">The maximum message size that has been configured for the recipient's organization or mailbox.</span></span> |
| <span data-ttu-id="70bb0-139">РеЦипиентскопе</span><span class="sxs-lookup"><span data-stu-id="70bb0-139">recipientScope</span></span> | <span data-ttu-id="70bb0-140">String</span><span class="sxs-lookup"><span data-stu-id="70bb0-140">String</span></span> | <span data-ttu-id="70bb0-141">Область получателя.</span><span class="sxs-lookup"><span data-stu-id="70bb0-141">The scope of the recipient.</span></span> <span data-ttu-id="70bb0-142">Возможные значения: `none`, `internal`, `external`, `externalPartner`, `externalNonParther`.</span><span class="sxs-lookup"><span data-stu-id="70bb0-142">Possible values are: `none`, `internal`, `external`, `externalPartner`, `externalNonParther`.</span></span> <span data-ttu-id="70bb0-143">Например, администратор может назначить другую организацию "партнером".</span><span class="sxs-lookup"><span data-stu-id="70bb0-143">For example, an administrator can set another organization to be its "partner".</span></span> <span data-ttu-id="70bb0-144">Область действия полезна, если администратору требуется, чтобы некоторые подсказки были доступны для определенных областей.</span><span class="sxs-lookup"><span data-stu-id="70bb0-144">The scope is useful if an administrator wants certain mailtips to be accessible to certain scopes.</span></span> <span data-ttu-id="70bb0-145">Кроме того, отправители могут уведомить пользователей о том, что их сообщения могут отказаться от Организации, помогая им принять правильные решения по работе со словами, тонами и содержимым.</span><span class="sxs-lookup"><span data-stu-id="70bb0-145">It's also useful to senders to inform them that their message may leave the organization, helping them make the correct decisions about wording, tone and content.</span></span>|
| <span data-ttu-id="70bb0-146">РеЦипиентсугжестионс</span><span class="sxs-lookup"><span data-stu-id="70bb0-146">recipientSuggestions</span></span> | <span data-ttu-id="70bb0-147">Коллекция [recipient](../resources/recipient.md)</span><span class="sxs-lookup"><span data-stu-id="70bb0-147">[recipient](../resources/recipient.md) collection</span></span> | <span data-ttu-id="70bb0-148">Получатели, предлагаемые в соответствии с предыдущими контекстами, в которых они отображаются в одном сообщении.</span><span class="sxs-lookup"><span data-stu-id="70bb0-148">Recipients suggested based on previous contexts where they appear in the same message.</span></span> |
| <span data-ttu-id="70bb0-149">Тоталмемберкаунт</span><span class="sxs-lookup"><span data-stu-id="70bb0-149">totalMemberCount</span></span> | <span data-ttu-id="70bb0-150">Int32</span><span class="sxs-lookup"><span data-stu-id="70bb0-150">Int32</span></span> | <span data-ttu-id="70bb0-151">Число участников, если получатель является списком рассылки.</span><span class="sxs-lookup"><span data-stu-id="70bb0-151">The number of members if the recipient is a distribution list.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="70bb0-152">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="70bb0-152">JSON representation</span></span>

<span data-ttu-id="70bb0-153">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="70bb0-153">Here is a JSON representation of the resource.</span></span>

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

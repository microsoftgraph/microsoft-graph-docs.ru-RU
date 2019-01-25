---
title: Тип ресурса подсказок
description: 'Информационные сообщения о получателе, отображаемых для пользователей, хотя они составлять сообщение. Например сообщение об отсутствии '
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 11e64c09a90d130b7656d4e87770e6df3fb67408
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29508414"
---
# <a name="mailtips-resource-type"></a><span data-ttu-id="971dd-104">Тип ресурса подсказок</span><span class="sxs-lookup"><span data-stu-id="971dd-104">mailTips resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="971dd-105">Информационные сообщения о получателе, отображаемых для пользователей, хотя они составлять сообщение.</span><span class="sxs-lookup"><span data-stu-id="971dd-105">Informative messages about a recipient, that are displayed to users while they are composing a message.</span></span> <span data-ttu-id="971dd-106">Например отсутствии сообщение как автоматического ответа для получателя сообщения.</span><span class="sxs-lookup"><span data-stu-id="971dd-106">For example, an out-of-office message as an automatic reply for a message recipient.</span></span>


## <a name="properties"></a><span data-ttu-id="971dd-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="971dd-107">Properties</span></span>
| <span data-ttu-id="971dd-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="971dd-108">Property</span></span>     | <span data-ttu-id="971dd-109">Тип</span><span class="sxs-lookup"><span data-stu-id="971dd-109">Type</span></span>   |<span data-ttu-id="971dd-110">Описание</span><span class="sxs-lookup"><span data-stu-id="971dd-110">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="971dd-111">automaticReplies</span><span class="sxs-lookup"><span data-stu-id="971dd-111">automaticReplies</span></span> | [<span data-ttu-id="971dd-112">automaticRepliesMailTips</span><span class="sxs-lookup"><span data-stu-id="971dd-112">automaticRepliesMailTips</span></span>](../resources/automaticrepliesmailtips.md) | <span data-ttu-id="971dd-113">Почтовые подсказки для автоматического ответа, если она была настроена для получателя.</span><span class="sxs-lookup"><span data-stu-id="971dd-113">Mail tips for automatic reply if it has been set up by the recipient.</span></span> |
| <span data-ttu-id="971dd-114">CustomMailTip</span><span class="sxs-lookup"><span data-stu-id="971dd-114">customMailTip</span></span> | <span data-ttu-id="971dd-115">String</span><span class="sxs-lookup"><span data-stu-id="971dd-115">String</span></span> | <span data-ttu-id="971dd-116">Совет настраиваемых почты, который может устанавливаться на почтовый ящик получателя.</span><span class="sxs-lookup"><span data-stu-id="971dd-116">A custom mail tip that can be set on the recipient's mailbox.</span></span> |
| <span data-ttu-id="971dd-117">DeliveryRestricted</span><span class="sxs-lookup"><span data-stu-id="971dd-117">deliveryRestricted</span></span>| <span data-ttu-id="971dd-118">Логическое</span><span class="sxs-lookup"><span data-stu-id="971dd-118">Boolean</span></span> | <span data-ttu-id="971dd-119">Ли почтовый ящик получателя restricted, например, прием сообщений только в стандартном списке отправителей, отклонение сообщения из предварительно заданных списка отправителей или принимать сообщения от только проверенных.</span><span class="sxs-lookup"><span data-stu-id="971dd-119">Whether the recipient's mailbox is restricted, for example, accepting messages from only a predefined list of senders, rejecting messages from a predefined list of senders, or accepting messages from only authenticated senders.</span></span> |
| <span data-ttu-id="971dd-120">emailAddress</span><span class="sxs-lookup"><span data-stu-id="971dd-120">emailAddress</span></span> | [<span data-ttu-id="971dd-121">emailAddress</span><span class="sxs-lookup"><span data-stu-id="971dd-121">emailAddress</span></span>](../resources/emailaddress.md) | <span data-ttu-id="971dd-122">Адрес электронной почты для получения подсказки для получателя.</span><span class="sxs-lookup"><span data-stu-id="971dd-122">The email address of the recipient to get mailtips for.</span></span> |
| <span data-ttu-id="971dd-123">error</span><span class="sxs-lookup"><span data-stu-id="971dd-123">error</span></span> | [<span data-ttu-id="971dd-124">mailTipsError</span><span class="sxs-lookup"><span data-stu-id="971dd-124">mailTipsError</span></span>](../resources/mailtipserror.md) | <span data-ttu-id="971dd-125">Ошибки, возникающие во время действия [getMailTips](../api/user-getmailtips.md) .</span><span class="sxs-lookup"><span data-stu-id="971dd-125">Errors that occur during the [getMailTips](../api/user-getmailtips.md) action.</span></span> |
| <span data-ttu-id="971dd-126">ExternalMemberCount</span><span class="sxs-lookup"><span data-stu-id="971dd-126">externalMemberCount</span></span> | <span data-ttu-id="971dd-127">Int32</span><span class="sxs-lookup"><span data-stu-id="971dd-127">Int32</span></span> | <span data-ttu-id="971dd-128">Число внешних участников, если получатель является списком рассылки.</span><span class="sxs-lookup"><span data-stu-id="971dd-128">The number of external members if the recipient is a distribution list.</span></span> |
| <span data-ttu-id="971dd-129">IsModerated</span><span class="sxs-lookup"><span data-stu-id="971dd-129">isModerated</span></span> |<span data-ttu-id="971dd-130">Логическое</span><span class="sxs-lookup"><span data-stu-id="971dd-130">Boolean</span></span>  | <span data-ttu-id="971dd-131">Отправка сообщений получателю, требуется ли утверждение.</span><span class="sxs-lookup"><span data-stu-id="971dd-131">Whether sending messages to the recipient requires approval.</span></span> <span data-ttu-id="971dd-132">Например если получатель является большой список рассылки и модератор установлен до утверждать сообщений, отправленных в этот список рассылки, или если отправка сообщений получателя требует утверждения руководителем получателя.</span><span class="sxs-lookup"><span data-stu-id="971dd-132">For example, if the recipient is a large distribution list and a moderator has been set up to approve messages sent to that distribution list, or if sending messages to a recipient requires approval of the recipient's manager.</span></span> |
| <span data-ttu-id="971dd-133">MailboxFull</span><span class="sxs-lookup"><span data-stu-id="971dd-133">mailboxFull</span></span> | <span data-ttu-id="971dd-134">Логическое</span><span class="sxs-lookup"><span data-stu-id="971dd-134">Boolean</span></span> | <span data-ttu-id="971dd-135">Состояние полный почтовый ящик получателя.</span><span class="sxs-lookup"><span data-stu-id="971dd-135">The mailbox full status of the recipient.</span></span> |
| <span data-ttu-id="971dd-136">MaxMessageSize</span><span class="sxs-lookup"><span data-stu-id="971dd-136">maxMessageSize</span></span> | <span data-ttu-id="971dd-137">Int32</span><span class="sxs-lookup"><span data-stu-id="971dd-137">Int32</span></span> | <span data-ttu-id="971dd-138">Максимальный размер сообщения, настроенного для организации или почтовый ящик получателя.</span><span class="sxs-lookup"><span data-stu-id="971dd-138">The maximum message size that has been configured for the recipient's organization or mailbox.</span></span> |
| <span data-ttu-id="971dd-139">recipientScope</span><span class="sxs-lookup"><span data-stu-id="971dd-139">recipientScope</span></span> | <span data-ttu-id="971dd-140">String</span><span class="sxs-lookup"><span data-stu-id="971dd-140">String</span></span> | <span data-ttu-id="971dd-141">Область получателя.</span><span class="sxs-lookup"><span data-stu-id="971dd-141">The scope of the recipient.</span></span> <span data-ttu-id="971dd-142">Возможные значения: `none`, `internal`, `external`, `externalPartner`, `externalNonParther`.</span><span class="sxs-lookup"><span data-stu-id="971dd-142">Possible values are: `none`, `internal`, `external`, `externalPartner`, `externalNonParther`.</span></span> <span data-ttu-id="971dd-143">Например администратор может установить другой организации, чтобы быть «партнер».</span><span class="sxs-lookup"><span data-stu-id="971dd-143">For example, an administrator can set another organization to be its "partner".</span></span> <span data-ttu-id="971dd-144">Область полезен в том случае, если администратор хочет определенных подсказки необходимо сделать доступным для определенных областей.</span><span class="sxs-lookup"><span data-stu-id="971dd-144">The scope is useful if an administrator wants certain mailtips to be accessible to certain scopes.</span></span> <span data-ttu-id="971dd-145">Также полезно для отправителей, информирующее о том, что сообщение может привести к организации, помогая им подкорректировать формулировки, тонового сигнала и контент.</span><span class="sxs-lookup"><span data-stu-id="971dd-145">It's also useful to senders to inform them that their message may leave the organization, helping them make the correct decisions about wording, tone and content.</span></span>|
| <span data-ttu-id="971dd-146">recipientSuggestions</span><span class="sxs-lookup"><span data-stu-id="971dd-146">recipientSuggestions</span></span> | <span data-ttu-id="971dd-147">Коллекция [recipient](../resources/recipient.md)</span><span class="sxs-lookup"><span data-stu-id="971dd-147">[recipient](../resources/recipient.md) collection</span></span> | <span data-ttu-id="971dd-148">Получатели предложенных на основе предыдущих контекстах, где они отображаются в то же сообщение.</span><span class="sxs-lookup"><span data-stu-id="971dd-148">Recipients suggested based on previous contexts where they appear in the same message.</span></span> |
| <span data-ttu-id="971dd-149">TotalMemberCount</span><span class="sxs-lookup"><span data-stu-id="971dd-149">totalMemberCount</span></span> | <span data-ttu-id="971dd-150">Int32</span><span class="sxs-lookup"><span data-stu-id="971dd-150">Int32</span></span> | <span data-ttu-id="971dd-151">Число участников, если получатель является списком рассылки.</span><span class="sxs-lookup"><span data-stu-id="971dd-151">The number of members if the recipient is a distribution list.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="971dd-152">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="971dd-152">JSON representation</span></span>

<span data-ttu-id="971dd-153">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="971dd-153">Here is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/mailtips.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

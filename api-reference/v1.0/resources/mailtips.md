# <a name="mailtips-resource-type"></a><span data-ttu-id="7e2a9-101">Тип ресурса mailTips</span><span class="sxs-lookup"><span data-stu-id="7e2a9-101">mailTips resource type</span></span>

<span data-ttu-id="7e2a9-102">Информационные сообщения о получателе, отображаемые для пользователей при составлении сообщения.</span><span class="sxs-lookup"><span data-stu-id="7e2a9-102">Informative messages about a recipient, that are displayed to users while they are composing a message.</span></span> <span data-ttu-id="7e2a9-103">Например, сообщение об отсутствии на рабочем месте, отправляемое получателем сообщения в качестве автоматического ответа.</span><span class="sxs-lookup"><span data-stu-id="7e2a9-103">For example, an out-of-office message as an automatic reply for a message recipient.</span></span>


## <a name="properties"></a><span data-ttu-id="7e2a9-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="7e2a9-104">Properties</span></span>
| <span data-ttu-id="7e2a9-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="7e2a9-105">Property</span></span>     | <span data-ttu-id="7e2a9-106">Тип</span><span class="sxs-lookup"><span data-stu-id="7e2a9-106">Type</span></span>   |<span data-ttu-id="7e2a9-107">Описание</span><span class="sxs-lookup"><span data-stu-id="7e2a9-107">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="7e2a9-108">automaticReplies</span><span class="sxs-lookup"><span data-stu-id="7e2a9-108">automaticReplies</span></span> | [<span data-ttu-id="7e2a9-109">automaticRepliesMailTips</span><span class="sxs-lookup"><span data-stu-id="7e2a9-109">automaticRepliesMailTips</span></span>](../resources/automaticrepliesmailtips.md) | <span data-ttu-id="7e2a9-110">Подсказки для автоматического ответа, если он настроен получателем.</span><span class="sxs-lookup"><span data-stu-id="7e2a9-110">Mail tips for automatic reply if it has been set up by the recipient.</span></span> |
| <span data-ttu-id="7e2a9-111">customMailTip</span><span class="sxs-lookup"><span data-stu-id="7e2a9-111">CustomMailTip</span></span> | <span data-ttu-id="7e2a9-112">String (строка)</span><span class="sxs-lookup"><span data-stu-id="7e2a9-112">String</span></span> | <span data-ttu-id="7e2a9-113">Настраиваемая подсказка, которую можно настроить для почтового ящика получателя.</span><span class="sxs-lookup"><span data-stu-id="7e2a9-113">A custom mail tip that can be set on the recipient's mailbox.</span></span> |
| <span data-ttu-id="7e2a9-114">deliveryRestricted</span><span class="sxs-lookup"><span data-stu-id="7e2a9-114">DeliveryRestricted</span></span>| <span data-ttu-id="7e2a9-115">Boolean (логический)</span><span class="sxs-lookup"><span data-stu-id="7e2a9-115">Boolean</span></span> | <span data-ttu-id="7e2a9-116">Указывает, ограничен ли почтовый ящик получателя, например, с приемом сообщений только от предопределенного списка отправителей, отклонением сообщений от предопределенного списка отправителей или приемом сообщений только от отправителей, прошедших проверку подлинности.</span><span class="sxs-lookup"><span data-stu-id="7e2a9-116">Whether the recipient's mailbox is restricted, for example, accepting messages from only a predefined list of senders, rejecting messages from a predefined list of senders, or accepting messages from only authenticated senders.</span></span> |
| <span data-ttu-id="7e2a9-117">emailAddress</span><span class="sxs-lookup"><span data-stu-id="7e2a9-117">emailAddress</span></span> | [<span data-ttu-id="7e2a9-118">emailAddress</span><span class="sxs-lookup"><span data-stu-id="7e2a9-118">emailAddress</span></span>](../resources/emailaddress.md) | <span data-ttu-id="7e2a9-119">Адрес электронной почты получателя для получения подсказок.</span><span class="sxs-lookup"><span data-stu-id="7e2a9-119">The email address of the recipient to get mailtips for.</span></span> |
| <span data-ttu-id="7e2a9-120">error</span><span class="sxs-lookup"><span data-stu-id="7e2a9-120">error</span></span> | [<span data-ttu-id="7e2a9-121">mailTipsError</span><span class="sxs-lookup"><span data-stu-id="7e2a9-121">mailTipsError</span></span>](../resources/mailtipserror.md) | <span data-ttu-id="7e2a9-122">Ошибки, возникающие во время действия [GetMailTips](../api/user_getmailtips.md).</span><span class="sxs-lookup"><span data-stu-id="7e2a9-122">Errors that occur during the [getMailTips](../api/user_getmailtips.md) action.</span></span> |
| <span data-ttu-id="7e2a9-123">externalMemberCount</span><span class="sxs-lookup"><span data-stu-id="7e2a9-123">ExternalMemberCount</span></span> | <span data-ttu-id="7e2a9-124">Int32</span><span class="sxs-lookup"><span data-stu-id="7e2a9-124">Int32</span></span> | <span data-ttu-id="7e2a9-125">Количество внешних участников, если получатель является списком рассылки.</span><span class="sxs-lookup"><span data-stu-id="7e2a9-125">The number of external members if the recipient is a distribution list.</span></span> |
| <span data-ttu-id="7e2a9-126">isModerated</span><span class="sxs-lookup"><span data-stu-id="7e2a9-126">IsModerated</span></span> |<span data-ttu-id="7e2a9-127">Boolean (логический)</span><span class="sxs-lookup"><span data-stu-id="7e2a9-127">Boolean</span></span>  | <span data-ttu-id="7e2a9-128">Указывает, требуется ли утверждение отправки сообщений получателю.</span><span class="sxs-lookup"><span data-stu-id="7e2a9-128">Whether sending messages to the recipient requires approval.</span></span> <span data-ttu-id="7e2a9-129">Например, для случаев, когда получатель представляет собой большой список рассылки, а модератор настроен для утверждения сообщений, отправленных в этот список рассылки, или когда отправка сообщений получателю требует утверждения менеджером получателя.</span><span class="sxs-lookup"><span data-stu-id="7e2a9-129">For example, if the recipient is a large distribution list and a moderator has been set up to approve messages sent to that distribution list, or if sending messages to a recipient requires approval of the recipient's manager.</span></span> |
| <span data-ttu-id="7e2a9-130">mailboxFull</span><span class="sxs-lookup"><span data-stu-id="7e2a9-130">MailboxFull</span></span> | <span data-ttu-id="7e2a9-131">Boolean (логический)</span><span class="sxs-lookup"><span data-stu-id="7e2a9-131">Boolean</span></span> | <span data-ttu-id="7e2a9-132">Переполненность почтового ящика получателя.</span><span class="sxs-lookup"><span data-stu-id="7e2a9-132">The mailbox full status of the recipient.</span></span> |
| <span data-ttu-id="7e2a9-133">maxMessageSize</span><span class="sxs-lookup"><span data-stu-id="7e2a9-133">MaxMessageSize</span></span> | <span data-ttu-id="7e2a9-134">Int32</span><span class="sxs-lookup"><span data-stu-id="7e2a9-134">Int32</span></span> | <span data-ttu-id="7e2a9-135">Максимальный размер сообщения, который настроен для организации или почтового ящика получателя.</span><span class="sxs-lookup"><span data-stu-id="7e2a9-135">The maximum message size that has been configured for the recipient's organization or mailbox.</span></span> |
| <span data-ttu-id="7e2a9-136">recipientScope</span><span class="sxs-lookup"><span data-stu-id="7e2a9-136">recipientScope</span></span> | <span data-ttu-id="7e2a9-137">String (строка)</span><span class="sxs-lookup"><span data-stu-id="7e2a9-137">String</span></span> | <span data-ttu-id="7e2a9-138">Область получателя.</span><span class="sxs-lookup"><span data-stu-id="7e2a9-138">The scope of the query.</span></span> <span data-ttu-id="7e2a9-139">Возможные значения: `none`, `internal`, `external`, `externalPartner`, `externalNonParther`.</span><span class="sxs-lookup"><span data-stu-id="7e2a9-139">Possible values are: `none`, `internal`, `external`, `externalPartner`, `externalNonParther`.</span></span> <span data-ttu-id="7e2a9-140">Например, администратор может назначить другую организацию своим "партнером".</span><span class="sxs-lookup"><span data-stu-id="7e2a9-140">For example, an administrator can set another organization to be its "partner".</span></span> <span data-ttu-id="7e2a9-141">Область полезна, если администратор желает, чтобы определенные подсказки были доступны для определенных областей.</span><span class="sxs-lookup"><span data-stu-id="7e2a9-141">The scope is useful if an administrator wants certain mailtips to be accessible to certain scopes.</span></span> <span data-ttu-id="7e2a9-142">Она также полезна для отправителей: они информируются о том, что их сообщение может покинуть пределы организации, что позволяет им пересмотреть формулировку, тон и содержимое сообщения.</span><span class="sxs-lookup"><span data-stu-id="7e2a9-142">It's also useful to senders to inform them that their message may leave the organization, helping them make the correct decisions about wording, tone and content.</span></span>|
| <span data-ttu-id="7e2a9-143">recipientSuggestions</span><span class="sxs-lookup"><span data-stu-id="7e2a9-143">recipientSuggestions</span></span> | <span data-ttu-id="7e2a9-144">Коллекция [recipient](../resources/recipient.md)</span><span class="sxs-lookup"><span data-stu-id="7e2a9-144">[recipient](../resources/recipient.md) collection</span></span> | <span data-ttu-id="7e2a9-145">Предложения получателей, которые основываются на предыдущем контексте, когда они фигурируют в таком же сообщении.</span><span class="sxs-lookup"><span data-stu-id="7e2a9-145">Recipients suggested based on previous contexts where they appear in the same message.</span></span> |
| <span data-ttu-id="7e2a9-146">totalMemberCount</span><span class="sxs-lookup"><span data-stu-id="7e2a9-146">TotalMemberCount</span></span> | <span data-ttu-id="7e2a9-147">Int32</span><span class="sxs-lookup"><span data-stu-id="7e2a9-147">Int32</span></span> | <span data-ttu-id="7e2a9-148">Число участников, если получатель является списком рассылки.</span><span class="sxs-lookup"><span data-stu-id="7e2a9-148">The number of members if the recipient is a distribution list.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="7e2a9-149">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7e2a9-149">JSON representation</span></span>

<span data-ttu-id="7e2a9-150">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7e2a9-150">Here is a JSON representation of the resource.</span></span>

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
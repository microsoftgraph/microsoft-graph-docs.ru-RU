# <a name="configuring-the-invitation-message"></a><span data-ttu-id="71cda-101">Настройка приглашения</span><span class="sxs-lookup"><span data-stu-id="71cda-101">Configuring the invitation message</span></span>

<span data-ttu-id="71cda-102">Объект invitedUserMessageInfo позволяет настроить сообщение [приглашение](invitation.md).</span><span class="sxs-lookup"><span data-stu-id="71cda-102">The invitedUserMessageInfo object allows you to configure the [invitation](invitation.md) message.</span></span>


## <a name="properties"></a><span data-ttu-id="71cda-103">Свойства</span><span class="sxs-lookup"><span data-stu-id="71cda-103">Properties</span></span>
| <span data-ttu-id="71cda-104">Свойство</span><span class="sxs-lookup"><span data-stu-id="71cda-104">Property</span></span>     | <span data-ttu-id="71cda-105">Тип</span><span class="sxs-lookup"><span data-stu-id="71cda-105">Type</span></span>   |<span data-ttu-id="71cda-106">Описание</span><span class="sxs-lookup"><span data-stu-id="71cda-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="71cda-107">ccRecipients</span><span class="sxs-lookup"><span data-stu-id="71cda-107">ccRecipients</span></span>|<span data-ttu-id="71cda-108">Коллекция [Recipient](recipient.md)</span><span class="sxs-lookup"><span data-stu-id="71cda-108">[Recipient](recipient.md) collection</span></span>|<span data-ttu-id="71cda-p101">Дополнительные получатели, которым следует отправить приглашение. В настоящее время поддерживается только 1 дополнительный получатель.</span><span class="sxs-lookup"><span data-stu-id="71cda-p101">Additional recipients the invitation message should be sent to. Currently only 1 additional recipient is supported.</span></span>|
|<span data-ttu-id="71cda-111">customizedMessageBody</span><span class="sxs-lookup"><span data-stu-id="71cda-111">customizedMessageBody</span></span>|<span data-ttu-id="71cda-112">Строка</span><span class="sxs-lookup"><span data-stu-id="71cda-112">String</span></span>|<span data-ttu-id="71cda-113">Ваш собственный текст сообщения, который можно отправлять вместо предоставляемого по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="71cda-113">Customized message body you want to send if you don't want the default message.</span></span>|
|<span data-ttu-id="71cda-114">messageLanguage</span><span class="sxs-lookup"><span data-stu-id="71cda-114">messageLanguage</span></span>|<span data-ttu-id="71cda-115">String (строка)</span><span class="sxs-lookup"><span data-stu-id="71cda-115">String</span></span>|<span data-ttu-id="71cda-p102">Выбранный вами язык для сообщения, которое отправляется по умолчанию. Если указано значение customizedMessageBody, это свойство игнорируется, и сообщение отправляется с помощью customizedMessageBody. Язык должен быть указан в формате ISO 639. Значение по умолчанию — en-US.</span><span class="sxs-lookup"><span data-stu-id="71cda-p102">The language you want to send the default message in. If the customizedMessageBody is specified, this property is ignored, and the message is sent using the customizedMessageBody. The language format should be in ISO 639. The default is en-US.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="71cda-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="71cda-120">JSON representation</span></span>
<span data-ttu-id="71cda-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="71cda-121">Here is a JSON representation of the resource</span></span>

<!-- {"blockType": "resource", "@odata.type": "microsoft.graph.invitedUserMessageInfo"} -->
```json
{
  "ccRecipients": [ {"@odata.type": "microsoft.graph.recipient"} ],
  "customizedMessageBody": "string",
  "messageLanguage": "string"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2016-22-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "invitedUserMessageInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

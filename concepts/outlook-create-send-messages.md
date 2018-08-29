# <a name="create-and-send-outlook-messages"></a>Создание и отправка сообщений Outlook

В Microsoft Graph электронные письма представлены ресурсом [message](../api-reference/v1.0/resources/message.md).

По умолчанию сообщения можно идентифицировать по уникальному идентификатору записи в свойстве **id**. При первом сохранении сообщения в качестве черновика или отправленного сообщения поставщик услуг хранилища назначает идентификатор записи этому сообщению. Этот идентификатор изменяется при копировании сообщения или его перемещении в другую папку, хранилище или PST-файл.

## <a name="creating-and-sending-mail"></a>Создание и отправка почты

В Outlook вы можете создавать и отправлять электронные письма в одном и том же действии [sendMail](../api-reference/v1.0/api/user_sendmail.md). Вы также можете [создать](../api-reference/v1.0/api/user_post_messages.md) черновик, затем [добавить содержимое](../api-reference/v1.0/api/message_update.md) и [отправить](../api-reference/v1.0/api/message_send.md) черновик.

Аналогично, при ответе на электронное письмо вы можете создавать и отправлять ответы в одном и том же действии ([ответить](../api-reference/v1.0/api/message_reply.md), [ответить всем](../api-reference/v1.0/api//message_replyall.md) или [переслать](../api-reference/v1.0/api/message_forward.md)). Кроме того, вы можете создать черновик для ответа ([ответить](../api-reference/v1.0/api/message_createreply.md), [ответить всем](../api-reference/v1.0/api//message_createreplyall.md) или [переслать](../api-reference/v1.0/api/message_createforward.md)), [добавить содержимое](../api-reference/v1.0/api/message_update.md), а затем [отправить ](../api-reference/v1.0/api/message_send.md) черновик позже.

Чтобы программным способом отличать черновики от отправленных писем, проверяйте свойство **isDraft**.

По умолчанию черновики сообщений сохраняются в папке `Drafts`, а отправленные сообщения — в папке `Sent Items`. Для удобства вы можете определить папки "Черновики" и "Отправленные", используя их [соответствующие хорошо известные имена папок](../api-reference/v1.0/resources/mailfolder.md). Например, вы можете выполнить указанные ниже действия, чтобы [получить сообщения](../api-reference/v1.0/api/user_list_messages.md) в папке "Черновики".

```http
GET /me/mailfolders('Drafts')
```

### <a name="body-format-and-malicious-script"></a>Формат текста и вредоносный скрипт

<!-- Remove the following 2 sections from the message.md topics
-->

Сообщение может иметь либо формат HTML, либо текстовый формат. По умолчанию в отклике GET текст сообщения возвращается в формате HTML.

При [получении сообщения](../api-reference/v1.0/api/message_get.md) вы можете задать указанный ниже заголовок запроса, чтобы система возвратила свойства **body** и **uniqueBody** в текстовом формате.

```http
Prefer: outlook.body-content-type="text"
```

Чтобы получить текст сообщения в формате HTML, задайте указанный ниже заголовок или просто пропустите его.

```http
Prefer: outlook.body-content-type="html"
```

Когда вы указываете какой-либо заголовок, успешный отклик будет включать соответствующий заголовок `Preference-Applied`.

- Чтобы получить результат выполнения запроса в текстовом формате: `Preference-Applied: outlook.body-content-type="text"`
- Чтобы получить результат выполнения запроса в формате HTML: `Preference-Applied: outlook.body-content-type="html"`

Если текст сообщения имеет формат HTML, то по умолчанию прежде чем возвратить текст сообщения в отклике REST, Outlook удаляет весь потенциально небезопасный HTML-код (например, код JavaScript), внедренный в свойство **body**.

Чтобы получить все исходное содержимое в формате HTML, добавьте следующий заголовок HTTP-запроса:

```http
Prefer: outlook.allow-unsafe-html
```

### <a name="differentiating-the-from-and-sender-properties"></a>Различия между свойствами from и sender

В процессе создания сообщения в большинстве случаев Outlook указывает в качестве значения свойств **from** и **sender** одного и того же пользователя, вошедшего в систему. Вы можете изменить эти свойства в указанных ниже ситуациях.

- Свойство **from** можно изменить, если администратор Exchange назначил другим пользователям права **sendAs** для почтового ящика. Для этого администратор может назначить его владельца, выбрав элемент **Разрешения для почтового ящика** на портале Azure, либо использовать Центр администрирования Exchange или командлет Add-ADPermission в Windows PowerShell. Затем программным способом можно задать свойство **from** одному из этих пользователей, обладающих правами **sendAs** для этого почтового ящика.
- Свойство **sender** можно изменить, если владелец почтового ящика предоставил одному или нескольким пользователям права на отправку сообщений из этого почтового ящика. Владелец почтового ящика может делегировать разрешения в Outlook. Когда представитель отправляет сообщение от имени владельца почтового ящика, Outlook присваивает свойству **sender** учетную запись представителя, а в качестве значения свойства **from** остается владелец почтового ящика. Вы можете программным способом задать в качестве значения свойства **sender** пользователя, получившего разрешения представителя для этого почтового ящика.

## <a name="using-mailtips-to-check-recipient-status-and-save-time-preview"></a>Проверка состояния получателя и экономия времени с помощью подсказок (ознакомительная версия)

С помощью [подсказок](../api-reference/beta/resources/mailtips.md) вы можете принимать обоснованные решения перед отправкой электронных писем.
Благодаря подсказкам можно получить ряд сведений, например о том, что почтовый ящик получателя доступен только для определенных отправителей, либо о том, что для отправки электронного письма получателю необходимо утверждение.

## <a name="integrating-with--social-gesture-preview"></a>Интеграция с социальными жестами (ознакомительная версия)

@Упоминания — это уведомления для пользователей, о том, что их упомянули в сообщениях. С помощью ресурса [mention](../api-reference/beta/resources/mention.md) приложения могут задавать и получать стандартный социальный жест в Интернете (префикс @) в письмах.
Вы можете выполнить указанные ниже действия.

- Создавать @упоминания при [составлении сообщений](../api-reference/beta/api/user_post_messages.md#request-2)
- [Получать все сообщения в почтовом ящике пользователя, содержащие @упоминание пользователя](../api-reference/beta/api/user_list_messages.md#request-2)
- [Получать все @упоминания в сообщении](../api-reference/beta/api/message_get.md#request-2)

## <a name="other-shared-capabilities"></a>Другие общие возможности

Используйте указанные ниже стандартные возможности, имеющиеся в объектах Microsoft Graph.

- Вы можете подписаться на [уведомления об изменениях](../api-reference/v1.0/resources/webhooks.md) сообщений. Вы будете получать их при возникновении изменений одного или нескольких типов, например при создании или изменении сообщений.
- [Вы можете отслеживать эти добавочные изменения сообщений в папке](delta_query_messages.md).
- Вы можете создавать [открытые расширения](extensibility_overview.md#open-extensions) или [расширения схемы](extensibility_overview.md#schema-extensions), чтобы добавлять пользовательские данные в экземпляры сообщений.
- Вы можете создавать [расширенные свойства](../api-reference/v1.0/resources/extended-properties-overview.md) в экземплярах сообщений, чтобы хранить пользовательские данные для свойств MAPI Outlook, когда эти свойства еще недоступны в метаданных API Microsoft Graph.

## <a name="next-steps"></a>Дальнейшие действия

Дополнительные сведения:

- [Зачем выполнять интеграцию с почтой Outlook?](outlook-mail-concept-overview.md)
- [Использование API почты](../api-reference/v1.0/resources/mail_api_overview.md) и [варианты использования](../api-reference/v1.0/resources/mail_api_overview.md#common-use-cases) в Microsoft Graph 1.0.


<!-- {
  "type": "#page.annotation",
  "suppressions": [
    "Error: /concepts/outlook-create-send-messages.md:
        BookmarkSkippedDocFileNotFound: Link '[creating a message](../api-reference/beta/api/user_post_messages.md#request-2)'.",
    "Error: /concepts/outlook-create-send-messages.md:
      BookmarkSkippedDocFileNotFound: Link '[Get all the messages in a user's mailbox that contain an @-mention of the user](../api-reference/beta/api/user_list_messages.md#request-2)'.",
    "Error: /concepts/outlook-create-send-messages.md:
      BookmarkSkippedDocFileNotFound: Link '[Get all the @-mention is a message](../api-reference/beta/api/message_get.md#request-2)'."
  ]
}-->

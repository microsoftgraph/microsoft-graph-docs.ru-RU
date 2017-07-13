<span data-ttu-id="82731-p117">Условия поиска указываются с использованием расширенного синтаксиса запросов (AQS). Результаты сортируются по дате и времени отправки сообщения.</span><span class="sxs-lookup"><span data-stu-id="82731-p117">Search criteria are expressed using Advanced Query Syntax (AQS). The results are sorted by the date and time that the message was sent.</span></span>

Условия поиска указываются с использованием расширенного синтаксиса запросов (AQS). Результаты сортируются по дате и времени отправки сообщения.

<span data-ttu-id="82731-194">Вы можете указать следующие свойства для объекта `message` в условии `$search`: `attachments`, `bccRecipients`, `body`, `category`, `ccRecipients`, `content`, `from`, `hasAttachments`, `participants`, `receivedDateTime`, `sender`, `subject`, `toRecipients`.</span><span class="sxs-lookup"><span data-stu-id="82731-194">You can specify the following properties on a `message` in a `$search` criterion: `attachments`, `bccRecipients`, `body`, `category`, `ccRecipients`, `content`, `from`, `hasAttachments`, `participants`, `receivedDateTime`, `sender`, `subject`, `toRecipients`</span></span>

<span data-ttu-id="82731-195">Если для поиска в сообщениях указано только значение, используются такие свойства поиска по умолчанию: `from`, `subject` и `body`.</span><span class="sxs-lookup"><span data-stu-id="82731-195">If you do a search on messages and specify only a value, the search is carried out on the default search properties of `from`, `subject` and `body`.</span></span>

<span data-ttu-id="82731-196">Следующий пример кода возвращает все сообщения из папки "Входящие" вошедшего пользователя, содержащие слово pizza в любом из трех свойств поиска по умолчанию:</span><span class="sxs-lookup"><span data-stu-id="82731-196">The following example returns all messages in the signed-in user's Inbox that contains "pizza" in any of the three default search properties:</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/messages?$search="pizza"
```

<span data-ttu-id="82731-197">Следующий пример кода выполняет поиск всех сообщений в папке "Входящие" пользователя, отправленных с определенного электронного адреса:</span><span class="sxs-lookup"><span data-stu-id="82731-197">The next example searches all messages in the user's Inbox that were sent from a specific email address:</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/messages?$search="from:help@contoso.com"
```

[graph-explorer]: https://graph.microsoft.io/en-us/graph-explorer
[odata-filter]: http://docs.oasis-open.org/odata/odata/v4.0/errata03/os/complete/part2-url-conventions/odata-v4.0-errata03-os-part2-url-conventions-complete.html#_Toc453752358
[odata-query]: http://docs.oasis-open.org/odata/odata/v4.0/errata03/os/complete/part2-url-conventions/odata-v4.0-errata03-os-part2-url-conventions-complete.html#_Toc453752356

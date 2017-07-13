<span data-ttu-id="39075-p119">Отправляйте код состояния `202 - Accepted` в ответе, отправляемом в Microsoft Graph. Если Microsoft Graph не получает код класса 2xx, он совершает несколько повторных попыток отправки уведомления.</span><span class="sxs-lookup"><span data-stu-id="39075-p119">Send a `202 - Accepted` status code in your response to Microsoft Graph. If Microsoft Graph doesn't receive a 2xx class code, it will retry resending the notification a number of times.</span></span>
3. Отправляйте код состояния `202 - Accepted` в ответе, отправляемом в Microsoft Graph. Если Microsoft Graph не получает код класса 2xx, он совершает несколько повторных попыток отправки уведомления.
  > <span data-ttu-id="39075-198">Код состояния `202 - Accepted` следует отправлять, даже если свойство clientState не совпадает со значением, отправленным в запросе на подписку.</span><span class="sxs-lookup"><span data-stu-id="39075-198">You should send a `202 - Accepted` status code even if the clientState property doesn't match the one submitted with the subscription request.</span></span>

<span data-ttu-id="39075-199">Повторяйте эти действия для других уведомлений в запросе.</span><span class="sxs-lookup"><span data-stu-id="39075-199">Repeat for other notifications in the request.</span></span>

# <span data-ttu-id="39075-200">Дополнительные ресурсы</span><span class="sxs-lookup"><span data-stu-id="39075-200">Additional resources</span></span>
<a id="additional-resources" class="xliff"></a>

* [<span data-ttu-id="39075-201">Тип ресурса Subscription</span><span class="sxs-lookup"><span data-stu-id="39075-201">Subscription resource type</span></span>](subscription.md)
* [<span data-ttu-id="39075-202">Получение подписки</span><span class="sxs-lookup"><span data-stu-id="39075-202">Get subscription</span></span>](../api/subscription_get.md)
* [<span data-ttu-id="39075-203">Создание подписки</span><span class="sxs-lookup"><span data-stu-id="39075-203">Create subscription</span></span>](../api/subscription_post_subscriptions.md)
* [<span data-ttu-id="39075-204">Пример Microsoft Graph Webhooks для Node.js</span><span class="sxs-lookup"><span data-stu-id="39075-204">Microsoft Graph Webhooks Sample for Node.js</span></span>](https://github.com/OfficeDev/Microsoft-Graph-Nodejs-Webhooks)
* [<span data-ttu-id="39075-205">Пример Microsoft Graph Webhooks для ASP.NET</span><span class="sxs-lookup"><span data-stu-id="39075-205">Microsoft Graph Webhooks Sample for ASP.NET</span></span>](https://github.com/OfficeDev/Microsoft-Graph-ASPNET-Webhooks)

<span data-ttu-id="2e402-p119">Теперь вы знаете, как вызывать Microsoft Graph, и можете создавать другие вызовы, необходимые для вашего приложения, используя справочник по API. Обратите внимание, что необходимые для вызовов разрешения настраиваются во время регистрации приложения.</span><span class="sxs-lookup"><span data-stu-id="2e402-p119">Now that you've seen how to make calls to Microsoft Graph, you can use the API reference to construct any other kinds of calls your app needs to make. However, bear in mind that your app needs to have the appropriate permissions configured on the app registration for the calls it makes.</span></span>

```
GET https://graph.microsoft.com/v1.0/me/messages?$select=subject,from,receivedDateTime&$top=25&$orderby=receivedDateTime%20DESC
Accept: application/json
Authorization: Bearer eyJ0eXAi...b66LoPVA
```

Теперь вы знаете, как вызывать Microsoft Graph, и можете создавать другие вызовы, необходимые для вашего приложения, используя справочник по API. Обратите внимание, что необходимые для вызовов разрешения настраиваются во время регистрации приложения.

## <a name="next-steps"></a><span data-ttu-id="2e402-189">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="2e402-189">Next steps</span></span>
- <span data-ttu-id="2e402-190">Попробуйте другие возможности REST API, используя [песочницу Graph](https://graph.microsoft.io/graph-explorer).</span><span class="sxs-lookup"><span data-stu-id="2e402-190">Try out more of the REST API using the [Graph explorer](https://graph.microsoft.io/graph-explorer).</span></span>

## <a name="see-also"></a><span data-ttu-id="2e402-191">См. также</span><span class="sxs-lookup"><span data-stu-id="2e402-191">See also</span></span>
- [<span data-ttu-id="2e402-192">Получение маркеров доступа для вызова Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="2e402-192">Get access tokens to call Microsoft Graph</span></span>](https://developer.microsoft.com/en-us/graph/docs/concepts/auth_overview)
- [<span data-ttu-id="2e402-193">Получение доступа от имени пользователя</span><span class="sxs-lookup"><span data-stu-id="2e402-193">Get access on behalf of a user</span></span>](https://developer.microsoft.com/en-us/graph/docs/concepts/auth_v2_user)
- [<span data-ttu-id="2e402-194">Получение доступа без пользователя</span><span class="sxs-lookup"><span data-stu-id="2e402-194">Get access without a user</span></span>](https://developer.microsoft.com/en-us/graph/docs/concepts/auth_v2_service)

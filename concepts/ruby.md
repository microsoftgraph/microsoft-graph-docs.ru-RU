<span data-ttu-id="005c2-p119">Чтобы создать сообщение, код извлекает имя пользователя из маркера сеанса и электронный адрес получателя из параметров, переданных формой. Затем код считывает текст сообщения из включенного в проект шаблона, интерполирует имя пользователя и электронный адрес и добавляет текст сообщения в текст HTTP-запроса.</span><span class="sxs-lookup"><span data-stu-id="005c2-p119">To create the email, the code pulls the user name from the session token and the recipient email address from the parameters passed from the form. The code then reads the email body from a template included in the project, interpolates the user name and email address, and attaches the email text as the HTTP request body.</span></span>

Чтобы создать сообщение, код извлекает имя пользователя из маркера сеанса и электронный адрес получателя из параметров, переданных формой. Затем код считывает текст сообщения из включенного в проект шаблона, интерполирует имя пользователя и электронный адрес и добавляет текст сообщения в текст HTTP-запроса.

<span data-ttu-id="005c2-194">Чтобы отправить сообщение, код создает HTTP-запрос, добавляет маркер доступа в качестве заголовка авторизации, а затем отправляет запрос конечной точке отправки почты.</span><span class="sxs-lookup"><span data-stu-id="005c2-194">To send the email, the code constructs the HTTP request, attaches the access token as an authorization header, and then posts the request to the send email endpoint.</span></span>

<span data-ttu-id="005c2-195">Наконец, код использует возвращенный код HTTP-ответа, чтобы сообщить пользователю, было ли сообщение успешно отправлено.</span><span class="sxs-lookup"><span data-stu-id="005c2-195">Finally, the code uses the HTTP response code returned to notify the user whether or not the email was successful.</span></span>

## <a name="run-the-app"></a><span data-ttu-id="005c2-196">Запуск приложения</span><span class="sxs-lookup"><span data-stu-id="005c2-196">Run the app</span></span>

1. <span data-ttu-id="005c2-197">Установите приложение Rails и зависимости с помощью приведенной ниже команды.</span><span class="sxs-lookup"><span data-stu-id="005c2-197">Install the Rails application and dependencies with the following command.</span></span>

    ```
    bundle install
    ```
2. <span data-ttu-id="005c2-198">Чтобы запустить приложение Rails, введите приведенную ниже команду.</span><span class="sxs-lookup"><span data-stu-id="005c2-198">To start the Rails application, type the following command.</span></span>

    ```
    rackup -p 3000
    ```
3. <span data-ttu-id="005c2-199">Введите адрес `http://localhost:3000` в веб-браузере.</span><span class="sxs-lookup"><span data-stu-id="005c2-199">Go to `http://localhost:3000` in your web browser.</span></span>

## <a name="see-also"></a><span data-ttu-id="005c2-200">См. также</span><span class="sxs-lookup"><span data-stu-id="005c2-200">See also</span></span>
- <span data-ttu-id="005c2-201">Попробуйте REST API, используя [песочницу Graph](https://graph.microsoft.io/graph-explorer).</span><span class="sxs-lookup"><span data-stu-id="005c2-201">Try out the REST API using the [Graph explorer](https://graph.microsoft.io/graph-explorer).</span></span>
- <span data-ttu-id="005c2-202">Просмотрите другие [примеры Microsoft Graph](https://github.com/microsoftgraph) на сайте GitHub.</span><span class="sxs-lookup"><span data-stu-id="005c2-202">Explore our other [Microsoft Graph samples](https://github.com/microsoftgraph) on GitHub.</span></span>
- [<span data-ttu-id="005c2-203">Получение маркеров доступа для вызова Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="005c2-203">Get access tokens to call Microsoft Graph</span></span>](https://developer.microsoft.com/en-us/graph/docs/concepts/auth_overview)
- [<span data-ttu-id="005c2-204">Получение доступа от имени пользователя</span><span class="sxs-lookup"><span data-stu-id="005c2-204">Get access on behalf of a user</span></span>](https://developer.microsoft.com/en-us/graph/docs/concepts/auth_v2_user)
- [<span data-ttu-id="005c2-205">Получение доступа без пользователя</span><span class="sxs-lookup"><span data-stu-id="005c2-205">Get access without a user</span></span>](https://developer.microsoft.com/en-us/graph/docs/concepts/auth_v2_service)



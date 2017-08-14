<span data-ttu-id="defe6-p103">В случае успешного выполнения этот метод возвращает код отклика `200, OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="defe6-p103">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>

В случае успешного выполнения этот метод возвращает код отклика `200, OK`. В тексте отклика не возвращается никаких данных.

## <a name="example"></a><span data-ttu-id="defe6-129">Пример</span><span class="sxs-lookup"><span data-stu-id="defe6-129">Example</span></span>
<span data-ttu-id="defe6-130">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="defe6-130">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="defe6-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="defe6-131">Request</span></span>
<span data-ttu-id="defe6-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="defe6-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "event_snoozereminder"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/events/{id}/snoozeReminder
Content-type: application/json
Content-length: 97

{
  "newReminderTime": {
    "dateTime": "dateTime-value",
    "timeZone": "timeZone-value"
  }
}
```

##### <a name="response"></a><span data-ttu-id="defe6-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="defe6-133">Response</span></span>
<span data-ttu-id="defe6-134">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="defe6-134">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "event: snoozeReminder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

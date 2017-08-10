<span data-ttu-id="d2c11-p112">Примечание. Показанный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d2c11-p112">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

Примечание. Показанный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.event",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 359

{
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/me/calendarview/delta?$skiptoken={_skipToken_}",
  "value": [
    {
      "originalStartTimeZone": "originalStartTimeZone-value",
      "originalEndTimeZone": "originalEndTimeZone-value",
      "responseStatus": {
        "response": "response-value",
        "time": "datetime-value"
      },
      "iCalUId": "iCalUId-value",
      "reminderMinutesBeforeStart": 99,
      "isReminderOn": true
    }
  ]
}
```

### <a name="see-also"></a><span data-ttu-id="d2c11-166">См. также</span><span class="sxs-lookup"><span data-stu-id="d2c11-166">See also</span></span>

- [<span data-ttu-id="d2c11-167">Отслеживание изменений данных Microsoft Graph с помощью разностного запроса</span><span class="sxs-lookup"><span data-stu-id="d2c11-167">Use delta query to track changes in Microsoft Graph data</span></span>](../../../concepts/delta_query_overview.md)
- [<span data-ttu-id="d2c11-168">Получение добавочных изменений событий в календаре</span><span class="sxs-lookup"><span data-stu-id="d2c11-168">Get incremental changes to events in a calendar</span></span>](../../../concepts/delta_query_events.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "event: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
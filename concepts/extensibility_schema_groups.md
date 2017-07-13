<span data-ttu-id="0d12f-p109">Приведенный ниже пример запроса ищет группу с расширением `graphlearn_courses`, для которой значение свойства `courseId` соответствует `123`, и получает свойства группы **displayName**, **id** и **description**, а также пользовательские данные расширения `graphlearn_courses`. (Выполняя реальный запрос, по необходимости применяйте URL-кодировку.)</span><span class="sxs-lookup"><span data-stu-id="0d12f-p109">The following example looks for the group that has the `graphlearn_courses` extension with a `courseId` property value matching `123`, and gets the group properties **displayName**, **id**, and **description**, and the custom data in the `graphlearn_courses` extension. (In the actual query, make sure you apply URL encoding as necessary.)</span></span>

Приведенный ниже пример запроса ищет группу с расширением `graphlearn_courses`, для которой значение свойства `courseId` соответствует `123`, и получает свойства группы **displayName**, **id** и **description**, а также пользовательские данные расширения `graphlearn_courses`. (Выполняя реальный запрос, по необходимости применяйте URL-кодировку.)

#### <span data-ttu-id="0d12f-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="0d12f-157">Request</span></span>
<a id="request" class="xliff"></a>

```http
GET https://graph.microsoft.com/v1.0/groups?$filter=graphlearn_courses/courseId eq ‘123’&$select=displayName,id,description,graphlearn_courses
```


##### <span data-ttu-id="0d12f-158">Ответ</span><span class="sxs-lookup"><span data-stu-id="0d12f-158">Response</span></span>
<a id="response" class="xliff"></a>
```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-length: 326
{
  "value": [
    {
      "displayName": "New Managers March 2017",
      "id": "14429ae5-3e74-41a2-9fa8-028fbb984637",
      "description": "New Managers training course for March 2017",
      "graphlearn_courses": {
        "@odata.type": "#microsoft.graph.ComplexExtensionValue",
        "courseId":"123",
        "courseName":"New Managers",
        "courseType":"Online"
      }
    }
  ]
}
```

## <span data-ttu-id="0d12f-159">См. также</span><span class="sxs-lookup"><span data-stu-id="0d12f-159">See also</span></span>
<a id="see-also" class="xliff"></a>

- [<span data-ttu-id="0d12f-160">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="0d12f-160">Add custom data to resources using extensions</span></span>](extensibility_overview.md)
- [<span data-ttu-id="0d12f-161">Добавление пользовательских данных в ресурсы user с помощью открытых расширений (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="0d12f-161">Add custom data to users using open extensions (preview)</span></span>](extensibility_open_users.md)
- <span data-ttu-id="0d12f-162">
  [Домены Office 365](https://technet.microsoft.com/en-us/library/office-365-domains.aspx)</span><span class="sxs-lookup"><span data-stu-id="0d12f-162">[Office 365 domains](https://technet.microsoft.com/en-us/library/office-365-domains.aspx)</span></span>
- [<span data-ttu-id="0d12f-163">Добавление и проверка домена для НОВОГО плана Office 365</span><span class="sxs-lookup"><span data-stu-id="0d12f-163">Adding and Verifying a Domain for the NEW Office 365</span></span>](http://office365support.ca/adding-and-verifying-a-domain-for-the-new-office-365/)
- [<span data-ttu-id="0d12f-164">Тип ресурса schemaExtension</span><span class="sxs-lookup"><span data-stu-id="0d12f-164">schemaExtension resource type</span></span>](../api-reference/v1.0/resources/schemaextension.md)
- [<span data-ttu-id="0d12f-165">Перечисление schemaExtensions</span><span class="sxs-lookup"><span data-stu-id="0d12f-165">List schemaExtensions</span></span>](../api-reference/v1.0/api/schemaextension_list.md)
- [<span data-ttu-id="0d12f-166">Создание schemaExtension</span><span class="sxs-lookup"><span data-stu-id="0d12f-166">Create schemaExtension</span></span>](../api-reference/v1.0/api/schemaextension_post_schemaextensions.md)
- [<span data-ttu-id="0d12f-167">Получение schemaExtension</span><span class="sxs-lookup"><span data-stu-id="0d12f-167">Get schemaExtension</span></span>](../api-reference/v1.0/api/schemaextension_get.md)
- [<span data-ttu-id="0d12f-168">Обновление schemaExtension</span><span class="sxs-lookup"><span data-stu-id="0d12f-168">Update schemaExtension</span></span>](../api-reference/v1.0/api/schemaextension_update.md)
- [<span data-ttu-id="0d12f-169">Удаление schemaExtension</span><span class="sxs-lookup"><span data-stu-id="0d12f-169">Delete schemaExtension</span></span>](../api-reference/v1.0/api/schemaextension_delete.md)

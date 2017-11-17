<span data-ttu-id="a6917-p107">Пользователь решает, что ему не больше не нужен перемещаемый профиль, и удаляет его. Это можно сделать с помощью запроса ```DELETE``` со значением открытого расширения.</span><span class="sxs-lookup"><span data-stu-id="a6917-p107">The user decides that they don't want a roaming profile anymore, so they delete it. This can be done with a ```DELETE``` request on the open extension value.</span></span>
Пользователь решает, что ему не больше не нужен перемещаемый профиль, и удаляет его. Это можно сделать с помощью запроса ```DELETE``` со значением открытого расширения.

##### <a name="request"></a><span data-ttu-id="a6917-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="a6917-135">Request</span></span>
```http
DELETE https://graph.microsoft.com/v1.0/me/extensions/com.contoso.roamingSettings
```

##### <a name="response"></a><span data-ttu-id="a6917-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="a6917-136">Response</span></span>
```
HTTP/1.1 204 No content
```

## <a name="see-also"></a><span data-ttu-id="a6917-137">См. также</span><span class="sxs-lookup"><span data-stu-id="a6917-137">See also</span></span>

- [<span data-ttu-id="a6917-138">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="a6917-138">Add custom data to resources using extensions</span></span>](extensibility_overview.md)
- [<span data-ttu-id="a6917-139">Добавление пользовательских данных в группы с помощью расширений схемы</span><span class="sxs-lookup"><span data-stu-id="a6917-139">Add custom data to groups using schema extensions</span></span>](extensibility_schema_groups.md)
- [<span data-ttu-id="a6917-140">Тип ресурса openTypeExtension</span><span class="sxs-lookup"><span data-stu-id="a6917-140">openTypeExtension resource type</span></span>](../api-reference/v1.0/resources/opentypeextension.md)
- [<span data-ttu-id="a6917-141">Создание открытого расширения</span><span class="sxs-lookup"><span data-stu-id="a6917-141">Create open extension</span></span>](../api-reference/v1.0/api/opentypeextension_post_opentypeextension.md)
- [<span data-ttu-id="a6917-142">Получение открытого расширения</span><span class="sxs-lookup"><span data-stu-id="a6917-142">Get open extension</span></span>](../api-reference/v1.0/api/opentypeextension_get.md)
- [<span data-ttu-id="a6917-143">Обновление открытого расширения</span><span class="sxs-lookup"><span data-stu-id="a6917-143">Update open extension</span></span>](../api-reference/v1.0/api/opentypeextension_update.md)
- [<span data-ttu-id="a6917-144">Удаление открытого расширения</span><span class="sxs-lookup"><span data-stu-id="a6917-144">Delete open extension</span></span>](../api-reference/v1.0/api/opentypeextension_delete.md)
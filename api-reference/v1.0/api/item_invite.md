<span data-ttu-id="612a7-p102">Сообщение с обычным форматированным текстом, включенное в приглашение на доступ. Максимальная длина составляет 2000 символов.</span><span class="sxs-lookup"><span data-stu-id="612a7-p102">A plain text formatted message that is included in the sharing invitation. Maximum length 2000 characters.</span></span>                                          | Сообщение с обычным форматированным текстом, включенное в приглашение на доступ. Максимальная длина составляет 2000 символов. |
| <span data-ttu-id="612a7-122">requireSignIn</span><span class="sxs-lookup"><span data-stu-id="612a7-122">requireSignIn</span></span>    | <span data-ttu-id="612a7-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="612a7-123">Boolean</span></span>                                         | <span data-ttu-id="612a7-124">Указывает, куда должен зайти получатель приглашения, чтобы просмотреть элемент, к которому предоставлен общий доступ.</span><span class="sxs-lookup"><span data-stu-id="612a7-124">Specifies where the recipient of the invitation is required to sign-in to view the shared item.</span></span>            |
| <span data-ttu-id="612a7-125">sendInvitation</span><span class="sxs-lookup"><span data-stu-id="612a7-125">sendInvitation</span></span>   | <span data-ttu-id="612a7-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="612a7-126">Boolean</span></span>                                         | <span data-ttu-id="612a7-127">Указывает, создано ли электронное письмо или запись (false) или разрешение (true).</span><span class="sxs-lookup"><span data-stu-id="612a7-127">Specifies if an email or post is generated (false) or if the permission is just created (true).</span></span>            |
| <span data-ttu-id="612a7-128">roles</span><span class="sxs-lookup"><span data-stu-id="612a7-128">roles</span></span>            | <span data-ttu-id="612a7-129">Collection(String)</span><span class="sxs-lookup"><span data-stu-id="612a7-129">Collection(String)</span></span>                              | <span data-ttu-id="612a7-130">Указывают роли, которые предоставляются получателям приглашения на доступ.</span><span class="sxs-lookup"><span data-stu-id="612a7-130">Specify the roles that are be granted to the recipients of the sharing invitation.</span></span>                         |

## <span data-ttu-id="612a7-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="612a7-131">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="612a7-132">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и объект коллекции [permission](../resources/permission.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="612a7-132">If successful, this method returns `200 OK` response code and [permission](../resources/permission.md) collection object in the response body.</span></span>

## <span data-ttu-id="612a7-133">Пример</span><span class="sxs-lookup"><span data-stu-id="612a7-133">Example</span></span>
<a id="example" class="xliff"></a>
<span data-ttu-id="612a7-134">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="612a7-134">Here is an example of how to call this API.</span></span>

##### <span data-ttu-id="612a7-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="612a7-135">Request</span></span>
<a id="request" class="xliff"></a>
<span data-ttu-id="612a7-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="612a7-136">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "item_invite"
}-->
```http
POST https://graph.microsoft.com/v1.0/drive/items/{item-id}/invite
Content-type: application/json

{
  "recipients": [
    {
      "email": "ryan@contoso.org"
    }
  ],
  "message": "Here's the file that we're collaborating on.",
  "requireSignIn": true,
  "sendInvitation": true,
  "roles": [ "write" ]
}
```

##### <span data-ttu-id="612a7-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="612a7-137">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="612a7-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="612a7-138">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.permission",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "grantedTo": {
        "user": {
          "displayName": "Ryan Gregg",
          "id": "42F177F1-22C0-4BE3-900D-4507125C5C20"
        }
      },
      "id": "CCFC7CA3-7A19-4D57-8CEF-149DB9DDFA62",
      "invitation": {
        "email": "ryan@contoso.com",
        "signInRequired": true
      },
      "roles": [ "write" ]
    }
  ]
}
```

## <span data-ttu-id="612a7-139">Заметки</span><span class="sxs-lookup"><span data-stu-id="612a7-139">Remarks</span></span>
<a id="remarks" class="xliff"></a>

* <span data-ttu-id="612a7-140">[Диски](../resources/drive.md), у которых для свойства **driveType** задано значение `personal` (личное хранилище OneDrive), не могут создавать и изменять разрешения в корневом ресурсе DriveItem.</span><span class="sxs-lookup"><span data-stu-id="612a7-140">[Drives](../resources/drive.md) with a **driveType** of `personal` (OneDrive Personal) cannot create or modify permissions on the root DriveItem.</span></span> 
* <span data-ttu-id="612a7-141">Список доступных ролей см. в таблице [Перечисление ролей](../resources/permission.md#roles-enumeration).</span><span class="sxs-lookup"><span data-stu-id="612a7-141">For a list of available roles, see [Roles enumeration](../resources/permission.md#roles-enumeration).</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->

<!-- {
  "type": "#page.annotation",
  "description": "item: invite",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

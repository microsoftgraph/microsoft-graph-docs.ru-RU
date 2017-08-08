<span data-ttu-id="57dfe-p101">Так как элемент [**SharedDriveItem**](../resources/shareddriveitem.md) содержит полезную информацию, большинство приложений будут стремиться получить прямой доступ к общему элементу [DriveItem](../resources/driveitem.md). Ресурс **SharedDriveItem** включает связи **корня** и **элементов**, которые могут получать доступ к содержимому в области общего элемента.</span><span class="sxs-lookup"><span data-stu-id="57dfe-p101">While the [**SharedDriveItem**](../resources/shareddriveitem.md) contains some useful information, most apps will want to directly access the shared [DriveItem](../resources/driveitem.md). The **SharedDriveItem** resource includes a **root** and **items** relationships which can access content within the scope of the shared item.</span></span>

Так как элемент [**SharedDriveItem**](../resources/shareddriveitem.md) содержит полезную информацию, большинство приложений будут стремиться получить прямой доступ к общему элементу [DriveItem](../resources/driveitem.md). Ресурс **SharedDriveItem** включает связи **корня** и **элементов**, которые могут получать доступ к содержимому в области общего элемента.

## <a name="example-single-file"></a><span data-ttu-id="57dfe-122">Пример (один файл)</span><span class="sxs-lookup"><span data-stu-id="57dfe-122">Example (single file)</span></span>

##### <a name="request"></a><span data-ttu-id="57dfe-123">Запрос</span><span class="sxs-lookup"><span data-stu-id="57dfe-123">Request</span></span>

<span data-ttu-id="57dfe-124">При запросе связи **корня** будет возвращен элемент **DriveItem**, к которому был предоставлен доступ.</span><span class="sxs-lookup"><span data-stu-id="57dfe-124">By requesting the **root** relationship, the **DriveItem** that was shared will be returned.</span></span>

```http
GET https://graph.microsoft.com/v1.0/shares/{shareIdOrUrl}/root
```

##### <a name="response"></a><span data-ttu-id="57dfe-125">Ответ</span><span class="sxs-lookup"><span data-stu-id="57dfe-125">Response</span></span>

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "id": "9FFFDB3C-5B87-4062-9606-1B008CA88E44",
  "name": "contoso project.docx",
  "eTag": "2246BD2D-7811-4660-BD0F-1CF36133677B,1",
  "file": {},
  "size": 109112
}
```

## <a name="example-shared-folder"></a><span data-ttu-id="57dfe-126">Пример (общая папка)</span><span class="sxs-lookup"><span data-stu-id="57dfe-126">Example (shared folder)</span></span>

##### <a name="request"></a><span data-ttu-id="57dfe-127">Запрос</span><span class="sxs-lookup"><span data-stu-id="57dfe-127">Request</span></span>

<span data-ttu-id="57dfe-128">При запросе связи **корня** и расширении **дочерней** коллекции будет возвращен элемент **DriveItem**, к которому был предоставлен доступ, а также файлы в общей папке.</span><span class="sxs-lookup"><span data-stu-id="57dfe-128">By requesting the **root** relationship and expanding the **children** collection, the **DriveItem** that was shared will be returned along with the files within the shared folder.</span></span>

```http
GET https://graph.microsoft.com/v1.0/shares/{shareIdOrUrl}/root?$expand=children
```

##### <a name="response"></a><span data-ttu-id="57dfe-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="57dfe-129">Response</span></span>

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "id": "9FFFDB3C-5B87-4062-9606-1B008CA88E44",
  "name": "Contoso Project",
  "eTag": "2246BD2D-7811-4660-BD0F-1CF36133677B,1",
  "folder": {}
  "size": 10911212,
  "children": [
    {
      "id": "AFBBDD79-868E-452D-AD4D-24697D4A4044",
      "name": "Propsoal.docx",
      "file": {},
      "size": 19001
    },
    {
      "id": "A91FE90A-2F2C-4EE6-B412-C4FFBA3F71A6",
      "name": "Update to Proposal.docx",
      "file": {},
      "size": 91001
    }
  ]
}
```

## <a name="transform-a-sharing-url"></a><span data-ttu-id="57dfe-130">Преобразование URL-адреса для совместного доступа</span><span class="sxs-lookup"><span data-stu-id="57dfe-130">Transform a sharing URL</span></span>

<span data-ttu-id="57dfe-131">Чтобы получить доступ к URL-адресу для совместного доступа с помощью API **общих ресурсов**, необходимо преобразовать URL-адрес в токен для совместного доступа.</span><span class="sxs-lookup"><span data-stu-id="57dfe-131">To access a sharing URL using the **shares** API, the URL needs to be transformed into a sharing token.</span></span>

<span data-ttu-id="57dfe-132">Чтобы преобразовать URL-адрес в токен для совместного доступа, выполните указанные ниже действия.</span><span class="sxs-lookup"><span data-stu-id="57dfe-132">To transform a URL into a sharing token:</span></span>

1. <span data-ttu-id="57dfe-133">Закодируйте URL-адрес для общего доступа с использованием кодировки Base64.</span><span class="sxs-lookup"><span data-stu-id="57dfe-133">Base64 encode the sharing URL.</span></span>
2. <span data-ttu-id="57dfe-134">Преобразуйте данные в кодировке Base64 в [формат URL-адреса с недополненной кодировкой Base64](https://en.wikipedia.org/wiki/Base64), выполнив указанные ниже действия.</span><span class="sxs-lookup"><span data-stu-id="57dfe-134">Convert the base64 encoded data to [unpadded base64url format](https://en.wikipedia.org/wiki/Base64) by:</span></span>
  1. <span data-ttu-id="57dfe-135">Удалите символы `=` в конце строки.</span><span class="sxs-lookup"><span data-stu-id="57dfe-135">Trim trailing `=` characters from the string</span></span>
  2. <span data-ttu-id="57dfe-136">Замените небезопасные символы URL-адреса на эквивалентные символы; замените `/` на `_`, а `+` — на `-`.</span><span class="sxs-lookup"><span data-stu-id="57dfe-136">Replace unsafe URL characters with an equivalent character; replace `/` with `_` and `+` with `-`.</span></span>
3. <span data-ttu-id="57dfe-137">Добавьте `u!` в начало строки.</span><span class="sxs-lookup"><span data-stu-id="57dfe-137">Append `u!` to the beginning of the string.</span></span>

<span data-ttu-id="57dfe-138">Например, указанный ниже метод C# преобразует входную строку в токен общего доступа.</span><span class="sxs-lookup"><span data-stu-id="57dfe-138">For example, the following C# method transforms an input string into a sharing token:</span></span>

```csharp
string UrlToSharingToken(string inputUrl) {
  var base64Value = System.Convert.ToBase64String(System.Text.Encoding.UTF8.GetBytes(inputUrl));
  return "u!" + base64Value.TrimEnd('=').Replace('/','_').Replace('+','-');
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update permission",
  "keywords": "",
  "section": "documentation",
  "tocPath": "OneDrive/Item/Update permission"
}-->

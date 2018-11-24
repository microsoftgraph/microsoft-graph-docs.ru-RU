# <a name="get-photo"></a><span data-ttu-id="4c830-101">Получение фотографии</span><span class="sxs-lookup"><span data-stu-id="4c830-101">Get photo</span></span>

<span data-ttu-id="4c830-102">Получение указанного объекта [profilePhoto](../resources/profilephoto.md) или его метаданных (свойств profilePhoto).</span><span class="sxs-lookup"><span data-stu-id="4c830-102">Get the specified [profilePhoto](../resources/profilephoto.md) or its metadata (profilePhoto properties).</span></span>

> <span data-ttu-id="4c830-103">**Примечание.** Эта операция в версии 1.0 поддерживает только рабочие или учебные почтовые ящики пользователя (не личные).</span><span class="sxs-lookup"><span data-stu-id="4c830-103">**Note** This operation in version 1.0 supports only a user's work or school mailboxes and not personal mailboxes.</span></span>

<span data-ttu-id="4c830-104">Поддерживаемые размеры фотографий в формате HD для Office 365: 48 x 48, 64 x 64, 96 x 96, 120 x 120, 240 x 240, 360 x 360, 432 x 432, 504 x 504 и 648 x 648.</span><span class="sxs-lookup"><span data-stu-id="4c830-104">The supported sizes of HD photos on Office 365 are as follows: '48x48', '64x64', '96x96', '120x120', '240x240', '360x360','432x432', '504x504', and '648x648'.</span></span> <span data-ttu-id="4c830-105">Фотографии могут быть любого размера, если они хранятся в Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="4c830-105">Photos can be any dimension if they are stored in Azure Active Directory.</span></span>

<span data-ttu-id="4c830-106">Вы можете получить метаданные самой большой доступной фотографии или указать размер и получить метаданные для этого размера.</span><span class="sxs-lookup"><span data-stu-id="4c830-106">You can get the metadata of the largest available photo, or specify a size to get the metadata for that photo size.</span></span>
<span data-ttu-id="4c830-107">Если запрашиваемый размер недоступен, вы можете получить меньший размер, загруженный пользователем.</span><span class="sxs-lookup"><span data-stu-id="4c830-107">If the size you request is not available, you can still get a smaller size that the user has uploaded and made available.</span></span>
<span data-ttu-id="4c830-108">Например, если пользователь загрузит фотографию размером 504 x 504 пикселя, для скачивания будут доступны все размеры, кроме 648 x 648.</span><span class="sxs-lookup"><span data-stu-id="4c830-108">For example, if the user uploads a photo that is 504x504 pixels, then all but the 648x648 size of photo will be available for download.</span></span>

## <a name="permissions"></a><span data-ttu-id="4c830-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4c830-109">Permissions</span></span>

<span data-ttu-id="4c830-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="4c830-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="4c830-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4c830-112">Permission type</span></span>      | <span data-ttu-id="4c830-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4c830-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4c830-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4c830-114">Delegated (work or school account)</span></span> | <span data-ttu-id="4c830-115">Для ресурса **user**:</span><span class="sxs-lookup"><span data-stu-id="4c830-115">For **user** resource:</span></span><br/><span data-ttu-id="4c830-116">User.Read, User.ReadBasic.All, User.Read.All, User.ReadWrite, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4c830-116">User.Read, User.ReadBasic.All, User.Read.All, User.ReadWrite, User.ReadWrite.All</span></span><br /><br /><span data-ttu-id="4c830-117">Для ресурса **group**:</span><span class="sxs-lookup"><span data-stu-id="4c830-117">For **group** resource:</span></span><br /><span data-ttu-id="4c830-118">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4c830-118">Group.Read.All, Group.ReadWrite.All</span></span><br /><br /><span data-ttu-id="4c830-119">Для ресурса **contact**:</span><span class="sxs-lookup"><span data-stu-id="4c830-119">For **contact** resource:</span></span><br /><span data-ttu-id="4c830-120">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4c830-120">Contacts.Read, Contacts.ReadWrite</span></span> |
|<span data-ttu-id="4c830-121">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4c830-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4c830-122">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="4c830-122">Not supported</span></span> |
|<span data-ttu-id="4c830-123">Разрешения приложений</span><span class="sxs-lookup"><span data-stu-id="4c830-123">Application</span></span>                        | <span data-ttu-id="4c830-124">Для ресурса **user**:</span><span class="sxs-lookup"><span data-stu-id="4c830-124">For **user** resource:</span></span><br/><span data-ttu-id="4c830-125">User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4c830-125">User.Read.All, User.ReadWrite.All</span></span><br /><br /><span data-ttu-id="4c830-126">Для ресурса **group**:</span><span class="sxs-lookup"><span data-stu-id="4c830-126">For **group** resource:</span></span><br /><span data-ttu-id="4c830-127">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4c830-127">Group.Read.All, Group.ReadWrite.All</span></span><br /><br /><span data-ttu-id="4c830-128">Для ресурса **contact**:</span><span class="sxs-lookup"><span data-stu-id="4c830-128">For **contact** resource:</span></span><br /><span data-ttu-id="4c830-129">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4c830-129">Contacts.Read, Contacts.ReadWrite</span></span> |


## <a name="http-request"></a><span data-ttu-id="4c830-130">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4c830-130">HTTP request</span></span> 

### <a name="get-the-photo"></a><span data-ttu-id="4c830-131">Получение фотографий</span><span class="sxs-lookup"><span data-stu-id="4c830-131">Get the photo</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/photo/$value
GET /users/{id | userPrincipalName}/photo/$value
GET /groups/{id}/photo/$value
GET /me/contacts/{id}/photo/$value
GET /users/{id | userPrincipalName}/contacts/{id}/photo/$value
GET /me/contactfolders/{contactFolderId}/contacts/{id}/photo/$value
GET /users/{id | userPrincipalName}/contactfolders/{contactFolderId}/contacts/{id}/photo/$value
```
### <a name="get-the-metadata-of-the-photo"></a><span data-ttu-id="4c830-132">Получение метаданных фотографии</span><span class="sxs-lookup"><span data-stu-id="4c830-132">Get the metadata of the photo</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/photo
GET /me/photos
GET /users/{id | userPrincipalName}/photo
GET /groups/{id}/photo
GET /me/contacts/{id}/photo
GET /users/{id | userPrincipalName}/contacts/{id}/photo
GET /me/contactfolders/{contactFolderId}/contacts/{id}/photo
GET /users/{id | userPrincipalName}/contactfolders/{contactFolderId}/contacts/{id}/photo
```

### <a name="get-the-metadata-for-a-specific-photo-size"></a><span data-ttu-id="4c830-133">Получить метаданные для определенного размера фотографии</span><span class="sxs-lookup"><span data-stu-id="4c830-133">Get the metadata for a specific photo size</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/photos/{size}
GET /users/{id | userPrincipalName}/photos/{size}
GET /groups/{id}/photos/{size}
GET /me/contacts/{id}/photos/{size}
GET /users/{id | userPrincipalName}/contacts/{id}/photos/{size}
GET /me/contactfolders/{contactFolderId}/contacts/{id}/photos/{size}
GET /users/{id | userPrincipalName}/contactfolders/{contactFolderId}/contacts/{id}/photos/{size}
```

## <a name="path-parameters"></a><span data-ttu-id="4c830-134">Параметры пути</span><span class="sxs-lookup"><span data-stu-id="4c830-134">Path parameters</span></span>

|<span data-ttu-id="4c830-135">Параметр</span><span class="sxs-lookup"><span data-stu-id="4c830-135">Parameter</span></span>|<span data-ttu-id="4c830-136">Тип</span><span class="sxs-lookup"><span data-stu-id="4c830-136">Type</span></span>|<span data-ttu-id="4c830-137">Описание</span><span class="sxs-lookup"><span data-stu-id="4c830-137">Description</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="4c830-138">size</span><span class="sxs-lookup"><span data-stu-id="4c830-138">size</span></span>  |<span data-ttu-id="4c830-139">String</span><span class="sxs-lookup"><span data-stu-id="4c830-139">String</span></span>  | <span data-ttu-id="4c830-140">Размер фотографии.</span><span class="sxs-lookup"><span data-stu-id="4c830-140">A photo size.</span></span> <span data-ttu-id="4c830-141">Поддерживаемые размеры фотографий в формате HD для Office 365: 48 x 48, 64 x 64, 96 x 96, 120 x 120, 240 x 240, 360 x 360, 432 x 432, 504 x 504 и 648 x 648.</span><span class="sxs-lookup"><span data-stu-id="4c830-141">The supported sizes of HD photos on Office 365 are as follows: '48x48', '64x64', '96x96', '120x120', '240x240', '360x360','432x432', '504x504', and '648x648'.</span></span> <span data-ttu-id="4c830-142">Фотографии могут быть любого размера, если они хранятся в Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="4c830-142">Photos can be any dimension if they are stored in Azure Active Directory.</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="4c830-143">Необязательные параметры запроса</span><span class="sxs-lookup"><span data-stu-id="4c830-143">Optional query parameters</span></span>
<span data-ttu-id="4c830-144">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="4c830-144">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4c830-145">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4c830-145">Request headers</span></span>
| <span data-ttu-id="4c830-146">Имя</span><span class="sxs-lookup"><span data-stu-id="4c830-146">Name</span></span>       | <span data-ttu-id="4c830-147">Тип</span><span class="sxs-lookup"><span data-stu-id="4c830-147">Type</span></span> | <span data-ttu-id="4c830-148">Описание</span><span class="sxs-lookup"><span data-stu-id="4c830-148">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="4c830-149">Authorization</span><span class="sxs-lookup"><span data-stu-id="4c830-149">Authorization</span></span>  | <span data-ttu-id="4c830-150">string</span><span class="sxs-lookup"><span data-stu-id="4c830-150">string</span></span>  | <span data-ttu-id="4c830-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4c830-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4c830-153">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4c830-153">Request body</span></span>
<span data-ttu-id="4c830-154">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4c830-154">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4c830-155">Ответ</span><span class="sxs-lookup"><span data-stu-id="4c830-155">Response</span></span>
### <a name="response-for-getting-the-photo"></a><span data-ttu-id="4c830-156">Отклик для запроса на получение фотографии</span><span class="sxs-lookup"><span data-stu-id="4c830-156">Response for getting the photo</span></span>
<span data-ttu-id="4c830-p106">При успешном выполнении этот метод возвращает код отклика `200 OK` и двоичные данные запрашиваемой фотографии.  Если фотография не существует, операция возвратит отклик `404 Not Found`.</span><span class="sxs-lookup"><span data-stu-id="4c830-p106">If successful, this method returns a `200 OK` response code and binary data of the requested photo.  If no photo exists, the operation returns `404 Not Found`.</span></span>
### <a name="response-for-getting-the-metadata-of-the-photo"></a><span data-ttu-id="4c830-159">Отклик для запроса на получение метаданных фотографии</span><span class="sxs-lookup"><span data-stu-id="4c830-159">Response for getting the metadata of the photo</span></span>
<span data-ttu-id="4c830-160">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [profilePhoto](../resources/profilePhoto.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4c830-160">If successful, this method returns a `200 OK` response code and [profilePhoto](../resources/profilePhoto.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="4c830-161">Пример</span><span class="sxs-lookup"><span data-stu-id="4c830-161">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="4c830-162">Запрос 1</span><span class="sxs-lookup"><span data-stu-id="4c830-162">Request 1</span></span>
<span data-ttu-id="4c830-163">Этот запрос возвращает фотографию пользователя, вошедшего в систему, с максимальным доступным размером.</span><span class="sxs-lookup"><span data-stu-id="4c830-163">This request gets the photo for the signed-in user, in the largest available size.</span></span>
<!-- {
  "blockType": "ignored"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/photo/$value
```

##### <a name="response-1"></a><span data-ttu-id="4c830-164">Отклик 1</span><span class="sxs-lookup"><span data-stu-id="4c830-164">Response 1</span></span>
<span data-ttu-id="4c830-p107">Содержит двоичные данные запрошенной фотографии. Код HTTP-отклика: 200.</span><span class="sxs-lookup"><span data-stu-id="4c830-p107">Contains the binary data of the requested photo. The HTTP response code is 200.</span></span>

##### <a name="request-2"></a><span data-ttu-id="4c830-167">Запрос 2</span><span class="sxs-lookup"><span data-stu-id="4c830-167">Request 2</span></span>
<span data-ttu-id="4c830-168">Этот запрос получает фотографию 48 x 48 для вошедшего пользователя.</span><span class="sxs-lookup"><span data-stu-id="4c830-168">This request gets the 48x48 photo for the signed-in user.</span></span>

<!-- {
  "blockType": "ignored"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/photos/48x48/$value
Content-Type: image/jpg
```

##### <a name="response-2"></a><span data-ttu-id="4c830-169">Ответ 2</span><span class="sxs-lookup"><span data-stu-id="4c830-169">Response 2</span></span>
<span data-ttu-id="4c830-170">Содержит двоичные данные запрошенной фотографии 48 x 48.</span><span class="sxs-lookup"><span data-stu-id="4c830-170">Contains the binary data of the requested 48x48 photo.</span></span> <span data-ttu-id="4c830-171">Код HTTP-ответа: 200.</span><span class="sxs-lookup"><span data-stu-id="4c830-171">The HTTP response code is 200.</span></span>

##### <a name="request-3"></a><span data-ttu-id="4c830-172">Запрос 3</span><span class="sxs-lookup"><span data-stu-id="4c830-172">Request 3</span></span>
<span data-ttu-id="4c830-173">Этот запрос возвращает метаданные фотографии вошедшего пользователя.</span><span class="sxs-lookup"><span data-stu-id="4c830-173">This request gets the metadata of the user photo of the signed-in user.</span></span>
<!-- {
  "blockType": "ignored"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/photo
```

##### <a name="response-3"></a><span data-ttu-id="4c830-174">Ответ 3</span><span class="sxs-lookup"><span data-stu-id="4c830-174">Response 3</span></span>

<span data-ttu-id="4c830-p109">В данных указанного ниже ответа содержатся метаданные фотографии. Примечание. Показанный здесь объект ответа может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="4c830-p109">The following response data shows the photo metadata. Note: The response object shown here may be truncated for brevity.</span></span>
<!-- {
  "blockType": "ignored"
}-->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Me/photo/$entity",
    "@odata.id": "https://graph.microsoft.com/v1.0/users('ddfcd489-628b-7d04-b48b-20075df800e5@1717622f-1d94-c0d4-9d74-f907ad6677b4')/photo",
    "@odata.mediaContentType": "image/jpeg",
    "@odata.mediaEtag": "\"BA09D118\"",
    "id": "240X240",
    "width": 240,
    "height": 240
}
```

<span data-ttu-id="4c830-p110">Ниже показаны данные отклика в случае, если фотография пользователя еще не выложена. Примечание. Показанный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="4c830-p110">The following response data shows the contents of a response when a photo hasn't already been uploaded for the user. Note: The response object shown here may be truncated for brevity.</span></span>

<!-- {
  "blockType": "ignored"
}-->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Me/photo/$entity",
    "@odata.id": "https://graph.microsoft.com/v1.0/users('ddfcd489-628b-7d04-b48b-20075df800e5@1717622f-1d94-c0d4-9d74-f907ad6677b4')/photo",
    "@odata.mediaContentType": "image/gif",
    "@odata.mediaEtag": "",
    "id": "1X1",
    "width": 1,
    "height": 1
}
```
## <a name="using-the-binary-data-of-the-requested-photo"></a><span data-ttu-id="4c830-179">Использование двоичных данных запрошенной фотографии</span><span class="sxs-lookup"><span data-stu-id="4c830-179">Using the binary data of the requested photo</span></span>

<span data-ttu-id="4c830-180">Когда вы используете конечную точку `/photo/$value` для получения двоичных данных для фотографии профиля, потребуется преобразовать эти данные в строку Base64, чтобы добавить их как вложение электронной почты.</span><span class="sxs-lookup"><span data-stu-id="4c830-180">When you use the `/photo/$value` endpoint to get the binary data for a profile photo, you'll need to convert the data into a base-64 string in order to add it as an email attachment.</span></span> <span data-ttu-id="4c830-181">Ниже приведен пример кода JavaScript, показывающий, как создать массив, который можно передать как значение параметра `Attachments` для [сообщения Outlook](user_post_messages.md).</span><span class="sxs-lookup"><span data-stu-id="4c830-181">Here is an example in JavaScript of how to create an array that you can pass as the value of the `Attachments` parameter of an [Outlook Message](user_post_messages.md).</span></span>

      const attachments = [{
        '@odata.type': '#microsoft.graph.fileAttachment',
        ContentBytes: file.toString('base64'),
        Name: 'mypic.jpg'
      }];

<span data-ttu-id="4c830-182">Ознакомиться с реализацией этого примера можно в статье [Пример подключения к Microsoft Graph для Node.js](https://github.com/microsoftgraph/nodejs-connect-rest-sample).</span><span class="sxs-lookup"><span data-stu-id="4c830-182">See the [Microsoft Graph Connect Sample for Node.js](https://github.com/microsoftgraph/nodejs-connect-rest-sample) for an implementation of this example.</span></span>

<span data-ttu-id="4c830-183">Если требуется, чтобы изображение отображалось на веб-странице, создайте объект в памяти на его основе и сделайте этот объект источником элемента изображения.</span><span class="sxs-lookup"><span data-stu-id="4c830-183">If you want to display the image on a web page, create an in-memory object from the image and make that object the source of an image element.</span></span> <span data-ttu-id="4c830-184">Ниже приведен пример кода JavaScript для этой операции.</span><span class="sxs-lookup"><span data-stu-id="4c830-184">Here is an example in JavaScript of this operation.</span></span>

    const url = window.URL || window.webkitURL;
    const blobUrl = url.createObjectURL(image.data);
    document.getElementById(imageElement).setAttribute("src", blobUrl);

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get photo",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

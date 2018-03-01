# <a name="get-photo"></a><span data-ttu-id="7d22f-101">Получение фотографии</span><span class="sxs-lookup"><span data-stu-id="7d22f-101">Get photo</span></span>

<span data-ttu-id="7d22f-102">Получение указанного объекта [profilePhoto](../resources/profilephoto.md) или его метаданных (свойств profilePhoto).</span><span class="sxs-lookup"><span data-stu-id="7d22f-102">Get the specified [profilePhoto](../resources/profilephoto.md) or its metadata (profilePhoto properties).</span></span>

<span data-ttu-id="7d22f-103">Операция GET выполняет поиск указанной фотографии в почтовом ящике пользователя в Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="7d22f-103">A GET operation looks for the specified photo in the user's mailbox on Exchange Online.</span></span>

> <span data-ttu-id="7d22f-104">**Примечание.** Эта операция в версии 1.0 поддерживает только рабочие или учебные почтовые ящики пользователя (не личные).</span><span class="sxs-lookup"><span data-stu-id="7d22f-104">**Note** This operation in version 1.0 supports only a user's work or school mailboxes and not personal mailboxes.</span></span>

## <a name="permissions"></a><span data-ttu-id="7d22f-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7d22f-105">Permissions</span></span>
<span data-ttu-id="7d22f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="7d22f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

*   <span data-ttu-id="7d22f-108">Фотография профиля любого пользователя в клиенте, в том числе вошедшего пользователя: User.ReadBasic.All, User.Read.All, User.ReadWrite.All.</span><span class="sxs-lookup"><span data-stu-id="7d22f-108">Profile photo of any user in the tenant including the signed-in user - User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span>
*   <span data-ttu-id="7d22f-109">Фотография конкретного вошедшего пользователя: User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All.</span><span class="sxs-lookup"><span data-stu-id="7d22f-109">Profile photo of specifically the signed-in user - User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span>
* <span data-ttu-id="7d22f-110">Фотография профиля **группы**: Group.Read.All, Group.ReadWrite.All.</span><span class="sxs-lookup"><span data-stu-id="7d22f-110">Profile photo of a **group** - Group.Read.All, Group.ReadWrite.All</span></span>
* <span data-ttu-id="7d22f-111">Фотография **контакта**: Contacts.Read, Contacts.ReadWrite.</span><span class="sxs-lookup"><span data-stu-id="7d22f-111">Photo of a **contact** - Contacts.Read, Contacts.ReadWrite</span></span>

## <a name="http-request-to-get-the-photo"></a><span data-ttu-id="7d22f-112">HTTP-запрос для получения фотографии</span><span class="sxs-lookup"><span data-stu-id="7d22f-112">HTTP request to get the photo</span></span>
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
## <a name="http-request-to-get-the-metadata-of-the-photo"></a><span data-ttu-id="7d22f-113">HTTP-запрос для получения метаданных фотографии</span><span class="sxs-lookup"><span data-stu-id="7d22f-113">HTTP request to get the metadata of the photo</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/photo
GET /users/{id | userPrincipalName}/photo
GET /groups/{id}/photo
GET /me/contacts/{id}/photo
GET /users/{id | userPrincipalName}/contacts/{id}/photo
GET /me/contactfolders/{contactFolderId}/contacts/{id}/photo
GET /users/{id | userPrincipalName}/contactfolders/{contactFolderId}/contacts/{id}/photo
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7d22f-114">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="7d22f-114">Optional query parameters</span></span>
<span data-ttu-id="7d22f-115">Этот метод поддерживает [параметры запросов OData](http://developer.microsoft.com/ru-RU/graph/docs/overview/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="7d22f-115">This method supports the [OData Query Parameters](http://developer.microsoft.com/ru-RU/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7d22f-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7d22f-116">Request headers</span></span>
| <span data-ttu-id="7d22f-117">Имя</span><span class="sxs-lookup"><span data-stu-id="7d22f-117">Name</span></span>       | <span data-ttu-id="7d22f-118">Тип</span><span class="sxs-lookup"><span data-stu-id="7d22f-118">Type</span></span> | <span data-ttu-id="7d22f-119">Описание</span><span class="sxs-lookup"><span data-stu-id="7d22f-119">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="7d22f-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="7d22f-120">Authorization</span></span>  | <span data-ttu-id="7d22f-121">string</span><span class="sxs-lookup"><span data-stu-id="7d22f-121">string</span></span>  | <span data-ttu-id="7d22f-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7d22f-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7d22f-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7d22f-124">Request body</span></span>
<span data-ttu-id="7d22f-125">Не указывайте основной текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7d22f-125">Do not supply a request body for this method.</span></span>
## <a name="response-for-getting-the-photo"></a><span data-ttu-id="7d22f-126">Отклик для запроса на получение фотографии</span><span class="sxs-lookup"><span data-stu-id="7d22f-126">Response for getting the photo</span></span>
<span data-ttu-id="7d22f-p103">При успешном выполнении этот метод возвращает код отклика `200 OK` и двоичные данные запрашиваемой фотографии.  Если фотография не существует, операция возвратит отклик `404 Not Found`.</span><span class="sxs-lookup"><span data-stu-id="7d22f-p103">If successful, this method returns a `200 OK` response code and binary data of the requested photo.  If no photo exists, the operation returns `404 Not Found`.</span></span>
## <a name="response-for-getting-the-metadata-of-the-photo"></a><span data-ttu-id="7d22f-129">Отклик для запроса на получение метаданных фотографии</span><span class="sxs-lookup"><span data-stu-id="7d22f-129">Response for getting the metadata of the photo</span></span>
<span data-ttu-id="7d22f-130">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [profilePhoto](../resources/profilePhoto.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7d22f-130">If successful, this method returns a `200 OK` response code and [profilePhoto](../resources/profilePhoto.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="7d22f-131">Пример</span><span class="sxs-lookup"><span data-stu-id="7d22f-131">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="7d22f-132">Запрос 1</span><span class="sxs-lookup"><span data-stu-id="7d22f-132">Request 1</span></span>
<span data-ttu-id="7d22f-133">Этот запрос возвращает фотографию пользователя, вошедшего в систему, с максимальным доступным размером.</span><span class="sxs-lookup"><span data-stu-id="7d22f-133">This request gets the photo for the signed-in user, in the largest available size.</span></span>
<!-- {
  "blockType": "ignored"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/photo/$value
```

##### <a name="response-1"></a><span data-ttu-id="7d22f-134">Отклик 1</span><span class="sxs-lookup"><span data-stu-id="7d22f-134">Response 1</span></span>
<span data-ttu-id="7d22f-p104">Содержит двоичные данные запрошенной фотографии. Код HTTP-отклика: 200.</span><span class="sxs-lookup"><span data-stu-id="7d22f-p104">Contains the binary data of the requested photo. The HTTP response code is 200.</span></span>

##### <a name="request-2"></a><span data-ttu-id="7d22f-137">Запрос 2</span><span class="sxs-lookup"><span data-stu-id="7d22f-137">Request 2</span></span>
<span data-ttu-id="7d22f-138">Этот запрос возвращает метаданные фотографии пользователя, выполнившего вход в систему.</span><span class="sxs-lookup"><span data-stu-id="7d22f-138">This request gets the metadata of the user photo of the signed-in user.</span></span>
<!-- {
  "blockType": "ignored"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/photo
```

##### <a name="response-2"></a><span data-ttu-id="7d22f-139">Отклик 2</span><span class="sxs-lookup"><span data-stu-id="7d22f-139">Response 2</span></span>

<span data-ttu-id="7d22f-p105">В данных указанного ниже отклика содержатся метаданные фотографии. Примечание. Показанный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="7d22f-p105">The following response data shows the photo metadata. Note: The response object shown here may be truncated for brevity.</span></span>
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

<span data-ttu-id="7d22f-p106">Ниже показаны данные отклика в случае, если фотография пользователя еще не выложена. Примечание. Показанный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="7d22f-p106">The following response data shows the contents of a response when a photo hasn't already been uploaded for the user. Note: The response object shown here may be truncated for brevity.</span></span>

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
## <a name="using-the-binary-data-of-the-requested-photo"></a><span data-ttu-id="7d22f-144">Использование двоичных данных запрошенной фотографии</span><span class="sxs-lookup"><span data-stu-id="7d22f-144">Using the binary data of the requested photo</span></span>

<span data-ttu-id="7d22f-145">Когда вы используете конечную точку `/photo/$value` для получения двоичных данных для фотографии профиля, потребуется преобразовать эти данные в строку Base64, чтобы добавить их как вложение электронной почты.</span><span class="sxs-lookup"><span data-stu-id="7d22f-145">When you use the `/photo/$value` endpoint to get the binary data for a profile photo, you'll need to convert the data into a base-64 string in order to add it as an email attachment.</span></span> <span data-ttu-id="7d22f-146">Ниже приведен пример кода JavaScript, показывающий, как создать массив, который можно передать как значение параметра `Attachments` для [сообщения Outlook](user_post_messages.md).</span><span class="sxs-lookup"><span data-stu-id="7d22f-146">Here is an example in JavaScript of how to create an array that you can pass as the value of the `Attachments` parameter of an [Outlook Message](user_post_messages.md).</span></span>

      const attachments = [{
        '@odata.type': '#microsoft.graph.fileAttachment',
        ContentBytes: file.toString('base64'),
        Name: 'mypic.jpg'
      }];

<span data-ttu-id="7d22f-147">Ознакомиться с реализацией этого примера можно в статье [Пример подключения к Microsoft Graph для Node.js](https://github.com/microsoftgraph/nodejs-connect-rest-sample).</span><span class="sxs-lookup"><span data-stu-id="7d22f-147">See the [Microsoft Graph Connect Sample for Node.js](https://github.com/microsoftgraph/nodejs-connect-rest-sample) for an implementation of this example.</span></span>

<span data-ttu-id="7d22f-148">Если требуется, чтобы изображение отображалось на веб-странице, создайте объект в памяти на его основе и сделайте этот объект источником элемента изображения.</span><span class="sxs-lookup"><span data-stu-id="7d22f-148">If you want to display the image on a web page, create an in-memory object from the image and make that object the source of an image element.</span></span> <span data-ttu-id="7d22f-149">Ниже приведен пример кода JavaScript для этой операции.</span><span class="sxs-lookup"><span data-stu-id="7d22f-149">Here is an example in JavaScript of this operation.</span></span>

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

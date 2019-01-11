---
title: Получение фотографии
description: Получение указанного объекта profilePhoto или его метаданных (свойств profilePhoto).
localization_priority: Priority
ms.openlocfilehash: 6b1a3e54b1145cc2fdcf8ed9e587652d4d7061c8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27833952"
---
# <a name="get-photo"></a><span data-ttu-id="8e798-103">Получение фотографии</span><span class="sxs-lookup"><span data-stu-id="8e798-103">Get photo</span></span>

<span data-ttu-id="8e798-104">Получение указанного объекта [profilePhoto](../resources/profilephoto.md) или его метаданных (свойств profilePhoto).</span><span class="sxs-lookup"><span data-stu-id="8e798-104">Get the specified [profilePhoto](../resources/profilephoto.md) or its metadata (profilePhoto properties).</span></span>

> <span data-ttu-id="8e798-105">**Примечание.** Эта операция в версии 1.0 поддерживает только рабочие или учебные почтовые ящики пользователя (не личные).</span><span class="sxs-lookup"><span data-stu-id="8e798-105">**Note** This operation in version 1.0 supports only a user's work or school mailboxes and not personal mailboxes.</span></span>

<span data-ttu-id="8e798-106">Поддерживаемые размеры фотографий в формате HD для Office 365: 48 x 48, 64 x 64, 96 x 96, 120 x 120, 240 x 240, 360 x 360, 432 x 432, 504 x 504 и 648 x 648.</span><span class="sxs-lookup"><span data-stu-id="8e798-106">The supported sizes of HD photos on Office 365 are as follows: '48x48', '64x64', '96x96', '120x120', '240x240', '360x360','432x432', '504x504', and '648x648'.</span></span> <span data-ttu-id="8e798-107">Фотографии могут быть любого размера, если они хранятся в Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="8e798-107">Photos can be any dimension if they are stored in Azure Active Directory.</span></span>

<span data-ttu-id="8e798-108">Вы можете получить метаданные самой большой доступной фотографии или указать размер и получить метаданные для этого размера.</span><span class="sxs-lookup"><span data-stu-id="8e798-108">You can get the metadata of the largest available photo, or specify a size to get the metadata for that photo size.</span></span>
<span data-ttu-id="8e798-109">Если запрашиваемый размер недоступен, вы можете получить меньший размер, загруженный пользователем.</span><span class="sxs-lookup"><span data-stu-id="8e798-109">If the size you request is not available, you can still get a smaller size that the user has uploaded and made available.</span></span>
<span data-ttu-id="8e798-110">Например, если пользователь загрузит фотографию размером 504 x 504 пикселя, для скачивания будут доступны все размеры, кроме 648 x 648.</span><span class="sxs-lookup"><span data-stu-id="8e798-110">For example, if the user uploads a photo that is 504x504 pixels, then all but the 648x648 size of photo will be available for download.</span></span>

## <a name="permissions"></a><span data-ttu-id="8e798-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8e798-111">Permissions</span></span>

<span data-ttu-id="8e798-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8e798-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8e798-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8e798-114">Permission type</span></span>      | <span data-ttu-id="8e798-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8e798-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8e798-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8e798-116">Delegated (work or school account)</span></span> | <span data-ttu-id="8e798-117">Для ресурса **user**:</span><span class="sxs-lookup"><span data-stu-id="8e798-117">For **user** resource:</span></span><br/><span data-ttu-id="8e798-118">User.Read, User.ReadBasic.All, User.Read.All, User.ReadWrite, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8e798-118">User.Read, User.ReadBasic.All, User.Read.All, User.ReadWrite, User.ReadWrite.All</span></span><br /><br /><span data-ttu-id="8e798-119">Для ресурса **group**:</span><span class="sxs-lookup"><span data-stu-id="8e798-119">For **group** resource:</span></span><br /><span data-ttu-id="8e798-120">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8e798-120">Group.Read.All, Group.ReadWrite.All</span></span><br /><br /><span data-ttu-id="8e798-121">Для ресурса **contact**:</span><span class="sxs-lookup"><span data-stu-id="8e798-121">For **contact** resource:</span></span><br /><span data-ttu-id="8e798-122">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8e798-122">Contacts.Read, Contacts.ReadWrite</span></span> |
|<span data-ttu-id="8e798-123">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8e798-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8e798-124">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="8e798-124">Not supported</span></span> |
|<span data-ttu-id="8e798-125">Разрешения приложений</span><span class="sxs-lookup"><span data-stu-id="8e798-125">Application</span></span>                        | <span data-ttu-id="8e798-126">Для ресурса **user**:</span><span class="sxs-lookup"><span data-stu-id="8e798-126">For **user** resource:</span></span><br/><span data-ttu-id="8e798-127">User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8e798-127">User.Read.All, User.ReadWrite.All</span></span><br /><br /><span data-ttu-id="8e798-128">Для ресурса **group**:</span><span class="sxs-lookup"><span data-stu-id="8e798-128">For **group** resource:</span></span><br /><span data-ttu-id="8e798-129">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8e798-129">Group.Read.All, Group.ReadWrite.All</span></span><br /><br /><span data-ttu-id="8e798-130">Для ресурса **contact**:</span><span class="sxs-lookup"><span data-stu-id="8e798-130">For **contact** resource:</span></span><br /><span data-ttu-id="8e798-131">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8e798-131">Contacts.Read, Contacts.ReadWrite</span></span> |


## <a name="http-request"></a><span data-ttu-id="8e798-132">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8e798-132">HTTP request</span></span> 

### <a name="get-the-photo"></a><span data-ttu-id="8e798-133">Получение фотографий</span><span class="sxs-lookup"><span data-stu-id="8e798-133">Get the photo</span></span>
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
### <a name="get-the-metadata-of-the-photo"></a><span data-ttu-id="8e798-134">Получение метаданных фотографии</span><span class="sxs-lookup"><span data-stu-id="8e798-134">Get the metadata of the photo</span></span>
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

### <a name="get-the-metadata-for-a-specific-photo-size"></a><span data-ttu-id="8e798-135">Получить метаданные для определенного размера фотографии</span><span class="sxs-lookup"><span data-stu-id="8e798-135">Get the metadata for a specific photo size</span></span>
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

## <a name="path-parameters"></a><span data-ttu-id="8e798-136">Параметры пути</span><span class="sxs-lookup"><span data-stu-id="8e798-136">Path parameters</span></span>

|<span data-ttu-id="8e798-137">Параметр</span><span class="sxs-lookup"><span data-stu-id="8e798-137">Parameter</span></span>|<span data-ttu-id="8e798-138">Тип</span><span class="sxs-lookup"><span data-stu-id="8e798-138">Type</span></span>|<span data-ttu-id="8e798-139">Описание</span><span class="sxs-lookup"><span data-stu-id="8e798-139">Description</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="8e798-140">size</span><span class="sxs-lookup"><span data-stu-id="8e798-140">size</span></span>  |<span data-ttu-id="8e798-141">String</span><span class="sxs-lookup"><span data-stu-id="8e798-141">String</span></span>  | <span data-ttu-id="8e798-142">Размер фотографии.</span><span class="sxs-lookup"><span data-stu-id="8e798-142">A photo size.</span></span> <span data-ttu-id="8e798-143">Поддерживаемые размеры фотографий в формате HD для Office 365: 48 x 48, 64 x 64, 96 x 96, 120 x 120, 240 x 240, 360 x 360, 432 x 432, 504 x 504 и 648 x 648.</span><span class="sxs-lookup"><span data-stu-id="8e798-143">The supported sizes of HD photos on Office 365 are as follows: '48x48', '64x64', '96x96', '120x120', '240x240', '360x360','432x432', '504x504', and '648x648'.</span></span> <span data-ttu-id="8e798-144">Фотографии могут быть любого размера, если они хранятся в Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="8e798-144">Photos can be any dimension if they are stored in Azure Active Directory.</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="8e798-145">Необязательные параметры запроса</span><span class="sxs-lookup"><span data-stu-id="8e798-145">Optional query parameters</span></span>
<span data-ttu-id="8e798-146">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="8e798-146">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8e798-147">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8e798-147">Request headers</span></span>
| <span data-ttu-id="8e798-148">Имя</span><span class="sxs-lookup"><span data-stu-id="8e798-148">Name</span></span>       | <span data-ttu-id="8e798-149">Тип</span><span class="sxs-lookup"><span data-stu-id="8e798-149">Type</span></span> | <span data-ttu-id="8e798-150">Описание</span><span class="sxs-lookup"><span data-stu-id="8e798-150">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="8e798-151">Authorization</span><span class="sxs-lookup"><span data-stu-id="8e798-151">Authorization</span></span>  | <span data-ttu-id="8e798-152">string</span><span class="sxs-lookup"><span data-stu-id="8e798-152">string</span></span>  | <span data-ttu-id="8e798-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8e798-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8e798-155">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="8e798-155">Request body</span></span>
<span data-ttu-id="8e798-156">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8e798-156">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8e798-157">Ответ</span><span class="sxs-lookup"><span data-stu-id="8e798-157">Response</span></span>
### <a name="response-for-getting-the-photo"></a><span data-ttu-id="8e798-158">Отклик для запроса на получение фотографии</span><span class="sxs-lookup"><span data-stu-id="8e798-158">Response for getting the photo</span></span>
<span data-ttu-id="8e798-p106">При успешном выполнении этот метод возвращает код отклика `200 OK` и двоичные данные запрашиваемой фотографии.  Если фотография не существует, операция возвратит отклик `404 Not Found`.</span><span class="sxs-lookup"><span data-stu-id="8e798-p106">If successful, this method returns a `200 OK` response code and binary data of the requested photo.  If no photo exists, the operation returns `404 Not Found`.</span></span>
### <a name="response-for-getting-the-metadata-of-the-photo"></a><span data-ttu-id="8e798-161">Отклик для запроса на получение метаданных фотографии</span><span class="sxs-lookup"><span data-stu-id="8e798-161">Response for getting the metadata of the photo</span></span>
<span data-ttu-id="8e798-162">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [profilePhoto](../resources/profilephoto.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8e798-162">If successful, this method returns a `200 OK` response code and [profilePhoto](../resources/profilephoto.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="8e798-163">Пример</span><span class="sxs-lookup"><span data-stu-id="8e798-163">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="8e798-164">Запрос 1</span><span class="sxs-lookup"><span data-stu-id="8e798-164">Request 1</span></span>
<span data-ttu-id="8e798-165">Этот запрос возвращает фотографию пользователя, вошедшего в систему, с максимальным доступным размером.</span><span class="sxs-lookup"><span data-stu-id="8e798-165">This request gets the photo for the signed-in user, in the largest available size.</span></span>
<!-- {
  "blockType": "ignored"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/photo/$value
```

##### <a name="response-1"></a><span data-ttu-id="8e798-166">Отклик 1</span><span class="sxs-lookup"><span data-stu-id="8e798-166">Response 1</span></span>
<span data-ttu-id="8e798-p107">Содержит двоичные данные запрошенной фотографии. Код HTTP-отклика: 200.</span><span class="sxs-lookup"><span data-stu-id="8e798-p107">Contains the binary data of the requested photo. The HTTP response code is 200.</span></span>

##### <a name="request-2"></a><span data-ttu-id="8e798-169">Запрос 2</span><span class="sxs-lookup"><span data-stu-id="8e798-169">Request 2</span></span>
<span data-ttu-id="8e798-170">Этот запрос получает фотографию 48 x 48 для вошедшего пользователя.</span><span class="sxs-lookup"><span data-stu-id="8e798-170">This request gets the 48x48 photo for the signed-in user.</span></span>

<!-- {
  "blockType": "ignored"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/photos/48x48/$value
Content-Type: image/jpg
```

##### <a name="response-2"></a><span data-ttu-id="8e798-171">Ответ 2</span><span class="sxs-lookup"><span data-stu-id="8e798-171">Response 2</span></span>
<span data-ttu-id="8e798-172">Содержит двоичные данные запрошенной фотографии 48 x 48.</span><span class="sxs-lookup"><span data-stu-id="8e798-172">Contains the binary data of the requested 48x48 photo.</span></span> <span data-ttu-id="8e798-173">Код HTTP-ответа: 200.</span><span class="sxs-lookup"><span data-stu-id="8e798-173">The HTTP response code is 200.</span></span>

##### <a name="request-3"></a><span data-ttu-id="8e798-174">Запрос 3</span><span class="sxs-lookup"><span data-stu-id="8e798-174">Request 3</span></span>
<span data-ttu-id="8e798-175">Этот запрос возвращает метаданные фотографии вошедшего пользователя.</span><span class="sxs-lookup"><span data-stu-id="8e798-175">This request gets the metadata of the user photo of the signed-in user.</span></span>
<!-- {
  "blockType": "ignored"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/photo
```

##### <a name="response-3"></a><span data-ttu-id="8e798-176">Ответ 3</span><span class="sxs-lookup"><span data-stu-id="8e798-176">Response 3</span></span>

<span data-ttu-id="8e798-p109">В данных указанного ниже ответа содержатся метаданные фотографии. Примечание. Показанный здесь объект ответа может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="8e798-p109">The following response data shows the photo metadata. Note: The response object shown here may be truncated for brevity.</span></span>
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

<span data-ttu-id="8e798-p110">Ниже показаны данные отклика в случае, если фотография пользователя еще не выложена. Примечание. Показанный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="8e798-p110">The following response data shows the contents of a response when a photo hasn't already been uploaded for the user. Note: The response object shown here may be truncated for brevity.</span></span>

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
## <a name="using-the-binary-data-of-the-requested-photo"></a><span data-ttu-id="8e798-181">Использование двоичных данных запрошенной фотографии</span><span class="sxs-lookup"><span data-stu-id="8e798-181">Using the binary data of the requested photo</span></span>

<span data-ttu-id="8e798-182">Когда вы используете конечную точку `/photo/$value` для получения двоичных данных для фотографии профиля, потребуется преобразовать эти данные в строку Base64, чтобы добавить их как вложение электронной почты.</span><span class="sxs-lookup"><span data-stu-id="8e798-182">When you use the `/photo/$value` endpoint to get the binary data for a profile photo, you'll need to convert the data into a base-64 string in order to add it as an email attachment.</span></span> <span data-ttu-id="8e798-183">Ниже приведен пример кода JavaScript, показывающий, как создать массив, который можно передать как значение параметра `Attachments` для [сообщения Outlook](user-post-messages.md).</span><span class="sxs-lookup"><span data-stu-id="8e798-183">Here is an example in JavaScript of how to create an array that you can pass as the value of the `Attachments` parameter of an [Outlook Message](user-post-messages.md).</span></span>

      const attachments = [{
        '@odata.type': '#microsoft.graph.fileAttachment',
        ContentBytes: file.toString('base64'),
        Name: 'mypic.jpg'
      }];

<span data-ttu-id="8e798-184">Ознакомиться с реализацией этого примера можно в статье [Пример подключения к Microsoft Graph для Node.js](https://github.com/microsoftgraph/nodejs-connect-rest-sample).</span><span class="sxs-lookup"><span data-stu-id="8e798-184">See the [Microsoft Graph Connect Sample for Node.js](https://github.com/microsoftgraph/nodejs-connect-rest-sample) for an implementation of this example.</span></span>

<span data-ttu-id="8e798-185">Если требуется, чтобы изображение отображалось на веб-странице, создайте объект в памяти на его основе и сделайте этот объект источником элемента изображения.</span><span class="sxs-lookup"><span data-stu-id="8e798-185">If you want to display the image on a web page, create an in-memory object from the image and make that object the source of an image element.</span></span> <span data-ttu-id="8e798-186">Ниже приведен пример кода JavaScript для этой операции.</span><span class="sxs-lookup"><span data-stu-id="8e798-186">Here is an example in JavaScript of this operation.</span></span>

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

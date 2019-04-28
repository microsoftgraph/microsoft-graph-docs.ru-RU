---
title: Получение фотографии
description: Получение указанного объекта profilePhoto или его метаданных (свойств profilePhoto).
localization_priority: Priority
ms.openlocfilehash: e0b115ecf3ce05d87856e553b111af537ffad0e3
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32576285"
---
# <a name="get-photo"></a><span data-ttu-id="9daec-103">Получение фотографии</span><span class="sxs-lookup"><span data-stu-id="9daec-103">Get photo</span></span>

<span data-ttu-id="9daec-104">Получение указанного объекта [profilePhoto](../resources/profilephoto.md) или его метаданных (свойств profilePhoto).</span><span class="sxs-lookup"><span data-stu-id="9daec-104">Get the specified [profilePhoto](../resources/profilephoto.md) or its metadata (profilePhoto properties).</span></span>

> <span data-ttu-id="9daec-105">**Примечание.** Эта операция в версии 1.0 поддерживает только рабочие или учебные почтовые ящики пользователя (не личные).</span><span class="sxs-lookup"><span data-stu-id="9daec-105">**Note** This operation in version 1.0 supports only a user's work or school mailboxes and not personal mailboxes.</span></span>

<span data-ttu-id="9daec-106">Поддерживаемые размеры фотографий в формате HD для Office 365: 48 x 48, 64 x 64, 96 x 96, 120 x 120, 240 x 240, 360 x 360, 432 x 432, 504 x 504 и 648 x 648.</span><span class="sxs-lookup"><span data-stu-id="9daec-106">The supported sizes of HD photos on Office 365 are as follows: 48x48, 64x64, 96x96, 120x120, 240x240, 360x360, 432x432, 504x504, and 648x648.</span></span> <span data-ttu-id="9daec-107">Фотографии могут быть любого размера, если они хранятся в Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="9daec-107">Photos can be any dimension if they are stored in Azure Active Directory.</span></span>

<span data-ttu-id="9daec-108">Вы можете получить метаданные самой большой доступной фотографии или указать размер и получить метаданные для этого размера.</span><span class="sxs-lookup"><span data-stu-id="9daec-108">You can get the metadata of the largest available photo, or specify a size to get the metadata for that photo size.</span></span>
<span data-ttu-id="9daec-109">Если запрашиваемый размер недоступен, вы можете получить меньший размер, загруженный пользователем.</span><span class="sxs-lookup"><span data-stu-id="9daec-109">If the size you request is not available, you can still get a smaller size that the user has uploaded and made available.</span></span>
<span data-ttu-id="9daec-110">Например, если пользователь загрузит фотографию размером 504 x 504 пикселя, для скачивания будут доступны все размеры, кроме 648 x 648.</span><span class="sxs-lookup"><span data-stu-id="9daec-110">For example, if the user uploads a photo that is 504x504 pixels, then all but the 648x648 size of photo will be available for download.</span></span>

## <a name="permissions"></a><span data-ttu-id="9daec-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9daec-111">Permissions</span></span>

<span data-ttu-id="9daec-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9daec-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9daec-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9daec-114">Permission type</span></span>      | <span data-ttu-id="9daec-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9daec-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9daec-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9daec-116">Delegated (work or school account)</span></span> | <span data-ttu-id="9daec-117">Для ресурса **user**:</span><span class="sxs-lookup"><span data-stu-id="9daec-117">For **user** resource:</span></span><br/><span data-ttu-id="9daec-118">User.Read, User.ReadBasic.All, User.Read.All, User.ReadWrite, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9daec-118">User.Read, User.ReadBasic.All, User.Read.All, User.ReadWrite, User.ReadWrite.All</span></span><br /><br /><span data-ttu-id="9daec-119">Для ресурса **group**:</span><span class="sxs-lookup"><span data-stu-id="9daec-119">For **group** resource:</span></span><br /><span data-ttu-id="9daec-120">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9daec-120">Group.Read.All, Group.ReadWrite.All</span></span><br /><br /><span data-ttu-id="9daec-121">Для ресурса **contact**:</span><span class="sxs-lookup"><span data-stu-id="9daec-121">For **contact** resource:</span></span><br /><span data-ttu-id="9daec-122">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9daec-122">Contacts.Read, Contacts.ReadWrite</span></span> |
|<span data-ttu-id="9daec-123">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9daec-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9daec-124">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="9daec-124">Not supported</span></span> |
|<span data-ttu-id="9daec-125">Разрешения приложений</span><span class="sxs-lookup"><span data-stu-id="9daec-125">Application</span></span>                        | <span data-ttu-id="9daec-126">Для ресурса **user**:</span><span class="sxs-lookup"><span data-stu-id="9daec-126">For **user** resource:</span></span><br/><span data-ttu-id="9daec-127">User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9daec-127">User.Read.All, User.ReadWrite.All</span></span><br /><br /><span data-ttu-id="9daec-128">Для ресурса **group**:</span><span class="sxs-lookup"><span data-stu-id="9daec-128">For **group** resource:</span></span><br /><span data-ttu-id="9daec-129">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9daec-129">Group.Read.All, Group.ReadWrite.All</span></span><br /><br /><span data-ttu-id="9daec-130">Для ресурса **contact**:</span><span class="sxs-lookup"><span data-stu-id="9daec-130">For **contact** resource:</span></span><br /><span data-ttu-id="9daec-131">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9daec-131">Contacts.Read, Contacts.ReadWrite</span></span> |


## <a name="http-request"></a><span data-ttu-id="9daec-132">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9daec-132">HTTP request</span></span> 

### <a name="get-the-photo"></a><span data-ttu-id="9daec-133">Получение фотографии</span><span class="sxs-lookup"><span data-stu-id="9daec-133">Get the photo</span></span>
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
### <a name="get-the-metadata-of-the-photo"></a><span data-ttu-id="9daec-134">Получение метаданных фотографии</span><span class="sxs-lookup"><span data-stu-id="9daec-134">Get the metadata of the photo</span></span>
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

### <a name="get-the-metadata-for-a-specific-photo-size"></a><span data-ttu-id="9daec-135">Получение метаданных фотографии определенного размера</span><span class="sxs-lookup"><span data-stu-id="9daec-135">Get the metadata for a specific photo size</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/photos/{size}
GET /users/{id | userPrincipalName}/photos/{size}
GET /groups/{id}/photos/{size}
```

## <a name="path-parameters"></a><span data-ttu-id="9daec-136">Параметры пути</span><span class="sxs-lookup"><span data-stu-id="9daec-136">Path parameters</span></span>

|<span data-ttu-id="9daec-137">Параметр</span><span class="sxs-lookup"><span data-stu-id="9daec-137">Parameter</span></span>|<span data-ttu-id="9daec-138">Тип</span><span class="sxs-lookup"><span data-stu-id="9daec-138">Type</span></span>|<span data-ttu-id="9daec-139">Описание</span><span class="sxs-lookup"><span data-stu-id="9daec-139">Description</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="9daec-140">size</span><span class="sxs-lookup"><span data-stu-id="9daec-140">size</span></span>  |<span data-ttu-id="9daec-141">String</span><span class="sxs-lookup"><span data-stu-id="9daec-141">String</span></span>  | <span data-ttu-id="9daec-142">Размер фотографии.</span><span class="sxs-lookup"><span data-stu-id="9daec-142">A photo size.</span></span> <span data-ttu-id="9daec-143">Поддерживаемые размеры фотографий в формате HD для Office 365: 48 x 48, 64 x 64, 96 x 96, 120 x 120, 240 x 240, 360 x 360, 432 x 432, 504 x 504 и 648 x 648.</span><span class="sxs-lookup"><span data-stu-id="9daec-143">The supported sizes of HD photos on Office 365 are as follows: 48x48, 64x64, 96x96, 120x120, 240x240, 360x360, 432x432, 504x504, and 648x648.</span></span> <span data-ttu-id="9daec-144">Фотографии могут быть любого размера, если они хранятся в Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="9daec-144">Photos can be any dimension if they are stored in Azure Active Directory.</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="9daec-145">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="9daec-145">Optional query parameters</span></span>
<span data-ttu-id="9daec-146">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="9daec-146">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9daec-147">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9daec-147">Request headers</span></span>
| <span data-ttu-id="9daec-148">Имя</span><span class="sxs-lookup"><span data-stu-id="9daec-148">Name</span></span>       | <span data-ttu-id="9daec-149">Тип</span><span class="sxs-lookup"><span data-stu-id="9daec-149">Type</span></span> | <span data-ttu-id="9daec-150">Описание</span><span class="sxs-lookup"><span data-stu-id="9daec-150">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="9daec-151">Authorization</span><span class="sxs-lookup"><span data-stu-id="9daec-151">Authorization</span></span>  | <span data-ttu-id="9daec-152">string</span><span class="sxs-lookup"><span data-stu-id="9daec-152">string</span></span>  | <span data-ttu-id="9daec-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9daec-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9daec-155">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9daec-155">Request body</span></span>
<span data-ttu-id="9daec-156">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9daec-156">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9daec-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="9daec-157">Response</span></span>
### <a name="response-for-getting-the-photo"></a><span data-ttu-id="9daec-158">Отклик для запроса на получение фотографии</span><span class="sxs-lookup"><span data-stu-id="9daec-158">Response for getting the photo</span></span>
<span data-ttu-id="9daec-p106">При успешном выполнении этот метод возвращает код отклика `200 OK` и двоичные данные запрашиваемой фотографии.  Если фотография не существует, операция возвратит отклик `404 Not Found`.</span><span class="sxs-lookup"><span data-stu-id="9daec-p106">If successful, this method returns a `200 OK` response code and binary data of the requested photo.  If no photo exists, the operation returns `404 Not Found`.</span></span>
### <a name="response-for-getting-the-metadata-of-the-photo"></a><span data-ttu-id="9daec-161">Отклик для запроса на получение метаданных фотографии</span><span class="sxs-lookup"><span data-stu-id="9daec-161">Response for getting the metadata of the photo</span></span>
<span data-ttu-id="9daec-162">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [profilePhoto](../resources/profilephoto.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9daec-162">If successful, this method returns a `200 OK` response code and [profilePhoto](../resources/profilephoto.md) object in the response body.</span></span>
## <a name="examples"></a><span data-ttu-id="9daec-163">Примеры</span><span class="sxs-lookup"><span data-stu-id="9daec-163">Examples</span></span>

### <a name="example-1-get-the-photo-for-the-signed-in-user-in-the-largest-available-size"></a><span data-ttu-id="9daec-164">Пример 1. Получение фотографии пользователя, вошедшего в систему, с максимальным доступным размером</span><span class="sxs-lookup"><span data-stu-id="9daec-164">Example 1: Get the photo of the signed-in user in the largest available size</span></span>
##### <a name="request"></a><span data-ttu-id="9daec-165">Запрос</span><span class="sxs-lookup"><span data-stu-id="9daec-165">Request</span></span>
<!-- {
  "blockType": "ignored"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/photo/$value
```

##### <a name="response"></a><span data-ttu-id="9daec-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="9daec-166">Response</span></span> 
<span data-ttu-id="9daec-167">Содержит двоичные данные запрошенной фотографии.</span><span class="sxs-lookup"><span data-stu-id="9daec-167">Contains the binary data of the requested photo.</span></span> <span data-ttu-id="9daec-168">Код HTTP-отклика: 200.</span><span class="sxs-lookup"><span data-stu-id="9daec-168">The HTTP response code is 200.</span></span>

### <a name="example-2-get-the-48x48-photo-for-the-signed-in-use"></a><span data-ttu-id="9daec-169">Пример 2. Получение фотографии 48 x 48 для вошедшего пользователя</span><span class="sxs-lookup"><span data-stu-id="9daec-169">Example 2: Get the 48x48 photo for the signed-in user</span></span>
##### <a name="request"></a><span data-ttu-id="9daec-170">Запрос</span><span class="sxs-lookup"><span data-stu-id="9daec-170">Request</span></span>
<!-- {
  "blockType": "ignored"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/photos/48x48/$value
Content-Type: image/jpg
```

##### <a name="response"></a><span data-ttu-id="9daec-171">Отклик</span><span class="sxs-lookup"><span data-stu-id="9daec-171">Response</span></span>
<span data-ttu-id="9daec-172">Содержит двоичные данные запрошенной фотографии 48 x 48.</span><span class="sxs-lookup"><span data-stu-id="9daec-172">Contains the binary data of the requested 48x48 photo.</span></span> <span data-ttu-id="9daec-173">Код HTTP-отклика: 200.</span><span class="sxs-lookup"><span data-stu-id="9daec-173">The HTTP response code is 200.</span></span>

### <a name="example-3-get-the-metadata-of-the-user-photo-of-the-signed-in-user"></a><span data-ttu-id="9daec-174">Пример 3. Получение метаданных фотографии вошедшего пользователя</span><span class="sxs-lookup"><span data-stu-id="9daec-174">Example 3: Get the metadata of the user photo of the signed-in user</span></span>
##### <a name="request"></a><span data-ttu-id="9daec-175">Запрос</span><span class="sxs-lookup"><span data-stu-id="9daec-175">Request</span></span>
<!-- {
  "blockType": "ignored"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/photo
```

##### <a name="response"></a><span data-ttu-id="9daec-176">Отклик</span><span class="sxs-lookup"><span data-stu-id="9daec-176">Response</span></span>

<span data-ttu-id="9daec-177">В данных указанного ниже отклика содержатся метаданные фотографии.</span><span class="sxs-lookup"><span data-stu-id="9daec-177">The following response data shows the photo metadata.</span></span> 

><span data-ttu-id="9daec-178">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="9daec-178">**Note:** The response object shown here might be shortened for readability.</span></span>
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

<span data-ttu-id="9daec-179">Ниже показаны данные отклика в случае, если фотография пользователя еще не выложена.</span><span class="sxs-lookup"><span data-stu-id="9daec-179">The following response data shows the contents of a response when a photo hasn't already been uploaded for the user.</span></span>

><span data-ttu-id="9daec-180">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="9daec-180">**Note:** The response object shown here might be shortened for readability.</span></span>

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
## <a name="using-the-binary-data-of-the-requested-photo"></a><span data-ttu-id="9daec-181">Использование двоичных данных запрошенной фотографии</span><span class="sxs-lookup"><span data-stu-id="9daec-181">Using the binary data of the requested photo</span></span>

<span data-ttu-id="9daec-182">Когда вы используете конечную точку `/photo/$value` для получения двоичных данных для фотографии профиля, потребуется преобразовать эти данные в строку Base64, чтобы добавить их как вложение электронной почты.</span><span class="sxs-lookup"><span data-stu-id="9daec-182">When you use the `/photo/$value` endpoint to get the binary data for a profile photo, you'll need to convert the data into a base-64 string in order to add it as an email attachment.</span></span> <span data-ttu-id="9daec-183">Ниже приведен пример кода JavaScript, показывающий, как создать массив, который можно передать как значение параметра `Attachments` для [сообщения Outlook](user-post-messages.md).</span><span class="sxs-lookup"><span data-stu-id="9daec-183">Here is an example in JavaScript of how to create an array that you can pass as the value of the `Attachments` parameter of an [Outlook Message](user-post-messages.md).</span></span>

      const attachments = [{
        '@odata.type': '#microsoft.graph.fileAttachment',
        ContentBytes: file.toString('base64'),
        Name: 'mypic.jpg'
      }];

<span data-ttu-id="9daec-184">Ознакомиться с реализацией этого примера можно в статье [Пример подключения к Microsoft Graph для Node.js](https://github.com/microsoftgraph/nodejs-connect-rest-sample).</span><span class="sxs-lookup"><span data-stu-id="9daec-184">See the [Microsoft Graph Connect Sample for Node.js](https://github.com/microsoftgraph/nodejs-connect-rest-sample) for an implementation of this example.</span></span>

<span data-ttu-id="9daec-185">Если требуется, чтобы изображение отображалось на веб-странице, создайте объект в памяти на его основе и сделайте этот объект источником элемента изображения.</span><span class="sxs-lookup"><span data-stu-id="9daec-185">If you want to display the image on a web page, create an in-memory object from the image and make that object the source of an image element.</span></span> <span data-ttu-id="9daec-186">Ниже приведен пример кода JavaScript для этой операции.</span><span class="sxs-lookup"><span data-stu-id="9daec-186">Here is an example in JavaScript of this operation.</span></span>

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

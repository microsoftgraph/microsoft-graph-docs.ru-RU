---
title: Получение фотографии
description: Получение указанного объекта profilePhoto или его метаданных (свойств profilePhoto).
localization_priority: Priority
author: ''
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: ae531d0e5bd8aa759f0c72a1fc3ac420467127e1
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36022301"
---
# <a name="get-photo"></a><span data-ttu-id="34ea5-103">Получение фотографии</span><span class="sxs-lookup"><span data-stu-id="34ea5-103">Get photo</span></span>

<span data-ttu-id="34ea5-104">Получение указанного объекта [profilePhoto](../resources/profilephoto.md) или его метаданных (свойств profilePhoto).</span><span class="sxs-lookup"><span data-stu-id="34ea5-104">Get the specified [profilePhoto](../resources/profilephoto.md) or its metadata (profilePhoto properties).</span></span>

> <span data-ttu-id="34ea5-105">**Примечание.** Эта операция в версии 1.0 поддерживает только рабочие или учебные почтовые ящики пользователя (не личные).</span><span class="sxs-lookup"><span data-stu-id="34ea5-105">**Note** This operation in version 1.0 supports only a user's work or school mailboxes and not personal mailboxes.</span></span>

<span data-ttu-id="34ea5-106">Поддерживаемые размеры фотографий в формате HD для Office 365: 48 x 48, 64 x 64, 96 x 96, 120 x 120, 240 x 240, 360 x 360, 432 x 432, 504 x 504 и 648 x 648.</span><span class="sxs-lookup"><span data-stu-id="34ea5-106">The supported sizes of HD photos on Office 365 are as follows: 48x48, 64x64, 96x96, 120x120, 240x240, 360x360, 432x432, 504x504, and 648x648.</span></span> <span data-ttu-id="34ea5-107">Фотографии могут быть любого размера, если они хранятся в Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="34ea5-107">Photos can be any dimension if they are stored in Azure Active Directory.</span></span>

<span data-ttu-id="34ea5-108">Вы можете получить метаданные самой большой доступной фотографии или указать размер и получить метаданные для этого размера.</span><span class="sxs-lookup"><span data-stu-id="34ea5-108">You can get the metadata of the largest available photo, or specify a size to get the metadata for that photo size.</span></span>
<span data-ttu-id="34ea5-109">Если запрашиваемый размер недоступен, вы можете получить меньший размер, загруженный пользователем.</span><span class="sxs-lookup"><span data-stu-id="34ea5-109">If the size you request is not available, you can still get a smaller size that the user has uploaded and made available.</span></span>
<span data-ttu-id="34ea5-110">Например, если пользователь загрузит фотографию размером 504 x 504 пикселя, для скачивания будут доступны все размеры, кроме 648 x 648.</span><span class="sxs-lookup"><span data-stu-id="34ea5-110">For example, if the user uploads a photo that is 504x504 pixels, all but the 648x648 size of photo will be available for download.</span></span>

## <a name="permissions"></a><span data-ttu-id="34ea5-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="34ea5-111">Permissions</span></span>

<span data-ttu-id="34ea5-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="34ea5-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="34ea5-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="34ea5-114">Permission type</span></span>      | <span data-ttu-id="34ea5-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="34ea5-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="34ea5-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="34ea5-116">Delegated (work or school account)</span></span> | <span data-ttu-id="34ea5-117">Для ресурса **user**:</span><span class="sxs-lookup"><span data-stu-id="34ea5-117">For **user** resource:</span></span><br/><span data-ttu-id="34ea5-118">User.Read, User.ReadBasic.All, User.Read.All, User.ReadWrite, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="34ea5-118">User.Read, User.ReadBasic.All, User.Read.All, User.ReadWrite, User.ReadWrite.All</span></span><br /><br /><span data-ttu-id="34ea5-119">Для ресурса **group**:</span><span class="sxs-lookup"><span data-stu-id="34ea5-119">For **group** resource:</span></span><br /><span data-ttu-id="34ea5-120">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="34ea5-120">Group.Read.All, Group.ReadWrite.All</span></span><br /><br /><span data-ttu-id="34ea5-121">Для ресурса **contact**:</span><span class="sxs-lookup"><span data-stu-id="34ea5-121">For **contact** resource:</span></span><br /><span data-ttu-id="34ea5-122">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="34ea5-122">Contacts.Read, Contacts.ReadWrite</span></span> |
|<span data-ttu-id="34ea5-123">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="34ea5-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="34ea5-124">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="34ea5-124">Not supported</span></span> |
|<span data-ttu-id="34ea5-125">Разрешения приложений</span><span class="sxs-lookup"><span data-stu-id="34ea5-125">Application</span></span>                        | <span data-ttu-id="34ea5-126">Для ресурса **user**:</span><span class="sxs-lookup"><span data-stu-id="34ea5-126">For **user** resource:</span></span><br/><span data-ttu-id="34ea5-127">User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="34ea5-127">User.Read.All, User.ReadWrite.All</span></span><br /><br /><span data-ttu-id="34ea5-128">Для ресурса **group**:</span><span class="sxs-lookup"><span data-stu-id="34ea5-128">For **group** resource:</span></span><br /><span data-ttu-id="34ea5-129">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="34ea5-129">Group.Read.All, Group.ReadWrite.All</span></span><br /><br /><span data-ttu-id="34ea5-130">Для ресурса **contact**:</span><span class="sxs-lookup"><span data-stu-id="34ea5-130">For **contact** resource:</span></span><br /><span data-ttu-id="34ea5-131">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="34ea5-131">Contacts.Read, Contacts.ReadWrite</span></span> |

> <span data-ttu-id="34ea5-132">**Примечание.** В настоящее время существует [известная проблема](https://docs.microsoft.com/ru-RU/graph/known-issues#groups) с доступом к фотографиям группы с помощью разрешений для приложений.</span><span class="sxs-lookup"><span data-stu-id="34ea5-132">**Note:**  There is currently a [known issue](https://docs.microsoft.com/ru-RU/graph/known-issues#groups) with accessing group photos using application permissions.</span></span>

## <a name="http-request"></a><span data-ttu-id="34ea5-133">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="34ea5-133">HTTP request</span></span> 

### <a name="get-the-photo"></a><span data-ttu-id="34ea5-134">Получение фотографии</span><span class="sxs-lookup"><span data-stu-id="34ea5-134">Get the photo</span></span>
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
### <a name="get-the-metadata-of-the-photo"></a><span data-ttu-id="34ea5-135">Получение метаданных фотографии</span><span class="sxs-lookup"><span data-stu-id="34ea5-135">Get the metadata of the photo</span></span>
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

### <a name="get-the-metadata-for-a-specific-photo-size"></a><span data-ttu-id="34ea5-136">Получение метаданных фотографии определенного размера</span><span class="sxs-lookup"><span data-stu-id="34ea5-136">Get the metadata for a specific photo size</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/photos/{size}
GET /users/{id | userPrincipalName}/photos/{size}
GET /groups/{id}/photos/{size}
```

## <a name="path-parameters"></a><span data-ttu-id="34ea5-137">Параметры пути</span><span class="sxs-lookup"><span data-stu-id="34ea5-137">Path parameters</span></span>

|<span data-ttu-id="34ea5-138">Параметр</span><span class="sxs-lookup"><span data-stu-id="34ea5-138">Parameter</span></span>|<span data-ttu-id="34ea5-139">Тип</span><span class="sxs-lookup"><span data-stu-id="34ea5-139">Type</span></span>|<span data-ttu-id="34ea5-140">Описание</span><span class="sxs-lookup"><span data-stu-id="34ea5-140">Description</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="34ea5-141">size</span><span class="sxs-lookup"><span data-stu-id="34ea5-141">size</span></span>  |<span data-ttu-id="34ea5-142">String</span><span class="sxs-lookup"><span data-stu-id="34ea5-142">String</span></span>  | <span data-ttu-id="34ea5-143">Размер фотографии.</span><span class="sxs-lookup"><span data-stu-id="34ea5-143">A photo size.</span></span> <span data-ttu-id="34ea5-144">Поддерживаемые размеры фотографий в формате HD для Office 365: 48 x 48, 64 x 64, 96 x 96, 120 x 120, 240 x 240, 360 x 360, 432 x 432, 504 x 504 и 648 x 648.</span><span class="sxs-lookup"><span data-stu-id="34ea5-144">The supported sizes of HD photos on Office 365 are as follows: 48x48, 64x64, 96x96, 120x120, 240x240, 360x360, 432x432, 504x504, and 648x648.</span></span> <span data-ttu-id="34ea5-145">Фотографии могут быть любого размера, если они хранятся в Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="34ea5-145">Photos can be any dimension if they are stored in Azure Active Directory.</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="34ea5-146">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="34ea5-146">Optional query parameters</span></span>
<span data-ttu-id="34ea5-147">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="34ea5-147">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="34ea5-148">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="34ea5-148">Request headers</span></span>
| <span data-ttu-id="34ea5-149">Имя</span><span class="sxs-lookup"><span data-stu-id="34ea5-149">Name</span></span>       | <span data-ttu-id="34ea5-150">Тип</span><span class="sxs-lookup"><span data-stu-id="34ea5-150">Type</span></span> | <span data-ttu-id="34ea5-151">Описание</span><span class="sxs-lookup"><span data-stu-id="34ea5-151">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="34ea5-152">Authorization</span><span class="sxs-lookup"><span data-stu-id="34ea5-152">Authorization</span></span>  | <span data-ttu-id="34ea5-153">string</span><span class="sxs-lookup"><span data-stu-id="34ea5-153">string</span></span>  | <span data-ttu-id="34ea5-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="34ea5-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="34ea5-156">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="34ea5-156">Request body</span></span>
<span data-ttu-id="34ea5-157">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="34ea5-157">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="34ea5-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="34ea5-158">Response</span></span>
### <a name="response-for-getting-the-photo"></a><span data-ttu-id="34ea5-159">Отклик для запроса на получение фотографии</span><span class="sxs-lookup"><span data-stu-id="34ea5-159">Response for getting the photo</span></span>
<span data-ttu-id="34ea5-p106">При успешном выполнении этот метод возвращает код отклика `200 OK` и двоичные данные запрашиваемой фотографии.  Если фотография не существует, операция возвратит отклик `404 Not Found`.</span><span class="sxs-lookup"><span data-stu-id="34ea5-p106">If successful, this method returns a `200 OK` response code and binary data of the requested photo.  If no photo exists, the operation returns `404 Not Found`.</span></span>
### <a name="response-for-getting-the-metadata-of-the-photo"></a><span data-ttu-id="34ea5-162">Отклик для запроса на получение метаданных фотографии</span><span class="sxs-lookup"><span data-stu-id="34ea5-162">Response for getting the metadata of the photo</span></span>
<span data-ttu-id="34ea5-163">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [profilePhoto](../resources/profilephoto.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="34ea5-163">If successful, this method returns a `200 OK` response code and [profilePhoto](../resources/profilephoto.md) object in the response body.</span></span>
## <a name="examples"></a><span data-ttu-id="34ea5-164">Примеры</span><span class="sxs-lookup"><span data-stu-id="34ea5-164">Examples</span></span>

### <a name="example-1-get-the-photo-for-the-signed-in-user-in-the-largest-available-size"></a><span data-ttu-id="34ea5-165">Пример 1. Получение фотографии пользователя, вошедшего в систему, с максимальным доступным размером</span><span class="sxs-lookup"><span data-stu-id="34ea5-165">Example 1: Get the photo for the signed-in user in the largest available size</span></span>
##### <a name="request"></a><span data-ttu-id="34ea5-166">Запрос</span><span class="sxs-lookup"><span data-stu-id="34ea5-166">Request</span></span>
<!-- {
  "blockType": "ignored"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/photo/$value
```

##### <a name="response"></a><span data-ttu-id="34ea5-167">Отклик</span><span class="sxs-lookup"><span data-stu-id="34ea5-167">Response</span></span> 
<span data-ttu-id="34ea5-168">Содержит двоичные данные запрошенной фотографии.</span><span class="sxs-lookup"><span data-stu-id="34ea5-168">Contains the binary data of the requested photo.</span></span> <span data-ttu-id="34ea5-169">Код HTTP-отклика: 200.</span><span class="sxs-lookup"><span data-stu-id="34ea5-169">The HTTP response code is 200.</span></span>

### <a name="example-2-get-the-48x48-photo-for-the-signed-in-use"></a><span data-ttu-id="34ea5-170">Пример 2. Получение фотографии 48 x 48 для вошедшего пользователя</span><span class="sxs-lookup"><span data-stu-id="34ea5-170">Example 2: Get the 48x48 photo for the signed-in use</span></span>
##### <a name="request"></a><span data-ttu-id="34ea5-171">Запрос</span><span class="sxs-lookup"><span data-stu-id="34ea5-171">Request</span></span>
<!-- {
  "blockType": "ignored"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/photos/48x48/$value
Content-Type: image/jpg
```

##### <a name="response"></a><span data-ttu-id="34ea5-172">Отклик</span><span class="sxs-lookup"><span data-stu-id="34ea5-172">Response</span></span>
<span data-ttu-id="34ea5-173">Содержит двоичные данные запрошенной фотографии 48 x 48.</span><span class="sxs-lookup"><span data-stu-id="34ea5-173">Contains the binary data of the requested 48x48 photo.</span></span> <span data-ttu-id="34ea5-174">Код HTTP-отклика: 200.</span><span class="sxs-lookup"><span data-stu-id="34ea5-174">The HTTP response code is 200.</span></span>

### <a name="example-3-get-the-metadata-of-the-user-photo-of-the-signed-in-user"></a><span data-ttu-id="34ea5-175">Пример 3. Получение метаданных фотографии вошедшего пользователя</span><span class="sxs-lookup"><span data-stu-id="34ea5-175">Example 3: Get the metadata of the user photo of the signed-in user</span></span>
##### <a name="request"></a><span data-ttu-id="34ea5-176">Запрос</span><span class="sxs-lookup"><span data-stu-id="34ea5-176">Request</span></span>
<!-- {
  "blockType": "ignored"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/photo
```

##### <a name="response"></a><span data-ttu-id="34ea5-177">Отклик</span><span class="sxs-lookup"><span data-stu-id="34ea5-177">Response</span></span>

<span data-ttu-id="34ea5-178">В данных указанного ниже отклика содержатся метаданные фотографии.</span><span class="sxs-lookup"><span data-stu-id="34ea5-178">The following response data shows the photo metadata.</span></span> 

><span data-ttu-id="34ea5-179">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="34ea5-179">**Note:** The response object shown here might be shortened for readability.</span></span>
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

<span data-ttu-id="34ea5-180">Ниже показаны данные отклика в случае, если фотография пользователя еще не выложена.</span><span class="sxs-lookup"><span data-stu-id="34ea5-180">The following response data shows the contents of a response when a photo hasn't already been uploaded for the user.</span></span>

><span data-ttu-id="34ea5-181">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="34ea5-181">**Note:** The response object shown here might be shortened for readability.</span></span>

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
## <a name="using-the-binary-data-of-the-requested-photo"></a><span data-ttu-id="34ea5-182">Использование двоичных данных запрошенной фотографии</span><span class="sxs-lookup"><span data-stu-id="34ea5-182">Using the binary data of the requested photo</span></span>

<span data-ttu-id="34ea5-183">Когда вы используете конечную точку `/photo/$value` для получения двоичных данных для фотографии профиля, потребуется преобразовать эти данные в строку Base64, чтобы добавить их как вложение электронной почты.</span><span class="sxs-lookup"><span data-stu-id="34ea5-183">When you use the `/photo/$value` endpoint to get the binary data for a profile photo, you'll need to convert the data into a base-64 string in order to add it as an email attachment.</span></span> <span data-ttu-id="34ea5-184">Ниже приведен пример кода JavaScript, показывающий, как создать массив, который можно передать как значение параметра `Attachments` для [сообщения Outlook](user-post-messages.md).</span><span class="sxs-lookup"><span data-stu-id="34ea5-184">Here is an example in JavaScript of how to create an array that you can pass as the value of the `Attachments` parameter of an [Outlook Message](user-post-messages.md).</span></span>

      const attachments = [{
        '@odata.type': '#microsoft.graph.fileAttachment',
        ContentBytes: file.toString('base64'),
        Name: 'mypic.jpg'
      }];

<span data-ttu-id="34ea5-185">Ознакомиться с реализацией этого примера можно в статье [Пример подключения к Microsoft Graph для Node.js](https://github.com/microsoftgraph/nodejs-connect-rest-sample).</span><span class="sxs-lookup"><span data-stu-id="34ea5-185">See the [Microsoft Graph Connect Sample for Node.js](https://github.com/microsoftgraph/nodejs-connect-rest-sample) for an implementation of this example.</span></span>

<span data-ttu-id="34ea5-186">Если требуется, чтобы изображение отображалось на веб-странице, создайте объект в памяти на его основе и сделайте этот объект источником элемента изображения.</span><span class="sxs-lookup"><span data-stu-id="34ea5-186">If you want to display the image on a web page, create an in-memory object from the image and make that object the source of an image element.</span></span> <span data-ttu-id="34ea5-187">Ниже приведен пример кода JavaScript для этой операции.</span><span class="sxs-lookup"><span data-stu-id="34ea5-187">Here is an example in JavaScript of this operation.</span></span>

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

---
title: Получение фотографии
description: Получение указанного объекта profilePhoto или его метаданных (свойств profilePhoto).
localization_priority: Priority
author: kevinbellinger
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: c3bd5a0d69ab392fc55ac1f44bfbe3dc6d74ad08
ms.sourcegitcommit: de175a11806f9e9ba3c916384e897aee1cc7f75c
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/09/2021
ms.locfileid: "49790617"
---
# <a name="get-photo"></a><span data-ttu-id="2bc5c-103">Получение фотографии</span><span class="sxs-lookup"><span data-stu-id="2bc5c-103">Get photo</span></span>

<span data-ttu-id="2bc5c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2bc5c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="2bc5c-105">Получение указанного объекта [profilePhoto](../resources/profilephoto.md) или его метаданных (свойств profilePhoto).</span><span class="sxs-lookup"><span data-stu-id="2bc5c-105">Get the specified [profilePhoto](../resources/profilephoto.md) or its metadata (profilePhoto properties).</span></span>

> <span data-ttu-id="2bc5c-106">**Примечание.** Эта операция в версии 1.0 поддерживает только рабочие или учебные почтовые ящики пользователя (не личные).</span><span class="sxs-lookup"><span data-stu-id="2bc5c-106">**Note** This operation in version 1.0 supports only a user's work or school mailboxes and not personal mailboxes.</span></span>

<span data-ttu-id="2bc5c-107">Поддерживаемые размеры фотографий в формате HD для Microsoft 365: 48 x 48, 64 x 64, 96 x 96, 120 x 120, 240 x 240, 360 x 360, 432 x 432, 504 x 504 и 648 x 648.</span><span class="sxs-lookup"><span data-stu-id="2bc5c-107">The supported sizes of HD photos on Microsoft 365 are as follows: 48x48, 64x64, 96x96, 120x120, 240x240, 360x360, 432x432, 504x504, and 648x648.</span></span> <span data-ttu-id="2bc5c-108">Фотографии могут быть любого размера, если они хранятся в Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="2bc5c-108">Photos can be any dimension if they are stored in Azure Active Directory.</span></span>

<span data-ttu-id="2bc5c-109">Вы можете получить метаданные самой большой доступной фотографии или указать размер и получить метаданные для этого размера.</span><span class="sxs-lookup"><span data-stu-id="2bc5c-109">You can get the metadata of the largest available photo, or specify a size to get the metadata for that photo size.</span></span>
<span data-ttu-id="2bc5c-110">Если запрашиваемый размер недоступен, вы можете получить меньший размер, загруженный пользователем.</span><span class="sxs-lookup"><span data-stu-id="2bc5c-110">If the size you request is not available, you can still get a smaller size that the user has uploaded and made available.</span></span>
<span data-ttu-id="2bc5c-111">Например, если пользователь загрузит фотографию размером 504 x 504 пикселя, для скачивания будут доступны все размеры, кроме 648 x 648.</span><span class="sxs-lookup"><span data-stu-id="2bc5c-111">For example, if the user uploads a photo that is 504x504 pixels, all but the 648x648 size of photo will be available for download.</span></span>

## <a name="permissions"></a><span data-ttu-id="2bc5c-112">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2bc5c-112">Permissions</span></span>

<span data-ttu-id="2bc5c-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2bc5c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2bc5c-115">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2bc5c-115">Permission type</span></span>      | <span data-ttu-id="2bc5c-116">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2bc5c-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2bc5c-117">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2bc5c-117">Delegated (work or school account)</span></span> | <span data-ttu-id="2bc5c-118">Для ресурса **user**:</span><span class="sxs-lookup"><span data-stu-id="2bc5c-118">For **user** resource:</span></span><br/><span data-ttu-id="2bc5c-119">User.Read, User.ReadBasic.All, User.Read.All, User.ReadWrite, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2bc5c-119">User.Read, User.ReadBasic.All, User.Read.All, User.ReadWrite, User.ReadWrite.All</span></span><br /><br /><span data-ttu-id="2bc5c-120">Для ресурса **group**:</span><span class="sxs-lookup"><span data-stu-id="2bc5c-120">For **group** resource:</span></span><br /><span data-ttu-id="2bc5c-121">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2bc5c-121">Group.Read.All, Group.ReadWrite.All</span></span><br /><br /><span data-ttu-id="2bc5c-122">Для ресурса **contact**:</span><span class="sxs-lookup"><span data-stu-id="2bc5c-122">For **contact** resource:</span></span><br /><span data-ttu-id="2bc5c-123">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2bc5c-123">Contacts.Read, Contacts.ReadWrite</span></span> |
|<span data-ttu-id="2bc5c-124">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2bc5c-124">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2bc5c-125">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="2bc5c-125">Not supported</span></span> |
|<span data-ttu-id="2bc5c-126">Для приложения</span><span class="sxs-lookup"><span data-stu-id="2bc5c-126">Application</span></span>                        | <span data-ttu-id="2bc5c-127">Для ресурса **user**:</span><span class="sxs-lookup"><span data-stu-id="2bc5c-127">For **user** resource:</span></span><br/><span data-ttu-id="2bc5c-128">User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2bc5c-128">User.Read.All, User.ReadWrite.All</span></span><br /><br /><span data-ttu-id="2bc5c-129">Для ресурса **group**:</span><span class="sxs-lookup"><span data-stu-id="2bc5c-129">For **group** resource:</span></span><br /><span data-ttu-id="2bc5c-130">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2bc5c-130">Group.Read.All, Group.ReadWrite.All</span></span><br /><br /><span data-ttu-id="2bc5c-131">Для ресурса **contact**:</span><span class="sxs-lookup"><span data-stu-id="2bc5c-131">For **contact** resource:</span></span><br /><span data-ttu-id="2bc5c-132">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2bc5c-132">Contacts.Read, Contacts.ReadWrite</span></span> |

> <span data-ttu-id="2bc5c-133">**Примечание.** В настоящее время существует [известная проблема](/graph/known-issues#groups) с доступом к фотографиям группы с помощью разрешений для приложений.</span><span class="sxs-lookup"><span data-stu-id="2bc5c-133">**Note:**  There is currently a [known issue](/graph/known-issues#groups) with accessing group photos using application permissions.</span></span>

## <a name="http-request"></a><span data-ttu-id="2bc5c-134">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2bc5c-134">HTTP request</span></span>

### <a name="get-the-photo"></a><span data-ttu-id="2bc5c-135">Получение фотографии</span><span class="sxs-lookup"><span data-stu-id="2bc5c-135">Get the photo</span></span>
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

### <a name="get-the-metadata-of-the-photo"></a><span data-ttu-id="2bc5c-136">Получение метаданных фотографии</span><span class="sxs-lookup"><span data-stu-id="2bc5c-136">Get the metadata of the photo</span></span>
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

### <a name="get-the-metadata-for-a-specific-photo-size"></a><span data-ttu-id="2bc5c-137">Получение метаданных фотографии определенного размера</span><span class="sxs-lookup"><span data-stu-id="2bc5c-137">Get the metadata for a specific photo size</span></span>
<!-- { "blockType": "ignored" } -->

```http
GET /me/photos/{size}
GET /users/{id | userPrincipalName}/photos/{size}
GET /groups/{id}/photos/{size}
```

## <a name="path-parameters"></a><span data-ttu-id="2bc5c-138">Параметры пути</span><span class="sxs-lookup"><span data-stu-id="2bc5c-138">Path parameters</span></span>

|<span data-ttu-id="2bc5c-139">Параметр</span><span class="sxs-lookup"><span data-stu-id="2bc5c-139">Parameter</span></span>|<span data-ttu-id="2bc5c-140">Тип</span><span class="sxs-lookup"><span data-stu-id="2bc5c-140">Type</span></span>|<span data-ttu-id="2bc5c-141">Описание</span><span class="sxs-lookup"><span data-stu-id="2bc5c-141">Description</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="2bc5c-142">size</span><span class="sxs-lookup"><span data-stu-id="2bc5c-142">size</span></span>  |<span data-ttu-id="2bc5c-143">String</span><span class="sxs-lookup"><span data-stu-id="2bc5c-143">String</span></span>  | <span data-ttu-id="2bc5c-144">Размер фотографии.</span><span class="sxs-lookup"><span data-stu-id="2bc5c-144">A photo size.</span></span> <span data-ttu-id="2bc5c-145">Поддерживаемые размеры фотографий в формате HD для Microsoft 365: 48 x 48, 64 x 64, 96 x 96, 120 x 120, 240 x 240, 360 x 360, 432 x 432, 504 x 504 и 648 x 648.</span><span class="sxs-lookup"><span data-stu-id="2bc5c-145">The supported sizes of HD photos on Microsoft 365 are as follows: 48x48, 64x64, 96x96, 120x120, 240x240, 360x360, 432x432, 504x504, and 648x648.</span></span> <span data-ttu-id="2bc5c-146">Фотографии могут быть любого размера, если они хранятся в Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="2bc5c-146">Photos can be any dimension if they are stored in Azure Active Directory.</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="2bc5c-147">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="2bc5c-147">Optional query parameters</span></span>
<span data-ttu-id="2bc5c-148">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="2bc5c-148">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2bc5c-149">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2bc5c-149">Request headers</span></span>

| <span data-ttu-id="2bc5c-150">Имя</span><span class="sxs-lookup"><span data-stu-id="2bc5c-150">Name</span></span>       | <span data-ttu-id="2bc5c-151">Тип</span><span class="sxs-lookup"><span data-stu-id="2bc5c-151">Type</span></span> | <span data-ttu-id="2bc5c-152">Описание</span><span class="sxs-lookup"><span data-stu-id="2bc5c-152">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="2bc5c-153">Authorization</span><span class="sxs-lookup"><span data-stu-id="2bc5c-153">Authorization</span></span>  | <span data-ttu-id="2bc5c-154">string</span><span class="sxs-lookup"><span data-stu-id="2bc5c-154">string</span></span>  | <span data-ttu-id="2bc5c-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2bc5c-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2bc5c-157">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2bc5c-157">Request body</span></span>
<span data-ttu-id="2bc5c-158">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2bc5c-158">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2bc5c-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="2bc5c-159">Response</span></span>
### <a name="response-for-getting-the-photo"></a><span data-ttu-id="2bc5c-160">Отклик для запроса на получение фотографии</span><span class="sxs-lookup"><span data-stu-id="2bc5c-160">Response for getting the photo</span></span>
<span data-ttu-id="2bc5c-p106">При успешном выполнении этот метод возвращает код отклика `200 OK` и двоичные данные запрашиваемой фотографии.  Если фотография не существует, операция возвратит отклик `404 Not Found`.</span><span class="sxs-lookup"><span data-stu-id="2bc5c-p106">If successful, this method returns a `200 OK` response code and binary data of the requested photo.  If no photo exists, the operation returns `404 Not Found`.</span></span>
### <a name="response-for-getting-the-metadata-of-the-photo"></a><span data-ttu-id="2bc5c-163">Отклик для запроса на получение метаданных фотографии</span><span class="sxs-lookup"><span data-stu-id="2bc5c-163">Response for getting the metadata of the photo</span></span>
<span data-ttu-id="2bc5c-164">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [profilePhoto](../resources/profilephoto.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2bc5c-164">If successful, this method returns a `200 OK` response code and [profilePhoto](../resources/profilephoto.md) object in the response body.</span></span>
## <a name="examples"></a><span data-ttu-id="2bc5c-165">Примеры</span><span class="sxs-lookup"><span data-stu-id="2bc5c-165">Examples</span></span>

### <a name="example-1-get-the-photo-for-the-signed-in-user-in-the-largest-available-size"></a><span data-ttu-id="2bc5c-166">Пример 1. Получение фотографии пользователя, вошедшего в систему, с максимальным доступным размером</span><span class="sxs-lookup"><span data-stu-id="2bc5c-166">Example 1: Get the photo for the signed-in user in the largest available size</span></span>
##### <a name="request"></a><span data-ttu-id="2bc5c-167">Запрос</span><span class="sxs-lookup"><span data-stu-id="2bc5c-167">Request</span></span>
<!-- {
  "blockType": "ignored"
}-->

```http
GET https://graph.microsoft.com/v1.0/me/photo/$value
```

##### <a name="response"></a><span data-ttu-id="2bc5c-168">Отклик</span><span class="sxs-lookup"><span data-stu-id="2bc5c-168">Response</span></span>
<span data-ttu-id="2bc5c-169">Содержит двоичные данные запрошенной фотографии.</span><span class="sxs-lookup"><span data-stu-id="2bc5c-169">Contains the binary data of the requested photo.</span></span> <span data-ttu-id="2bc5c-170">Код HTTP-отклика: 200.</span><span class="sxs-lookup"><span data-stu-id="2bc5c-170">The HTTP response code is 200.</span></span>

### <a name="example-2-get-the-48x48-photo-for-the-signed-in-user"></a><span data-ttu-id="2bc5c-171">Пример 2. Получение фотографии 48 x 48 для вошедшего пользователя</span><span class="sxs-lookup"><span data-stu-id="2bc5c-171">Example 2: Get the 48x48 photo for the signed-in user</span></span>
##### <a name="request"></a><span data-ttu-id="2bc5c-172">Запрос</span><span class="sxs-lookup"><span data-stu-id="2bc5c-172">Request</span></span>
<!-- {
  "blockType": "ignored"
}-->

```http
GET https://graph.microsoft.com/v1.0/me/photos/48x48/$value
Content-Type: image/jpg
```

##### <a name="response"></a><span data-ttu-id="2bc5c-173">Отклик</span><span class="sxs-lookup"><span data-stu-id="2bc5c-173">Response</span></span>
<span data-ttu-id="2bc5c-174">Содержит двоичные данные запрошенной фотографии 48 x 48.</span><span class="sxs-lookup"><span data-stu-id="2bc5c-174">Contains the binary data of the requested 48x48 photo.</span></span> <span data-ttu-id="2bc5c-175">Код HTTP-отклика: 200.</span><span class="sxs-lookup"><span data-stu-id="2bc5c-175">The HTTP response code is 200.</span></span>

### <a name="example-3-get-the-metadata-of-the-user-photo-of-the-signed-in-user"></a><span data-ttu-id="2bc5c-176">Пример 3. Получение метаданных фотографии вошедшего пользователя</span><span class="sxs-lookup"><span data-stu-id="2bc5c-176">Example 3: Get the metadata of the user photo of the signed-in user</span></span>
##### <a name="request"></a><span data-ttu-id="2bc5c-177">Запрос</span><span class="sxs-lookup"><span data-stu-id="2bc5c-177">Request</span></span>
<!-- {
  "blockType": "ignored"
}-->

```http
GET https://graph.microsoft.com/v1.0/me/photo
```

##### <a name="response"></a><span data-ttu-id="2bc5c-178">Отклик</span><span class="sxs-lookup"><span data-stu-id="2bc5c-178">Response</span></span>

<span data-ttu-id="2bc5c-179">В данных указанного ниже отклика содержатся метаданные фотографии.</span><span class="sxs-lookup"><span data-stu-id="2bc5c-179">The following response data shows the photo metadata.</span></span>

><span data-ttu-id="2bc5c-180">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="2bc5c-180">**Note:** The response object shown here might be shortened for readability.</span></span>
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

<span data-ttu-id="2bc5c-181">Ниже показаны данные отклика в случае, если фотография пользователя еще не выложена.</span><span class="sxs-lookup"><span data-stu-id="2bc5c-181">The following response data shows the contents of a response when a photo hasn't already been uploaded for the user.</span></span>

><span data-ttu-id="2bc5c-182">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="2bc5c-182">**Note:** The response object shown here might be shortened for readability.</span></span>

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

## <a name="using-the-binary-data-of-the-requested-photo"></a><span data-ttu-id="2bc5c-183">Использование двоичных данных запрошенной фотографии</span><span class="sxs-lookup"><span data-stu-id="2bc5c-183">Using the binary data of the requested photo</span></span>

<span data-ttu-id="2bc5c-184">Когда вы используете конечную точку `/photo/$value` для получения двоичных данных для фотографии профиля, потребуется преобразовать эти данные в строку Base64, чтобы добавить их как вложение электронной почты.</span><span class="sxs-lookup"><span data-stu-id="2bc5c-184">When you use the `/photo/$value` endpoint to get the binary data for a profile photo, you'll need to convert the data into a base-64 string in order to add it as an email attachment.</span></span> <span data-ttu-id="2bc5c-185">Ниже приведен пример кода JavaScript, показывающий, как создать массив, который можно передать как значение параметра `Attachments` для [сообщения Outlook](user-post-messages.md).</span><span class="sxs-lookup"><span data-stu-id="2bc5c-185">Here is an example in JavaScript of how to create an array that you can pass as the value of the `Attachments` parameter of an [Outlook Message](user-post-messages.md).</span></span>

```java
const attachments = [{
  '@odata.type': '#microsoft.graph.fileAttachment',
  ContentBytes: file.toString('base64'),
  Name: 'mypic.jpg'
}];
```

<span data-ttu-id="2bc5c-186">Ознакомиться с реализацией этого примера можно в статье [Пример подключения к Microsoft Graph для Node.js](https://github.com/microsoftgraph/nodejs-connect-rest-sample).</span><span class="sxs-lookup"><span data-stu-id="2bc5c-186">See the [Microsoft Graph Connect Sample for Node.js](https://github.com/microsoftgraph/nodejs-connect-rest-sample) for an implementation of this example.</span></span>

<span data-ttu-id="2bc5c-187">Если требуется, чтобы изображение отображалось на веб-странице, создайте объект в памяти на его основе и сделайте этот объект источником элемента изображения.</span><span class="sxs-lookup"><span data-stu-id="2bc5c-187">If you want to display the image on a web page, create an in-memory object from the image and make that object the source of an image element.</span></span> <span data-ttu-id="2bc5c-188">Ниже приведен пример кода JavaScript для этой операции.</span><span class="sxs-lookup"><span data-stu-id="2bc5c-188">Here is an example in JavaScript of this operation.</span></span>

```javascript
const url = window.URL || window.webkitURL;
const blobUrl = url.createObjectURL(image.data);
document.getElementById(imageElement).setAttribute("src", blobUrl);
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get photo",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


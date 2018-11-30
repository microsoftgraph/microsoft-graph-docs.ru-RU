---
title: Получение фотографии
description: Получите указанный profilePhoto или метаданных (**profilePhoto** свойства).
ms.openlocfilehash: 6374680e37d409a89b61d3e2244b45ccb29869e7
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27082784"
---
# <a name="get-photo"></a><span data-ttu-id="9411d-103">Получение фотографии</span><span class="sxs-lookup"><span data-stu-id="9411d-103">Get photo</span></span>

> <span data-ttu-id="9411d-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="9411d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9411d-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9411d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9411d-106">Получите указанный [profilePhoto](../resources/profilephoto.md) или метаданных (**profilePhoto** свойства).</span><span class="sxs-lookup"><span data-stu-id="9411d-106">Get the specified [profilePhoto](../resources/profilephoto.md) or its metadata (**profilePhoto** properties).</span></span>

<span data-ttu-id="9411d-107">GET фотографий операция первая попытка получить указанного фотографий с Office 365.</span><span class="sxs-lookup"><span data-stu-id="9411d-107">A GET photo operation first attempt to retrieve the specified photo from Office 365.</span></span> <span data-ttu-id="9411d-108">Если фотографии не поддерживается в Office 365, API пытается получить фотографии из Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="9411d-108">If the photo is not available in Office 365, the API attempts to retrieve the photo from Azure Active Directory.</span></span>

<span data-ttu-id="9411d-109">Поддерживаемые размеры фотографий в формате HD для Office 365: 48 x 48, 64 x 64, 96 x 96, 120 x 120, 240 x 240, 360 x 360, 432 x 432, 504 x 504 и 648 x 648.</span><span class="sxs-lookup"><span data-stu-id="9411d-109">The supported sizes of HD photos on Office 365 are as follows: '48x48', '64x64', '96x96', '120x120', '240x240', '360x360','432x432', '504x504', and '648x648'.</span></span> <span data-ttu-id="9411d-110">Фотографии могут быть любого размера, если они хранятся в Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="9411d-110">Photos can be any dimension if they are stored in Azure Active Directory.</span></span>

<span data-ttu-id="9411d-111">Вы можете получить метаданные самой большой доступной фотографии или указать размер и получить метаданные для этого размера.</span><span class="sxs-lookup"><span data-stu-id="9411d-111">You can get the metadata of the largest available photo, or specify a size to get the metadata for that photo size.</span></span>
<span data-ttu-id="9411d-112">Если запрашиваемый размер недоступен, вы можете получить меньший размер, загруженный пользователем.</span><span class="sxs-lookup"><span data-stu-id="9411d-112">If the size you request is not available, you can still get a smaller size that the user has uploaded and made available.</span></span>
<span data-ttu-id="9411d-113">Например, если пользователь загрузит фотографию размером 504 x 504 пикселя, для скачивания будут доступны все размеры, кроме 648 x 648.</span><span class="sxs-lookup"><span data-stu-id="9411d-113">For example, if the user uploads a photo that is 504x504 pixels, then all but the 648x648 size of photo will be available for download.</span></span>
<span data-ttu-id="9411d-114">Если указанный размер недоступен в почтовом ящике пользователя или Azure Active Directory, возвращается размер 1 x 1 и остальные метаданные.</span><span class="sxs-lookup"><span data-stu-id="9411d-114">If the specified size is not available in the user's mailbox or in Azure Active Directory, the size of '1x1' is returned with the rest of metadata.</span></span>

## <a name="permissions"></a><span data-ttu-id="9411d-115">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9411d-115">Permissions</span></span>
<span data-ttu-id="9411d-p105">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9411d-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

> <span data-ttu-id="9411d-118">**Примечание:** Операцию GET фотографий в бета-версии поддерживает работой, школа или личных учетных записей пользователя.</span><span class="sxs-lookup"><span data-stu-id="9411d-118">**Note:** The GET photo operation in beta supports a user's work, school, or personal accounts.</span></span> <span data-ttu-id="9411d-119">Операцию GET метаданных фотографий тем не менее, поддерживает только пользователя рабочий или школа учетных записей и не личных учетных записей.</span><span class="sxs-lookup"><span data-stu-id="9411d-119">The GET photo metadata operation, however, supports only the user's work or school accounts and not personal accounts.</span></span>

|<span data-ttu-id="9411d-120">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9411d-120">Permission type</span></span>      | <span data-ttu-id="9411d-121">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9411d-121">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9411d-122">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9411d-122">Delegated (work or school account)</span></span> | <span data-ttu-id="9411d-123">Для ресурса **user**:</span><span class="sxs-lookup"><span data-stu-id="9411d-123">For **user** resource:</span></span><br/><span data-ttu-id="9411d-124">User.Read, User.ReadBasic.All, User.Read.All, User.ReadWrite, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9411d-124">User.Read, User.ReadBasic.All, User.Read.All, User.ReadWrite, User.ReadWrite.All</span></span><br /><br /><span data-ttu-id="9411d-125">Для ресурса **group**:</span><span class="sxs-lookup"><span data-stu-id="9411d-125">For **group** resource:</span></span><br /><span data-ttu-id="9411d-126">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9411d-126">Group.Read.All, Group.ReadWrite.All</span></span><br /><br /><span data-ttu-id="9411d-127">Для ресурса **contact**:</span><span class="sxs-lookup"><span data-stu-id="9411d-127">For **contact** resource:</span></span><br /><span data-ttu-id="9411d-128">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9411d-128">Contacts.Read, Contacts.ReadWrite</span></span> |
|<span data-ttu-id="9411d-129">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9411d-129">Delegated (personal Microsoft account)</span></span>  <br /> <span data-ttu-id="9411d-130">**Примечание**: операция метаданных не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9411d-130">**Note**: Metadata operation is not supported.</span></span> | <span data-ttu-id="9411d-131">Для ресурса **user**:</span><span class="sxs-lookup"><span data-stu-id="9411d-131">For **user** resource:</span></span><br/><span data-ttu-id="9411d-132">User.Read, User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9411d-132">User.Read, User.ReadWrite</span></span><br /><br /><span data-ttu-id="9411d-133">Для ресурса **contact**:</span><span class="sxs-lookup"><span data-stu-id="9411d-133">For **contact** resource:</span></span><br /><span data-ttu-id="9411d-134">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9411d-134">Contacts.Read, Contacts.ReadWrite</span></span> |
|<span data-ttu-id="9411d-135">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9411d-135">Application</span></span>                        | <span data-ttu-id="9411d-136">Для ресурса **user**:</span><span class="sxs-lookup"><span data-stu-id="9411d-136">For **user** resource:</span></span><br/><span data-ttu-id="9411d-137">User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9411d-137">User.Read.All, User.ReadWrite.All</span></span><br /><br /><span data-ttu-id="9411d-138">Для ресурса **group**:</span><span class="sxs-lookup"><span data-stu-id="9411d-138">For **group** resource:</span></span><br /><span data-ttu-id="9411d-139">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9411d-139">Group.Read.All, Group.ReadWrite.All</span></span><br /><br /><span data-ttu-id="9411d-140">Для ресурса **contact**:</span><span class="sxs-lookup"><span data-stu-id="9411d-140">For **contact** resource:</span></span><br /><span data-ttu-id="9411d-141">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9411d-141">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="9411d-142">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9411d-142">HTTP request</span></span> 

### <a name="get-the-photo"></a><span data-ttu-id="9411d-143">Получение фотографий</span><span class="sxs-lookup"><span data-stu-id="9411d-143">Get the photo</span></span>
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
### <a name="get-the-metadata-of-the-photo"></a><span data-ttu-id="9411d-144">Получение метаданных фотографии</span><span class="sxs-lookup"><span data-stu-id="9411d-144">Get the metadata of the photo</span></span>
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

### <a name="get-the-metadata-for-a-specific-photo-size"></a><span data-ttu-id="9411d-145">Получить метаданные для определенного размера фотографии</span><span class="sxs-lookup"><span data-stu-id="9411d-145">Get the metadata for a specific photo size</span></span>
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

## <a name="path-parameters"></a><span data-ttu-id="9411d-146">Параметры пути</span><span class="sxs-lookup"><span data-stu-id="9411d-146">Path parameters</span></span>

|<span data-ttu-id="9411d-147">**Параметр**</span><span class="sxs-lookup"><span data-stu-id="9411d-147">**Parameter**</span></span>|<span data-ttu-id="9411d-148">**Тип**</span><span class="sxs-lookup"><span data-stu-id="9411d-148">**Type**</span></span>|<span data-ttu-id="9411d-149">**Описание**</span><span class="sxs-lookup"><span data-stu-id="9411d-149">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="9411d-150">size</span><span class="sxs-lookup"><span data-stu-id="9411d-150">size</span></span>  |<span data-ttu-id="9411d-151">String</span><span class="sxs-lookup"><span data-stu-id="9411d-151">String</span></span>  | <span data-ttu-id="9411d-152">Размер фотографии.</span><span class="sxs-lookup"><span data-stu-id="9411d-152">A photo size.</span></span> <span data-ttu-id="9411d-153">Поддерживаемые размеры фотографий в формате HD для Office 365: 48 x 48, 64 x 64, 96 x 96, 120 x 120, 240 x 240, 360 x 360, 432 x 432, 504 x 504 и 648 x 648.</span><span class="sxs-lookup"><span data-stu-id="9411d-153">The supported sizes of HD photos on Office 365 are as follows: '48x48', '64x64', '96x96', '120x120', '240x240', '360x360','432x432', '504x504', and '648x648'.</span></span> <span data-ttu-id="9411d-154">Фотографии могут быть любого размера, если они хранятся в Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="9411d-154">Photos can be any dimension if they are stored in Azure Active Directory.</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="9411d-155">Необязательные параметры запроса</span><span class="sxs-lookup"><span data-stu-id="9411d-155">Optional query parameters</span></span>
<span data-ttu-id="9411d-156">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="9411d-156">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9411d-157">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9411d-157">Request headers</span></span>
| <span data-ttu-id="9411d-158">Имя</span><span class="sxs-lookup"><span data-stu-id="9411d-158">Name</span></span>       | <span data-ttu-id="9411d-159">Тип</span><span class="sxs-lookup"><span data-stu-id="9411d-159">Type</span></span> | <span data-ttu-id="9411d-160">Описание</span><span class="sxs-lookup"><span data-stu-id="9411d-160">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="9411d-161">Authorization</span><span class="sxs-lookup"><span data-stu-id="9411d-161">Authorization</span></span>  | <span data-ttu-id="9411d-162">string</span><span class="sxs-lookup"><span data-stu-id="9411d-162">string</span></span>  | <span data-ttu-id="9411d-p108">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9411d-p108">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9411d-165">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9411d-165">Request body</span></span>
<span data-ttu-id="9411d-166">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9411d-166">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9411d-167">Ответ</span><span class="sxs-lookup"><span data-stu-id="9411d-167">Response</span></span>
### <a name="response-for-getting-the-photo"></a><span data-ttu-id="9411d-168">Отклик для запроса на получение фотографии</span><span class="sxs-lookup"><span data-stu-id="9411d-168">Response for getting the photo</span></span>
<span data-ttu-id="9411d-p109">При успешном выполнении этот метод возвращает код отклика `200 OK` и двоичные данные запрашиваемой фотографии.  Если фотография не существует, операция возвратит отклик `404 Not Found`.</span><span class="sxs-lookup"><span data-stu-id="9411d-p109">If successful, this method returns a `200 OK` response code and binary data of the requested photo.  If no photo exists, the operation returns `404 Not Found`.</span></span>
### <a name="response-for-getting-the-metadata-of-the-photo"></a><span data-ttu-id="9411d-171">Отклик для запроса на получение метаданных фотографии</span><span class="sxs-lookup"><span data-stu-id="9411d-171">Response for getting the metadata of the photo</span></span>
<span data-ttu-id="9411d-172">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [profilePhoto](../resources/profilephoto.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9411d-172">If successful, this method returns a `200 OK` response code and [profilePhoto](../resources/profilephoto.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9411d-173">Пример</span><span class="sxs-lookup"><span data-stu-id="9411d-173">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="9411d-174">Запрос 1</span><span class="sxs-lookup"><span data-stu-id="9411d-174">Request 1</span></span>
<span data-ttu-id="9411d-175">Этот запрос возвращает фотографию пользователя, вошедшего в систему, с максимальным доступным размером.</span><span class="sxs-lookup"><span data-stu-id="9411d-175">This request gets the photo for the signed-in user, in the largest available size.</span></span>

<!-- {
  "blockType": "ignored"
}-->
```http
GET https://graph.microsoft.com/beta/me/photo/$value
Content-Type: image/jpg
```

##### <a name="response-1"></a><span data-ttu-id="9411d-176">Отклик 1</span><span class="sxs-lookup"><span data-stu-id="9411d-176">Response 1</span></span>
<span data-ttu-id="9411d-p110">Содержит двоичные данные запрошенной фотографии. Код HTTP-отклика: 200.</span><span class="sxs-lookup"><span data-stu-id="9411d-p110">Contains the binary data of the requested photo. The HTTP response code is 200.</span></span>

##### <a name="request-2"></a><span data-ttu-id="9411d-179">Запрос 2</span><span class="sxs-lookup"><span data-stu-id="9411d-179">Request 2</span></span>
<span data-ttu-id="9411d-180">Этот запрос получает фотографию 48 x 48 для вошедшего пользователя.</span><span class="sxs-lookup"><span data-stu-id="9411d-180">This request gets the 48x48 photo for the signed-in user.</span></span>

<!-- {
  "blockType": "ignored"
}-->
```http
GET https://graph.microsoft.com/beta/me/photos/48x48/$value
Content-Type: image/jpg
```

##### <a name="response-2"></a><span data-ttu-id="9411d-181">Ответ 2</span><span class="sxs-lookup"><span data-stu-id="9411d-181">Response 2</span></span>
<span data-ttu-id="9411d-182">Содержит двоичные данные запрошенной фотографии 48 x 48.</span><span class="sxs-lookup"><span data-stu-id="9411d-182">Contains the binary data of the requested 48x48 photo.</span></span> <span data-ttu-id="9411d-183">Код HTTP-ответа: 200.</span><span class="sxs-lookup"><span data-stu-id="9411d-183">The HTTP response code is 200.</span></span>

##### <a name="request-3"></a><span data-ttu-id="9411d-184">Запрос 3</span><span class="sxs-lookup"><span data-stu-id="9411d-184">Request 3</span></span>
<span data-ttu-id="9411d-185">Этот запрос возвращает метаданные фотографии вошедшего пользователя.</span><span class="sxs-lookup"><span data-stu-id="9411d-185">This request gets the metadata of the user photo of the signed-in user.</span></span>

<!-- {
  "blockType": "ignored"
}-->
```http
GET https://graph.microsoft.com/beta/me/photo
```

##### <a name="response-3"></a><span data-ttu-id="9411d-186">Ответ 3</span><span class="sxs-lookup"><span data-stu-id="9411d-186">Response 3</span></span>
<span data-ttu-id="9411d-p112">В данных указанного ниже ответа содержатся метаданные фотографии. Примечание. Показанный здесь объект ответа может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="9411d-p112">The following response data shows the photo metadata. Note: The response object shown here may be truncated for brevity.</span></span>

<!-- {
  "blockType": "ignored"
}-->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Me/photo/$entity",
    "@odata.id": "https://graph.microsoft.com/beta/users('ddfcd489-628b-7d04-b48b-20075df800e5@1717622f-1d94-c0d4-9d74-f907ad6677b4')/photo",
    "@odata.mediaContentType": "image/jpeg",
    "@odata.mediaEtag": "\"BA09D118\"",
    "id": "240X240",
    "width": 240,
    "height": 240
}
```

<span data-ttu-id="9411d-p113">Ниже показаны данные отклика в случае, если фотография пользователя еще не выложена. Примечание. Показанный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="9411d-p113">The following response data shows the contents of a response when a photo hasn't already been uploaded for the user. Note: The response object shown here may be truncated for brevity.</span></span>

<!-- {
  "blockType": "ignored"
}-->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Me/photo/$entity",
    "@odata.id": "https://graph.microsoft.com/beta/users('ddfcd489-628b-7d04-b48b-20075df800e5@1717622f-1d94-c0d4-9d74-f907ad6677b4')/photo",
    "@odata.mediaContentType": "image/gif",
    "@odata.mediaEtag": "",
    "id": "1X1",
    "width": 1,
    "height": 1
}
```
## <a name="using-the-binary-data-of-the-requested-photo"></a><span data-ttu-id="9411d-191">Использование двоичных данных запрошенной фотографии</span><span class="sxs-lookup"><span data-stu-id="9411d-191">Using the binary data of the requested photo</span></span>

<span data-ttu-id="9411d-192">Когда вы используете конечную точку `/photo/$value` для получения двоичных данных для фотографии профиля, потребуется преобразовать эти данные в строку Base64, чтобы добавить их как вложение электронной почты.</span><span class="sxs-lookup"><span data-stu-id="9411d-192">When you use the `/photo/$value` endpoint to get the binary data for a profile photo, you'll need to convert the data into a base-64 string in order to add it as an email attachment.</span></span> <span data-ttu-id="9411d-193">Ниже приведен пример кода JavaScript, показывающий, как создать массив, который можно передать как значение параметра `Attachments` для [сообщения Outlook](user-post-messages.md).</span><span class="sxs-lookup"><span data-stu-id="9411d-193">Here is an example in JavaScript of how to create an array that you can pass as the value of the `Attachments` parameter of an [Outlook Message](user-post-messages.md).</span></span>

      const attachments = [{
        '@odata.type': '#microsoft.graph.fileAttachment',
        ContentBytes: file.toString('base64'),
        Name: 'mypic.jpg'
      }];

<span data-ttu-id="9411d-194">Ознакомиться с реализацией этого примера можно в статье [Пример подключения к Microsoft Graph для Node.js](https://github.com/microsoftgraph/nodejs-connect-rest-sample).</span><span class="sxs-lookup"><span data-stu-id="9411d-194">See the [Microsoft Graph Connect Sample for Node.js](https://github.com/microsoftgraph/nodejs-connect-rest-sample) for an implementation of this example.</span></span>

<span data-ttu-id="9411d-195">Если требуется, чтобы изображение отображалось на веб-странице, создайте объект в памяти на его основе и сделайте этот объект источником элемента изображения.</span><span class="sxs-lookup"><span data-stu-id="9411d-195">If you want to display the image on a web page, create an in-memory object from the image and make that object the source of an image element.</span></span> <span data-ttu-id="9411d-196">Ниже приведен пример кода JavaScript для этой операции.</span><span class="sxs-lookup"><span data-stu-id="9411d-196">Here is an example in JavaScript of this operation.</span></span>

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

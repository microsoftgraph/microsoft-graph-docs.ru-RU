---
title: Получение фотографии
description: Получение указанного объекта profilePhoto или его метаданных (свойств **profilePhoto**).
localization_priority: Priority
ms.openlocfilehash: 759c0ff3ac2585f43ea38963e10b001250702c56
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29509632"
---
# <a name="get-photo"></a><span data-ttu-id="e910f-103">Получение фотографии</span><span class="sxs-lookup"><span data-stu-id="e910f-103">Get photo</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e910f-104">Получение указанного объекта [profilePhoto](../resources/profilephoto.md) или его метаданных (свойств **profilePhoto**).</span><span class="sxs-lookup"><span data-stu-id="e910f-104">Get the specified [profilePhoto](../resources/profilephoto.md) or its metadata (**profilePhoto** properties).</span></span>

<span data-ttu-id="e910f-105">Операция GET photo сначала пытается получить указанную фотографию из Office 365.</span><span class="sxs-lookup"><span data-stu-id="e910f-105">A GET photo operation first attempt to retrieve the specified photo from Office 365.</span></span> <span data-ttu-id="e910f-106">Если фотография недоступна в Office 365, API пытается получить ее из Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="e910f-106">If the photo is not available in Office 365, the API attempts to retrieve the photo from Azure Active Directory.</span></span>

<span data-ttu-id="e910f-107">Поддерживаемые размеры фотографий в формате HD для Office 365: 48 x 48, 64 x 64, 96 x 96, 120 x 120, 240 x 240, 360 x 360, 432 x 432, 504 x 504 и 648 x 648.</span><span class="sxs-lookup"><span data-stu-id="e910f-107">The supported sizes of HD photos on Office 365 are as follows: '48x48', '64x64', '96x96', '120x120', '240x240', '360x360','432x432', '504x504', and '648x648'.</span></span> <span data-ttu-id="e910f-108">Фотографии могут быть любого размера, если они хранятся в Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="e910f-108">Photos can be any dimension if they are stored in Azure Active Directory.</span></span>

<span data-ttu-id="e910f-109">Вы можете получить метаданные самой большой доступной фотографии или указать размер и получить метаданные для этого размера.</span><span class="sxs-lookup"><span data-stu-id="e910f-109">You can get the metadata of the largest available photo, or specify a size to get the metadata for that photo size.</span></span>
<span data-ttu-id="e910f-110">Если запрашиваемый размер недоступен, вы можете получить меньший размер, загруженный пользователем.</span><span class="sxs-lookup"><span data-stu-id="e910f-110">If the size you request is not available, you can still get a smaller size that the user has uploaded and made available.</span></span>
<span data-ttu-id="e910f-111">Например, если пользователь загрузит фотографию размером 504 x 504 пикселя, для скачивания будут доступны все размеры, кроме 648 x 648.</span><span class="sxs-lookup"><span data-stu-id="e910f-111">For example, if the user uploads a photo that is 504x504 pixels, then all but the 648x648 size of photo will be available for download.</span></span>
<span data-ttu-id="e910f-112">Если указанный размер недоступен в почтовом ящике пользователя или Azure Active Directory, возвращается размер 1 x 1 и остальные метаданные.</span><span class="sxs-lookup"><span data-stu-id="e910f-112">If the specified size is not available in the user's mailbox or in Azure Active Directory, the size of '1x1' is returned with the rest of metadata.</span></span>

## <a name="permissions"></a><span data-ttu-id="e910f-113">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e910f-113">Permissions</span></span>
<span data-ttu-id="e910f-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e910f-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

> <span data-ttu-id="e910f-116">**Примечание.** Операция GET photo в бета-версии поддерживается для рабочих, учебных и личных учетных записей пользователя.</span><span class="sxs-lookup"><span data-stu-id="e910f-116">**Note:** The GET photo operation in beta supports a user's work, school, or personal accounts.</span></span> <span data-ttu-id="e910f-117">Однако операция GET photo metadata поддерживается только для рабочих или учебных, но не личных учетных записей пользователя.</span><span class="sxs-lookup"><span data-stu-id="e910f-117">The GET photo metadata operation, however, supports only the user's work or school accounts and not personal accounts.</span></span>

|<span data-ttu-id="e910f-118">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e910f-118">Permission type</span></span>      | <span data-ttu-id="e910f-119">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e910f-119">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e910f-120">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e910f-120">Delegated (work or school account)</span></span> | <span data-ttu-id="e910f-121">Для ресурса **user**:</span><span class="sxs-lookup"><span data-stu-id="e910f-121">For **user** resource:</span></span><br/><span data-ttu-id="e910f-122">User.Read, User.ReadBasic.All, User.Read.All, User.ReadWrite, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e910f-122">User.Read, User.ReadBasic.All, User.Read.All, User.ReadWrite, User.ReadWrite.All</span></span><br /><br /><span data-ttu-id="e910f-123">Для ресурса **group**:</span><span class="sxs-lookup"><span data-stu-id="e910f-123">For **group** resource:</span></span><br /><span data-ttu-id="e910f-124">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e910f-124">Group.Read.All, Group.ReadWrite.All</span></span><br /><br /><span data-ttu-id="e910f-125">Для ресурса **contact**:</span><span class="sxs-lookup"><span data-stu-id="e910f-125">For **contact** resource:</span></span><br /><span data-ttu-id="e910f-126">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e910f-126">Contacts.Read, Contacts.ReadWrite</span></span> |
|<span data-ttu-id="e910f-127">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e910f-127">Delegated (personal Microsoft account)</span></span>  <br /> <span data-ttu-id="e910f-128">**Примечание**. Операция получения метаданных не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e910f-128">**Note**: Metadata operation is not supported.</span></span> | <span data-ttu-id="e910f-129">Для ресурса **user**:</span><span class="sxs-lookup"><span data-stu-id="e910f-129">For **user** resource:</span></span><br/><span data-ttu-id="e910f-130">User.Read, User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e910f-130">User.Read, User.ReadWrite</span></span><br /><br /><span data-ttu-id="e910f-131">Для ресурса **contact**:</span><span class="sxs-lookup"><span data-stu-id="e910f-131">For **contact** resource:</span></span><br /><span data-ttu-id="e910f-132">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e910f-132">Contacts.Read, Contacts.ReadWrite</span></span> |
|<span data-ttu-id="e910f-133">Для приложения</span><span class="sxs-lookup"><span data-stu-id="e910f-133">Application</span></span>                        | <span data-ttu-id="e910f-134">Для ресурса **user**:</span><span class="sxs-lookup"><span data-stu-id="e910f-134">For **user** resource:</span></span><br/><span data-ttu-id="e910f-135">User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e910f-135">User.Read.All, User.ReadWrite.All</span></span><br /><br /><span data-ttu-id="e910f-136">Для ресурса **group**:</span><span class="sxs-lookup"><span data-stu-id="e910f-136">For **group** resource:</span></span><br /><span data-ttu-id="e910f-137">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e910f-137">Group.Read.All, Group.ReadWrite.All</span></span><br /><br /><span data-ttu-id="e910f-138">Для ресурса **contact**:</span><span class="sxs-lookup"><span data-stu-id="e910f-138">For **contact** resource:</span></span><br /><span data-ttu-id="e910f-139">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e910f-139">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="e910f-140">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e910f-140">HTTP request</span></span> 

### <a name="get-the-photo"></a><span data-ttu-id="e910f-141">Получение фотографии</span><span class="sxs-lookup"><span data-stu-id="e910f-141">Get the photo</span></span>
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
### <a name="get-the-metadata-of-the-photo"></a><span data-ttu-id="e910f-142">Получение метаданных фотографии</span><span class="sxs-lookup"><span data-stu-id="e910f-142">Get the metadata of the photo</span></span>
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

### <a name="get-the-metadata-for-a-specific-photo-size"></a><span data-ttu-id="e910f-143">Получение метаданных фотографии определенного размера</span><span class="sxs-lookup"><span data-stu-id="e910f-143">Get the metadata for a specific photo size</span></span>
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

## <a name="path-parameters"></a><span data-ttu-id="e910f-144">Параметры пути</span><span class="sxs-lookup"><span data-stu-id="e910f-144">Path parameters</span></span>

|<span data-ttu-id="e910f-145">**Параметр**</span><span class="sxs-lookup"><span data-stu-id="e910f-145">**Parameter**</span></span>|<span data-ttu-id="e910f-146">**Тип**</span><span class="sxs-lookup"><span data-stu-id="e910f-146">**Type**</span></span>|<span data-ttu-id="e910f-147">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e910f-147">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="e910f-148">size</span><span class="sxs-lookup"><span data-stu-id="e910f-148">size</span></span>  |<span data-ttu-id="e910f-149">String</span><span class="sxs-lookup"><span data-stu-id="e910f-149">String</span></span>  | <span data-ttu-id="e910f-150">Размер фотографии.</span><span class="sxs-lookup"><span data-stu-id="e910f-150">A photo size.</span></span> <span data-ttu-id="e910f-151">Поддерживаемые размеры фотографий в формате HD для Office 365: 48 x 48, 64 x 64, 96 x 96, 120 x 120, 240 x 240, 360 x 360, 432 x 432, 504 x 504 и 648 x 648.</span><span class="sxs-lookup"><span data-stu-id="e910f-151">The supported sizes of HD photos on Office 365 are as follows: '48x48', '64x64', '96x96', '120x120', '240x240', '360x360','432x432', '504x504', and '648x648'.</span></span> <span data-ttu-id="e910f-152">Фотографии могут быть любого размера, если они хранятся в Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="e910f-152">Photos can be any dimension if they are stored in Azure Active Directory.</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="e910f-153">Необязательные параметры запроса</span><span class="sxs-lookup"><span data-stu-id="e910f-153">Optional query parameters</span></span>
<span data-ttu-id="e910f-154">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="e910f-154">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e910f-155">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e910f-155">Request headers</span></span>
| <span data-ttu-id="e910f-156">Имя</span><span class="sxs-lookup"><span data-stu-id="e910f-156">Name</span></span>       | <span data-ttu-id="e910f-157">Тип</span><span class="sxs-lookup"><span data-stu-id="e910f-157">Type</span></span> | <span data-ttu-id="e910f-158">Описание</span><span class="sxs-lookup"><span data-stu-id="e910f-158">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="e910f-159">Authorization</span><span class="sxs-lookup"><span data-stu-id="e910f-159">Authorization</span></span>  | <span data-ttu-id="e910f-160">string</span><span class="sxs-lookup"><span data-stu-id="e910f-160">string</span></span>  | <span data-ttu-id="e910f-p107">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e910f-p107">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e910f-163">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e910f-163">Request body</span></span>
<span data-ttu-id="e910f-164">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e910f-164">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e910f-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="e910f-165">Response</span></span>
### <a name="response-for-getting-the-photo"></a><span data-ttu-id="e910f-166">Отклик для запроса на получение фотографии</span><span class="sxs-lookup"><span data-stu-id="e910f-166">Response for getting the photo</span></span>
<span data-ttu-id="e910f-p108">При успешном выполнении этот метод возвращает код отклика `200 OK` и двоичные данные запрашиваемой фотографии.  Если фотография не существует, операция возвратит отклик `404 Not Found`.</span><span class="sxs-lookup"><span data-stu-id="e910f-p108">If successful, this method returns a `200 OK` response code and binary data of the requested photo.  If no photo exists, the operation returns `404 Not Found`.</span></span>
### <a name="response-for-getting-the-metadata-of-the-photo"></a><span data-ttu-id="e910f-169">Отклик для запроса на получение метаданных фотографии</span><span class="sxs-lookup"><span data-stu-id="e910f-169">Response for getting the metadata of the photo</span></span>
<span data-ttu-id="e910f-170">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [profilePhoto](../resources/profilephoto.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e910f-170">If successful, this method returns a `200 OK` response code and [profilePhoto](../resources/profilephoto.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e910f-171">Пример</span><span class="sxs-lookup"><span data-stu-id="e910f-171">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="e910f-172">Запрос 1</span><span class="sxs-lookup"><span data-stu-id="e910f-172">Request 1</span></span>
<span data-ttu-id="e910f-173">Этот запрос возвращает фотографию пользователя, вошедшего в систему, с максимальным доступным размером.</span><span class="sxs-lookup"><span data-stu-id="e910f-173">This request gets the photo for the signed-in user, in the largest available size.</span></span>

<!-- {
  "blockType": "ignored"
}-->
```http
GET https://graph.microsoft.com/beta/me/photo/$value
Content-Type: image/jpg
```

##### <a name="response-1"></a><span data-ttu-id="e910f-174">Отклик 1</span><span class="sxs-lookup"><span data-stu-id="e910f-174">Response 1</span></span>
<span data-ttu-id="e910f-p109">Содержит двоичные данные запрошенной фотографии. Код HTTP-отклика: 200.</span><span class="sxs-lookup"><span data-stu-id="e910f-p109">Contains the binary data of the requested photo. The HTTP response code is 200.</span></span>

##### <a name="request-2"></a><span data-ttu-id="e910f-177">Запрос 2</span><span class="sxs-lookup"><span data-stu-id="e910f-177">Request 2</span></span>
<span data-ttu-id="e910f-178">Этот запрос получает фотографию 48 x 48 для вошедшего пользователя.</span><span class="sxs-lookup"><span data-stu-id="e910f-178">This request gets the 48x48 photo for the signed-in user.</span></span>

<!-- {
  "blockType": "ignored"
}-->
```http
GET https://graph.microsoft.com/beta/me/photos/48x48/$value
Content-Type: image/jpg
```

##### <a name="response-2"></a><span data-ttu-id="e910f-179">Отклик 2</span><span class="sxs-lookup"><span data-stu-id="e910f-179">Response 2</span></span>
<span data-ttu-id="e910f-180">Содержит двоичные данные запрошенной фотографии 48 x 48.</span><span class="sxs-lookup"><span data-stu-id="e910f-180">Contains the binary data of the requested 48x48 photo.</span></span> <span data-ttu-id="e910f-181">Код HTTP-ответа: 200.</span><span class="sxs-lookup"><span data-stu-id="e910f-181">The HTTP response code is 200.</span></span>

##### <a name="request-3"></a><span data-ttu-id="e910f-182">Запрос 3</span><span class="sxs-lookup"><span data-stu-id="e910f-182">Request 3</span></span>
<span data-ttu-id="e910f-183">Этот запрос возвращает метаданные фотографии вошедшего пользователя.</span><span class="sxs-lookup"><span data-stu-id="e910f-183">This request gets the metadata of the user photo of the signed-in user.</span></span>

<!-- {
  "blockType": "ignored"
}-->
```http
GET https://graph.microsoft.com/beta/me/photo
```

##### <a name="response-3"></a><span data-ttu-id="e910f-184">Отклик 3</span><span class="sxs-lookup"><span data-stu-id="e910f-184">Response 3</span></span>
<span data-ttu-id="e910f-p111">В данных указанного ниже отклика содержатся метаданные фотографии. Примечание. Показанный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="e910f-p111">The following response data shows the photo metadata. Note: The response object shown here may be truncated for brevity.</span></span>

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

<span data-ttu-id="e910f-p112">Ниже показаны данные отклика в случае, если фотография пользователя еще не выложена. Примечание. Показанный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="e910f-p112">The following response data shows the contents of a response when a photo hasn't already been uploaded for the user. Note: The response object shown here may be truncated for brevity.</span></span>

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
## <a name="using-the-binary-data-of-the-requested-photo"></a><span data-ttu-id="e910f-189">Использование двоичных данных запрошенной фотографии</span><span class="sxs-lookup"><span data-stu-id="e910f-189">Using the binary data of the requested photo</span></span>

<span data-ttu-id="e910f-190">Когда вы используете конечную точку `/photo/$value` для получения двоичных данных для фотографии профиля, потребуется преобразовать эти данные в строку Base64, чтобы добавить их как вложение электронной почты.</span><span class="sxs-lookup"><span data-stu-id="e910f-190">When you use the `/photo/$value` endpoint to get the binary data for a profile photo, you'll need to convert the data into a base-64 string in order to add it as an email attachment.</span></span> <span data-ttu-id="e910f-191">Ниже приведен пример кода JavaScript, показывающий, как создать массив, который можно передать как значение параметра `Attachments` для [сообщения Outlook](user-post-messages.md).</span><span class="sxs-lookup"><span data-stu-id="e910f-191">Here is an example in JavaScript of how to create an array that you can pass as the value of the `Attachments` parameter of an [Outlook Message](user-post-messages.md).</span></span>

      const attachments = [{
        '@odata.type': '#microsoft.graph.fileAttachment',
        ContentBytes: file.toString('base64'),
        Name: 'mypic.jpg'
      }];

<span data-ttu-id="e910f-192">Ознакомиться с реализацией этого примера можно в статье [Пример подключения к Microsoft Graph для Node.js](https://github.com/microsoftgraph/nodejs-connect-rest-sample).</span><span class="sxs-lookup"><span data-stu-id="e910f-192">See the [Microsoft Graph Connect Sample for Node.js](https://github.com/microsoftgraph/nodejs-connect-rest-sample) for an implementation of this example.</span></span>

<span data-ttu-id="e910f-193">Если требуется, чтобы изображение отображалось на веб-странице, создайте объект в памяти на его основе и сделайте этот объект источником элемента изображения.</span><span class="sxs-lookup"><span data-stu-id="e910f-193">If you want to display the image on a web page, create an in-memory object from the image and make that object the source of an image element.</span></span> <span data-ttu-id="e910f-194">Ниже приведен пример кода JavaScript для этой операции.</span><span class="sxs-lookup"><span data-stu-id="e910f-194">Here is an example in JavaScript of this operation.</span></span>

    const url = window.URL || window.webkitURL;
    const blobUrl = url.createObjectURL(image.data);
    document.getElementById(imageElement).setAttribute("src", blobUrl);

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get photo",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/profilephoto-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

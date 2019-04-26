---
title: Получение фотографии
description: Получение указанного объекта profilePhoto или его метаданных (свойств **profilePhoto**).
localization_priority: Priority
ms.openlocfilehash: 422b9cb39b7af6527341070cbe35f3bfb59d504d
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33337175"
---
# <a name="get-photo"></a><span data-ttu-id="d1dac-103">Получение фотографии</span><span class="sxs-lookup"><span data-stu-id="d1dac-103">Get photo</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d1dac-104">Получение указанного объекта [profilePhoto](../resources/profilephoto.md) или его метаданных (свойств **profilePhoto**).</span><span class="sxs-lookup"><span data-stu-id="d1dac-104">Get the specified [profilePhoto](../resources/profilephoto.md) or its metadata (**profilePhoto** properties).</span></span>

<span data-ttu-id="d1dac-105">Метод GET photo сначала пытается получить указанную фотографию из Office 365.</span><span class="sxs-lookup"><span data-stu-id="d1dac-105">A GET photo method first attempts to retrieve the specified photo from Office 365.</span></span> <span data-ttu-id="d1dac-106">Если фотография недоступна в Office 365, API пытается получить ее из Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="d1dac-106">If the photo is not available in Office 365, the API attempts to retrieve the photo from Azure Active Directory.</span></span>

<span data-ttu-id="d1dac-107">Поддерживаемые размеры фотографий в формате HD для Office 365: 48 x 48, 64 x 64, 96 x 96, 120 x 120, 240 x 240, 360 x 360, 432 x 432, 504 x 504 и 648 x 648.</span><span class="sxs-lookup"><span data-stu-id="d1dac-107">The supported sizes of HD photos in Office 365 are as follows: 48x48, 64x64, 96x96, 120x120, 240x240, 360x360, 432x432, 504x504, and 648x648.</span></span> <span data-ttu-id="d1dac-108">Фотографии могут быть любого размера, если они хранятся в Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="d1dac-108">Photos can be any dimension if they are stored in Azure Active Directory.</span></span>

<span data-ttu-id="d1dac-109">Вы можете получить метаданные самой большой доступной фотографии или указать размер и получить метаданные для этого размера.</span><span class="sxs-lookup"><span data-stu-id="d1dac-109">You can get the metadata of the largest available photo, or specify a size to get the metadata for that photo size.</span></span>
<span data-ttu-id="d1dac-110">Если запрашиваемый размер недоступен, вы можете получить меньший размер, загруженный пользователем.</span><span class="sxs-lookup"><span data-stu-id="d1dac-110">If the size you request is not available, you can still get a smaller size that the user has uploaded and made available.</span></span>
<span data-ttu-id="d1dac-111">Например, если пользователь загрузит фотографию размером 504 x 504 пикселя, для скачивания будут доступны все размеры, кроме 648 x 648.</span><span class="sxs-lookup"><span data-stu-id="d1dac-111">For example, if the user uploads a photo that is 504x504 pixels, all but the 648x648 size of the photo will be available for download.</span></span>
<span data-ttu-id="d1dac-112">Если указанный размер недоступен в почтовом ящике пользователя или Azure Active Directory, возвращается размер 1 x 1 и остальные метаданные.</span><span class="sxs-lookup"><span data-stu-id="d1dac-112">If the specified size is not available in the user's mailbox or in Azure Active Directory, the size 1x1 is returned with the rest of the  metadata.</span></span>

## <a name="permissions"></a><span data-ttu-id="d1dac-113">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d1dac-113">Permissions</span></span>
<span data-ttu-id="d1dac-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d1dac-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

> <span data-ttu-id="d1dac-116">**Примечание.** Метод GET photo в бета-версии поддерживается для рабочих, учебных и личных учетных записей пользователя.</span><span class="sxs-lookup"><span data-stu-id="d1dac-116">**Note:** The GET photo method in beta supports a user's work, school, or personal accounts.</span></span> <span data-ttu-id="d1dac-117">Однако метод GET photo metadata поддерживается только для рабочих или учебных, но не личных учетных записей пользователя.</span><span class="sxs-lookup"><span data-stu-id="d1dac-117">The GET photo metadata method, however, supports only the user's work or school accounts and not personal accounts.</span></span>

|<span data-ttu-id="d1dac-118">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d1dac-118">Permission type</span></span>      | <span data-ttu-id="d1dac-119">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d1dac-119">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d1dac-120">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d1dac-120">Delegated (work or school account)</span></span> | <span data-ttu-id="d1dac-121">Для ресурса **user**:</span><span class="sxs-lookup"><span data-stu-id="d1dac-121">For **user** resource:</span></span><br/><span data-ttu-id="d1dac-122">User.Read, User.ReadBasic.All, User.Read.All, User.ReadWrite, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d1dac-122">User.Read, User.ReadBasic.All, User.Read.All, User.ReadWrite, User.ReadWrite.All</span></span><br /><br /><span data-ttu-id="d1dac-123">Для ресурса **group**:</span><span class="sxs-lookup"><span data-stu-id="d1dac-123">For **group** resource:</span></span><br /><span data-ttu-id="d1dac-124">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d1dac-124">Group.Read.All, Group.ReadWrite.All</span></span><br /><br /><span data-ttu-id="d1dac-125">Для ресурса **contact**:</span><span class="sxs-lookup"><span data-stu-id="d1dac-125">For **contact** resource:</span></span><br /><span data-ttu-id="d1dac-126">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d1dac-126">Contacts.Read, Contacts.ReadWrite</span></span> |
|<span data-ttu-id="d1dac-127">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d1dac-127">Delegated (personal Microsoft account)</span></span>  <br /> <span data-ttu-id="d1dac-128">**Примечание**. Операция получения метаданных не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d1dac-128">**Note**: Metadata operation is not supported.</span></span> | <span data-ttu-id="d1dac-129">Для ресурса **user**:</span><span class="sxs-lookup"><span data-stu-id="d1dac-129">For **user** resource:</span></span><br/><span data-ttu-id="d1dac-130">User.Read, User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d1dac-130">User.Read, User.ReadWrite</span></span><br /><br /><span data-ttu-id="d1dac-131">Для ресурса **contact**:</span><span class="sxs-lookup"><span data-stu-id="d1dac-131">For **contact** resource:</span></span><br /><span data-ttu-id="d1dac-132">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d1dac-132">Contacts.Read, Contacts.ReadWrite</span></span> |
|<span data-ttu-id="d1dac-133">Для приложения</span><span class="sxs-lookup"><span data-stu-id="d1dac-133">Application</span></span>                        | <span data-ttu-id="d1dac-134">Для ресурса **user**:</span><span class="sxs-lookup"><span data-stu-id="d1dac-134">For **user** resource:</span></span><br/><span data-ttu-id="d1dac-135">User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d1dac-135">User.Read.All, User.ReadWrite.All</span></span><br /><br /><span data-ttu-id="d1dac-136">Для ресурса **group**:</span><span class="sxs-lookup"><span data-stu-id="d1dac-136">For **group** resource:</span></span><br /><span data-ttu-id="d1dac-137">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d1dac-137">Group.Read.All, Group.ReadWrite.All</span></span><br /><br /><span data-ttu-id="d1dac-138">Для ресурса **contact**:</span><span class="sxs-lookup"><span data-stu-id="d1dac-138">For **contact** resource:</span></span><br /><span data-ttu-id="d1dac-139">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d1dac-139">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="d1dac-140">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d1dac-140">HTTP request</span></span> 

### <a name="get-the-photo"></a><span data-ttu-id="d1dac-141">Получение фотографии</span><span class="sxs-lookup"><span data-stu-id="d1dac-141">Get the photo</span></span>
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
### <a name="get-the-metadata-of-the-photo"></a><span data-ttu-id="d1dac-142">Получение метаданных фотографии</span><span class="sxs-lookup"><span data-stu-id="d1dac-142">Get the metadata of the photo</span></span>
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

### <a name="get-the-metadata-for-a-specific-photo-size"></a><span data-ttu-id="d1dac-143">Получение метаданных фотографии определенного размера</span><span class="sxs-lookup"><span data-stu-id="d1dac-143">Get the metadata for a specific photo size</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/photos/{size}
GET /users/{id | userPrincipalName}/photos/{size}
GET /groups/{id}/photos/{size}
```

## <a name="path-parameters"></a><span data-ttu-id="d1dac-144">Параметры пути</span><span class="sxs-lookup"><span data-stu-id="d1dac-144">Path parameters</span></span>

|<span data-ttu-id="d1dac-145">**Параметр**</span><span class="sxs-lookup"><span data-stu-id="d1dac-145">**Parameter**</span></span>|<span data-ttu-id="d1dac-146">**Тип**</span><span class="sxs-lookup"><span data-stu-id="d1dac-146">**Type**</span></span>|<span data-ttu-id="d1dac-147">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d1dac-147">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="d1dac-148">size</span><span class="sxs-lookup"><span data-stu-id="d1dac-148">size</span></span>  |<span data-ttu-id="d1dac-149">String</span><span class="sxs-lookup"><span data-stu-id="d1dac-149">String</span></span>  | <span data-ttu-id="d1dac-150">Размер фотографии.</span><span class="sxs-lookup"><span data-stu-id="d1dac-150">A photo size.</span></span> <span data-ttu-id="d1dac-151">Поддерживаемые размеры фотографий в формате HD для Office 365: 48 x 48, 64 x 64, 96 x 96, 120 x 120, 240 x 240, 360 x 360, 432 x 432, 504 x 504 и 648 x 648.</span><span class="sxs-lookup"><span data-stu-id="d1dac-151">The supported sizes of HD photos on Office 365 are as follows: 48x48, 64x64, 96x96, 120x120, 240x240, 360x360, 432x432, 504x504, and 648x648.</span></span> <span data-ttu-id="d1dac-152">Фотографии могут быть любого размера, если они хранятся в Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="d1dac-152">Photos can be any dimension if they are stored in Azure Active Directory.</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="d1dac-153">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="d1dac-153">Optional query parameters</span></span>
<span data-ttu-id="d1dac-154">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="d1dac-154">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d1dac-155">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d1dac-155">Request headers</span></span>
| <span data-ttu-id="d1dac-156">Имя</span><span class="sxs-lookup"><span data-stu-id="d1dac-156">Name</span></span>       | <span data-ttu-id="d1dac-157">Тип</span><span class="sxs-lookup"><span data-stu-id="d1dac-157">Type</span></span> | <span data-ttu-id="d1dac-158">Описание</span><span class="sxs-lookup"><span data-stu-id="d1dac-158">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="d1dac-159">Authorization</span><span class="sxs-lookup"><span data-stu-id="d1dac-159">Authorization</span></span>  | <span data-ttu-id="d1dac-160">string</span><span class="sxs-lookup"><span data-stu-id="d1dac-160">string</span></span>  | <span data-ttu-id="d1dac-p107">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d1dac-p107">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d1dac-163">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d1dac-163">Request body</span></span>
<span data-ttu-id="d1dac-164">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d1dac-164">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d1dac-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="d1dac-165">Response</span></span>
### <a name="response-for-getting-the-photo"></a><span data-ttu-id="d1dac-166">Отклик для запроса на получение фотографии</span><span class="sxs-lookup"><span data-stu-id="d1dac-166">Response for getting the photo</span></span>
<span data-ttu-id="d1dac-p108">При успешном выполнении этот метод возвращает код отклика `200 OK` и двоичные данные запрашиваемой фотографии.  Если фотография не существует, операция возвратит отклик `404 Not Found`.</span><span class="sxs-lookup"><span data-stu-id="d1dac-p108">If successful, this method returns a `200 OK` response code and binary data of the requested photo.  If no photo exists, the operation returns `404 Not Found`.</span></span>
### <a name="response-for-getting-the-metadata-of-the-photo"></a><span data-ttu-id="d1dac-169">Отклик для запроса на получение метаданных фотографии</span><span class="sxs-lookup"><span data-stu-id="d1dac-169">Response for getting the metadata of the photo</span></span>
<span data-ttu-id="d1dac-170">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [profilePhoto](../resources/profilephoto.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d1dac-170">If successful, this method returns a `200 OK` response code and a [profilePhoto](../resources/profilephoto.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d1dac-171">Примеры</span><span class="sxs-lookup"><span data-stu-id="d1dac-171">Examples</span></span>

### <a name="example-1-get-the-photo-of-the-signed-in-user-in-the-largest-available-size"></a><span data-ttu-id="d1dac-172">Пример 1. Получение фотографии пользователя, вошедшего в систему, с максимальным доступным размером</span><span class="sxs-lookup"><span data-stu-id="d1dac-172">Example 1: Get the photo of the signed-in user in the largest available size</span></span>

##### <a name="request"></a><span data-ttu-id="d1dac-173">Запрос</span><span class="sxs-lookup"><span data-stu-id="d1dac-173">Request</span></span>

<!-- {
  "blockType": "ignored"
}-->
```http
GET https://graph.microsoft.com/beta/me/photo/$value
Content-Type: image/jpg
```

##### <a name="response"></a><span data-ttu-id="d1dac-174">Отклик</span><span class="sxs-lookup"><span data-stu-id="d1dac-174">Response</span></span>
<span data-ttu-id="d1dac-175">Содержит двоичные данные запрошенной фотографии.</span><span class="sxs-lookup"><span data-stu-id="d1dac-175">Contains the binary data of the requested photo.</span></span> <span data-ttu-id="d1dac-176">Код HTTP-отклика: 200.</span><span class="sxs-lookup"><span data-stu-id="d1dac-176">The HTTP response code is 200.</span></span>

### <a name="example-2-get-the-48x48-photo-for-the-signed-in-user"></a><span data-ttu-id="d1dac-177">Пример 2. Получение фотографии 48 x 48 для вошедшего пользователя</span><span class="sxs-lookup"><span data-stu-id="d1dac-177">Example 2: Get the 48x48 photo for the signed-in user</span></span>

##### <a name="request"></a><span data-ttu-id="d1dac-178">Запрос</span><span class="sxs-lookup"><span data-stu-id="d1dac-178">Request</span></span>
<!-- {
  "blockType": "ignored"
}-->
```http
GET https://graph.microsoft.com/beta/me/photos/48x48/$value
Content-Type: image/jpg
```

##### <a name="response"></a><span data-ttu-id="d1dac-179">Отклик</span><span class="sxs-lookup"><span data-stu-id="d1dac-179">Response</span></span>
<span data-ttu-id="d1dac-180">Содержит двоичные данные запрошенной фотографии 48 x 48.</span><span class="sxs-lookup"><span data-stu-id="d1dac-180">Contains the binary data of the requested 48x48 photo.</span></span> <span data-ttu-id="d1dac-181">Код HTTP-отклика: 200.</span><span class="sxs-lookup"><span data-stu-id="d1dac-181">The HTTP response code is 200.</span></span>

### <a name="example-3-get-the-metadata-of-the-user-photo-of-the-signed-in-user"></a><span data-ttu-id="d1dac-182">Пример 3. Получение метаданных фотографии вошедшего пользователя</span><span class="sxs-lookup"><span data-stu-id="d1dac-182">Example 3: Get the metadata of the user photo of the signed-in user</span></span>

##### <a name="request"></a><span data-ttu-id="d1dac-183">Запрос</span><span class="sxs-lookup"><span data-stu-id="d1dac-183">Request</span></span>

<!-- {
  "blockType": "ignored"
}-->
```http
GET https://graph.microsoft.com/beta/me/photo
```

##### <a name="response"></a><span data-ttu-id="d1dac-184">Отклик</span><span class="sxs-lookup"><span data-stu-id="d1dac-184">Response</span></span>
<span data-ttu-id="d1dac-185">В данных указанного ниже отклика содержатся метаданные фотографии.</span><span class="sxs-lookup"><span data-stu-id="d1dac-185">The following response data shows the photo metadata.</span></span> 

><span data-ttu-id="d1dac-186">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="d1dac-186">**Note:** The response object shown here might be shortened for readability.</span></span>

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

<span data-ttu-id="d1dac-187">Ниже показаны данные отклика в случае, если фотография пользователя еще не выложена.</span><span class="sxs-lookup"><span data-stu-id="d1dac-187">The following response data shows the contents of a response when a photo hasn't already been uploaded for the user.</span></span> 

><span data-ttu-id="d1dac-188">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="d1dac-188">**Note:** The response object shown here might be shortened for readability.</span></span>

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
## <a name="using-the-binary-data-of-the-requested-photo"></a><span data-ttu-id="d1dac-189">Использование двоичных данных запрошенной фотографии</span><span class="sxs-lookup"><span data-stu-id="d1dac-189">Using the binary data of the requested photo</span></span>

<span data-ttu-id="d1dac-190">Когда вы используете конечную точку `/photo/$value` для получения двоичных данных для фотографии профиля, потребуется преобразовать эти данные в строку Base64, чтобы добавить их как вложение электронной почты.</span><span class="sxs-lookup"><span data-stu-id="d1dac-190">When you use the `/photo/$value` endpoint to get the binary data for a profile photo, you'll need to convert the data into a base-64 string in order to add it as an email attachment.</span></span> <span data-ttu-id="d1dac-191">В следующем примере кода JavaScript показано, как создать массив, который можно передать как значение параметра `Attachments` для [сообщения Outlook](user-post-messages.md).</span><span class="sxs-lookup"><span data-stu-id="d1dac-191">The following JavaScript example shows how to create an array that you can pass as the value of the `Attachments` parameter of an [Outlook message](user-post-messages.md).</span></span>

      const attachments = [{
        '@odata.type': '#microsoft.graph.fileAttachment',
        ContentBytes: file.toString('base64'),
        Name: 'mypic.jpg'
      }];

<span data-ttu-id="d1dac-192">Ознакомиться с реализацией этого примера можно в статье [Пример подключения к Microsoft Graph для Node.js](https://github.com/microsoftgraph/nodejs-connect-rest-sample).</span><span class="sxs-lookup"><span data-stu-id="d1dac-192">See the [Microsoft Graph Connect Sample for Node.js](https://github.com/microsoftgraph/nodejs-connect-rest-sample) for an implementation of this example.</span></span>

<span data-ttu-id="d1dac-193">Если требуется, чтобы изображение отображалось на веб-странице, создайте объект в памяти на его основе и сделайте этот объект источником элемента изображения.</span><span class="sxs-lookup"><span data-stu-id="d1dac-193">If you want to display the image on a web page, create an in-memory object from the image and make that object the source of an image element.</span></span> <span data-ttu-id="d1dac-194">Ниже приведен пример кода JavaScript для этой операции.</span><span class="sxs-lookup"><span data-stu-id="d1dac-194">Here is an example in JavaScript of this operation.</span></span>

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
  "suppressions": []
}
-->

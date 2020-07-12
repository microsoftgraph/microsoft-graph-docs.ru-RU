---
title: Получение фотографии
description: Получение указанного объекта profilePhoto или его метаданных (свойств **profilePhoto**).
localization_priority: Priority
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 77c5485adbbe27e5758d27663ef893e98ca2519e
ms.sourcegitcommit: 41a5bd5868685c10181f6285d5ac91c6dad556e2
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/04/2020
ms.locfileid: "45038674"
---
# <a name="get-photo"></a><span data-ttu-id="cacbf-103">Получение фотографии</span><span class="sxs-lookup"><span data-stu-id="cacbf-103">Get photo</span></span>

<span data-ttu-id="cacbf-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cacbf-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cacbf-105">Получение указанного объекта [profilePhoto](../resources/profilephoto.md) или его метаданных (свойств **profilePhoto**) из Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="cacbf-105">Get the specified [profilePhoto](../resources/profilephoto.md) or its metadata (**profilePhoto** properties) from Microsoft 365.</span></span>

> <span data-ttu-id="cacbf-106">**Примечание**. При попытке ПОЛУЧИТЬ фотографию **пользователя** эта операция сначала делает попытку получить указанную фотографию из Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="cacbf-106">**Note**: When attempting to GET a **user** photo, this operation first attempts to retrieve the specified photo from Microsoft 365.</span></span> <span data-ttu-id="cacbf-107">Если фотография недоступна в Microsoft 365, API пытается получить ее из Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="cacbf-107">If the photo is not available in Microsoft 365, the API attempts to retrieve the photo from Azure Active Directory.</span></span>

<span data-ttu-id="cacbf-108">Поддерживаемые размеры фотографий в формате HD для Microsoft 365: 48 x 48, 64 x 64, 96 x 96, 120 x 120, 240 x 240, 360 x 360, 432 x 432, 504 x 504 и 648 x 648.</span><span class="sxs-lookup"><span data-stu-id="cacbf-108">The supported sizes of HD photos in Microsoft 365 are as follows: 48x48, 64x64, 96x96, 120x120, 240x240, 360x360, 432x432, 504x504, and 648x648.</span></span> <span data-ttu-id="cacbf-109">Фотографии могут быть любого размера, если они хранятся в Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="cacbf-109">Photos can be any dimension if they are stored in Azure Active Directory.</span></span>

<span data-ttu-id="cacbf-110">Вы можете получить метаданные самой большой доступной фотографии или указать размер и получить метаданные для этого размера.</span><span class="sxs-lookup"><span data-stu-id="cacbf-110">You can get the metadata of the largest available photo, or specify a size to get the metadata for that photo size.</span></span>
<span data-ttu-id="cacbf-111">Если запрашиваемый размер недоступен, вы можете получить меньший размер, загруженный пользователем.</span><span class="sxs-lookup"><span data-stu-id="cacbf-111">If the size you request is not available, you can still get a smaller size that the user has uploaded and made available.</span></span>
<span data-ttu-id="cacbf-112">Например, если пользователь загрузит фотографию размером 504 x 504 пикселя, для скачивания будут доступны все размеры, кроме 648 x 648.</span><span class="sxs-lookup"><span data-stu-id="cacbf-112">For example, if the user uploads a photo that is 504x504 pixels, all but the 648x648 size of the photo will be available for download.</span></span>
<span data-ttu-id="cacbf-113">Если указанный размер недоступен в почтовом ящике пользователя или Azure Active Directory, возвращается размер 1 x 1 и остальные метаданные.</span><span class="sxs-lookup"><span data-stu-id="cacbf-113">If the specified size is not available in the user's mailbox or in Azure Active Directory, the size 1x1 is returned with the rest of the  metadata.</span></span>

## <a name="permissions"></a><span data-ttu-id="cacbf-114">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cacbf-114">Permissions</span></span>
<span data-ttu-id="cacbf-115">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="cacbf-115">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="cacbf-116">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cacbf-116">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

> <span data-ttu-id="cacbf-117">**Примечание.** Метод GET photo в бета-версии поддерживается для рабочих, учебных и личных учетных записей пользователя.</span><span class="sxs-lookup"><span data-stu-id="cacbf-117">**Note:** The GET photo method in beta supports a user's work, school, or personal accounts.</span></span> <span data-ttu-id="cacbf-118">Однако метод GET photo metadata поддерживается только для рабочих или учебных, но не личных учетных записей пользователя.</span><span class="sxs-lookup"><span data-stu-id="cacbf-118">The GET photo metadata method, however, supports only the user's work or school accounts and not personal accounts.</span></span>

|<span data-ttu-id="cacbf-119">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cacbf-119">Permission type</span></span>      | <span data-ttu-id="cacbf-120">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cacbf-120">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cacbf-121">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cacbf-121">Delegated (work or school account)</span></span> | <span data-ttu-id="cacbf-122">Для ресурса **user**:</span><span class="sxs-lookup"><span data-stu-id="cacbf-122">For **user** resource:</span></span><br/><span data-ttu-id="cacbf-123">User.Read, User.ReadBasic.All, User.Read.All, User.ReadWrite, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cacbf-123">User.Read, User.ReadBasic.All, User.Read.All, User.ReadWrite, User.ReadWrite.All</span></span><br /><br /><span data-ttu-id="cacbf-124">Для ресурса **group**:</span><span class="sxs-lookup"><span data-stu-id="cacbf-124">For **group** resource:</span></span><br /><span data-ttu-id="cacbf-125">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cacbf-125">Group.Read.All, Group.ReadWrite.All</span></span><br /><br /><span data-ttu-id="cacbf-126">Для ресурса **contact**:</span><span class="sxs-lookup"><span data-stu-id="cacbf-126">For **contact** resource:</span></span><br /><span data-ttu-id="cacbf-127">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cacbf-127">Contacts.Read, Contacts.ReadWrite</span></span> |
|<span data-ttu-id="cacbf-128">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cacbf-128">Delegated (personal Microsoft account)</span></span>  <br /> <span data-ttu-id="cacbf-129">**Примечание**. Операция получения метаданных не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cacbf-129">**Note**: Metadata operation is not supported.</span></span> | <span data-ttu-id="cacbf-130">Для ресурса **user**:</span><span class="sxs-lookup"><span data-stu-id="cacbf-130">For **user** resource:</span></span><br/><span data-ttu-id="cacbf-131">User.Read, User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cacbf-131">User.Read, User.ReadWrite</span></span><br /><br /><span data-ttu-id="cacbf-132">Для ресурса **contact**:</span><span class="sxs-lookup"><span data-stu-id="cacbf-132">For **contact** resource:</span></span><br /><span data-ttu-id="cacbf-133">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cacbf-133">Contacts.Read, Contacts.ReadWrite</span></span> |
|<span data-ttu-id="cacbf-134">Для приложения</span><span class="sxs-lookup"><span data-stu-id="cacbf-134">Application</span></span>                        | <span data-ttu-id="cacbf-135">Для ресурса **user**:</span><span class="sxs-lookup"><span data-stu-id="cacbf-135">For **user** resource:</span></span><br/><span data-ttu-id="cacbf-136">User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cacbf-136">User.Read.All, User.ReadWrite.All</span></span><br /><br /><span data-ttu-id="cacbf-137">Для ресурса **group**:</span><span class="sxs-lookup"><span data-stu-id="cacbf-137">For **group** resource:</span></span><br /><span data-ttu-id="cacbf-138">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cacbf-138">Group.Read.All, Group.ReadWrite.All</span></span><br /><br /><span data-ttu-id="cacbf-139">Для ресурса **contact**:</span><span class="sxs-lookup"><span data-stu-id="cacbf-139">For **contact** resource:</span></span><br /><span data-ttu-id="cacbf-140">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cacbf-140">Contacts.Read, Contacts.ReadWrite</span></span> |

> <span data-ttu-id="cacbf-141">**Примечание.** В настоящее время существует [известная проблема](/graph/known-issues#groups) с доступом к фотографиям группы с помощью разрешений для приложений.</span><span class="sxs-lookup"><span data-stu-id="cacbf-141">**Note:**  There is currently a [known issue](/graph/known-issues#groups) with accessing group photos using application permissions.</span></span>

## <a name="http-request"></a><span data-ttu-id="cacbf-142">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cacbf-142">HTTP request</span></span>

### <a name="get-the-photo"></a><span data-ttu-id="cacbf-143">Получение фотографии</span><span class="sxs-lookup"><span data-stu-id="cacbf-143">Get the photo</span></span>
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
### <a name="get-the-metadata-of-the-photo"></a><span data-ttu-id="cacbf-144">Получение метаданных фотографии</span><span class="sxs-lookup"><span data-stu-id="cacbf-144">Get the metadata of the photo</span></span>
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

### <a name="get-the-metadata-for-a-specific-photo-size"></a><span data-ttu-id="cacbf-145">Получение метаданных фотографии определенного размера</span><span class="sxs-lookup"><span data-stu-id="cacbf-145">Get the metadata for a specific photo size</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/photos/{size}
GET /users/{id | userPrincipalName}/photos/{size}
GET /groups/{id}/photos/{size}
```

## <a name="path-parameters"></a><span data-ttu-id="cacbf-146">Параметры пути</span><span class="sxs-lookup"><span data-stu-id="cacbf-146">Path parameters</span></span>

|<span data-ttu-id="cacbf-147">**Параметр**</span><span class="sxs-lookup"><span data-stu-id="cacbf-147">**Parameter**</span></span>|<span data-ttu-id="cacbf-148">**Тип**</span><span class="sxs-lookup"><span data-stu-id="cacbf-148">**Type**</span></span>|<span data-ttu-id="cacbf-149">**Описание**</span><span class="sxs-lookup"><span data-stu-id="cacbf-149">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="cacbf-150">size</span><span class="sxs-lookup"><span data-stu-id="cacbf-150">size</span></span>  |<span data-ttu-id="cacbf-151">String</span><span class="sxs-lookup"><span data-stu-id="cacbf-151">String</span></span>  | <span data-ttu-id="cacbf-152">Размер фотографии.</span><span class="sxs-lookup"><span data-stu-id="cacbf-152">A photo size.</span></span> <span data-ttu-id="cacbf-153">Поддерживаемые размеры фотографий в формате HD для Microsoft 365: 48 x 48, 64 x 64, 96 x 96, 120 x 120, 240 x 240, 360 x 360, 432 x 432, 504 x 504 и 648 x 648.</span><span class="sxs-lookup"><span data-stu-id="cacbf-153">The supported sizes of HD photos on Microsoft 365 are as follows: 48x48, 64x64, 96x96, 120x120, 240x240, 360x360, 432x432, 504x504, and 648x648.</span></span> <span data-ttu-id="cacbf-154">Фотографии могут быть любого размера, если они хранятся в Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="cacbf-154">Photos can be any dimension if they are stored in Azure Active Directory.</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="cacbf-155">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="cacbf-155">Optional query parameters</span></span>
<span data-ttu-id="cacbf-156">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="cacbf-156">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cacbf-157">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cacbf-157">Request headers</span></span>
| <span data-ttu-id="cacbf-158">Имя</span><span class="sxs-lookup"><span data-stu-id="cacbf-158">Name</span></span>       | <span data-ttu-id="cacbf-159">Тип</span><span class="sxs-lookup"><span data-stu-id="cacbf-159">Type</span></span> | <span data-ttu-id="cacbf-160">Описание</span><span class="sxs-lookup"><span data-stu-id="cacbf-160">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="cacbf-161">Authorization</span><span class="sxs-lookup"><span data-stu-id="cacbf-161">Authorization</span></span>  | <span data-ttu-id="cacbf-162">string</span><span class="sxs-lookup"><span data-stu-id="cacbf-162">string</span></span>  | <span data-ttu-id="cacbf-163">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="cacbf-163">Bearer {token}.</span></span> <span data-ttu-id="cacbf-164">Required.</span><span class="sxs-lookup"><span data-stu-id="cacbf-164">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cacbf-165">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cacbf-165">Request body</span></span>
<span data-ttu-id="cacbf-166">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="cacbf-166">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cacbf-167">Отклик</span><span class="sxs-lookup"><span data-stu-id="cacbf-167">Response</span></span>
### <a name="response-for-getting-the-photo"></a><span data-ttu-id="cacbf-168">Отклик для запроса на получение фотографии</span><span class="sxs-lookup"><span data-stu-id="cacbf-168">Response for getting the photo</span></span>
<span data-ttu-id="cacbf-169">If successful, this method returns a `200 OK` response code and binary data of the requested photo.</span><span class="sxs-lookup"><span data-stu-id="cacbf-169">If successful, this method returns a `200 OK` response code and binary data of the requested photo.</span></span>  <span data-ttu-id="cacbf-170">If no photo exists, the operation returns `404 Not Found`.</span><span class="sxs-lookup"><span data-stu-id="cacbf-170">If no photo exists, the operation returns `404 Not Found`.</span></span>
### <a name="response-for-getting-the-metadata-of-the-photo"></a><span data-ttu-id="cacbf-171">Отклик для запроса на получение метаданных фотографии</span><span class="sxs-lookup"><span data-stu-id="cacbf-171">Response for getting the metadata of the photo</span></span>
<span data-ttu-id="cacbf-172">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [profilePhoto](../resources/profilephoto.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="cacbf-172">If successful, this method returns a `200 OK` response code and a [profilePhoto](../resources/profilephoto.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="cacbf-173">Примеры</span><span class="sxs-lookup"><span data-stu-id="cacbf-173">Examples</span></span>

### <a name="example-1-get-the-photo-of-the-signed-in-user-in-the-largest-available-size"></a><span data-ttu-id="cacbf-174">Пример 1. Получение фотографии пользователя, вошедшего в систему, с максимальным доступным размером</span><span class="sxs-lookup"><span data-stu-id="cacbf-174">Example 1: Get the photo of the signed-in user in the largest available size</span></span>

##### <a name="request"></a><span data-ttu-id="cacbf-175">Запрос</span><span class="sxs-lookup"><span data-stu-id="cacbf-175">Request</span></span>

<!-- {
  "blockType": "ignored"
}-->
```http
GET https://graph.microsoft.com/beta/me/photo/$value
Content-Type: image/jpg
```

##### <a name="response"></a><span data-ttu-id="cacbf-176">Отклик</span><span class="sxs-lookup"><span data-stu-id="cacbf-176">Response</span></span>
<span data-ttu-id="cacbf-177">Содержит двоичные данные запрошенной фотографии.</span><span class="sxs-lookup"><span data-stu-id="cacbf-177">Contains the binary data of the requested photo.</span></span> <span data-ttu-id="cacbf-178">Код HTTP-отклика: 200.</span><span class="sxs-lookup"><span data-stu-id="cacbf-178">The HTTP response code is 200.</span></span>

### <a name="example-2-get-the-48x48-photo-for-the-signed-in-user"></a><span data-ttu-id="cacbf-179">Пример 2. Получение фотографии 48 x 48 для вошедшего пользователя</span><span class="sxs-lookup"><span data-stu-id="cacbf-179">Example 2: Get the 48x48 photo for the signed-in user</span></span>

##### <a name="request"></a><span data-ttu-id="cacbf-180">Запрос</span><span class="sxs-lookup"><span data-stu-id="cacbf-180">Request</span></span>
<!-- {
  "blockType": "ignored"
}-->
```http
GET https://graph.microsoft.com/beta/me/photos/48x48/$value
Content-Type: image/jpg
```

##### <a name="response"></a><span data-ttu-id="cacbf-181">Отклик</span><span class="sxs-lookup"><span data-stu-id="cacbf-181">Response</span></span>
<span data-ttu-id="cacbf-182">Содержит двоичные данные запрошенной фотографии 48 x 48.</span><span class="sxs-lookup"><span data-stu-id="cacbf-182">Contains the binary data of the requested 48x48 photo.</span></span> <span data-ttu-id="cacbf-183">Код HTTP-отклика: 200.</span><span class="sxs-lookup"><span data-stu-id="cacbf-183">The HTTP response code is 200.</span></span>

### <a name="example-3-get-the-metadata-of-the-user-photo-of-the-signed-in-user"></a><span data-ttu-id="cacbf-184">Пример 3. Получение метаданных фотографии вошедшего пользователя</span><span class="sxs-lookup"><span data-stu-id="cacbf-184">Example 3: Get the metadata of the user photo of the signed-in user</span></span>

##### <a name="request"></a><span data-ttu-id="cacbf-185">Запрос</span><span class="sxs-lookup"><span data-stu-id="cacbf-185">Request</span></span>

<!-- {
  "blockType": "ignored"
}-->
```http
GET https://graph.microsoft.com/beta/me/photo
```

##### <a name="response"></a><span data-ttu-id="cacbf-186">Отклик</span><span class="sxs-lookup"><span data-stu-id="cacbf-186">Response</span></span>
<span data-ttu-id="cacbf-187">В данных указанного ниже отклика содержатся метаданные фотографии.</span><span class="sxs-lookup"><span data-stu-id="cacbf-187">The following response data shows the photo metadata.</span></span>

><span data-ttu-id="cacbf-188">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="cacbf-188">**Note:** The response object shown here might be shortened for readability.</span></span>

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

<span data-ttu-id="cacbf-189">Ниже показаны данные отклика в случае, если фотография пользователя еще не выложена.</span><span class="sxs-lookup"><span data-stu-id="cacbf-189">The following response data shows the contents of a response when a photo hasn't already been uploaded for the user.</span></span>

><span data-ttu-id="cacbf-190">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="cacbf-190">**Note:** The response object shown here might be shortened for readability.</span></span>

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
## <a name="using-the-binary-data-of-the-requested-photo"></a><span data-ttu-id="cacbf-191">Использование двоичных данных запрошенной фотографии</span><span class="sxs-lookup"><span data-stu-id="cacbf-191">Using the binary data of the requested photo</span></span>

<span data-ttu-id="cacbf-192">Когда вы используете конечную точку `/photo/$value` для получения двоичных данных для фотографии профиля, потребуется преобразовать эти данные в строку Base64, чтобы добавить их как вложение электронной почты.</span><span class="sxs-lookup"><span data-stu-id="cacbf-192">When you use the `/photo/$value` endpoint to get the binary data for a profile photo, you'll need to convert the data into a base-64 string in order to add it as an email attachment.</span></span> <span data-ttu-id="cacbf-193">В следующем примере кода JavaScript показано, как создать массив, который можно передать как значение параметра `Attachments` для [сообщения Outlook](user-post-messages.md).</span><span class="sxs-lookup"><span data-stu-id="cacbf-193">The following JavaScript example shows how to create an array that you can pass as the value of the `Attachments` parameter of an [Outlook message](user-post-messages.md).</span></span>

      const attachments = [{
        '@odata.type': '#microsoft.graph.fileAttachment',
        ContentBytes: file.toString('base64'),
        Name: 'mypic.jpg'
      }];

<span data-ttu-id="cacbf-194">Ознакомиться с реализацией этого примера можно в статье [Пример подключения к Microsoft Graph для Node.js](https://github.com/microsoftgraph/nodejs-connect-rest-sample).</span><span class="sxs-lookup"><span data-stu-id="cacbf-194">See the [Microsoft Graph Connect Sample for Node.js](https://github.com/microsoftgraph/nodejs-connect-rest-sample) for an implementation of this example.</span></span>

<span data-ttu-id="cacbf-195">Если требуется, чтобы изображение отображалось на веб-странице, создайте объект в памяти на его основе и сделайте этот объект источником элемента изображения.</span><span class="sxs-lookup"><span data-stu-id="cacbf-195">If you want to display the image on a web page, create an in-memory object from the image and make that object the source of an image element.</span></span> <span data-ttu-id="cacbf-196">Ниже приведен пример кода JavaScript для этой операции.</span><span class="sxs-lookup"><span data-stu-id="cacbf-196">Here is an example in JavaScript of this operation.</span></span>

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

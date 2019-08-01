---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Отправка приглашения на доступ к элементу
localization_priority: Normal
ms.prod: sharepoint
description: Отправляет приглашение к совместному использованию ресурса DriveItem.
doc_type: apiPageType
ms.openlocfilehash: 3f245cc3b518502f39a6ca2928ea31719661d27b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36015427"
---
# <a name="send-a-sharing-invitation"></a><span data-ttu-id="6abf3-103">Отправка приглашения к совместному использованию</span><span class="sxs-lookup"><span data-stu-id="6abf3-103">Send a sharing invitation</span></span>

<span data-ttu-id="6abf3-104">Отправляет приглашение к совместному использованию ресурса **DriveItem**.</span><span class="sxs-lookup"><span data-stu-id="6abf3-104">Sends a sharing invitation for a **DriveItem**.</span></span>
<span data-ttu-id="6abf3-105">Приглашение к совместному использованию предоставляет разрешения получателям и при необходимости отправляет им сообщение электронной почты с [ссылкой для совместного доступа][].</span><span class="sxs-lookup"><span data-stu-id="6abf3-105">A sharing invitation provides permissions to the recipients and optionally sends them an email with a [sharing link][].</span></span>

## <a name="permissions"></a><span data-ttu-id="6abf3-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6abf3-106">Permissions</span></span>

<span data-ttu-id="6abf3-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6abf3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6abf3-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6abf3-109">Permission type</span></span>      | <span data-ttu-id="6abf3-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6abf3-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6abf3-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6abf3-111">Delegated (work or school account)</span></span> | <span data-ttu-id="6abf3-112">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6abf3-112">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="6abf3-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6abf3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6abf3-114">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6abf3-114">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="6abf3-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6abf3-115">Application</span></span> | <span data-ttu-id="6abf3-116">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6abf3-116">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6abf3-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6abf3-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{drive-id}/items/{item-id}/invite
POST /groups/{group-id}/drive/items/{item-id}/invite
POST /me/drive/items/{item-id}/invite
POST /sites/{siteId}/drive/items/{itemId}/invite
POST /users/{userId}/drive/items/{itemId}/invite
```

## <a name="request-body"></a><span data-ttu-id="6abf3-118">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="6abf3-118">Request body</span></span>

<span data-ttu-id="6abf3-119">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="6abf3-119">In the request body, provide a JSON object with the following parameters.</span></span>

<!-- { "blockType": "ignored", "scopes": "files.readwrite" } -->

```json
{
  "requireSignIn": false,
  "sendInvitation": false,
  "roles": [ "read | write"],
  "recipients": [
    { "@odata.type": "microsoft.graph.driveRecipient" },
    { "@odata.type": "microsoft.graph.driveRecipient" }
  ],
  "message": "string"
}
```

| <span data-ttu-id="6abf3-120">Параметр</span><span class="sxs-lookup"><span data-stu-id="6abf3-120">Parameter</span></span>        | <span data-ttu-id="6abf3-121">Тип</span><span class="sxs-lookup"><span data-stu-id="6abf3-121">Type</span></span>                           | <span data-ttu-id="6abf3-122">Описание</span><span class="sxs-lookup"><span data-stu-id="6abf3-122">Description</span></span>
|:-----------------|:-------------------------------|:-------------------------
| <span data-ttu-id="6abf3-123">recipients</span><span class="sxs-lookup"><span data-stu-id="6abf3-123">recipients</span></span>       | <span data-ttu-id="6abf3-124">Collection([DriveRecipient][])</span><span class="sxs-lookup"><span data-stu-id="6abf3-124">Collection([DriveRecipient][])</span></span> | <span data-ttu-id="6abf3-125">Коллекция получателей, которые будут получать доступ и приглашение к совместному использованию.</span><span class="sxs-lookup"><span data-stu-id="6abf3-125">A collection of recipients who will receive access and the sharing invitation.</span></span>
| <span data-ttu-id="6abf3-126">message</span><span class="sxs-lookup"><span data-stu-id="6abf3-126">message</span></span>          | <span data-ttu-id="6abf3-127">String</span><span class="sxs-lookup"><span data-stu-id="6abf3-127">String</span></span>                         | <span data-ttu-id="6abf3-p103">Сообщение с обычным форматированным текстом, включенное в приглашение на доступ. Максимальная длина составляет 2000 символов.</span><span class="sxs-lookup"><span data-stu-id="6abf3-p103">A plain text formatted message that is included in the sharing invitation. Maximum length 2000 characters.</span></span>
| <span data-ttu-id="6abf3-130">requireSignIn</span><span class="sxs-lookup"><span data-stu-id="6abf3-130">requireSignIn</span></span>    | <span data-ttu-id="6abf3-131">Boolean</span><span class="sxs-lookup"><span data-stu-id="6abf3-131">Boolean</span></span>                        | <span data-ttu-id="6abf3-132">Указывает, требуется ли получателю приглашения на вход для просмотра общего элемента.</span><span class="sxs-lookup"><span data-stu-id="6abf3-132">Specifies whether the recipient of the invitation is required to sign-in to view the shared item.</span></span>
| <span data-ttu-id="6abf3-133">sendInvitation</span><span class="sxs-lookup"><span data-stu-id="6abf3-133">sendInvitation</span></span>   | <span data-ttu-id="6abf3-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="6abf3-134">Boolean</span></span>                        | <span data-ttu-id="6abf3-135">Если этот параметр имеет значение true, получателю отправляется [ссылка для совместного доступа][] .</span><span class="sxs-lookup"><span data-stu-id="6abf3-135">If true, a [sharing link][] is sent to the recipient.</span></span> <span data-ttu-id="6abf3-136">В противном случае разрешение предоставляется напрямую без отправки уведомления.</span><span class="sxs-lookup"><span data-stu-id="6abf3-136">Otherwise, a permission is granted directly without sending a notification.</span></span>
| <span data-ttu-id="6abf3-137">roles</span><span class="sxs-lookup"><span data-stu-id="6abf3-137">roles</span></span>            | <span data-ttu-id="6abf3-138">Collection(String)</span><span class="sxs-lookup"><span data-stu-id="6abf3-138">Collection(String)</span></span>             | <span data-ttu-id="6abf3-139">Укажите роли, которые должны быть предоставлены получателям приглашения к совместному использованию.</span><span class="sxs-lookup"><span data-stu-id="6abf3-139">Specify the roles that are to be granted to the recipients of the sharing invitation.</span></span>

## <a name="example"></a><span data-ttu-id="6abf3-140">Пример</span><span class="sxs-lookup"><span data-stu-id="6abf3-140">Example</span></span>

<span data-ttu-id="6abf3-141">В этом примере показано, как отправить приглашение к совместному использованию пользователю с адресом электронной почты "ryan@contoso.com" с сообщением о том, что файл работает совместно.</span><span class="sxs-lookup"><span data-stu-id="6abf3-141">This example sends a sharing invitation to a user with email address "ryan@contoso.com" with a message about a file being collaborated on.</span></span>
<span data-ttu-id="6abf3-142">Приглашение предоставляет пользователю Ryan доступ для чтения и записи к файлу.</span><span class="sxs-lookup"><span data-stu-id="6abf3-142">The invitation grants Ryan read-write access to the file.</span></span>

### <a name="http-request"></a><span data-ttu-id="6abf3-143">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6abf3-143">HTTP Request</span></span>

<span data-ttu-id="6abf3-144">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект коллекции [permission](../resources/permission.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="6abf3-144">If successful, this method returns `200 OK` response code and [permission](../resources/permission.md) collection object in the response body.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="6abf3-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="6abf3-145">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "send-sharing-invite", "scopes": "files.readwrite", "target": "action" } -->

```json
POST /me/drive/items/{item-id}/invite
Content-type: application/json

{
  "recipients": [
    {
      "email": "ryan@contoso.com"
    }
  ],
  "message": "Here's the file that we're collaborating on.",
  "requireSignIn": true,
  "sendInvitation": true,
  "roles": [ "write" ]
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="6abf3-146">C#</span><span class="sxs-lookup"><span data-stu-id="6abf3-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/send-sharing-invite-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6abf3-147">Javascript</span><span class="sxs-lookup"><span data-stu-id="6abf3-147">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/send-sharing-invite-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="6abf3-148">Цель — C</span><span class="sxs-lookup"><span data-stu-id="6abf3-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/send-sharing-invite-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="6abf3-149">Java</span><span class="sxs-lookup"><span data-stu-id="6abf3-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/send-sharing-invite-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="6abf3-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="6abf3-150">Response</span></span>

<span data-ttu-id="6abf3-151">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="6abf3-151">Here is an example of the response.</span></span>

<!-- { "blockType": "response", "@odata.type": "Collection(microsoft.graph.permission)", "truncated": true } -->

```json
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "grantedTo": {
        "user": {
          "displayName": "Ryan Gregg",
          "id": "42F177F1-22C0-4BE3-900D-4507125C5C20"
        }
      },
      "id": "CCFC7CA3-7A19-4D57-8CEF-149DB9DDFA62",
      "invitation": {
        "email": "ryan@contoso.com",
        "signInRequired": true
      },
      "roles": [ "write" ]
    }
  ]
}
```

## <a name="remarks"></a><span data-ttu-id="6abf3-152">Примечания</span><span class="sxs-lookup"><span data-stu-id="6abf3-152">Remarks</span></span>

* <span data-ttu-id="6abf3-153">[Дискам](../resources/drive.md), у которых параметр **driveType** имеет значение `personal` (OneDrive персональный), не удастся создать или изменить разрешения в корневой папке ресурса DriveItem.</span><span class="sxs-lookup"><span data-stu-id="6abf3-153">[Drives](../resources/drive.md) with a **driveType** of `personal` (OneDrive personal) cannot create or modify permissions on the root DriveItem.</span></span>
* <span data-ttu-id="6abf3-154">Список доступных ролей см. в разделе [Перечисление ролей](../resources/permission.md#roles-enumeration).</span><span class="sxs-lookup"><span data-stu-id="6abf3-154">For a list of available roles, see [Roles enumeration](../resources/permission.md#roles-enumeration).</span></span>

## <a name="error-responses"></a><span data-ttu-id="6abf3-155">Отклики с ошибками</span><span class="sxs-lookup"><span data-stu-id="6abf3-155">Error Responses</span></span>

<span data-ttu-id="6abf3-156">Дополнительные сведения о том, как возвращаются ошибки, см. в статье [Ошибки][error-response].</span><span class="sxs-lookup"><span data-stu-id="6abf3-156">Read the [Error Responses][error-response] topic for more information about how errors are returned.</span></span>


[driveRecipient]: ../resources/driverecipient.md
[error-response]: /graph/errors
[Ссылка совместного доступа]: ../resources/permission.md#sharing-links
[sharing link]: ../resources/permission.md#sharing-links

<!-- {
  "type": "#page.annotation",
  "description": "Add permissions to an item and optionally send a sharing notification.",
  "keywords": "retrieve,item,metadata",
  "section": "documentation",
  "tocPath": "Sharing/Add permissions",
  "suppressions": [
  ]
} -->

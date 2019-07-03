---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Отправка приглашения на доступ к элементу
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: ab9f23961733a37082f48c111974c2116462aeee
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35445424"
---
# <a name="send-a-sharing-invitation"></a><span data-ttu-id="a1a35-102">Отправка приглашения к совместному использованию</span><span class="sxs-lookup"><span data-stu-id="a1a35-102">Send a sharing invitation</span></span>

<span data-ttu-id="a1a35-103">Отправляет приглашение к совместному использованию ресурса **DriveItem**.</span><span class="sxs-lookup"><span data-stu-id="a1a35-103">Sends a sharing invitation for a **DriveItem**.</span></span>
<span data-ttu-id="a1a35-104">Приглашение к совместному использованию предоставляет разрешения получателям и при необходимости отправляет им сообщение электронной почты с [ссылкой для совместного доступа][].</span><span class="sxs-lookup"><span data-stu-id="a1a35-104">A sharing invitation provides permissions to the recipients and optionally sends them an email with a [sharing link][].</span></span>

## <a name="permissions"></a><span data-ttu-id="a1a35-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a1a35-105">Permissions</span></span>

<span data-ttu-id="a1a35-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a1a35-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a1a35-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a1a35-108">Permission type</span></span>      | <span data-ttu-id="a1a35-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a1a35-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a1a35-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a1a35-110">Delegated (work or school account)</span></span> | <span data-ttu-id="a1a35-111">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a1a35-111">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="a1a35-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a1a35-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a1a35-113">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a1a35-113">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="a1a35-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a1a35-114">Application</span></span> | <span data-ttu-id="a1a35-115">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a1a35-115">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a1a35-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a1a35-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{drive-id}/items/{item-id}/invite
POST /groups/{group-id}/drive/items/{item-id}/invite
POST /me/drive/items/{item-id}/invite
POST /sites/{siteId}/drive/items/{itemId}/invite
POST /users/{userId}/drive/items/{itemId}/invite
```

## <a name="request-body"></a><span data-ttu-id="a1a35-117">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a1a35-117">Request body</span></span>

<span data-ttu-id="a1a35-118">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="a1a35-118">In the request body, provide a JSON object with the following parameters.</span></span>

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

| <span data-ttu-id="a1a35-119">Параметр</span><span class="sxs-lookup"><span data-stu-id="a1a35-119">Parameter</span></span>        | <span data-ttu-id="a1a35-120">Тип</span><span class="sxs-lookup"><span data-stu-id="a1a35-120">Type</span></span>                           | <span data-ttu-id="a1a35-121">Описание</span><span class="sxs-lookup"><span data-stu-id="a1a35-121">Description</span></span>
|:-----------------|:-------------------------------|:-------------------------
| <span data-ttu-id="a1a35-122">recipients</span><span class="sxs-lookup"><span data-stu-id="a1a35-122">recipients</span></span>       | <span data-ttu-id="a1a35-123">Collection([DriveRecipient][])</span><span class="sxs-lookup"><span data-stu-id="a1a35-123">Collection([DriveRecipient][])</span></span> | <span data-ttu-id="a1a35-124">Коллекция получателей, которые будут получать доступ и приглашение к совместному использованию.</span><span class="sxs-lookup"><span data-stu-id="a1a35-124">A collection of recipients who will receive access and the sharing invitation.</span></span>
| <span data-ttu-id="a1a35-125">message</span><span class="sxs-lookup"><span data-stu-id="a1a35-125">message</span></span>          | <span data-ttu-id="a1a35-126">String</span><span class="sxs-lookup"><span data-stu-id="a1a35-126">String</span></span>                         | <span data-ttu-id="a1a35-p103">Сообщение с обычным форматированным текстом, включенное в приглашение на доступ. Максимальная длина составляет 2000 символов.</span><span class="sxs-lookup"><span data-stu-id="a1a35-p103">A plain text formatted message that is included in the sharing invitation. Maximum length 2000 characters.</span></span>
| <span data-ttu-id="a1a35-129">requireSignIn</span><span class="sxs-lookup"><span data-stu-id="a1a35-129">requireSignIn</span></span>    | <span data-ttu-id="a1a35-130">Boolean</span><span class="sxs-lookup"><span data-stu-id="a1a35-130">Boolean</span></span>                        | <span data-ttu-id="a1a35-131">Указывает, требуется ли получателю приглашения на вход для просмотра общего элемента.</span><span class="sxs-lookup"><span data-stu-id="a1a35-131">Specifies whether the recipient of the invitation is required to sign-in to view the shared item.</span></span>
| <span data-ttu-id="a1a35-132">sendInvitation</span><span class="sxs-lookup"><span data-stu-id="a1a35-132">sendInvitation</span></span>   | <span data-ttu-id="a1a35-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="a1a35-133">Boolean</span></span>                        | <span data-ttu-id="a1a35-134">Если этот параметр имеет значение true, получателю отправляется [ссылка для совместного доступа][] .</span><span class="sxs-lookup"><span data-stu-id="a1a35-134">If true, a [sharing link][] is sent to the recipient.</span></span> <span data-ttu-id="a1a35-135">В противном случае разрешение предоставляется напрямую без отправки уведомления.</span><span class="sxs-lookup"><span data-stu-id="a1a35-135">Otherwise, a permission is granted directly without sending a notification.</span></span>
| <span data-ttu-id="a1a35-136">roles</span><span class="sxs-lookup"><span data-stu-id="a1a35-136">roles</span></span>            | <span data-ttu-id="a1a35-137">Collection(String)</span><span class="sxs-lookup"><span data-stu-id="a1a35-137">Collection(String)</span></span>             | <span data-ttu-id="a1a35-138">Укажите роли, которые должны быть предоставлены получателям приглашения к совместному использованию.</span><span class="sxs-lookup"><span data-stu-id="a1a35-138">Specify the roles that are to be granted to the recipients of the sharing invitation.</span></span>

## <a name="example"></a><span data-ttu-id="a1a35-139">Пример</span><span class="sxs-lookup"><span data-stu-id="a1a35-139">Example</span></span>

<span data-ttu-id="a1a35-140">В этом примере показано, как отправить приглашение к совместному использованию пользователю с адресом электронной почты "ryan@contoso.com" с сообщением о том, что файл работает совместно.</span><span class="sxs-lookup"><span data-stu-id="a1a35-140">This example sends a sharing invitation to a user with email address "ryan@contoso.com" with a message about a file being collaborated on.</span></span>
<span data-ttu-id="a1a35-141">Приглашение предоставляет пользователю Ryan доступ для чтения и записи к файлу.</span><span class="sxs-lookup"><span data-stu-id="a1a35-141">The invitation grants Ryan read-write access to the file.</span></span>

### <a name="http-request"></a><span data-ttu-id="a1a35-142">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a1a35-142">HTTP Request</span></span>

<span data-ttu-id="a1a35-143">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект коллекции [permission](../resources/permission.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="a1a35-143">If successful, this method returns `200 OK` response code and [permission](../resources/permission.md) collection object in the response body.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="a1a35-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="a1a35-144">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="a1a35-145">C#</span><span class="sxs-lookup"><span data-stu-id="a1a35-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/send-sharing-invite-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a1a35-146">Javascript</span><span class="sxs-lookup"><span data-stu-id="a1a35-146">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/send-sharing-invite-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a1a35-147">Цель — C</span><span class="sxs-lookup"><span data-stu-id="a1a35-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/send-sharing-invite-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="a1a35-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="a1a35-148">Response</span></span>

<span data-ttu-id="a1a35-149">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="a1a35-149">Here is an example of the response.</span></span>

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

## <a name="remarks"></a><span data-ttu-id="a1a35-150">Примечания</span><span class="sxs-lookup"><span data-stu-id="a1a35-150">Remarks</span></span>

* <span data-ttu-id="a1a35-151">[Дискам](../resources/drive.md), у которых параметр **driveType** имеет значение `personal` (OneDrive персональный), не удастся создать или изменить разрешения в корневой папке ресурса DriveItem.</span><span class="sxs-lookup"><span data-stu-id="a1a35-151">[Drives](../resources/drive.md) with a **driveType** of `personal` (OneDrive personal) cannot create or modify permissions on the root DriveItem.</span></span>
* <span data-ttu-id="a1a35-152">Список доступных ролей см. в разделе [Перечисление ролей](../resources/permission.md#roles-enumeration).</span><span class="sxs-lookup"><span data-stu-id="a1a35-152">For a list of available roles, see [Roles enumeration](../resources/permission.md#roles-enumeration).</span></span>

## <a name="error-responses"></a><span data-ttu-id="a1a35-153">Отклики с ошибками</span><span class="sxs-lookup"><span data-stu-id="a1a35-153">Error Responses</span></span>

<span data-ttu-id="a1a35-154">Дополнительные сведения о том, как возвращаются ошибки, см. в статье [Ошибки][error-response].</span><span class="sxs-lookup"><span data-stu-id="a1a35-154">Read the [Error Responses][error-response] topic for more information about how errors are returned.</span></span>


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

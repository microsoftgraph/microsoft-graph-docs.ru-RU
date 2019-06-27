---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Отправка приглашения на доступ к элементу
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 37e2bc8a383f5078c413ccc37f369442f55b597c
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35272865"
---
# <a name="send-a-sharing-invitation"></a><span data-ttu-id="ef380-102">Отправка приглашения к совместному использованию</span><span class="sxs-lookup"><span data-stu-id="ef380-102">Send a sharing invitation</span></span>

<span data-ttu-id="ef380-103">Отправляет приглашение к совместному использованию ресурса **DriveItem**.</span><span class="sxs-lookup"><span data-stu-id="ef380-103">Sends a sharing invitation for a **DriveItem**.</span></span>
<span data-ttu-id="ef380-104">Приглашение к совместному использованию предоставляет разрешения получателям и при необходимости отправляет им сообщение электронной почты с [ссылкой для совместного доступа][].</span><span class="sxs-lookup"><span data-stu-id="ef380-104">A sharing invitation provides permissions to the recipients and optionally sends them an email with a [sharing link][].</span></span>

## <a name="permissions"></a><span data-ttu-id="ef380-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ef380-105">Permissions</span></span>

<span data-ttu-id="ef380-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ef380-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ef380-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ef380-108">Permission type</span></span>      | <span data-ttu-id="ef380-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ef380-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ef380-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ef380-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ef380-111">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ef380-111">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="ef380-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ef380-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ef380-113">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ef380-113">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="ef380-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ef380-114">Application</span></span> | <span data-ttu-id="ef380-115">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ef380-115">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ef380-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ef380-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{drive-id}/items/{item-id}/invite
POST /groups/{group-id}/drive/items/{item-id}/invite
POST /me/drive/items/{item-id}/invite
POST /sites/{siteId}/drive/items/{itemId}/invite
POST /users/{userId}/drive/items/{itemId}/invite
```

## <a name="request-body"></a><span data-ttu-id="ef380-117">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ef380-117">Request body</span></span>

<span data-ttu-id="ef380-118">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="ef380-118">In the request body, provide a JSON object with the following parameters.</span></span>

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

| <span data-ttu-id="ef380-119">Параметр</span><span class="sxs-lookup"><span data-stu-id="ef380-119">Parameter</span></span>        | <span data-ttu-id="ef380-120">Тип</span><span class="sxs-lookup"><span data-stu-id="ef380-120">Type</span></span>                           | <span data-ttu-id="ef380-121">Описание</span><span class="sxs-lookup"><span data-stu-id="ef380-121">Description</span></span>
|:-----------------|:-------------------------------|:-------------------------
| <span data-ttu-id="ef380-122">recipients</span><span class="sxs-lookup"><span data-stu-id="ef380-122">recipients</span></span>       | <span data-ttu-id="ef380-123">Collection([DriveRecipient][])</span><span class="sxs-lookup"><span data-stu-id="ef380-123">Collection([DriveRecipient][])</span></span> | <span data-ttu-id="ef380-124">Коллекция получателей, которые будут получать доступ и приглашение к совместному использованию.</span><span class="sxs-lookup"><span data-stu-id="ef380-124">A collection of recipients who will receive access and the sharing invitation.</span></span>
| <span data-ttu-id="ef380-125">message</span><span class="sxs-lookup"><span data-stu-id="ef380-125">message</span></span>          | <span data-ttu-id="ef380-126">String</span><span class="sxs-lookup"><span data-stu-id="ef380-126">String</span></span>                         | <span data-ttu-id="ef380-p103">Сообщение с обычным форматированным текстом, включенное в приглашение на доступ. Максимальная длина составляет 2000 символов.</span><span class="sxs-lookup"><span data-stu-id="ef380-p103">A plain text formatted message that is included in the sharing invitation. Maximum length 2000 characters.</span></span>
| <span data-ttu-id="ef380-129">requireSignIn</span><span class="sxs-lookup"><span data-stu-id="ef380-129">requireSignIn</span></span>    | <span data-ttu-id="ef380-130">Boolean</span><span class="sxs-lookup"><span data-stu-id="ef380-130">Boolean</span></span>                        | <span data-ttu-id="ef380-131">Указывает, требуется ли получателю приглашения на вход для просмотра общего элемента.</span><span class="sxs-lookup"><span data-stu-id="ef380-131">Specifies whether the recipient of the invitation is required to sign-in to view the shared item.</span></span>
| <span data-ttu-id="ef380-132">sendInvitation</span><span class="sxs-lookup"><span data-stu-id="ef380-132">sendInvitation</span></span>   | <span data-ttu-id="ef380-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="ef380-133">Boolean</span></span>                        | <span data-ttu-id="ef380-134">Если этот параметр имеет значение true, получателю отправляется [ссылка для совместного доступа][] .</span><span class="sxs-lookup"><span data-stu-id="ef380-134">If true, a [sharing link][] is sent to the recipient.</span></span> <span data-ttu-id="ef380-135">В противном случае разрешение предоставляется напрямую без отправки уведомления.</span><span class="sxs-lookup"><span data-stu-id="ef380-135">Otherwise, a permission is granted directly without sending a notification.</span></span>
| <span data-ttu-id="ef380-136">roles</span><span class="sxs-lookup"><span data-stu-id="ef380-136">roles</span></span>            | <span data-ttu-id="ef380-137">Collection(String)</span><span class="sxs-lookup"><span data-stu-id="ef380-137">Collection(String)</span></span>             | <span data-ttu-id="ef380-138">Укажите роли, которые должны быть предоставлены получателям приглашения к совместному использованию.</span><span class="sxs-lookup"><span data-stu-id="ef380-138">Specify the roles that are to be granted to the recipients of the sharing invitation.</span></span>

## <a name="example"></a><span data-ttu-id="ef380-139">Пример</span><span class="sxs-lookup"><span data-stu-id="ef380-139">Example</span></span>

<span data-ttu-id="ef380-140">В этом примере показано, как отправить приглашение к совместному использованию пользователю с адресом электронной почты "ryan@contoso.com" с сообщением о том, что файл работает совместно.</span><span class="sxs-lookup"><span data-stu-id="ef380-140">This example sends a sharing invitation to a user with email address "ryan@contoso.com" with a message about a file being collaborated on.</span></span>
<span data-ttu-id="ef380-141">Приглашение предоставляет пользователю Ryan доступ для чтения и записи к файлу.</span><span class="sxs-lookup"><span data-stu-id="ef380-141">The invitation grants Ryan read-write access to the file.</span></span>

### <a name="http-request"></a><span data-ttu-id="ef380-142">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ef380-142">HTTP Request</span></span>

<span data-ttu-id="ef380-143">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект коллекции [permission](../resources/permission.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="ef380-143">If successful, this method returns `200 OK` response code and [permission](../resources/permission.md) collection object in the response body.</span></span>

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

### <a name="response"></a><span data-ttu-id="ef380-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="ef380-144">Response</span></span>

<span data-ttu-id="ef380-145">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ef380-145">Here is an example of the response.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="ef380-146">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="ef380-146">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="ef380-147">C#</span><span class="sxs-lookup"><span data-stu-id="ef380-147">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/send-sharing-invite-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ef380-148">Javascript</span><span class="sxs-lookup"><span data-stu-id="ef380-148">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/send-sharing-invite-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="ef380-149">Цель — C</span><span class="sxs-lookup"><span data-stu-id="ef380-149">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/send-sharing-invite-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="remarks"></a><span data-ttu-id="ef380-150">Замечания</span><span class="sxs-lookup"><span data-stu-id="ef380-150">Remarks</span></span>

* <span data-ttu-id="ef380-151">[Дискам](../resources/drive.md), у которых параметр **driveType** имеет значение `personal` (OneDrive персональный), не удастся создать или изменить разрешения в корневой папке ресурса DriveItem.</span><span class="sxs-lookup"><span data-stu-id="ef380-151">[Drives](../resources/drive.md) with a **driveType** of `personal` (OneDrive personal) cannot create or modify permissions on the root DriveItem.</span></span>
* <span data-ttu-id="ef380-152">Список доступных ролей см. в разделе [Перечисление ролей](../resources/permission.md#roles-enumeration).</span><span class="sxs-lookup"><span data-stu-id="ef380-152">For a list of available roles, see [Roles enumeration](../resources/permission.md#roles-enumeration).</span></span>

## <a name="error-responses"></a><span data-ttu-id="ef380-153">Отклики с ошибками</span><span class="sxs-lookup"><span data-stu-id="ef380-153">Error Responses</span></span>

<span data-ttu-id="ef380-154">Дополнительные сведения о том, как возвращаются ошибки, см. в статье [Ошибки][error-response].</span><span class="sxs-lookup"><span data-stu-id="ef380-154">Read the [Error Responses][error-response] topic for more information about how errors are returned.</span></span>


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
    "Error: /api-reference/v1.0/api/driveitem-invite.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/driveitem-invite.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/driveitem-invite.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
} -->

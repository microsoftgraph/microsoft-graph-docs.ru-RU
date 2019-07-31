---
author: kevklam
ms.author: kevinlam
title: Предоставление разрешения
description: Предоставление доступа к списку пользователей для использования указанной ссылки
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: ca427092b169b0a7e9ea13697ee0252c354f3246
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35992453"
---
# <a name="grant-permission"></a><span data-ttu-id="1ddba-103">Предоставление разрешения</span><span class="sxs-lookup"><span data-stu-id="1ddba-103">Grant permission</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1ddba-104">Предоставление пользователям доступа к ссылке, представленной [разрешением][].</span><span class="sxs-lookup"><span data-stu-id="1ddba-104">Grant users access to a link represented by a [permission][].</span></span>

## <a name="permissions"></a><span data-ttu-id="1ddba-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1ddba-105">Permissions</span></span>

<span data-ttu-id="1ddba-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1ddba-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1ddba-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1ddba-108">Permission type</span></span>                   | <span data-ttu-id="1ddba-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1ddba-109">Permissions (from least to most privileged)</span></span>              |
|:----------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="1ddba-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1ddba-110">Delegated (work or school account)</span></span> | <span data-ttu-id="1ddba-111">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1ddba-111">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="1ddba-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1ddba-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1ddba-113">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="1ddba-113">Not supported</span></span>    |
|<span data-ttu-id="1ddba-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1ddba-114">Application</span></span> | <span data-ttu-id="1ddba-115">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1ddba-115">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1ddba-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1ddba-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /shares/{encoded-sharing-url}/permission/grant
```

## <a name="request-headers"></a><span data-ttu-id="1ddba-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1ddba-117">Request headers</span></span>

| <span data-ttu-id="1ddba-118">Имя</span><span class="sxs-lookup"><span data-stu-id="1ddba-118">Name</span></span>          | <span data-ttu-id="1ddba-119">Описание</span><span class="sxs-lookup"><span data-stu-id="1ddba-119">Description</span></span>  |
|:------------- |:------------ |
| <span data-ttu-id="1ddba-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1ddba-120">Authorization</span></span> | <span data-ttu-id="1ddba-121">Носитель \{токен\}.</span><span class="sxs-lookup"><span data-stu-id="1ddba-121">Bearer \{token\}.</span></span> <span data-ttu-id="1ddba-122">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="1ddba-122">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1ddba-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1ddba-123">Request body</span></span>

<span data-ttu-id="1ddba-124">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="1ddba-124">In the request body, provide a JSON object with the following parameters.</span></span>

<!-- { "blockType": "ignored", "scopes": "files.readwrite" } -->

```json
{
  "recipients": [
    { "@odata.type": "microsoft.graph.driveRecipient" }
  ],
  "roles": [ "read | write"]
}
```

| <span data-ttu-id="1ddba-125">Параметр</span><span class="sxs-lookup"><span data-stu-id="1ddba-125">Parameter</span></span>          | <span data-ttu-id="1ddba-126">Тип</span><span class="sxs-lookup"><span data-stu-id="1ddba-126">Type</span></span>                           | <span data-ttu-id="1ddba-127">Описание</span><span class="sxs-lookup"><span data-stu-id="1ddba-127">Description</span></span>
|:-------------------|:-------------------------------|:-------------------------
| <span data-ttu-id="1ddba-128">recipients</span><span class="sxs-lookup"><span data-stu-id="1ddba-128">recipients</span></span>         | <span data-ttu-id="1ddba-129">Коллекция ([driveRecipient][])</span><span class="sxs-lookup"><span data-stu-id="1ddba-129">Collection([driveRecipient][])</span></span> | <span data-ttu-id="1ddba-130">Коллекция получателей, которые будут получать доступ.</span><span class="sxs-lookup"><span data-stu-id="1ddba-130">A collection of recipients who will receive access.</span></span>
| <span data-ttu-id="1ddba-131">roles</span><span class="sxs-lookup"><span data-stu-id="1ddba-131">roles</span></span>              | <span data-ttu-id="1ddba-132">Collection(String)</span><span class="sxs-lookup"><span data-stu-id="1ddba-132">Collection(String)</span></span>             | <span data-ttu-id="1ddba-133">Если ссылка является ссылкой "существующий доступ", указывает роли, которые будут предоставляться пользователям.</span><span class="sxs-lookup"><span data-stu-id="1ddba-133">If the link is an "existing access" link, specifies roles to be granted to the users.</span></span> <span data-ttu-id="1ddba-134">В противном случае он должен быть сопоставлен с ролью ссылки.</span><span class="sxs-lookup"><span data-stu-id="1ddba-134">Otherwise must match the role of the link.</span></span>

<span data-ttu-id="1ddba-135">Список доступных ролей см. в таблице [Перечисление ролей](../resources/permission.md#roles-enumeration-values).</span><span class="sxs-lookup"><span data-stu-id="1ddba-135">For a list of available roles, see [Roles enumeration](../resources/permission.md#roles-enumeration-values).</span></span>

## <a name="response"></a><span data-ttu-id="1ddba-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="1ddba-136">Response</span></span>

<span data-ttu-id="1ddba-137">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию [разрешений][] в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1ddba-137">If successful, this method returns a `200 OK` response code and a [permission][] collection in the response body.</span></span>

<span data-ttu-id="1ddba-138">[Разрешение][] , представляющее обновленную ссылку, всегда будет возвращено в результирующем наборе при успешном выполнении.</span><span class="sxs-lookup"><span data-stu-id="1ddba-138">A [permission][] representing the updated link will always be returned in the result set on success.</span></span> <span data-ttu-id="1ddba-139">Обновленную ссылку можно определить по наличию аспекта Link, содержащего свойство Scope.</span><span class="sxs-lookup"><span data-stu-id="1ddba-139">The updated link can be identified by the presence of a 'link' facet containing the 'scope' property.</span></span> <span data-ttu-id="1ddba-140">В некоторых случаях может быть возможно, что у обновленной ссылки другой URL-адрес, чем у исходной ссылки, в этом случае следует использовать новый URL-адрес.</span><span class="sxs-lookup"><span data-stu-id="1ddba-140">In some cases it may be possible that the updated link has a different URL than the original link, in which case the new URL should be used.</span></span>

<span data-ttu-id="1ddba-141">Ознакомьтесь с разделом [ответы об ошибках][error-response] для получения дополнительных сведений об возвращении ошибок.</span><span class="sxs-lookup"><span data-stu-id="1ddba-141">Read the [Error Responses][error-response] topic for more info about how errors are returned.</span></span>


## <a name="example"></a><span data-ttu-id="1ddba-142">Пример</span><span class="sxs-lookup"><span data-stu-id="1ddba-142">Example</span></span>

<span data-ttu-id="1ddba-143">В этом примере пользователям john@contoso.com и ryan@external.com предоставляется доступ к ссылке для общего доступа, не изменяя другие существующие разрешения на эту ссылку.</span><span class="sxs-lookup"><span data-stu-id="1ddba-143">This example grants the users john@contoso.com and ryan@external.com access to a sharing link without modifying other existing permissions on the link.</span></span>

### <a name="request"></a><span data-ttu-id="1ddba-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="1ddba-144">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="1ddba-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="1ddba-145">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "send-sharing-invite", "scopes": "files.readwrite", "target": "action" } -->

```json
POST https://graph.microsoft.com/beta/shares/{encoded-sharing-url}/permission/grant
Content-type: application/json

{
  "recipients": [
    {
      "email": "john@contoso.com"
    },
    {
      "email": "ryan@external.com"
    }
  ],
  "roles": ["read"]
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="1ddba-146">C#</span><span class="sxs-lookup"><span data-stu-id="1ddba-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/send-sharing-invite-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1ddba-147">Javascript</span><span class="sxs-lookup"><span data-stu-id="1ddba-147">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/send-sharing-invite-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="1ddba-148">Цель — C</span><span class="sxs-lookup"><span data-stu-id="1ddba-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/send-sharing-invite-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="1ddba-149">Java</span><span class="sxs-lookup"><span data-stu-id="1ddba-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/send-sharing-invite-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="1ddba-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="1ddba-150">Response</span></span>

<!-- { "blockType": "response", "@odata.type": "Collection(microsoft.graph.permission)", "truncated": true } -->

```json
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "hasPassword": false,
      "id": "5fab944a-47ec-48d0-a9b5-5178a926d00f",
      "link": {
        "preventsDownload": false,
        "scope": "users",
        "type": "view",
        "webUrl": "https://contoso.sharepoint.com/:t:/g/design/EZexPoDjW4dMtKFUfAl6BK4BvIUuss52hLYzihBfx-PD6Q"
      },
      "roles": [
        "read"
      ]
    }
  ]
}
```

><span data-ttu-id="1ddba-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1ddba-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<span data-ttu-id="1ddba-153">Если ссылка является [существующей](../resources/permission.md#existing-access-link) , будут возвращены дополнительные разрешения, представляющие следующее:</span><span class="sxs-lookup"><span data-stu-id="1ddba-153">If the link is an [existing access](../resources/permission.md#existing-access-link) link, additional permissions will be returned representing the following:</span></span>

- <span data-ttu-id="1ddba-154">Разрешения типа "пользователь", представляющие получателей, которым был успешно предоставлен доступ.</span><span class="sxs-lookup"><span data-stu-id="1ddba-154">User-type permissions representing recipients who were successfully granted access.</span></span> <span data-ttu-id="1ddba-155">Они могут быть идентифицированы по присутствию свойства **грантедто** .</span><span class="sxs-lookup"><span data-stu-id="1ddba-155">These can be identified by presence of the **grantedTo** property.</span></span>
- <span data-ttu-id="1ddba-156">Разрешения типа ссылки, представляющие приглашения, которые необходимо отправить неизвестным внешним пользователям для получения доступа.</span><span class="sxs-lookup"><span data-stu-id="1ddba-156">Link-type permissions representing invitations that need to be sent to unrecognized external users for them to gain access.</span></span> <span data-ttu-id="1ddba-157">Они могут быть идентифицированы по наличию аспекта [приглашения](../resources/sharinginvitation.md) .</span><span class="sxs-lookup"><span data-stu-id="1ddba-157">These can be identified by the presence of an [invitation](../resources/sharinginvitation.md) facet.</span></span> <span data-ttu-id="1ddba-158">Эти записи будут содержать [ссылку][sharing-link] с URL-адресом приглашения, а коллекция грантедтоидентитиес будет указывать пользователей, которым должна быть отправлена ссылка.</span><span class="sxs-lookup"><span data-stu-id="1ddba-158">These entries will contain a [link][sharing-link] with the invitation URL, and the grantedToIdentities collection will indicate the users to whom the link should be sent.</span></span>

<!-- { "blockType": "response", "@odata.type": "Collection(microsoft.graph.permission)", "truncated": true } -->

```json
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "hasPassword": false,
      "id": "00000000-0000-0000-0000-000000000000",
      "link": {
        "preventsDownload": false,
        "scope": "existingAccess",
        "type": "view",
        "webUrl": "https://contoso.sharepoint.com/teams/design/shareddocs/Document.docx"
      },
      "roles": [
        "read"
      ]
    },
    {
      "grantedTo": {
        "user": {
          "displayName": "John Smith",
          "email": "john@contoso.com",
          "id": "47aecee2-d061-4730-8ecb-4c61360441ae"
        }
      },
      "id": "aTowIy5mfG1lbWJlcnNoaXB8bGltaXRlZDJAa2xhbW9kYi5vbm1pY3Jvc29mdC5jb20",
      "roles": [
        "read"
      ]
    },
    {
      "grantedToIdentities": [
        {
          "user": {
            "email": "ryan@external.com"
          }
        }
      ],
      "invitation": {
        "signInRequired": true
      },
      "roles": [
        "read"
      ],
      "link": {
        "type": "view",
        "webUrl": "https://contoso.sharepoint.com/:t:/g/teams/design/EZexPoDjW4dMtKFUfAl6BK4Bw_F7gFH63O310A7lDtK0mQ"
      }
    }
  ]
}

```

><span data-ttu-id="1ddba-159">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="1ddba-159">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="1ddba-160">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1ddba-160">All the properties will be returned from an actual call.</span></span>



[driveRecipient]: ../resources/driverecipient.md
[error-response]: /graph/errors
[permission]: ../resources/permission.md
[sharing-link]: ../resources/sharinglink.md

<!-- {
  "type": "#page.annotation",
  "description": "Add permissions to an item and optionally send a sharing notification.",
  "keywords": "retrieve,item,metadata",
  "section": "documentation",
  "tocPath": "Sharing/Add permissions"
} -->

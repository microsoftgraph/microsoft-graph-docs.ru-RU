---
author: learafa
ms.author: learafa
title: Предоставление разрешения
description: Предоставление доступа к списку пользователей для использования указанной ссылки
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 374a070f0b7de60cd8d66f543d035fd82848056a
ms.sourcegitcommit: 6db0b7a473594653dda332ce7da45ea2ad90772b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/04/2020
ms.locfileid: "43146389"
---
# <a name="permission-grant"></a><span data-ttu-id="a13d4-103">разрешение: Grant</span><span class="sxs-lookup"><span data-stu-id="a13d4-103">permission: grant</span></span>

<span data-ttu-id="a13d4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a13d4-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a13d4-105">Предоставление пользователям доступа к ссылке, представленной [разрешением][].</span><span class="sxs-lookup"><span data-stu-id="a13d4-105">Grant users access to a link represented by a [permission][].</span></span>

## <a name="permissions"></a><span data-ttu-id="a13d4-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a13d4-106">Permissions</span></span>

<span data-ttu-id="a13d4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a13d4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a13d4-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a13d4-109">Permission type</span></span>                   | <span data-ttu-id="a13d4-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a13d4-110">Permissions (from least to most privileged)</span></span>              |
|:----------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="a13d4-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a13d4-111">Delegated (work or school account)</span></span> | <span data-ttu-id="a13d4-112">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a13d4-112">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="a13d4-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a13d4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a13d4-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="a13d4-114">Not supported</span></span>    |
|<span data-ttu-id="a13d4-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a13d4-115">Application</span></span> | <span data-ttu-id="a13d4-116">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a13d4-116">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a13d4-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a13d4-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /shares/{encoded-sharing-url}/permission/grant
```

## <a name="request-headers"></a><span data-ttu-id="a13d4-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a13d4-118">Request headers</span></span>

| <span data-ttu-id="a13d4-119">Имя</span><span class="sxs-lookup"><span data-stu-id="a13d4-119">Name</span></span>          | <span data-ttu-id="a13d4-120">Описание</span><span class="sxs-lookup"><span data-stu-id="a13d4-120">Description</span></span>  |
|:------------- |:------------ |
| <span data-ttu-id="a13d4-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="a13d4-121">Authorization</span></span> | <span data-ttu-id="a13d4-122">Носитель \{токен\}.</span><span class="sxs-lookup"><span data-stu-id="a13d4-122">Bearer \{token\}.</span></span> <span data-ttu-id="a13d4-123">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="a13d4-123">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a13d4-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a13d4-124">Request body</span></span>

<span data-ttu-id="a13d4-125">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="a13d4-125">In the request body, provide a JSON object with the following parameters.</span></span>

<!-- { "blockType": "ignored", "scopes": "files.readwrite" } -->

```json
{
  "recipients": [
    { "@odata.type": "microsoft.graph.driveRecipient" }
  ],
  "roles": [ "read | write"]
}
```

| <span data-ttu-id="a13d4-126">Параметр</span><span class="sxs-lookup"><span data-stu-id="a13d4-126">Parameter</span></span>          | <span data-ttu-id="a13d4-127">Тип</span><span class="sxs-lookup"><span data-stu-id="a13d4-127">Type</span></span>                           | <span data-ttu-id="a13d4-128">Описание</span><span class="sxs-lookup"><span data-stu-id="a13d4-128">Description</span></span>
|:-------------------|:-------------------------------|:-------------------------
| <span data-ttu-id="a13d4-129">recipients</span><span class="sxs-lookup"><span data-stu-id="a13d4-129">recipients</span></span>         | <span data-ttu-id="a13d4-130">Коллекция ([driveRecipient][])</span><span class="sxs-lookup"><span data-stu-id="a13d4-130">Collection([driveRecipient][])</span></span> | <span data-ttu-id="a13d4-131">Коллекция получателей, которые будут получать доступ.</span><span class="sxs-lookup"><span data-stu-id="a13d4-131">A collection of recipients who will receive access.</span></span>
| <span data-ttu-id="a13d4-132">roles</span><span class="sxs-lookup"><span data-stu-id="a13d4-132">roles</span></span>              | <span data-ttu-id="a13d4-133">Collection(String)</span><span class="sxs-lookup"><span data-stu-id="a13d4-133">Collection(String)</span></span>             | <span data-ttu-id="a13d4-134">Если ссылка является ссылкой "существующий доступ", указывает роли, которые будут предоставляться пользователям.</span><span class="sxs-lookup"><span data-stu-id="a13d4-134">If the link is an "existing access" link, specifies roles to be granted to the users.</span></span> <span data-ttu-id="a13d4-135">В противном случае он должен быть сопоставлен с ролью ссылки.</span><span class="sxs-lookup"><span data-stu-id="a13d4-135">Otherwise must match the role of the link.</span></span>

<span data-ttu-id="a13d4-136">Список доступных ролей приведен в разделе [значения свойств Roles](../resources/permission.md#roles-property-values).</span><span class="sxs-lookup"><span data-stu-id="a13d4-136">For a list of available roles, see [roles property values](../resources/permission.md#roles-property-values).</span></span>

## <a name="response"></a><span data-ttu-id="a13d4-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="a13d4-137">Response</span></span>

<span data-ttu-id="a13d4-138">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию [разрешений][] в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a13d4-138">If successful, this method returns a `200 OK` response code and a [permission][] collection in the response body.</span></span>

<span data-ttu-id="a13d4-139">[Разрешение][] , представляющее обновленную ссылку, всегда будет возвращено в результирующем наборе при успешном выполнении.</span><span class="sxs-lookup"><span data-stu-id="a13d4-139">A [permission][] representing the updated link will always be returned in the result set on success.</span></span> <span data-ttu-id="a13d4-140">Обновленную ссылку можно определить по наличию аспекта Link, содержащего свойство Scope.</span><span class="sxs-lookup"><span data-stu-id="a13d4-140">The updated link can be identified by the presence of a 'link' facet containing the 'scope' property.</span></span> <span data-ttu-id="a13d4-141">В некоторых случаях может быть возможно, что у обновленной ссылки другой URL-адрес, чем у исходной ссылки, в этом случае следует использовать новый URL-адрес.</span><span class="sxs-lookup"><span data-stu-id="a13d4-141">In some cases it may be possible that the updated link has a different URL than the original link, in which case the new URL should be used.</span></span>

<span data-ttu-id="a13d4-142">Ознакомьтесь с разделом [ответы об ошибках][error-response] для получения дополнительных сведений об возвращении ошибок.</span><span class="sxs-lookup"><span data-stu-id="a13d4-142">Read the [Error Responses][error-response] topic for more info about how errors are returned.</span></span>


## <a name="example"></a><span data-ttu-id="a13d4-143">Пример</span><span class="sxs-lookup"><span data-stu-id="a13d4-143">Example</span></span>

<span data-ttu-id="a13d4-144">В этом примере пользователям john@contoso.com и ryan@external.com предоставляется доступ к ссылке для общего доступа, не изменяя другие существующие разрешения на эту ссылку.</span><span class="sxs-lookup"><span data-stu-id="a13d4-144">This example grants the users john@contoso.com and ryan@external.com access to a sharing link without modifying other existing permissions on the link.</span></span>

### <a name="request"></a><span data-ttu-id="a13d4-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="a13d4-145">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="a13d4-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="a13d4-146">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "permission-grant", "scopes": "files.readwrite", "target": "action" } -->

```json
POST https://graph.microsoft.com/v1.0/shares/{encoded-sharing-url}/permission/grant
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
# <a name="c"></a>[<span data-ttu-id="a13d4-147">C#</span><span class="sxs-lookup"><span data-stu-id="a13d4-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/permission-grant-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a13d4-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a13d4-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/permission-grant-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a13d4-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a13d4-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/permission-grant-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a13d4-150">Java</span><span class="sxs-lookup"><span data-stu-id="a13d4-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/permission-grant-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="a13d4-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="a13d4-151">Response</span></span>

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

><span data-ttu-id="a13d4-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a13d4-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<span data-ttu-id="a13d4-154">Если ссылка является [существующей](../resources/permission.md) , будут возвращены дополнительные разрешения, представляющие следующее:</span><span class="sxs-lookup"><span data-stu-id="a13d4-154">If the link is an [existing access](../resources/permission.md) link, additional permissions will be returned representing the following:</span></span>

- <span data-ttu-id="a13d4-155">Разрешения типа "пользователь", представляющие получателей, которым был успешно предоставлен доступ.</span><span class="sxs-lookup"><span data-stu-id="a13d4-155">User-type permissions representing recipients who were successfully granted access.</span></span> <span data-ttu-id="a13d4-156">Они могут быть идентифицированы по присутствию свойства **грантедто** .</span><span class="sxs-lookup"><span data-stu-id="a13d4-156">These can be identified by presence of the **grantedTo** property.</span></span>
- <span data-ttu-id="a13d4-157">Разрешения типа ссылки, представляющие приглашения, которые необходимо отправить неизвестным внешним пользователям для получения доступа.</span><span class="sxs-lookup"><span data-stu-id="a13d4-157">Link-type permissions representing invitations that need to be sent to unrecognized external users for them to gain access.</span></span> <span data-ttu-id="a13d4-158">Они могут быть идентифицированы по наличию аспекта [приглашения](../resources/sharinginvitation.md) .</span><span class="sxs-lookup"><span data-stu-id="a13d4-158">These can be identified by the presence of an [invitation](../resources/sharinginvitation.md) facet.</span></span> <span data-ttu-id="a13d4-159">Эти записи будут содержать [ссылку][sharing-link] с URL-адресом приглашения, а коллекция грантедтоидентитиес будет указывать пользователей, которым должна быть отправлена ссылка.</span><span class="sxs-lookup"><span data-stu-id="a13d4-159">These entries will contain a [link][sharing-link] with the invitation URL, and the grantedToIdentities collection will indicate the users to whom the link should be sent.</span></span>

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

><span data-ttu-id="a13d4-160">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="a13d4-160">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="a13d4-161">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a13d4-161">All the properties will be returned from an actual call.</span></span>



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

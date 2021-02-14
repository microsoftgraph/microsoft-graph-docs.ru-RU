---
author: learafa
title: Предоставление разрешения
description: Предоставление списку пользователей доступа для использования указанной ссылки
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 9a2ce74ff01293f6546c34d91a0545e2a228bc96
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/14/2021
ms.locfileid: "50238647"
---
# <a name="permission-grant"></a><span data-ttu-id="213a0-103">permission: grant</span><span class="sxs-lookup"><span data-stu-id="213a0-103">permission: grant</span></span>

<span data-ttu-id="213a0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="213a0-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="213a0-105">Предоставление пользователям доступа к ссылке, представленной [разрешением.][]</span><span class="sxs-lookup"><span data-stu-id="213a0-105">Grant users access to a link represented by a [permission][].</span></span>

## <a name="permissions"></a><span data-ttu-id="213a0-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="213a0-106">Permissions</span></span>

<span data-ttu-id="213a0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="213a0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="213a0-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="213a0-109">Permission type</span></span>                   | <span data-ttu-id="213a0-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="213a0-110">Permissions (from least to most privileged)</span></span>              |
|:----------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="213a0-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="213a0-111">Delegated (work or school account)</span></span> | <span data-ttu-id="213a0-112">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="213a0-112">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="213a0-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="213a0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="213a0-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="213a0-114">Not supported</span></span>    |
|<span data-ttu-id="213a0-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="213a0-115">Application</span></span> | <span data-ttu-id="213a0-116">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="213a0-116">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="213a0-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="213a0-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /shares/{encoded-sharing-url}/permission/grant
```

## <a name="request-headers"></a><span data-ttu-id="213a0-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="213a0-118">Request headers</span></span>

| <span data-ttu-id="213a0-119">Имя</span><span class="sxs-lookup"><span data-stu-id="213a0-119">Name</span></span>          | <span data-ttu-id="213a0-120">Описание</span><span class="sxs-lookup"><span data-stu-id="213a0-120">Description</span></span>  |
|:------------- |:------------ |
| <span data-ttu-id="213a0-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="213a0-121">Authorization</span></span> | <span data-ttu-id="213a0-122">Носитель \{токен\}.</span><span class="sxs-lookup"><span data-stu-id="213a0-122">Bearer \{token\}.</span></span> <span data-ttu-id="213a0-123">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="213a0-123">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="213a0-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="213a0-124">Request body</span></span>

<span data-ttu-id="213a0-125">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="213a0-125">In the request body, provide a JSON object with the following parameters.</span></span>

<!-- { "blockType": "ignored", "scopes": "files.readwrite" } -->

```json
{
  "recipients": [
    { "@odata.type": "microsoft.graph.driveRecipient" }
  ],
  "roles": [ "read | write"]
}
```

| <span data-ttu-id="213a0-126">Параметр</span><span class="sxs-lookup"><span data-stu-id="213a0-126">Parameter</span></span>          | <span data-ttu-id="213a0-127">Тип</span><span class="sxs-lookup"><span data-stu-id="213a0-127">Type</span></span>                           | <span data-ttu-id="213a0-128">Описание</span><span class="sxs-lookup"><span data-stu-id="213a0-128">Description</span></span>
|:-------------------|:-------------------------------|:-------------------------
| <span data-ttu-id="213a0-129">recipients</span><span class="sxs-lookup"><span data-stu-id="213a0-129">recipients</span></span>         | <span data-ttu-id="213a0-130">Collection([driveRecipient][])</span><span class="sxs-lookup"><span data-stu-id="213a0-130">Collection([driveRecipient][])</span></span> | <span data-ttu-id="213a0-131">Коллекция получателей, которые получат доступ.</span><span class="sxs-lookup"><span data-stu-id="213a0-131">A collection of recipients who will receive access.</span></span>
| <span data-ttu-id="213a0-132">roles</span><span class="sxs-lookup"><span data-stu-id="213a0-132">roles</span></span>              | <span data-ttu-id="213a0-133">Collection(String)</span><span class="sxs-lookup"><span data-stu-id="213a0-133">Collection(String)</span></span>             | <span data-ttu-id="213a0-134">Если ссылка является ссылкой "существующий доступ", указывает роли, которые необходимо предоставить пользователям.</span><span class="sxs-lookup"><span data-stu-id="213a0-134">If the link is an "existing access" link, specifies roles to be granted to the users.</span></span> <span data-ttu-id="213a0-135">В противном случае должен соответствовать роли ссылки.</span><span class="sxs-lookup"><span data-stu-id="213a0-135">Otherwise must match the role of the link.</span></span>

<span data-ttu-id="213a0-136">Список доступных ролей см. в [значениях свойств ролей.](../resources/permission.md#roles-property-values)</span><span class="sxs-lookup"><span data-stu-id="213a0-136">For a list of available roles, see [roles property values](../resources/permission.md#roles-property-values).</span></span>

## <a name="response"></a><span data-ttu-id="213a0-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="213a0-137">Response</span></span>

<span data-ttu-id="213a0-138">В случае успеха этот метод возвращает код отклика и коллекцию `200 OK` [разрешений][] в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="213a0-138">If successful, this method returns a `200 OK` response code and a [permission][] collection in the response body.</span></span>

<span data-ttu-id="213a0-139">[Разрешение,][] представляющее обновленную ссылку, всегда возвращается в наборе результатов при успешном обновлении.</span><span class="sxs-lookup"><span data-stu-id="213a0-139">A [permission][] representing the updated link will always be returned in the result set on success.</span></span> <span data-ttu-id="213a0-140">Обновленную ссылку можно определить по наличия аспекту "link", содержащего свойство "scope".</span><span class="sxs-lookup"><span data-stu-id="213a0-140">The updated link can be identified by the presence of a 'link' facet containing the 'scope' property.</span></span> <span data-ttu-id="213a0-141">В некоторых случаях возможно, что обновленный URL-адрес отличается от исходной ссылки. В этом случае следует использовать новый URL-адрес.</span><span class="sxs-lookup"><span data-stu-id="213a0-141">In some cases it may be possible that the updated link has a different URL than the original link, in which case the new URL should be used.</span></span>

<span data-ttu-id="213a0-142">Дополнительные сведения о возвращении ошибок см. в статье [Отклики с ошибками][error-response].</span><span class="sxs-lookup"><span data-stu-id="213a0-142">Read the [Error Responses][error-response] topic for more info about how errors are returned.</span></span>


## <a name="example"></a><span data-ttu-id="213a0-143">Пример</span><span class="sxs-lookup"><span data-stu-id="213a0-143">Example</span></span>

<span data-ttu-id="213a0-144">В этом примере пользователям john@contoso.com и ryan@external.com доступ к ссылке общего доступа без изменения других существующих разрешений на ссылку.</span><span class="sxs-lookup"><span data-stu-id="213a0-144">This example grants the users john@contoso.com and ryan@external.com access to a sharing link without modifying other existing permissions on the link.</span></span>

### <a name="request"></a><span data-ttu-id="213a0-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="213a0-145">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="213a0-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="213a0-146">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="213a0-147">C#</span><span class="sxs-lookup"><span data-stu-id="213a0-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/permission-grant-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="213a0-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="213a0-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/permission-grant-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="213a0-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="213a0-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/permission-grant-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="213a0-150">Java</span><span class="sxs-lookup"><span data-stu-id="213a0-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/permission-grant-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="213a0-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="213a0-151">Response</span></span>

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

><span data-ttu-id="213a0-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="213a0-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<span data-ttu-id="213a0-154">Если ссылка является [существующей ссылкой](../resources/permission.md) доступа, будут возвращены дополнительные разрешения, представляющие следующие:</span><span class="sxs-lookup"><span data-stu-id="213a0-154">If the link is an [existing access](../resources/permission.md) link, additional permissions will be returned representing the following:</span></span>

- <span data-ttu-id="213a0-155">Разрешения типа пользователя, представляющие получателей, которым был успешно предоставлен доступ.</span><span class="sxs-lookup"><span data-stu-id="213a0-155">User-type permissions representing recipients who were successfully granted access.</span></span> <span data-ttu-id="213a0-156">Их можно определить по наличия свойства **grantedTo.**</span><span class="sxs-lookup"><span data-stu-id="213a0-156">These can be identified by presence of the **grantedTo** property.</span></span>
- <span data-ttu-id="213a0-157">Разрешения типа ссылки, представляющие приглашения, которые необходимо отправить неудавающимся внешним пользователям для получения доступа.</span><span class="sxs-lookup"><span data-stu-id="213a0-157">Link-type permissions representing invitations that need to be sent to unrecognized external users for them to gain access.</span></span> <span data-ttu-id="213a0-158">Их можно определить по наличия [аспектов приглашения.](../resources/sharinginvitation.md)</span><span class="sxs-lookup"><span data-stu-id="213a0-158">These can be identified by the presence of an [invitation](../resources/sharinginvitation.md) facet.</span></span> <span data-ttu-id="213a0-159">Эти записи будут [][sharing-link] содержать ссылку с URL-адресом приглашения, а коллекция grantedToIdentities будет указывать пользователей, которым следует отправить ссылку.</span><span class="sxs-lookup"><span data-stu-id="213a0-159">These entries will contain a [link][sharing-link] with the invitation URL, and the grantedToIdentities collection will indicate the users to whom the link should be sent.</span></span>

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

><span data-ttu-id="213a0-160">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="213a0-160">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="213a0-161">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="213a0-161">All the properties will be returned from an actual call.</span></span>



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


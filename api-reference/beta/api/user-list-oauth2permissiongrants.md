---
title: Перечисление oauth2PermissionGrants
description: Получение списка объектов oAuth2PermissionGrant, представляющих делегированные разрешения разрешений.
localization_priority: Priority
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: psignoret
ms.openlocfilehash: 0f115dbff82a706ac9fd99148e5683fc0650c429
ms.sourcegitcommit: 7a6231aeb570ff45d01b3db3df07a411f9f60fd1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/27/2020
ms.locfileid: "44383884"
---
# <a name="list-oauth2permissiongrants"></a><span data-ttu-id="c5c4c-103">Перечисление oauth2PermissionGrants</span><span class="sxs-lookup"><span data-stu-id="c5c4c-103">List oauth2PermissionGrants</span></span>

<span data-ttu-id="c5c4c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c5c4c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c5c4c-105">Получение списка объектов [oAuth2PermissionGrant](../resources/oAuth2PermissionGrant.md) , которые представляют делегированные разрешения, предоставленные для предоставления клиентскому приложению доступа к API от имени пользователя.</span><span class="sxs-lookup"><span data-stu-id="c5c4c-105">Retrieve a list of [oAuth2PermissionGrant](../resources/oAuth2PermissionGrant.md) entities, which represent delegated permissions granted to enable a client application to access an API on behalf of the user.</span></span>

> [!NOTE]
> <span data-ttu-id="c5c4c-106">Запрос делегированных разрешений, предоставленных пользователю, будет возвращать только делегированные разрешения, предоставленные специально для данного пользователя.</span><span class="sxs-lookup"><span data-stu-id="c5c4c-106">Querying the delegated permission grants for a user will only return delegated permissions grants that are specifically for the given user.</span></span> <span data-ttu-id="c5c4c-107">Делегированные разрешения, предоставленные от имени всех пользователей в Организации, _не_ включаются в ответ.</span><span class="sxs-lookup"><span data-stu-id="c5c4c-107">Delegated permissions granted on behalf of all users in the organization are _not_ included in the response.</span></span>

## <a name="permissions"></a><span data-ttu-id="c5c4c-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c5c4c-108">Permissions</span></span>

<span data-ttu-id="c5c4c-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c5c4c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c5c4c-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c5c4c-111">Permission type</span></span>      | <span data-ttu-id="c5c4c-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c5c4c-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c5c4c-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c5c4c-113">Delegated (work or school account)</span></span> | <span data-ttu-id="c5c4c-114">Directory. Read. ALL, Делегатедпермиссионгрант. ReadWrite. ALL, Directory. ReadWrite. ALL, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="c5c4c-114">Directory.Read.All, DelegatedPermissionGrant.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="c5c4c-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c5c4c-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c5c4c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c5c4c-116">Not supported.</span></span>    |
|<span data-ttu-id="c5c4c-117">Сервер приложений</span><span class="sxs-lookup"><span data-stu-id="c5c4c-117">Application</span></span> | <span data-ttu-id="c5c4c-118">Directory. Read. ALL, Делегатедпермиссионгрант. ReadWrite. ALL, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="c5c4c-118">Directory.Read.All, DelegatedPermissionGrant.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c5c4c-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c5c4c-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/oauth2PermissionGrants
GET /users/{id | userPrincipalName}/oauth2PermissionGrants
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c5c4c-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="c5c4c-120">Optional query parameters</span></span>

<span data-ttu-id="c5c4c-121">Этот метод поддерживает [параметры запросов OData](/graph/query_parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="c5c4c-121">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c5c4c-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c5c4c-122">Request headers</span></span>

| <span data-ttu-id="c5c4c-123">Имя</span><span class="sxs-lookup"><span data-stu-id="c5c4c-123">Name</span></span>           | <span data-ttu-id="c5c4c-124">Описание</span><span class="sxs-lookup"><span data-stu-id="c5c4c-124">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="c5c4c-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c5c4c-125">Authorization</span></span>  | <span data-ttu-id="c5c4c-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c5c4c-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c5c4c-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c5c4c-128">Request body</span></span>

<span data-ttu-id="c5c4c-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c5c4c-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c5c4c-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="c5c4c-130">Response</span></span>

<span data-ttu-id="c5c4c-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c5c4c-131">If successful, this method returns a `200 OK` response code and a collection of [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c5c4c-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="c5c4c-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c5c4c-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="c5c4c-133">Request</span></span>

<span data-ttu-id="c5c4c-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c5c4c-134">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="c5c4c-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="c5c4c-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_user_oAuth2PermissionGrants"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/users/{id}/oauth2PermissionGrants
```
# <a name="c"></a>[<span data-ttu-id="c5c4c-136">C#</span><span class="sxs-lookup"><span data-stu-id="c5c4c-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-user-oauth2permissiongrants-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c5c4c-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c5c4c-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-user-oauth2permissiongrants-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c5c4c-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c5c4c-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-user-oauth2permissiongrants-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="c5c4c-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="c5c4c-139">Response</span></span>

<span data-ttu-id="c5c4c-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c5c4c-140">Here is an example of the response.</span></span> 

> <span data-ttu-id="c5c4c-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c5c4c-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.oAuth2PermissionGrant",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 253

{
  "value": [
    {
      "id": "id-value",
      "clientId": "clientId-value",
      "consentType": "consentType-value",
      "principalId": "principalId-value",
      "resourceId": "resourceId-value",
      "scope": "scope-value",
      "startTime": "datetime-value",
      "expiryTime": "datetime-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List oAuth2PermissionGrants",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

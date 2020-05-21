---
title: Перечисление oauth2PermissionGrants
description: Получение списка объектов oAuth2PermissionGrant, представляющих делегированные разрешения разрешений.
localization_priority: Priority
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: a50470caa8a210f01926307d6faa6e7812cdcba5
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/21/2020
ms.locfileid: "44332574"
---
# <a name="list-oauth2permissiongrants"></a><span data-ttu-id="d985f-103">Перечисление oauth2PermissionGrants</span><span class="sxs-lookup"><span data-stu-id="d985f-103">List oauth2PermissionGrants</span></span>

<span data-ttu-id="d985f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d985f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d985f-105">Получение списка объектов [oAuth2PermissionGrant](../resources/oAuth2PermissionGrant.md) , которые представляют делегированные разрешения, предоставленные для предоставления клиентскому приложению доступа к API от имени пользователя.</span><span class="sxs-lookup"><span data-stu-id="d985f-105">Retrieve a list of [oAuth2PermissionGrant](../resources/oAuth2PermissionGrant.md) entities, which represent delegated permissions granted to enable a client application to access an API on behalf of the user.</span></span>

> [!NOTE]
> <span data-ttu-id="d985f-106">Запрос делегированных разрешений, предоставленных пользователю, будет возвращать только делегированные разрешения, предоставленные специально для данного пользователя.</span><span class="sxs-lookup"><span data-stu-id="d985f-106">Querying the delegated permission grants for a user will only return delegated permissions grants that are specifically for the given user.</span></span> <span data-ttu-id="d985f-107">Делегированные разрешения, предоставленные от имени всех пользователей в Организации, _не_ включаются в ответ.</span><span class="sxs-lookup"><span data-stu-id="d985f-107">Delegated permissions granted on behalf of all users in the organization are _not_ included in the response.</span></span>

## <a name="permissions"></a><span data-ttu-id="d985f-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d985f-108">Permissions</span></span>

<span data-ttu-id="d985f-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d985f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d985f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d985f-111">Permission type</span></span>      | <span data-ttu-id="d985f-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d985f-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d985f-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d985f-113">Delegated (work or school account)</span></span> | <span data-ttu-id="d985f-114">Directory. Read. ALL, Делегатедпермиссионгрант. ReadWrite. ALL, Directory. ReadWrite. ALL, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="d985f-114">Directory.Read.All, DelegatedPermissionGrant.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="d985f-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d985f-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d985f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d985f-116">Not supported.</span></span>    |
|<span data-ttu-id="d985f-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d985f-117">Application</span></span> | <span data-ttu-id="d985f-118">Directory. Read. ALL, Делегатедпермиссионгрант. ReadWrite. ALL, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="d985f-118">Directory.Read.All, DelegatedPermissionGrant.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d985f-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d985f-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/oauth2PermissionGrants
GET /users/{id | userPrincipalName}/oauth2PermissionGrants
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d985f-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="d985f-120">Optional query parameters</span></span>

<span data-ttu-id="d985f-121">Этот метод поддерживает [параметры запросов OData](/graph/query_parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="d985f-121">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d985f-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d985f-122">Request headers</span></span>

| <span data-ttu-id="d985f-123">Имя</span><span class="sxs-lookup"><span data-stu-id="d985f-123">Name</span></span>           | <span data-ttu-id="d985f-124">Описание</span><span class="sxs-lookup"><span data-stu-id="d985f-124">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="d985f-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d985f-125">Authorization</span></span>  | <span data-ttu-id="d985f-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d985f-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d985f-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d985f-128">Request body</span></span>

<span data-ttu-id="d985f-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d985f-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d985f-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="d985f-130">Response</span></span>

<span data-ttu-id="d985f-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d985f-131">If successful, this method returns a `200 OK` response code and a collection of [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d985f-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="d985f-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d985f-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="d985f-133">Request</span></span>

<span data-ttu-id="d985f-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d985f-134">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="d985f-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="d985f-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_user_oAuth2PermissionGrants"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/users/{id}/oauth2PermissionGrants
```
# <a name="c"></a>[<span data-ttu-id="d985f-136">C#</span><span class="sxs-lookup"><span data-stu-id="d985f-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-user-oauth2permissiongrants-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d985f-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d985f-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-user-oauth2permissiongrants-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d985f-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d985f-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-user-oauth2permissiongrants-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d985f-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="d985f-139">Response</span></span>

<span data-ttu-id="d985f-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d985f-140">Here is an example of the response.</span></span> 

> <span data-ttu-id="d985f-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d985f-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

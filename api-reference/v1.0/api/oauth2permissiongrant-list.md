---
title: Список oAuth2PermissionGrants
description: Получение списка объектов oauth2PermissionGrant, представляющих делегированную дотации разрешений.
localization_priority: Normal
doc_type: apiPageType
ms.prod: identity-and-sign-in
author: psignoret
ms.openlocfilehash: 11fbc184213f485ae70b19c8997f3eabd3211d7f
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52050432"
---
# <a name="list-oauth2permissiongrants"></a><span data-ttu-id="b2439-103">Перечисление oauth2PermissionGrants</span><span class="sxs-lookup"><span data-stu-id="b2439-103">List oauth2PermissionGrants</span></span>

<span data-ttu-id="b2439-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b2439-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b2439-105">Получение списка [объектов oAuth2PermissionGrant,](../resources/oauth2permissiongrant.md) представляющих делегированную лицензию, выданную для клиентских приложений для доступа к API от имени пользователей, входиющих в нее.</span><span class="sxs-lookup"><span data-stu-id="b2439-105">Retrieve a list of [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) objects, representing delegated permissions which have been granted for client applications to access APIs on behalf of signed-in users.</span></span>

## <a name="permissions"></a><span data-ttu-id="b2439-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b2439-106">Permissions</span></span>

<span data-ttu-id="b2439-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b2439-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b2439-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b2439-109">Permission type</span></span>      | <span data-ttu-id="b2439-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b2439-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b2439-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b2439-111">Delegated (work or school account)</span></span> | <span data-ttu-id="b2439-112">Directory.Read.All, DelegatedPermissionGrant.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b2439-112">Directory.Read.All, DelegatedPermissionGrant.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="b2439-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b2439-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b2439-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b2439-114">Not supported.</span></span>    |
|<span data-ttu-id="b2439-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b2439-115">Application</span></span> | <span data-ttu-id="b2439-116">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b2439-116">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b2439-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b2439-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /oauth2PermissionGrants
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b2439-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="b2439-118">Optional query parameters</span></span>

<span data-ttu-id="b2439-119">Этот метод поддерживает [параметры запросов OData](/graph/query_parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="b2439-119">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b2439-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b2439-120">Request headers</span></span>

| <span data-ttu-id="b2439-121">Имя</span><span class="sxs-lookup"><span data-stu-id="b2439-121">Name</span></span>          | <span data-ttu-id="b2439-122">Описание</span><span class="sxs-lookup"><span data-stu-id="b2439-122">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="b2439-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b2439-123">Authorization</span></span> | <span data-ttu-id="b2439-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b2439-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b2439-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b2439-126">Request body</span></span>

<span data-ttu-id="b2439-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b2439-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b2439-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="b2439-128">Response</span></span>

<span data-ttu-id="b2439-129">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b2439-129">If successful, this method returns a `200 OK` response code and collection of [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b2439-130">Пример</span><span class="sxs-lookup"><span data-stu-id="b2439-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="b2439-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="b2439-131">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="b2439-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="b2439-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_oauth2permissiongrants"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/oauth2PermissionGrants
```
# <a name="c"></a>[<span data-ttu-id="b2439-133">C#</span><span class="sxs-lookup"><span data-stu-id="b2439-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-oauth2permissiongrants-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b2439-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b2439-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-oauth2permissiongrants-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b2439-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b2439-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-oauth2permissiongrants-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b2439-136">Java</span><span class="sxs-lookup"><span data-stu-id="b2439-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-oauth2permissiongrants-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="b2439-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="b2439-137">Response</span></span>

> <span data-ttu-id="b2439-138">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="b2439-138">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.oAuth2PermissionGrant",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 259

{
  "value": [
    {
      "id": "id-value",
      "clientId": "clientId-value",
      "consentType": "consentType-value",
      "principalId": "principalId-value",
      "resourceId": "resourceId-value",
      "scope": "scope-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List oauth2PermissionGrants",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


---
title: Перечисление oauth2PermissionGrants
description: Извлечение списка объектов oAuth2PermissionGrant, представляющих предоставленные делегированные разрешения.
localization_priority: Priority
doc_type: apiPageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: eb2f7cef7db877080360e1798d568f76239ed3ea
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52053470"
---
# <a name="list-oauth2permissiongrants"></a><span data-ttu-id="81fe0-103">Перечисление oauth2PermissionGrants</span><span class="sxs-lookup"><span data-stu-id="81fe0-103">List oauth2PermissionGrants</span></span>

<span data-ttu-id="81fe0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="81fe0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="81fe0-105">Извлечение списка объектов [oAuth2PermissionGrant](../resources/oAuth2PermissionGrant.md), представляющих делегированные разрешения, предоставленные субъекту-службе (представляет клиентское приложение) для доступа к API от имени пользователя.</span><span class="sxs-lookup"><span data-stu-id="81fe0-105">Retrieve a list of [oAuth2PermissionGrant](../resources/oAuth2PermissionGrant.md) entities, representing delegated permissions granted to the service principal (representing the client application) to access an API on behalf of a user.</span></span>

## <a name="permissions"></a><span data-ttu-id="81fe0-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="81fe0-106">Permissions</span></span>

<span data-ttu-id="81fe0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="81fe0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="81fe0-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="81fe0-109">Permission type</span></span>      | <span data-ttu-id="81fe0-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="81fe0-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="81fe0-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="81fe0-111">Delegated (work or school account)</span></span> | <span data-ttu-id="81fe0-112">Directory.Read.All, DelegatedPermissionGrant.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="81fe0-112">Directory.Read.All, DelegatedPermissionGrant.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="81fe0-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="81fe0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="81fe0-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="81fe0-114">Not supported.</span></span>    |
|<span data-ttu-id="81fe0-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="81fe0-115">Application</span></span> | <span data-ttu-id="81fe0-116">Directory.Read.All, DelegatedPermissionGrant.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="81fe0-116">Directory.Read.All, DelegatedPermissionGrant.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="81fe0-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="81fe0-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /servicePrincipals/{id}/oauth2PermissionGrants
```

## <a name="optional-query-parameters"></a><span data-ttu-id="81fe0-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="81fe0-118">Optional query parameters</span></span>

<span data-ttu-id="81fe0-119">Этот метод поддерживает [параметры запросов OData](/graph/query_parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="81fe0-119">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="81fe0-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="81fe0-120">Request headers</span></span>

| <span data-ttu-id="81fe0-121">Имя</span><span class="sxs-lookup"><span data-stu-id="81fe0-121">Name</span></span>           | <span data-ttu-id="81fe0-122">Описание</span><span class="sxs-lookup"><span data-stu-id="81fe0-122">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="81fe0-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="81fe0-123">Authorization</span></span>  | <span data-ttu-id="81fe0-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="81fe0-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="81fe0-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="81fe0-126">Request body</span></span>

<span data-ttu-id="81fe0-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="81fe0-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="81fe0-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="81fe0-128">Response</span></span>

<span data-ttu-id="81fe0-129">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="81fe0-129">If successful, this method returns a `200 OK` response code and collection of [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="81fe0-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="81fe0-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="81fe0-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="81fe0-131">Request</span></span>

<span data-ttu-id="81fe0-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="81fe0-132">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="81fe0-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="81fe0-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_servicePrincipal_oAuth2PermissionGrants"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/oauth2PermissionGrants
```
# <a name="c"></a>[<span data-ttu-id="81fe0-134">C#</span><span class="sxs-lookup"><span data-stu-id="81fe0-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-serviceprincipal-oauth2permissiongrants-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="81fe0-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="81fe0-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-serviceprincipal-oauth2permissiongrants-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="81fe0-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="81fe0-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-serviceprincipal-oauth2permissiongrants-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="81fe0-137">Java</span><span class="sxs-lookup"><span data-stu-id="81fe0-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-serviceprincipal-oauth2permissiongrants-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="81fe0-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="81fe0-138">Response</span></span>

<span data-ttu-id="81fe0-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="81fe0-139">Here is an example of the response.</span></span> 

> <span data-ttu-id="81fe0-140">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="81fe0-140">**Note:** The response object shown here might be shortened for readability.</span></span>

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



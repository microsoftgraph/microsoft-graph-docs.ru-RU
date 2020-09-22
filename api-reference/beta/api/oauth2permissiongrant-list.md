---
title: Список oAuth2PermissionGrants
description: Получение списка объектов oauth2PermissionGrant, представляющих делегированные разрешения разрешений.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: psignoret
ms.openlocfilehash: 9f88803c36f3d2f26694f77dcc2f7fe5a9daefab
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48064740"
---
# <a name="list-oauth2permissiongrants"></a><span data-ttu-id="8fd15-103">Перечисление oauth2PermissionGrants</span><span class="sxs-lookup"><span data-stu-id="8fd15-103">List oauth2PermissionGrants</span></span>

<span data-ttu-id="8fd15-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8fd15-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8fd15-105">Получение списка объектов [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) , представляющих делегированные разрешения, которые были предоставлены клиентским приложениям для доступа к API от имени пользователей, выполнивших вход в систему.</span><span class="sxs-lookup"><span data-stu-id="8fd15-105">Retrieve a list of [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) objects, representing delegated permissions which have been granted for client applications to access APIs on behalf of signed-in users.</span></span>

## <a name="permissions"></a><span data-ttu-id="8fd15-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8fd15-106">Permissions</span></span>

<span data-ttu-id="8fd15-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8fd15-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8fd15-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8fd15-109">Permission type</span></span>      | <span data-ttu-id="8fd15-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8fd15-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8fd15-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8fd15-111">Delegated (work or school account)</span></span> | <span data-ttu-id="8fd15-112">Directory. Read. ALL, Делегатедпермиссионгрант. ReadWrite. ALL, Directory. ReadWrite. ALL, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="8fd15-112">Directory.Read.All, DelegatedPermissionGrant.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="8fd15-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8fd15-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8fd15-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8fd15-114">Not supported.</span></span>    |
|<span data-ttu-id="8fd15-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8fd15-115">Application</span></span> | <span data-ttu-id="8fd15-116">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8fd15-116">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8fd15-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8fd15-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /oauth2PermissionGrants
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8fd15-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="8fd15-118">Optional query parameters</span></span>

<span data-ttu-id="8fd15-119">Этот метод поддерживает [параметры запросов OData](/graph/query_parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="8fd15-119">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8fd15-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8fd15-120">Request headers</span></span>

| <span data-ttu-id="8fd15-121">Имя</span><span class="sxs-lookup"><span data-stu-id="8fd15-121">Name</span></span> | <span data-ttu-id="8fd15-122">Описание</span><span class="sxs-lookup"><span data-stu-id="8fd15-122">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="8fd15-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8fd15-123">Authorization</span></span>  | <span data-ttu-id="8fd15-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8fd15-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8fd15-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8fd15-126">Request body</span></span>

<span data-ttu-id="8fd15-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8fd15-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8fd15-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="8fd15-128">Response</span></span>

<span data-ttu-id="8fd15-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8fd15-129">If successful, this method returns a `200 OK` response code and collection of [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8fd15-130">Пример</span><span class="sxs-lookup"><span data-stu-id="8fd15-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="8fd15-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="8fd15-131">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="8fd15-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="8fd15-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_oauth2permissiongrants"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/oauth2PermissionGrants
```
# <a name="c"></a>[<span data-ttu-id="8fd15-133">C#</span><span class="sxs-lookup"><span data-stu-id="8fd15-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-oauth2permissiongrants-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8fd15-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8fd15-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-oauth2permissiongrants-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8fd15-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8fd15-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-oauth2permissiongrants-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="8fd15-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="8fd15-136">Response</span></span>

> <span data-ttu-id="8fd15-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8fd15-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "description": "List oauth2PermissionGrants",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->



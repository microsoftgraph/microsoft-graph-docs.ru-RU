---
title: Перечисление servicePrincipals
description: Получение списка объектов servicePrincipal.
author: sureshja
localization_priority: Priority
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: db4cb7cb35e29cf73f58a312add83d87d1f13920
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/14/2020
ms.locfileid: "48459111"
---
# <a name="list-serviceprincipals"></a><span data-ttu-id="b4d43-103">Перечисление servicePrincipals</span><span class="sxs-lookup"><span data-stu-id="b4d43-103">List servicePrincipals</span></span>

<span data-ttu-id="b4d43-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b4d43-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b4d43-105">Получение списка объектов [servicePrincipal](../resources/serviceprincipal.md).</span><span class="sxs-lookup"><span data-stu-id="b4d43-105">Retrieve a list of [servicePrincipal](../resources/serviceprincipal.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="b4d43-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b4d43-106">Permissions</span></span>

<span data-ttu-id="b4d43-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b4d43-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b4d43-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b4d43-109">Permission type</span></span>      | <span data-ttu-id="b4d43-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b4d43-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b4d43-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b4d43-111">Delegated (work or school account)</span></span> | <span data-ttu-id="b4d43-112">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b4d43-112">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="b4d43-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b4d43-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b4d43-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b4d43-114">Not supported.</span></span>    |
|<span data-ttu-id="b4d43-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b4d43-115">Application</span></span> | <span data-ttu-id="b4d43-116">Application.Read.All, Application.ReadWrite.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="b4d43-116">Application.Read.All, Application.ReadWrite.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b4d43-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b4d43-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals
```
## <a name="optional-query-parameters"></a><span data-ttu-id="b4d43-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="b4d43-118">Optional query parameters</span></span>

<span data-ttu-id="b4d43-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="b4d43-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b4d43-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b4d43-120">Request headers</span></span>
| <span data-ttu-id="b4d43-121">Имя</span><span class="sxs-lookup"><span data-stu-id="b4d43-121">Name</span></span>           | <span data-ttu-id="b4d43-122">Описание</span><span class="sxs-lookup"><span data-stu-id="b4d43-122">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="b4d43-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b4d43-123">Authorization</span></span>  | <span data-ttu-id="b4d43-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b4d43-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b4d43-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b4d43-126">Request body</span></span>

<span data-ttu-id="b4d43-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b4d43-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b4d43-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="b4d43-128">Response</span></span>

<span data-ttu-id="b4d43-129">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [servicePrincipal](../resources/serviceprincipal.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b4d43-129">If successful, this method returns a `200 OK` response code and collection of [servicePrincipal](../resources/serviceprincipal.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b4d43-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="b4d43-130">Examples</span></span>
### <a name="request"></a><span data-ttu-id="b4d43-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="b4d43-131">Request</span></span>
<span data-ttu-id="b4d43-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b4d43-132">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="b4d43-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="b4d43-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_serviceprincipal"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/serviceprincipals
```
# <a name="c"></a>[<span data-ttu-id="b4d43-134">C#</span><span class="sxs-lookup"><span data-stu-id="b4d43-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-serviceprincipal-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b4d43-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b4d43-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-serviceprincipal-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b4d43-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b4d43-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-serviceprincipal-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b4d43-137">Java</span><span class="sxs-lookup"><span data-stu-id="b4d43-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-serviceprincipal-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="b4d43-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="b4d43-138">Response</span></span>
<span data-ttu-id="b4d43-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b4d43-139">Here is an example of the response.</span></span> 

> <span data-ttu-id="b4d43-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b4d43-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.servicePrincipal",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [{
        "id": "59e617e5-e447-4adc-8b88-00af644d7c92",
        "deletedDateTime": null,
        "accountEnabled": true,
        "appDisplayName": "My App",
        "appId": "65415bb1-9267-4313-bbf5-ae259732ee12",
        "appOwnerOrganizationId": "1bc1c026-2f7b-48a5-98da-afa2fd8bc7bc",
        "appRoleAssignmentRequired": false,
        "displayName": "foo",
        "homepage": null,
        "logoutUrl": null,
        "publisherName": "Contoso",
        "replyUrls": [],
        "servicePrincipalNames": [
        "f1bd758f-4a1a-4b71-aa20-a248a22a8928"
        ],
        "tags": [],
        "addIns": [],
        "appRoles": [],
        "info": {
        "termsOfServiceUrl": null,
        "supportUrl": null,
        "privacyStatementUrl": null,
        "marketingUrl": null,
        "logoUrl": null
        },
        "keyCredentials": [],
        "oauth2PermissionScopes": [],
        "passwordCredentials": []
    }]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List servicePrincipals",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

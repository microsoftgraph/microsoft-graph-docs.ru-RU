---
title: Получение объекта servicePrincipal
description: Получение свойств и связей объекта serviceprincipal.
author: sureshja
localization_priority: Priority
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 54e15ef2fa6ac1888c5c5b9ea519ecbaf961bb74
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/14/2020
ms.locfileid: "48459251"
---
# <a name="get-serviceprincipal"></a><span data-ttu-id="fb955-103">Получение объекта servicePrincipal</span><span class="sxs-lookup"><span data-stu-id="fb955-103">Get servicePrincipal</span></span>

<span data-ttu-id="fb955-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fb955-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="fb955-105">Получение свойств и связей объекта [servicePrincipal](../resources/serviceprincipal.md).</span><span class="sxs-lookup"><span data-stu-id="fb955-105">Retrieve the properties and relationships of a [servicePrincipal](../resources/serviceprincipal.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="fb955-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fb955-106">Permissions</span></span>
<span data-ttu-id="fb955-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fb955-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fb955-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fb955-109">Permission type</span></span>      | <span data-ttu-id="fb955-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fb955-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fb955-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fb955-111">Delegated (work or school account)</span></span> | <span data-ttu-id="fb955-112">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="fb955-112">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="fb955-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fb955-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fb955-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fb955-114">Not supported.</span></span>    |
|<span data-ttu-id="fb955-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fb955-115">Application</span></span> | <span data-ttu-id="fb955-116">Application.Read.All, Application.ReadWrite.All, Application.ReadWrite.OwnedBy, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="fb955-116">Application.Read.All, Application.ReadWrite.All, Application.ReadWrite.OwnedBy, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="fb955-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fb955-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fb955-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="fb955-118">Optional query parameters</span></span>
<span data-ttu-id="fb955-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="fb955-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fb955-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fb955-120">Request headers</span></span>
| <span data-ttu-id="fb955-121">Имя</span><span class="sxs-lookup"><span data-stu-id="fb955-121">Name</span></span>           | <span data-ttu-id="fb955-122">Описание</span><span class="sxs-lookup"><span data-stu-id="fb955-122">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="fb955-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fb955-123">Authorization</span></span>  | <span data-ttu-id="fb955-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fb955-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="fb955-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fb955-126">Request body</span></span>
<span data-ttu-id="fb955-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="fb955-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fb955-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="fb955-128">Response</span></span>
<span data-ttu-id="fb955-129">В случае успеха этот метод возвращает код отклика `200 OK` и объект [servicePrincipal](../resources/serviceprincipal.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="fb955-129">If successful, this method returns a `200 OK` response code and a [servicePrincipal](../resources/serviceprincipal.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="fb955-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="fb955-130">Examples</span></span>
### <a name="request"></a><span data-ttu-id="fb955-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="fb955-131">Request</span></span>
<span data-ttu-id="fb955-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fb955-132">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="fb955-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="fb955-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_serviceprincipal"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/servicePrincipals/{id}
```
# <a name="c"></a>[<span data-ttu-id="fb955-134">C#</span><span class="sxs-lookup"><span data-stu-id="fb955-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-serviceprincipal-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fb955-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fb955-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-serviceprincipal-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fb955-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fb955-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-serviceprincipal-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="fb955-137">Java</span><span class="sxs-lookup"><span data-stu-id="fb955-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-serviceprincipal-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="fb955-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="fb955-138">Response</span></span>
<span data-ttu-id="fb955-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="fb955-139">Here is an example of the response.</span></span> 

><span data-ttu-id="fb955-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fb955-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.servicePrincipal"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "accountEnabled": true,
  "addIns": [],
  "alternativeNames": ["http://contoso/a7770d29-4321-41a6-b863-ca11d6639448"],
  "appDisplayName": "My app",
  "appId": "appId-value",
  "appOwnerOrganizationId": "65415bb1-9267-4313-bbf5-ae259732ee12",
  "appRoleAssignmentRequired":true,
  "appRoles": [],
  "displayName": "My app instance in tenant",
  "endpoints": [],
  "homepage": null,
  "id": "00af5dfb-85da-4b41-a677-0c6b86dd34f8",
  "info": {
    "termsOfServiceUrl": null,
    "supportUrl": null,
    "privacyStatementUrl": null,
    "marketingUrl": null,
    "logoUrl": null
  },
  "keyCredentials": [],
  "logoutUrl": null,
  "oauth2PermissionScopes": [],
  "passwordCredentials": [],
  "publisherName": null,
  "replyUrls": [],
  "servicePrincipalNames": [],
  "servicePrincipalType": null,
  "tags": [],
  "tokenEncryptionKeyId": null
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get servicePrincipal",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

---
title: Список приложений
description: Извлечение списка объектов приложений, связанных с соединитетелемGroup.
localization_priority: Normal
author: japere
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 85b9e7eb24d880ea6fe82a7461bfec20594cee97
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52047177"
---
# <a name="list-applications-assigned-to-a-connectorgroup"></a><span data-ttu-id="0bd88-103">Список приложений, назначенных соединителиГруп</span><span class="sxs-lookup"><span data-stu-id="0bd88-103">List applications assigned to a connectorGroup</span></span>

<span data-ttu-id="0bd88-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0bd88-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0bd88-105">Получение списка объектов [приложений,](../resources/application.md) связанных с [соединителиГруп.](../resources/connectorgroup.md)</span><span class="sxs-lookup"><span data-stu-id="0bd88-105">Retrieve a list of [application](../resources/application.md) objects associated with the [connectorGroup](../resources/connectorgroup.md).</span></span> <span data-ttu-id="0bd88-106">Этот список содержит все приложения, заданной определенной группе соединитений.</span><span class="sxs-lookup"><span data-stu-id="0bd88-106">This list contains all applications assigned to the specific connector group.</span></span>

## <a name="permissions"></a><span data-ttu-id="0bd88-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0bd88-107">Permissions</span></span>
<span data-ttu-id="0bd88-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0bd88-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0bd88-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0bd88-110">Permission type</span></span>      | <span data-ttu-id="0bd88-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0bd88-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0bd88-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0bd88-112">Delegated (work or school account)</span></span> | <span data-ttu-id="0bd88-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="0bd88-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="0bd88-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0bd88-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0bd88-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0bd88-115">Not supported.</span></span>    |
|<span data-ttu-id="0bd88-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0bd88-116">Application</span></span> | <span data-ttu-id="0bd88-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0bd88-117">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="0bd88-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0bd88-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /onPremisesPublishingProfiles/applicationProxy/connectorGroups/{id}/applications
```
## <a name="optional-query-parameters"></a><span data-ttu-id="0bd88-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="0bd88-119">Optional query parameters</span></span>
<span data-ttu-id="0bd88-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="0bd88-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0bd88-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0bd88-121">Request headers</span></span>
| <span data-ttu-id="0bd88-122">Имя</span><span class="sxs-lookup"><span data-stu-id="0bd88-122">Name</span></span>      |<span data-ttu-id="0bd88-123">Описание</span><span class="sxs-lookup"><span data-stu-id="0bd88-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="0bd88-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="0bd88-124">Authorization</span></span>  | <span data-ttu-id="0bd88-125">Носителер.</span><span class="sxs-lookup"><span data-stu-id="0bd88-125">Bearer.</span></span> <span data-ttu-id="0bd88-126">Обязательна</span><span class="sxs-lookup"><span data-stu-id="0bd88-126">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="0bd88-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0bd88-127">Request body</span></span>
<span data-ttu-id="0bd88-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0bd88-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0bd88-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="0bd88-129">Response</span></span>

<span data-ttu-id="0bd88-130">В случае успешного применения этот метод возвращает код отклика и `200 OK` коллекцию объектов приложений в тексте [](../resources/application.md) отклика.</span><span class="sxs-lookup"><span data-stu-id="0bd88-130">If successful, this method returns a `200 OK` response code and collection of [application](../resources/application.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0bd88-131">Пример</span><span class="sxs-lookup"><span data-stu-id="0bd88-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0bd88-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="0bd88-132">Request</span></span>
<span data-ttu-id="0bd88-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0bd88-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="0bd88-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="0bd88-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_applications"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/onPremisesPublishingProfiles/applicationProxy/connectorGroups/{id}/applications
```
# <a name="c"></a>[<span data-ttu-id="0bd88-135">C#</span><span class="sxs-lookup"><span data-stu-id="0bd88-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-applications-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0bd88-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0bd88-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-applications-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0bd88-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0bd88-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-applications-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0bd88-138">Java</span><span class="sxs-lookup"><span data-stu-id="0bd88-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-applications-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="0bd88-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="0bd88-139">Response</span></span>
<span data-ttu-id="0bd88-140">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="0bd88-140">The following is an example of the response.</span></span> <span data-ttu-id="0bd88-141">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="0bd88-141">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.application",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 420

{
  "value": [
    {
      "id": "id-value",
      "onPremisesPublishing": {
        "externalUrl": "externalUrl-value",
        "internalUrl": "internalUrl-value",
        "externalAuthenticationType": "externalAuthenticationType-value",
        "isTranslateHostHeaderEnabled": true,
        "isTranslateLinksInBodyEnabled": true,
        "isOnPremPublishingEnabled": true,
        "applicationServerTimeout": "applicationServerTimeout-value",
        "applicationType": "applicationType-value",
        "verifiedCustomDomainKeyCredential": {
          "customKeyIdentifier": "customKeyIdentifier-value",
          "endDate": "datetime-value",
          "keyId": "keyId-value",
          "startDate": "datetime-value",
          "type": "type-value",
          "usage": "usage-value",
          "value": "value-value"
        },
        "verifiedCustomDomainPasswordCredential": {
          "customKeyIdentifier": "customKeyIdentifier-value",
          "endDate": "datetime-value",
          "keyId": "keyId-value",
          "startDate": "datetime-value",
          "value": "value-value"
        },
        "verifiedCustomDomainCertificatesMetadata": {
          "thumbprint": "thumbprint-value",
          "subjectName": "subjectName-value",
          "issuerName": "issuerName-value",
          "issueDate": "datetime-value",
          "expiryDate": "datetime-value"
        },
        "singleSignOnSettings": {
          "SingleSignOnMode": "SingleSignOnMode-value",
          "KerberosSignOnSettings": {
            "KerberosServicePrincipalName": "KerberosServicePrincipalName-value",
            "KerberosSignOnMappingAttributeType": "KerberosSignOnMappingAttributeType-value"
          }
        },
        "isHttpOnlyCookieEnabled": true,
        "isSecureCookieEnabled": true,
        "isPersistentCookieEnabled": true
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List applications",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


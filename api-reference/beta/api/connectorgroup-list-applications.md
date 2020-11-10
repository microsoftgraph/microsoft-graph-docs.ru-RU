---
title: Список приложений
description: Получение списка объектов приложения, связанных с Коннекторграуп.
localization_priority: Normal
author: japere
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: a4c0dee137cc721cba180784e4f8d36a795a01aa
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48957407"
---
# <a name="list-applications-assigned-to-a-connectorgroup"></a><span data-ttu-id="016be-103">Список приложений, назначенных Коннекторграуп</span><span class="sxs-lookup"><span data-stu-id="016be-103">List applications assigned to a connectorGroup</span></span>

<span data-ttu-id="016be-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="016be-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="016be-105">Получение списка объектов [приложения](../resources/application.md) , связанных с [коннекторграуп](../resources/connectorgroup.md).</span><span class="sxs-lookup"><span data-stu-id="016be-105">Retrieve a list of [application](../resources/application.md) objects associated with the [connectorGroup](../resources/connectorgroup.md).</span></span> <span data-ttu-id="016be-106">Этот список содержит все приложения, назначенные определенной группе соединителей.</span><span class="sxs-lookup"><span data-stu-id="016be-106">This list contains all applications assigned to the specific connector group.</span></span>

## <a name="permissions"></a><span data-ttu-id="016be-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="016be-107">Permissions</span></span>
<span data-ttu-id="016be-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="016be-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="016be-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="016be-110">Permission type</span></span>      | <span data-ttu-id="016be-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="016be-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="016be-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="016be-112">Delegated (work or school account)</span></span> | <span data-ttu-id="016be-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="016be-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="016be-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="016be-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="016be-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="016be-115">Not supported.</span></span>    |
|<span data-ttu-id="016be-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="016be-116">Application</span></span> | <span data-ttu-id="016be-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="016be-117">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="016be-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="016be-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /onPremisesPublishingProfiles/applicationProxy/connectorGroups/{id}/applications
```
## <a name="optional-query-parameters"></a><span data-ttu-id="016be-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="016be-119">Optional query parameters</span></span>
<span data-ttu-id="016be-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="016be-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="016be-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="016be-121">Request headers</span></span>
| <span data-ttu-id="016be-122">Имя</span><span class="sxs-lookup"><span data-stu-id="016be-122">Name</span></span>      |<span data-ttu-id="016be-123">Описание</span><span class="sxs-lookup"><span data-stu-id="016be-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="016be-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="016be-124">Authorization</span></span>  | <span data-ttu-id="016be-125">Носителя.</span><span class="sxs-lookup"><span data-stu-id="016be-125">Bearer.</span></span> <span data-ttu-id="016be-126">Обязательный</span><span class="sxs-lookup"><span data-stu-id="016be-126">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="016be-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="016be-127">Request body</span></span>
<span data-ttu-id="016be-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="016be-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="016be-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="016be-129">Response</span></span>

<span data-ttu-id="016be-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [Application](../resources/application.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="016be-130">If successful, this method returns a `200 OK` response code and collection of [application](../resources/application.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="016be-131">Пример</span><span class="sxs-lookup"><span data-stu-id="016be-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="016be-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="016be-132">Request</span></span>
<span data-ttu-id="016be-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="016be-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="016be-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="016be-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_applications"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/onPremisesPublishingProfiles/applicationProxy/connectorGroups/{id}/applications
```
# <a name="c"></a>[<span data-ttu-id="016be-135">C#</span><span class="sxs-lookup"><span data-stu-id="016be-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-applications-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="016be-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="016be-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-applications-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="016be-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="016be-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-applications-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="016be-138">Java</span><span class="sxs-lookup"><span data-stu-id="016be-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-applications-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="016be-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="016be-139">Response</span></span>
<span data-ttu-id="016be-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="016be-140">The following is an example of the response.</span></span> <span data-ttu-id="016be-141">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="016be-141">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="016be-142">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="016be-142">All of the properties will be returned from an actual call.</span></span>
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

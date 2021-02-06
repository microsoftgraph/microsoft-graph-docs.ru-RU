---
title: Список приложений
description: Получение списка объектов приложений, связанных с соединитетелемGroup.
localization_priority: Normal
author: japere
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 3a25be9468f43e0bcaf911980a4f5e41a1e537f7
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50129977"
---
# <a name="list-applications-assigned-to-a-connectorgroup"></a><span data-ttu-id="3c54b-103">Список приложений, которые назначены соединителиГруппе</span><span class="sxs-lookup"><span data-stu-id="3c54b-103">List applications assigned to a connectorGroup</span></span>

<span data-ttu-id="3c54b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3c54b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3c54b-105">Получение списка объектов [приложений,](../resources/application.md) связанных с [connectorGroup.](../resources/connectorgroup.md)</span><span class="sxs-lookup"><span data-stu-id="3c54b-105">Retrieve a list of [application](../resources/application.md) objects associated with the [connectorGroup](../resources/connectorgroup.md).</span></span> <span data-ttu-id="3c54b-106">Этот список содержит все приложения, которые назначены определенной группе соединитений.</span><span class="sxs-lookup"><span data-stu-id="3c54b-106">This list contains all applications assigned to the specific connector group.</span></span>

## <a name="permissions"></a><span data-ttu-id="3c54b-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3c54b-107">Permissions</span></span>
<span data-ttu-id="3c54b-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3c54b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3c54b-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3c54b-110">Permission type</span></span>      | <span data-ttu-id="3c54b-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3c54b-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3c54b-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3c54b-112">Delegated (work or school account)</span></span> | <span data-ttu-id="3c54b-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="3c54b-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="3c54b-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3c54b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3c54b-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3c54b-115">Not supported.</span></span>    |
|<span data-ttu-id="3c54b-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3c54b-116">Application</span></span> | <span data-ttu-id="3c54b-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3c54b-117">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="3c54b-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3c54b-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /onPremisesPublishingProfiles/applicationProxy/connectorGroups/{id}/applications
```
## <a name="optional-query-parameters"></a><span data-ttu-id="3c54b-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="3c54b-119">Optional query parameters</span></span>
<span data-ttu-id="3c54b-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="3c54b-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3c54b-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3c54b-121">Request headers</span></span>
| <span data-ttu-id="3c54b-122">Имя</span><span class="sxs-lookup"><span data-stu-id="3c54b-122">Name</span></span>      |<span data-ttu-id="3c54b-123">Описание</span><span class="sxs-lookup"><span data-stu-id="3c54b-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="3c54b-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3c54b-124">Authorization</span></span>  | <span data-ttu-id="3c54b-125">Bearer.</span><span class="sxs-lookup"><span data-stu-id="3c54b-125">Bearer.</span></span> <span data-ttu-id="3c54b-126">Обязательна</span><span class="sxs-lookup"><span data-stu-id="3c54b-126">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="3c54b-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3c54b-127">Request body</span></span>
<span data-ttu-id="3c54b-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3c54b-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3c54b-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="3c54b-129">Response</span></span>

<span data-ttu-id="3c54b-130">В случае успеха этот метод возвращает код отклика и коллекцию объектов `200 OK` [приложения](../resources/application.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3c54b-130">If successful, this method returns a `200 OK` response code and collection of [application](../resources/application.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3c54b-131">Пример</span><span class="sxs-lookup"><span data-stu-id="3c54b-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3c54b-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="3c54b-132">Request</span></span>
<span data-ttu-id="3c54b-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3c54b-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="3c54b-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="3c54b-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_applications"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/onPremisesPublishingProfiles/applicationProxy/connectorGroups/{id}/applications
```
# <a name="c"></a>[<span data-ttu-id="3c54b-135">C#</span><span class="sxs-lookup"><span data-stu-id="3c54b-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-applications-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3c54b-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3c54b-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-applications-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3c54b-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3c54b-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-applications-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3c54b-138">Java</span><span class="sxs-lookup"><span data-stu-id="3c54b-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-applications-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="3c54b-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="3c54b-139">Response</span></span>
<span data-ttu-id="3c54b-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="3c54b-140">The following is an example of the response.</span></span> <span data-ttu-id="3c54b-141">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="3c54b-141">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="3c54b-142">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3c54b-142">All of the properties will be returned from an actual call.</span></span>
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


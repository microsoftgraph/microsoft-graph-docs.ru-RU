---
title: Список приложений
description: Получение списка объектов приложения, связанных с Коннекторграуп.
localization_priority: Normal
author: japere
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 546bc83891aa81d5c687906275df5d5a05bdd8bb
ms.sourcegitcommit: b2e216de4a649606c961b3ed2aa3eb8a65f2355c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2020
ms.locfileid: "44555784"
---
# <a name="list-applications-assigned-to-a-connectorgroup"></a><span data-ttu-id="1a8da-103">Список приложений, назначенных Коннекторграуп</span><span class="sxs-lookup"><span data-stu-id="1a8da-103">List applications assigned to a connectorGroup</span></span>

<span data-ttu-id="1a8da-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1a8da-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1a8da-105">Получение списка объектов [приложения](../resources/application.md) , связанных с [коннекторграуп](../resources/connectorgroup.md).</span><span class="sxs-lookup"><span data-stu-id="1a8da-105">Retrieve a list of [application](../resources/application.md) objects associated with the [connectorGroup](../resources/connectorgroup.md).</span></span> <span data-ttu-id="1a8da-106">Этот список содержит все приложения, назначенные определенной группе соединителей.</span><span class="sxs-lookup"><span data-stu-id="1a8da-106">This list contains all applications assigned to the specific connector group.</span></span>

## <a name="permissions"></a><span data-ttu-id="1a8da-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1a8da-107">Permissions</span></span>
<span data-ttu-id="1a8da-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1a8da-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1a8da-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1a8da-110">Permission type</span></span>      | <span data-ttu-id="1a8da-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1a8da-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1a8da-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1a8da-112">Delegated (work or school account)</span></span> | <span data-ttu-id="1a8da-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="1a8da-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="1a8da-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1a8da-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1a8da-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1a8da-115">Not supported.</span></span>    |
|<span data-ttu-id="1a8da-116">Сервер приложений</span><span class="sxs-lookup"><span data-stu-id="1a8da-116">Application</span></span> | <span data-ttu-id="1a8da-117">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1a8da-117">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1a8da-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1a8da-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /onPremisesPublishingProfiles/applicationProxy/connectorGroups/{id}/applications
```
## <a name="optional-query-parameters"></a><span data-ttu-id="1a8da-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="1a8da-119">Optional query parameters</span></span>
<span data-ttu-id="1a8da-120">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="1a8da-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1a8da-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1a8da-121">Request headers</span></span>
| <span data-ttu-id="1a8da-122">Имя</span><span class="sxs-lookup"><span data-stu-id="1a8da-122">Name</span></span>      |<span data-ttu-id="1a8da-123">Описание</span><span class="sxs-lookup"><span data-stu-id="1a8da-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="1a8da-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="1a8da-124">Authorization</span></span>  | <span data-ttu-id="1a8da-125">Носителя.</span><span class="sxs-lookup"><span data-stu-id="1a8da-125">Bearer.</span></span> <span data-ttu-id="1a8da-126">Обязательное</span><span class="sxs-lookup"><span data-stu-id="1a8da-126">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="1a8da-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1a8da-127">Request body</span></span>
<span data-ttu-id="1a8da-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1a8da-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1a8da-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="1a8da-129">Response</span></span>

<span data-ttu-id="1a8da-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [Application](../resources/application.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1a8da-130">If successful, this method returns a `200 OK` response code and collection of [application](../resources/application.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1a8da-131">Пример</span><span class="sxs-lookup"><span data-stu-id="1a8da-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1a8da-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="1a8da-132">Request</span></span>
<span data-ttu-id="1a8da-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1a8da-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_applications"
}-->
```http
GET https://graph.microsoft.com/beta/onPremisesPublishingProfiles/applicationProxy/connectorGroups/{id}/applications
```
##### <a name="response"></a><span data-ttu-id="1a8da-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="1a8da-134">Response</span></span>
<span data-ttu-id="1a8da-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="1a8da-135">The following is an example of the response.</span></span> <span data-ttu-id="1a8da-136">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="1a8da-136">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="1a8da-137">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1a8da-137">All of the properties will be returned from an actual call.</span></span>
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

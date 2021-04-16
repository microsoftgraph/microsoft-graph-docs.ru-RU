---
title: 'applicationTemplate: instantiate'
description: Добавьте экземпляр приложения из галереи приложений Azure AD в каталог.
localization_priority: Normal
author: luleonpla
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 34fe3ae80b34497cfe3313031cd1d3e2f5f7a91c
ms.sourcegitcommit: be09568fa07ab793cd1db500f537ca94ca9e5b4a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51836971"
---
# <a name="applicationtemplate-instantiate"></a><span data-ttu-id="272ab-103">applicationTemplate: instantiate</span><span class="sxs-lookup"><span data-stu-id="272ab-103">applicationTemplate: instantiate</span></span>

<span data-ttu-id="272ab-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="272ab-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="272ab-105">Добавьте экземпляр приложения из галереи приложений Azure AD в каталог.</span><span class="sxs-lookup"><span data-stu-id="272ab-105">Add an instance of an application from the Azure AD application gallery into your directory.</span></span>

## <a name="permissions"></a><span data-ttu-id="272ab-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="272ab-106">Permissions</span></span>

<span data-ttu-id="272ab-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="272ab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="272ab-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="272ab-109">Permission type</span></span>                        | <span data-ttu-id="272ab-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="272ab-110">Permissions (from least to most privileged)</span></span>        |
| :------------------------------------- | :------------------------------------------------- |
| <span data-ttu-id="272ab-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="272ab-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="272ab-112">Application.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="272ab-112">Application.ReadWrite.All, Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="272ab-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="272ab-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="272ab-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="272ab-114">Not supported.</span></span>                                     |
| <span data-ttu-id="272ab-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="272ab-115">Application</span></span>                            | <span data-ttu-id="272ab-116">Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="272ab-116">Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="272ab-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="272ab-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /applicationTemplates/{id}/instantiate
```

## <a name="request-headers"></a><span data-ttu-id="272ab-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="272ab-118">Request headers</span></span>

| <span data-ttu-id="272ab-119">Имя</span><span class="sxs-lookup"><span data-stu-id="272ab-119">Name</span></span>          | <span data-ttu-id="272ab-120">Описание</span><span class="sxs-lookup"><span data-stu-id="272ab-120">Description</span></span>   |
| :------------ | :------------ |
| <span data-ttu-id="272ab-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="272ab-121">Authorization</span></span> | <span data-ttu-id="272ab-122">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="272ab-122">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="272ab-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="272ab-123">Request body</span></span>

<span data-ttu-id="272ab-124">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="272ab-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="272ab-125">Параметр</span><span class="sxs-lookup"><span data-stu-id="272ab-125">Parameter</span></span>   | <span data-ttu-id="272ab-126">Тип</span><span class="sxs-lookup"><span data-stu-id="272ab-126">Type</span></span>   | <span data-ttu-id="272ab-127">Описание</span><span class="sxs-lookup"><span data-stu-id="272ab-127">Description</span></span>                    |
| :---------- | :----- | :----------------------------- |
| <span data-ttu-id="272ab-128">displayName</span><span class="sxs-lookup"><span data-stu-id="272ab-128">displayName</span></span> | <span data-ttu-id="272ab-129">String</span><span class="sxs-lookup"><span data-stu-id="272ab-129">String</span></span> | <span data-ttu-id="272ab-130">Настраиваемая фамилия приложения</span><span class="sxs-lookup"><span data-stu-id="272ab-130">Custom name of the application</span></span> |

## <a name="response"></a><span data-ttu-id="272ab-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="272ab-131">Response</span></span>

<span data-ttu-id="272ab-132">В случае успешного применения этот метод возвращает код отклика и `201 OK` новый [объект applicationServicePrincipal](../resources/applicationserviceprincipal.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="272ab-132">If successful, this method returns a `201 OK` response code and a new [applicationServicePrincipal](../resources/applicationserviceprincipal.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="272ab-133">Примеры</span><span class="sxs-lookup"><span data-stu-id="272ab-133">Examples</span></span>

<span data-ttu-id="272ab-134">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="272ab-134">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="272ab-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="272ab-135">Request</span></span>

<span data-ttu-id="272ab-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="272ab-136">The following is an example of the request.</span></span>

> <span data-ttu-id="272ab-137">Этот API можно использовать для мгновенного обмена приложениями, не в [галерее.](/azure/active-directory/manage-apps/add-non-gallery-app)</span><span class="sxs-lookup"><span data-stu-id="272ab-137">You can use this API to instantiate [non-gallery apps](/azure/active-directory/manage-apps/add-non-gallery-app).</span></span> <span data-ttu-id="272ab-138">Используйте следующий ID для **applicationTemplate:** `8adf8e6e-67b2-4cf2-a259-e3dc5476c621` .</span><span class="sxs-lookup"><span data-stu-id="272ab-138">Use the following ID for **applicationTemplate**: `8adf8e6e-67b2-4cf2-a259-e3dc5476c621`.</span></span>


# <a name="http"></a>[<span data-ttu-id="272ab-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="272ab-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "applicationtemplate_instantiate"
}-->

```http
POST https://graph.microsoft.com/v1.0/applicationTemplates/{id}/instantiate
Content-type: application/json

{
  "displayName": "My custom name"
}
```
# <a name="c"></a>[<span data-ttu-id="272ab-140">C#</span><span class="sxs-lookup"><span data-stu-id="272ab-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/applicationtemplate-instantiate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="272ab-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="272ab-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/applicationtemplate-instantiate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="272ab-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="272ab-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/applicationtemplate-instantiate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="272ab-143">Java</span><span class="sxs-lookup"><span data-stu-id="272ab-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/applicationtemplate-instantiate-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="272ab-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="272ab-144">Response</span></span>

<span data-ttu-id="272ab-145">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="272ab-145">The following is an example of the response.</span></span>

> <span data-ttu-id="272ab-146">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="272ab-146">**Note:** The response object shown here might be shortened for readability.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.applicationServicePrincipal"
} -->

```http
HTTP/1.1 201 OK
Content-type: application/json

{
   "servicePrincipal":{
      "accountEnabled":true,
      "addIns":[],
      "alternativeNames":[
         "http://contoso/a7770d29-4321-41a6-b863-ca11d6639448"
      ],
      "appDisplayName":"appDisplayName-value",
      "appId":"appId-value",
      "appOwnerOrganizationId":"appOwnerOrganizationId-value",
      "appRoleAssignmentRequired":true,
      "appRoles":[],
      "displayName":"Display name",
      "endpoints":[],
      "homepage":null,
      "id":"id-value",
      "info":{
         "termsOfServiceUrl":null,
         "supportUrl":null,
         "privacyStatementUrl":null,
         "marketingUrl":null,
         "logoUrl":null
      },
      "keyCredentials":[],
      "logoutUrl":null,
      "oauth2PermissionScopes":[],
      "passwordCredentials":[],
      "publisherName":null,
      "replyUrls":[],
      "servicePrincipalNames":[],
      "servicePrincipalType":null,
      "tags":[],
      "tokenEncryptionKeyId":null
   },
   "application":{
      "id":"id-value",
      "isFallbackPublicClient":null,
      "appId":"appId-value",
      "applicationTemplateId":null,
      "identifierUris":[],
      "createdDateTime":"2019-09-17T19:10:35.2742618Z",
      "displayName":"Display name",
      "isDeviceOnlyAuthSupported":null,
      "groupMembershipClaims":null,
      "optionalClaims":null,
      "addIns":[],
      "publisherDomain":"contoso.onmicrosoft.com",
      "signInAudience":"AzureADMyOrg",
      "tags":[],
      "tokenEncryptionKeyId":null,
      "api":{
         "requestedAccessTokenVersion":2,
         "acceptMappedClaims":null,
         "knownClientApplications":[],
         "oauth2PermissionScopes":[],
         "preAuthorizedApplications":[]
      },
      "appRoles":[],
      "publicClient":{
         "redirectUris":[]
      },
      "info":{
         "termsOfServiceUrl":null,
         "supportUrl":null,
         "privacyStatementUrl":null,
         "marketingUrl":null,
         "logoUrl":null
      },
      "keyCredentials":[],
      "parentalControlSettings":{
         "countriesBlockedForMinors":[],
         "legalAgeGroupRule":"Allow"
      },
      "passwordCredentials":[],
      "requiredResourceAccess":[ ],
      "web":{
         "redirectUris":[],
         "homePageUrl":null,
         "logoutUrl":null,
         "implicitGrantSettings":{
            "enableIdTokenIssuance":false,
            "enableAccessTokenIssuance":false
         }
      }
   }
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "applicationTemplate: instantiate",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

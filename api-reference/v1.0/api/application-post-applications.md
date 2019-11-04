---
title: Создание приложения
description: Создайте новое приложение.
author: davidmu1
localization_priority: Priority
doc_type: apiPageType
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 3b4c0401342c3bf40cd7018542ece48c9c91a64f
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939700"
---
# <a name="create-application"></a><span data-ttu-id="403b4-103">Создание приложения</span><span class="sxs-lookup"><span data-stu-id="403b4-103">Create application</span></span>

<span data-ttu-id="403b4-104">Создайте новый объект [application](../resources/application.md).</span><span class="sxs-lookup"><span data-stu-id="403b4-104">Create a new [](../resources/application.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="403b4-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="403b4-105">Permissions</span></span>
<span data-ttu-id="403b4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="403b4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="403b4-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="403b4-108">Permission type</span></span>      | <span data-ttu-id="403b4-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="403b4-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="403b4-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="403b4-110">Delegated (work or school account)</span></span> | <span data-ttu-id="403b4-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="403b4-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="403b4-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="403b4-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="403b4-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="403b4-113">Not supported.</span></span>    |
|<span data-ttu-id="403b4-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="403b4-114">Application</span></span> | <span data-ttu-id="403b4-115">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="403b4-115">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="403b4-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="403b4-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /applications
```

## <a name="request-headers"></a><span data-ttu-id="403b4-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="403b4-117">Request headers</span></span>
| <span data-ttu-id="403b4-118">Имя</span><span class="sxs-lookup"><span data-stu-id="403b4-118">Name</span></span>       | <span data-ttu-id="403b4-119">Тип</span><span class="sxs-lookup"><span data-stu-id="403b4-119">Type</span></span> | <span data-ttu-id="403b4-120">Описание</span><span class="sxs-lookup"><span data-stu-id="403b4-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="403b4-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="403b4-121">Authorization</span></span>  | <span data-ttu-id="403b4-122">string</span><span class="sxs-lookup"><span data-stu-id="403b4-122">string</span></span>  | <span data-ttu-id="403b4-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="403b4-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="403b4-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="403b4-125">Request body</span></span>
<span data-ttu-id="403b4-126">В тексте запроса должно быть представление объекта [application](../resources/application.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="403b4-126">In the request body, supply a JSON representation of [application](../resources/application.md) object.</span></span> <span data-ttu-id="403b4-127">Текст запроса должен включать обязательное свойство **displayName**.</span><span class="sxs-lookup"><span data-stu-id="403b4-127">The request body must contain  **displayName**, which is a required property.</span></span>

## <a name="response"></a><span data-ttu-id="403b4-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="403b4-128">Response</span></span>

<span data-ttu-id="403b4-129">В случае успеха этот метод возвращает код отклика `201 Created` и объект [application](../resources/application.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="403b4-129">If successful, this method returns `201 Created` response code and [application](../resources/application.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="403b4-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="403b4-130">Examples</span></span>
### <a name="request"></a><span data-ttu-id="403b4-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="403b4-131">Request</span></span>
<span data-ttu-id="403b4-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="403b4-132">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_application_from_applications"
}-->
```http
POST https://graph.microsoft.com/v1.0/applications
Content-type: application/json
Content-length: 67

{
  "displayName": "Display name"
}
```

### <a name="response"></a><span data-ttu-id="403b4-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="403b4-133">Response</span></span>
<span data-ttu-id="403b4-134">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="403b4-134">Here is an example of the response.</span></span> 

> <span data-ttu-id="403b4-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="403b4-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.application"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 1145

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#applications/$entity",
    "id": "03ef14b0-ca33-4840-8f4f-d6e91916010e",
    "deletedDateTime": null,
    "isFallbackPublicClient": null,
    "appId": "631a96bc-a705-4eda-9f99-fdaf9f54f6a2",
    "applicationTemplateId": null,
    "identifierUris": [],
    "createdDateTime": "2019-09-17T19:10:35.2742618Z",
    "displayName": "Display name",
    "isDeviceOnlyAuthSupported": null,
    "groupMembershipClaims": null,
    "optionalClaims": null,
    "addIns": [],
    "publisherDomain": "contoso.onmicrosoft.com",
    "signInAudience": "AzureADandPersonalMicrosoftAccount",
    "tags": [],
    "tokenEncryptionKeyId": null,
    "api": {
        "requestedAccessTokenVersion": 2,
        "acceptMappedClaims": null,
        "knownClientApplications": [],
        "oauth2PermissionScopes": [],
        "preAuthorizedApplications": []
    },
    "appRoles": [],
    "publicClient": {
        "redirectUris": []
    },
    "info": {
        "termsOfServiceUrl": null,
        "supportUrl": null,
        "privacyStatementUrl": null,
        "marketingUrl": null,
        "logoUrl": null
    },
    "keyCredentials": [],
    "parentalControlSettings": {
        "countriesBlockedForMinors": [],
        "legalAgeGroupRule": "Allow"
    },
    "passwordCredentials": [],
    "requiredResourceAccess": [],
    "web": {
        "redirectUris": [],
        "homePageUrl": null,
        "logoutUrl": null,
        "implicitGrantSettings": {
            "enableIdTokenIssuance": false,
            "enableAccessTokenIssuance": false
        }
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create application",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

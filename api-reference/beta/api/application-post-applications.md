---
title: Создание приложения
description: Создайте новое приложение.
author: sureshja
localization_priority: Priority
doc_type: apiPageType
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 005de9ffadbe5264e595a59b59ae4d4e6c2a4842
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/19/2020
ms.locfileid: "44289311"
---
# <a name="create-application"></a><span data-ttu-id="fd4d7-103">Создание приложения</span><span class="sxs-lookup"><span data-stu-id="fd4d7-103">Create application</span></span>

<span data-ttu-id="fd4d7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fd4d7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fd4d7-105">Создайте новый объект [application](../resources/application.md).</span><span class="sxs-lookup"><span data-stu-id="fd4d7-105">Create a new [application](../resources/application.md) object.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="fd4d7-106">Добавление [**пассвордкредентиал**](../resources/passwordcredential.md) при создании приложений не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fd4d7-106">Adding [**passwordCredential**](../resources/passwordcredential.md) when creating applications is not supported.</span></span> <span data-ttu-id="fd4d7-107">Используйте метод [аддпассворд](application-addpassword.md) , чтобы добавить пароли для приложения.</span><span class="sxs-lookup"><span data-stu-id="fd4d7-107">Use the [addPassword](application-addpassword.md) method to add passwords for an application.</span></span>

## <a name="permissions"></a><span data-ttu-id="fd4d7-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fd4d7-108">Permissions</span></span>
<span data-ttu-id="fd4d7-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fd4d7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="fd4d7-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fd4d7-111">Permission type</span></span>      | <span data-ttu-id="fd4d7-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fd4d7-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fd4d7-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fd4d7-113">Delegated (work or school account)</span></span> | <span data-ttu-id="fd4d7-114">Application. ReadWrite. ALL, Directory. ReadWrite. ALL, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="fd4d7-114">Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="fd4d7-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fd4d7-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fd4d7-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fd4d7-116">Not supported.</span></span>    |
|<span data-ttu-id="fd4d7-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fd4d7-117">Application</span></span> | <span data-ttu-id="fd4d7-118">Application. ReadWrite. Овнедби, Application. ReadWrite. ALL, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="fd4d7-118">Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="fd4d7-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fd4d7-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /applications
```

## <a name="request-headers"></a><span data-ttu-id="fd4d7-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fd4d7-120">Request headers</span></span>
| <span data-ttu-id="fd4d7-121">Имя</span><span class="sxs-lookup"><span data-stu-id="fd4d7-121">Name</span></span>           | <span data-ttu-id="fd4d7-122">Описание</span><span class="sxs-lookup"><span data-stu-id="fd4d7-122">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="fd4d7-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fd4d7-123">Authorization</span></span>  | <span data-ttu-id="fd4d7-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fd4d7-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="fd4d7-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="fd4d7-126">Content-Type</span></span>   | <span data-ttu-id="fd4d7-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fd4d7-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="fd4d7-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fd4d7-129">Request body</span></span>
<span data-ttu-id="fd4d7-130">В тексте запроса должно быть представление объекта [application](../resources/application.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fd4d7-130">In the request body, supply a JSON representation of [application](../resources/application.md) object.</span></span> <span data-ttu-id="fd4d7-131">Текст запроса должен включать обязательное свойство **displayName**.</span><span class="sxs-lookup"><span data-stu-id="fd4d7-131">The request body must contain  **displayName**, which is a required property.</span></span>

## <a name="response"></a><span data-ttu-id="fd4d7-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="fd4d7-132">Response</span></span>

<span data-ttu-id="fd4d7-133">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [application](../resources/application.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="fd4d7-133">If successful, this method returns `201 Created` response code and an [application](../resources/application.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="fd4d7-134">Примеры</span><span class="sxs-lookup"><span data-stu-id="fd4d7-134">Examples</span></span>
### <a name="request"></a><span data-ttu-id="fd4d7-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="fd4d7-135">Request</span></span>
<span data-ttu-id="fd4d7-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fd4d7-136">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="fd4d7-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="fd4d7-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_application_from_applications"
}-->
```http
POST https://graph.microsoft.com/beta/applications
Content-type: application/json
Content-length: 67

{
  "displayName": "Display name"
}
```
# <a name="c"></a>[<span data-ttu-id="fd4d7-138">C#</span><span class="sxs-lookup"><span data-stu-id="fd4d7-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-application-from-applications-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fd4d7-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fd4d7-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-application-from-applications-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fd4d7-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fd4d7-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-application-from-applications-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="fd4d7-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="fd4d7-141">Response</span></span>
<span data-ttu-id="fd4d7-142">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="fd4d7-142">Here is an example of the response.</span></span> 

> <span data-ttu-id="fd4d7-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fd4d7-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#applications/$entity",
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

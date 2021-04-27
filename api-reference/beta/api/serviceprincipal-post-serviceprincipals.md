---
title: Создание объекта serviceprincipal
description: Создание нового объекта serviceprincipal.
author: sureshja
localization_priority: Priority
doc_type: apiPageType
ms.prod: applications
ms.openlocfilehash: 5d3373f0aa90fd794d43cf41601c1190187c98a8
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52051881"
---
# <a name="create-serviceprincipal"></a><span data-ttu-id="08e66-103">Создание объекта servicePrincipal</span><span class="sxs-lookup"><span data-stu-id="08e66-103">Create servicePrincipal</span></span>

<span data-ttu-id="08e66-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="08e66-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="08e66-105">Создание нового объекта [servicePrincipal](../resources/serviceprincipal.md).</span><span class="sxs-lookup"><span data-stu-id="08e66-105">Create a new [servicePrincipal](../resources/serviceprincipal.md) object.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="08e66-106">Добавление [**passwordCredential**](../resources/passwordcredential.md) при создании объектов servicePrincipal не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="08e66-106">Adding [**passwordCredential**](../resources/passwordcredential.md) when creating servicePrincipals is not supported.</span></span> <span data-ttu-id="08e66-107">Используйте метод [addPassword](serviceprincipal-addpassword.md), чтобы добавлять пароли для servicePrincipal.</span><span class="sxs-lookup"><span data-stu-id="08e66-107">Use the [addPassword](serviceprincipal-addpassword.md) method to add passwords for a servicePrincipal.</span></span>

## <a name="permissions"></a><span data-ttu-id="08e66-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="08e66-108">Permissions</span></span>
<span data-ttu-id="08e66-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="08e66-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="08e66-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="08e66-111">Permission type</span></span>      | <span data-ttu-id="08e66-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="08e66-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="08e66-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="08e66-113">Delegated (work or school account)</span></span> | <span data-ttu-id="08e66-114">Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="08e66-114">Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="08e66-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="08e66-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="08e66-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="08e66-116">Not supported.</span></span>    |
|<span data-ttu-id="08e66-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="08e66-117">Application</span></span> | <span data-ttu-id="08e66-118">Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="08e66-118">Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="08e66-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="08e66-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals
```

## <a name="request-headers"></a><span data-ttu-id="08e66-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="08e66-120">Request headers</span></span>
| <span data-ttu-id="08e66-121">Имя</span><span class="sxs-lookup"><span data-stu-id="08e66-121">Name</span></span>       | <span data-ttu-id="08e66-122">Описание</span><span class="sxs-lookup"><span data-stu-id="08e66-122">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="08e66-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="08e66-123">Authorization</span></span> | <span data-ttu-id="08e66-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="08e66-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="08e66-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="08e66-126">Content-Type</span></span> | <span data-ttu-id="08e66-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="08e66-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="08e66-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="08e66-129">Request body</span></span>
<span data-ttu-id="08e66-130">Предоставьте в тексте запроса описание объекта [serviceprincipal](../resources/serviceprincipal.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="08e66-130">In the request body, supply a JSON representation of a [serviceprincipal](../resources/serviceprincipal.md) object.</span></span> <span data-ttu-id="08e66-131">Текст запроса должен содержать **appId**.</span><span class="sxs-lookup"><span data-stu-id="08e66-131">The request body must contain  **appId**.</span></span>

## <a name="response"></a><span data-ttu-id="08e66-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="08e66-132">Response</span></span>

<span data-ttu-id="08e66-133">В случае успеха этот метод возвращает код отклика `201 Created` и объект [serviceprincipal](../resources/serviceprincipal.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="08e66-133">If successful, this method returns a `201 Created` response code and a [serviceprincipal](../resources/serviceprincipal.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="08e66-134">Примеры</span><span class="sxs-lookup"><span data-stu-id="08e66-134">Examples</span></span>
### <a name="request"></a><span data-ttu-id="08e66-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="08e66-135">Request</span></span>
<span data-ttu-id="08e66-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="08e66-136">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="08e66-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="08e66-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_serviceprincipal_from_serviceprincipals"
}-->
```http
POST https://graph.microsoft.com/beta/servicePrincipals
Content-type: application/json

{
  "appId": "65415bb1-9267-4313-bbf5-ae259732ee12",
}
```
# <a name="c"></a>[<span data-ttu-id="08e66-138">C#</span><span class="sxs-lookup"><span data-stu-id="08e66-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-serviceprincipal-from-serviceprincipals-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="08e66-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="08e66-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-serviceprincipal-from-serviceprincipals-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="08e66-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="08e66-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-serviceprincipal-from-serviceprincipals-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="08e66-141">Java</span><span class="sxs-lookup"><span data-stu-id="08e66-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-serviceprincipal-from-serviceprincipals-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="08e66-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="08e66-142">Response</span></span>
<span data-ttu-id="08e66-143">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="08e66-143">Here is an example of the response.</span></span> 

> <span data-ttu-id="08e66-144">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="08e66-144">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.servicePrincipal"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#servicePrincipals/$entity",
    "id": "59e617e5-e447-4adc-8b88-00af644d7c92",
    "deletedDateTime": null,
    "accountEnabled": true,
    "appDisplayName": "My App",
    "appId": "65415bb1-9267-4313-bbf5-ae259732ee12",
    "applicationTemplateId": null,
    "appOwnerOrganizationId": "1bc1c026-2f7b-48a5-98da-afa2fd8bc7bc",
    "appRoleAssignmentRequired": false,
    "displayName": "foo",
    "errorUrl": null,
    "homepage": null,
    "loginUrl": null,
    "logoutUrl": null,
    "notificationEmailAddresses": [],
    "preferredSingleSignOnMode": null,
    "preferredTokenSigningKeyEndDateTime": null,
    "preferredTokenSigningKeyThumbprint": null,
    "publisherName": "Contoso",
    "replyUrls": [],
    "samlMetadataUrl": null,
    "samlSingleSignOnSettings": null,
    "servicePrincipalNames": [
        "f1bd758f-4a1a-4b71-aa20-a248a22a8928"
    ],
    "signInAudience": "AzureADandPersonalMicrosoftAccount",
    "tags": [],
    "addIns": [],
    "api": {
        "resourceSpecificApplicationPermissions": []
    },
    "appRoles": [],
    "info": {
        "termsOfServiceUrl": null,
        "supportUrl": null,
        "privacyStatementUrl": null,
        "marketingUrl": null,
        "logoUrl": null
    },
    "keyCredentials": [],
    "publishedPermissionScopes": [],
    "passwordCredentials": []
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create serviceprincipal",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->




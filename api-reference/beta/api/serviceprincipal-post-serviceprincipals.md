---
title: Создание объекта serviceprincipal
description: Создание нового объекта serviceprincipal.
author: sureshja
localization_priority: Priority
doc_type: apiPageType
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 8d5ba0f54498f7c9315aa339aca78d29b04fcfee
ms.sourcegitcommit: eafb1629e52450dab0da6a1fb6d1ddfa878777c6
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/16/2020
ms.locfileid: "49082092"
---
# <a name="create-serviceprincipal"></a><span data-ttu-id="8ddf7-103">Создание объекта servicePrincipal</span><span class="sxs-lookup"><span data-stu-id="8ddf7-103">Create servicePrincipal</span></span>

<span data-ttu-id="8ddf7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8ddf7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8ddf7-105">Создание нового объекта [servicePrincipal](../resources/serviceprincipal.md).</span><span class="sxs-lookup"><span data-stu-id="8ddf7-105">Create a new [servicePrincipal](../resources/serviceprincipal.md) object.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="8ddf7-106">Добавление [**passwordCredential**](../resources/passwordcredential.md) при создании объектов servicePrincipal не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8ddf7-106">Adding [**passwordCredential**](../resources/passwordcredential.md) when creating servicePrincipals is not supported.</span></span> <span data-ttu-id="8ddf7-107">Используйте метод [addPassword](serviceprincipal-addpassword.md), чтобы добавлять пароли для servicePrincipal.</span><span class="sxs-lookup"><span data-stu-id="8ddf7-107">Use the [addPassword](serviceprincipal-addpassword.md) method to add passwords for a servicePrincipal.</span></span>

## <a name="permissions"></a><span data-ttu-id="8ddf7-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8ddf7-108">Permissions</span></span>
<span data-ttu-id="8ddf7-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8ddf7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="8ddf7-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8ddf7-111">Permission type</span></span>      | <span data-ttu-id="8ddf7-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8ddf7-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8ddf7-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8ddf7-113">Delegated (work or school account)</span></span> | <span data-ttu-id="8ddf7-114">Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="8ddf7-114">Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="8ddf7-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8ddf7-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8ddf7-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8ddf7-116">Not supported.</span></span>    |
|<span data-ttu-id="8ddf7-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8ddf7-117">Application</span></span> | <span data-ttu-id="8ddf7-118">Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8ddf7-118">Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8ddf7-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8ddf7-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals
```

## <a name="request-headers"></a><span data-ttu-id="8ddf7-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8ddf7-120">Request headers</span></span>
| <span data-ttu-id="8ddf7-121">Имя</span><span class="sxs-lookup"><span data-stu-id="8ddf7-121">Name</span></span>       | <span data-ttu-id="8ddf7-122">Описание</span><span class="sxs-lookup"><span data-stu-id="8ddf7-122">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="8ddf7-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8ddf7-123">Authorization</span></span> | <span data-ttu-id="8ddf7-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8ddf7-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="8ddf7-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8ddf7-126">Content-Type</span></span> | <span data-ttu-id="8ddf7-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8ddf7-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8ddf7-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8ddf7-129">Request body</span></span>
<span data-ttu-id="8ddf7-130">Предоставьте в тексте запроса описание объекта [serviceprincipal](../resources/serviceprincipal.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8ddf7-130">In the request body, supply a JSON representation of a [serviceprincipal](../resources/serviceprincipal.md) object.</span></span> <span data-ttu-id="8ddf7-131">Текст запроса должен содержать **appId**.</span><span class="sxs-lookup"><span data-stu-id="8ddf7-131">The request body must contain  **appId**.</span></span>

## <a name="response"></a><span data-ttu-id="8ddf7-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="8ddf7-132">Response</span></span>

<span data-ttu-id="8ddf7-133">В случае успеха этот метод возвращает код отклика `201 Created` и объект [serviceprincipal](../resources/serviceprincipal.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8ddf7-133">If successful, this method returns a `201 Created` response code and a [serviceprincipal](../resources/serviceprincipal.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8ddf7-134">Примеры</span><span class="sxs-lookup"><span data-stu-id="8ddf7-134">Examples</span></span>
### <a name="request"></a><span data-ttu-id="8ddf7-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="8ddf7-135">Request</span></span>
<span data-ttu-id="8ddf7-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8ddf7-136">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="8ddf7-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="8ddf7-137">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="8ddf7-138">C#</span><span class="sxs-lookup"><span data-stu-id="8ddf7-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-serviceprincipal-from-serviceprincipals-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8ddf7-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8ddf7-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-serviceprincipal-from-serviceprincipals-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8ddf7-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8ddf7-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-serviceprincipal-from-serviceprincipals-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8ddf7-141">Java</span><span class="sxs-lookup"><span data-stu-id="8ddf7-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-serviceprincipal-from-serviceprincipals-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="8ddf7-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="8ddf7-142">Response</span></span>
<span data-ttu-id="8ddf7-143">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="8ddf7-143">Here is an example of the response.</span></span> 

> <span data-ttu-id="8ddf7-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8ddf7-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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



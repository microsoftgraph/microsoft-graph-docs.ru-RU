---
title: Создание serviceprincipal
description: Создание нового объекта serviceprincipal.
author: davidmu1
localization_priority: Priority
doc_type: apiPageType
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 439f7c4e41d665eaaa7ce41b2b4372fdd9016388
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/19/2020
ms.locfileid: "44291099"
---
# <a name="create-serviceprincipal"></a><span data-ttu-id="c958f-103">Создание servicePrincipal</span><span class="sxs-lookup"><span data-stu-id="c958f-103">Create servicePrincipal</span></span>

<span data-ttu-id="c958f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c958f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c958f-105">Создание нового объекта [servicePrincipal](../resources/serviceprincipal.md) .</span><span class="sxs-lookup"><span data-stu-id="c958f-105">Create a new [servicePrincipal](../resources/serviceprincipal.md) object.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="c958f-106">Добавление [**пассвордкредентиал**](../resources/passwordcredential.md) при создании сервицепринЦипалс не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c958f-106">Adding [**passwordCredential**](../resources/passwordcredential.md) when creating servicePrincipals is not supported.</span></span> <span data-ttu-id="c958f-107">Используйте метод [аддпассворд](serviceprincipal-addpassword.md) , чтобы добавить пароли для объекта servicePrincipal.</span><span class="sxs-lookup"><span data-stu-id="c958f-107">Use the [addPassword](serviceprincipal-addpassword.md) method to add passwords for a servicePrincipal.</span></span>

## <a name="permissions"></a><span data-ttu-id="c958f-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c958f-108">Permissions</span></span>
<span data-ttu-id="c958f-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c958f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="c958f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c958f-111">Permission type</span></span>      | <span data-ttu-id="c958f-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c958f-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c958f-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c958f-113">Delegated (work or school account)</span></span> | <span data-ttu-id="c958f-114">Application. ReadWrite. ALL, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="c958f-114">Application.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c958f-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c958f-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c958f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c958f-116">Not supported.</span></span>    |
|<span data-ttu-id="c958f-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c958f-117">Application</span></span> | <span data-ttu-id="c958f-118">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c958f-118">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c958f-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c958f-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /serviceprincipals
```

## <a name="request-headers"></a><span data-ttu-id="c958f-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c958f-120">Request headers</span></span>
| <span data-ttu-id="c958f-121">Имя</span><span class="sxs-lookup"><span data-stu-id="c958f-121">Name</span></span>       | <span data-ttu-id="c958f-122">Описание</span><span class="sxs-lookup"><span data-stu-id="c958f-122">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="c958f-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c958f-123">Authorization</span></span> | <span data-ttu-id="c958f-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c958f-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="c958f-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c958f-126">Content-Type</span></span> | <span data-ttu-id="c958f-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c958f-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c958f-129">Основной текст запроса</span><span class="sxs-lookup"><span data-stu-id="c958f-129">Request body</span></span>
<span data-ttu-id="c958f-130">В тексте запроса добавьте представление объекта [serviceprincipal](../resources/serviceprincipal.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c958f-130">In the request body, supply a JSON representation of a [serviceprincipal](../resources/serviceprincipal.md) object.</span></span> <span data-ttu-id="c958f-131">Текст запроса должен содержать **AppID**.</span><span class="sxs-lookup"><span data-stu-id="c958f-131">The request body must contain  **appId**.</span></span>

## <a name="response"></a><span data-ttu-id="c958f-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="c958f-132">Response</span></span>

<span data-ttu-id="c958f-133">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [serviceprincipal](../resources/serviceprincipal.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c958f-133">If successful, this method returns a `201 Created` response code and a [serviceprincipal](../resources/serviceprincipal.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c958f-134">Примеры</span><span class="sxs-lookup"><span data-stu-id="c958f-134">Examples</span></span>
### <a name="request"></a><span data-ttu-id="c958f-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="c958f-135">Request</span></span>
<span data-ttu-id="c958f-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c958f-136">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_serviceprincipal_from_serviceprincipals"
}-->
```http
POST https://graph.microsoft.com/v1.0/serviceprincipals
Content-type: application/json

{
  "appId": "65415bb1-9267-4313-bbf5-ae259732ee12",
}
```

### <a name="response"></a><span data-ttu-id="c958f-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="c958f-137">Response</span></span>
<span data-ttu-id="c958f-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c958f-138">Here is an example of the response.</span></span> 

> <span data-ttu-id="c958f-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c958f-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.servicePrincipal"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#servicePrincipals/$entity",
    "id": "59e617e5-e447-4adc-8b88-00af644d7c92",
    "deletedDateTime": null,
    "accountEnabled": true,
    "appDisplayName": "My App",
    "appId": "65415bb1-9267-4313-bbf5-ae259732ee12",
    "appOwnerOrganizationId": "1bc1c026-2f7b-48a5-98da-afa2fd8bc7bc",
    "appRoleAssignmentRequired": false,
    "displayName": "foo",
    "homepage": null,
    "logoutUrl": null,
    "publisherName": "Contoso",
    "replyUrls": [],
    "servicePrincipalNames": [
        "f1bd758f-4a1a-4b71-aa20-a248a22a8928"
    ],
    "tags": [],
    "addIns": [],
    "appRoles": [],
    "info": {
        "termsOfServiceUrl": null,
        "supportUrl": null,
        "privacyStatementUrl": null,
        "marketingUrl": null,
        "logoUrl": null
    },
    "keyCredentials": [],
    "oauth2PermissionScopes": [],
    "passwordCredentials": []
}
```

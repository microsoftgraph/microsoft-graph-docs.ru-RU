---
title: Get authorizationPolicy
description: Извлечение свойств и связей объекта authorizationPolicy.
localization_priority: Normal
author: abhijeetsinha
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 7ffb4e245e9a24f5ed33576dbd414891ee5d28ac
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50434918"
---
# <a name="get-authorizationpolicy"></a><span data-ttu-id="47e19-103">Get authorizationPolicy</span><span class="sxs-lookup"><span data-stu-id="47e19-103">Get authorizationPolicy</span></span>

<span data-ttu-id="47e19-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="47e19-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="47e19-105">Извлечение свойств [объекта authorizationPolicy.](../resources/authorizationpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="47e19-105">Retrieve the properties of an [authorizationPolicy](../resources/authorizationpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="47e19-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="47e19-106">Permissions</span></span>

<span data-ttu-id="47e19-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="47e19-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="47e19-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="47e19-109">Permission type</span></span>                        | <span data-ttu-id="47e19-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="47e19-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="47e19-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="47e19-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="47e19-112">Policy.Read.All, Policy.ReadWrite.Authorization</span><span class="sxs-lookup"><span data-stu-id="47e19-112">Policy.Read.All, Policy.ReadWrite.Authorization</span></span> |
| <span data-ttu-id="47e19-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="47e19-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="47e19-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="47e19-114">Not supported.</span></span> |
| <span data-ttu-id="47e19-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="47e19-115">Application</span></span>                            | <span data-ttu-id="47e19-116">Policy.Read.All, Policy.ReadWrite.Authorization</span><span class="sxs-lookup"><span data-stu-id="47e19-116">Policy.Read.All, Policy.ReadWrite.Authorization</span></span> |

## <a name="http-request"></a><span data-ttu-id="47e19-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="47e19-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /policies/authorizationPolicy
```

## <a name="request-headers"></a><span data-ttu-id="47e19-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="47e19-118">Request headers</span></span>

| <span data-ttu-id="47e19-119">Имя</span><span class="sxs-lookup"><span data-stu-id="47e19-119">Name</span></span>      |<span data-ttu-id="47e19-120">Описание</span><span class="sxs-lookup"><span data-stu-id="47e19-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="47e19-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="47e19-121">Authorization</span></span> | <span data-ttu-id="47e19-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="47e19-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="47e19-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="47e19-124">Request body</span></span>

<span data-ttu-id="47e19-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="47e19-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="47e19-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="47e19-126">Response</span></span>

<span data-ttu-id="47e19-127">В случае успешной работы этот метод возвращает код ответа и один объект `200 OK` [authorizationPolicy](../resources/authorizationpolicy.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="47e19-127">If successful, this method returns a `200 OK` response code and the single [authorizationPolicy](../resources/authorizationpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="47e19-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="47e19-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="47e19-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="47e19-129">Request</span></span>

<span data-ttu-id="47e19-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="47e19-130">The following is an example of the request.</span></span>

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/policies/authorizationPolicy
```
---

### <a name="response"></a><span data-ttu-id="47e19-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="47e19-131">Response</span></span>

<span data-ttu-id="47e19-132">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="47e19-132">The following is an example of the response.</span></span>

> <span data-ttu-id="47e19-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="47e19-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authorizationPolicy"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#policies/authorizationPolicy/$entity",
    "id": "authorizationPolicy",
    "allowInvitesFrom": "everyone",
    "allowedToSignUpEmailBasedSubscriptions": true,
    "allowedToUseSSPR": true,
    "allowEmailVerifiedUsersToJoinOrganization": true,
    "blockMsolPowerShell": null,
    "displayName": "Authorization Policy",
    "description": "Used to manage authorization related settings across the company.",
    "defaultUserRolePermissions": {
        "allowedToCreateApps": true,
        "allowedToCreateSecurityGroups": true,
        "allowedToReadOtherUsers": true,
        "permissionGrantPoliciesAssigned": [
            "just-user-read"
        ]
    }
}
```

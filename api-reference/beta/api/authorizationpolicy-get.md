---
title: Get authorizationPolicy
description: Извлечение свойств и связей объекта authorizationPolicy.
localization_priority: Normal
author: abhijeetsinha
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: ca66332d7461dfe4e2fc298fffab9ed0cff6e795
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52047954"
---
# <a name="get-authorizationpolicy"></a><span data-ttu-id="442aa-103">Get authorizationPolicy</span><span class="sxs-lookup"><span data-stu-id="442aa-103">Get authorizationPolicy</span></span>

<span data-ttu-id="442aa-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="442aa-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="442aa-105">Извлечение свойств [объекта authorizationPolicy.](../resources/authorizationpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="442aa-105">Retrieve the properties of an [authorizationPolicy](../resources/authorizationpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="442aa-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="442aa-106">Permissions</span></span>

<span data-ttu-id="442aa-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="442aa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="442aa-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="442aa-109">Permission type</span></span>                        | <span data-ttu-id="442aa-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="442aa-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="442aa-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="442aa-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="442aa-112">Policy.Read.All, Policy.ReadWrite.Authorization</span><span class="sxs-lookup"><span data-stu-id="442aa-112">Policy.Read.All, Policy.ReadWrite.Authorization</span></span> |
| <span data-ttu-id="442aa-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="442aa-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="442aa-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="442aa-114">Not supported.</span></span> |
| <span data-ttu-id="442aa-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="442aa-115">Application</span></span>                            | <span data-ttu-id="442aa-116">Policy.Read.All, Policy.ReadWrite.Authorization</span><span class="sxs-lookup"><span data-stu-id="442aa-116">Policy.Read.All, Policy.ReadWrite.Authorization</span></span> |

## <a name="http-request"></a><span data-ttu-id="442aa-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="442aa-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /policies/authorizationPolicy/authorizationPolicy
```

## <a name="request-headers"></a><span data-ttu-id="442aa-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="442aa-118">Request headers</span></span>

| <span data-ttu-id="442aa-119">Имя</span><span class="sxs-lookup"><span data-stu-id="442aa-119">Name</span></span>      |<span data-ttu-id="442aa-120">Описание</span><span class="sxs-lookup"><span data-stu-id="442aa-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="442aa-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="442aa-121">Authorization</span></span> | <span data-ttu-id="442aa-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="442aa-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="442aa-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="442aa-124">Request body</span></span>

<span data-ttu-id="442aa-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="442aa-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="442aa-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="442aa-126">Response</span></span>

<span data-ttu-id="442aa-127">В случае успешной работы этот метод возвращает код ответа и один объект `200 OK` [authorizationPolicy](../resources/authorizationpolicy.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="442aa-127">If successful, this method returns a `200 OK` response code and the single [authorizationPolicy](../resources/authorizationpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="442aa-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="442aa-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="442aa-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="442aa-129">Request</span></span>

<span data-ttu-id="442aa-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="442aa-130">The following is an example of the request.</span></span>

```msgraph-interactive
GET https://graph.microsoft.com/beta/policies/authorizationPolicy/authorizationPolicy
```
---

### <a name="response"></a><span data-ttu-id="442aa-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="442aa-131">Response</span></span>

<span data-ttu-id="442aa-132">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="442aa-132">The following is an example of the response.</span></span>

> <span data-ttu-id="442aa-133">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="442aa-133">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authorizationPolicy"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#policies/authorizationPolicy/$entity",
    "id": "authorizationPolicy",
    "displayName": "Authorization Policy",
    "description": "Used to manage authorization related settings across the company.",
    "enabledPreviewFeatures": [],
    "guestUserRoleId": "10dae51f-b6af-4016-8d66-8c2a99b929b3",
    "blockMsolPowerShell": ""
    "defaultUserRolePermissions": {
        "allowedToCreateApps": true,
        "allowedToCreateSecurityGroups": false,
        "allowedToReadOtherUsers": true
    }
    "allowedToSignUpEmailBasedSubscriptions": false,
    "allowedToUseSSPR": true,
    "allowEmailVerifiedUsersToJoinOrganization": true,
    "permissionGrantPolicyIdsAssignedToDefaultUserRole": [
        "managePermissionGrantsForSelf.microsoft-user-default-low"
    ]
}
```



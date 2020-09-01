---
title: Получение Аусоризатионполици
description: Получение свойств и связей объекта Аусоризатионполици.
localization_priority: Normal
author: abhijeetsinha
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 3f0629cf7be5898c91cc9b5f5212fac56db96ffe
ms.sourcegitcommit: 2c6e16dd8381945de6adf1eea020c142969b7801
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/01/2020
ms.locfileid: "47319395"
---
# <a name="get-authorizationpolicy"></a><span data-ttu-id="a349a-103">Получение Аусоризатионполици</span><span class="sxs-lookup"><span data-stu-id="a349a-103">Get authorizationPolicy</span></span>

<span data-ttu-id="a349a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a349a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a349a-105">Получение свойств объекта [аусоризатионполици](../resources/authorizationpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="a349a-105">Retrieve the properties of an [authorizationPolicy](../resources/authorizationpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="a349a-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a349a-106">Permissions</span></span>

<span data-ttu-id="a349a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a349a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a349a-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a349a-109">Permission type</span></span>                        | <span data-ttu-id="a349a-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a349a-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="a349a-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a349a-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="a349a-112">Policy. Read. ALL, Policy. ReadWrite. Authorization</span><span class="sxs-lookup"><span data-stu-id="a349a-112">Policy.Read.All, Policy.ReadWrite.Authorization</span></span> |
| <span data-ttu-id="a349a-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a349a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a349a-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a349a-114">Not supported.</span></span> |
| <span data-ttu-id="a349a-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="a349a-115">Application</span></span>                            | <span data-ttu-id="a349a-116">Policy. Read. ALL, Policy. ReadWrite. Authorization</span><span class="sxs-lookup"><span data-stu-id="a349a-116">Policy.Read.All, Policy.ReadWrite.Authorization</span></span> |

## <a name="http-request"></a><span data-ttu-id="a349a-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a349a-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /policies/authorizationPolicy/authorizationPolicy
```

## <a name="request-headers"></a><span data-ttu-id="a349a-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a349a-118">Request headers</span></span>

| <span data-ttu-id="a349a-119">Имя</span><span class="sxs-lookup"><span data-stu-id="a349a-119">Name</span></span>      |<span data-ttu-id="a349a-120">Описание</span><span class="sxs-lookup"><span data-stu-id="a349a-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="a349a-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a349a-121">Authorization</span></span> | <span data-ttu-id="a349a-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a349a-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a349a-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a349a-124">Request body</span></span>

<span data-ttu-id="a349a-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a349a-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a349a-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="a349a-126">Response</span></span>

<span data-ttu-id="a349a-127">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и один объект [аусоризатионполици](../resources/authorizationpolicy.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="a349a-127">If successful, this method returns a `200 OK` response code and the single [authorizationPolicy](../resources/authorizationpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a349a-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="a349a-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a349a-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="a349a-129">Request</span></span>

<span data-ttu-id="a349a-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a349a-130">The following is an example of the request.</span></span>

```msgraph-interactive
GET https://graph.microsoft.com/beta/policies/authorizationPolicy/authorizationPolicy
```
---

### <a name="response"></a><span data-ttu-id="a349a-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="a349a-131">Response</span></span>

<span data-ttu-id="a349a-132">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="a349a-132">The following is an example of the response.</span></span>

> <span data-ttu-id="a349a-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a349a-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
}
```

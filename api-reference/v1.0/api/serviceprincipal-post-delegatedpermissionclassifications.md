---
title: Создание делегированияПермиссия
description: Классифицировать разрешение, добавив делегированнуюПермиссию к директору службы API.
localization_priority: Normal
doc_type: apiPageType
ms.prod: applications
author: psignoret
ms.openlocfilehash: adf21db353939dedd926792ddd0d3b7205e1ec2e
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52050313"
---
# <a name="create-delegatedpermissionclassification"></a><span data-ttu-id="7760e-103">Создание делегированияПермиссия</span><span class="sxs-lookup"><span data-stu-id="7760e-103">Create delegatedPermissionClassification</span></span>

<span data-ttu-id="7760e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7760e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7760e-105">Классифицировать делегированное разрешение, добавив [делегированнуюПермиссификацию](../resources/delegatedpermissionclassification.md) в [службуPrincipal,](../resources/servicePrincipal.md) представляющую API.</span><span class="sxs-lookup"><span data-stu-id="7760e-105">Classify a delegated permission by adding a [delegatedPermissionClassification](../resources/delegatedpermissionclassification.md) to the [servicePrincipal](../resources/servicePrincipal.md) representing the API.</span></span>

## <a name="permissions"></a><span data-ttu-id="7760e-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7760e-106">Permissions</span></span>

<span data-ttu-id="7760e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7760e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7760e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7760e-109">Permission type</span></span>      | <span data-ttu-id="7760e-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7760e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7760e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7760e-111">Delegated (work or school account)</span></span> | <span data-ttu-id="7760e-112">PermissionGrantPolicy.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7760e-112">PermissionGrantPolicy.ReadWrite.All</span></span> |
|<span data-ttu-id="7760e-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7760e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7760e-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7760e-114">Not supported.</span></span>    |
|<span data-ttu-id="7760e-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7760e-115">Application</span></span> | <span data-ttu-id="7760e-116">PermissionGrantPolicy.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7760e-116">PermissionGrantPolicy.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7760e-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7760e-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/delegatedPermissionClassifications
```

## <a name="request-headers"></a><span data-ttu-id="7760e-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7760e-118">Request headers</span></span>

| <span data-ttu-id="7760e-119">Имя</span><span class="sxs-lookup"><span data-stu-id="7760e-119">Name</span></span>       | <span data-ttu-id="7760e-120">Описание</span><span class="sxs-lookup"><span data-stu-id="7760e-120">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="7760e-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7760e-121">Authorization</span></span> | <span data-ttu-id="7760e-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7760e-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="7760e-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7760e-124">Content-type</span></span> | <span data-ttu-id="7760e-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7760e-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7760e-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7760e-127">Request body</span></span>

<span data-ttu-id="7760e-128">В теле запроса поставляют представление JSON объекта [делегированияПермиссииКлассификация.](../resources/delegatedpermissionclassification.md)</span><span class="sxs-lookup"><span data-stu-id="7760e-128">In the request body, supply a JSON representation of an [delegatedPermissionClassification](../resources/delegatedpermissionclassification.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="7760e-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="7760e-129">Response</span></span>

<span data-ttu-id="7760e-130">В случае успешной работы этот метод возвращает код ответа и объект `201 Created` [делегированияПермиссииКлассификация](../resources/delegatedpermissionclassification.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="7760e-130">If successful, this method returns a `201 Created` response code and an [delegatedPermissionClassification](../resources/delegatedpermissionclassification.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7760e-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="7760e-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="7760e-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="7760e-132">Request</span></span>

<span data-ttu-id="7760e-133">В следующем примере делегированная разрешения "User.Read" классифицируется как "низкий".</span><span class="sxs-lookup"><span data-stu-id="7760e-133">In the following example, the delegated permission "User.Read" is being classified "low".</span></span>


# <a name="http"></a>[<span data-ttu-id="7760e-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="7760e-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "serviceprincipal_create_delegatedpermissionclassification"
}-->

```http
POST https://graph.microsoft.com/v1.0/servicePrincipals/{id}/delegatedPermissionClassifications
Content-Type: application/json

{
  "permissionId": "e1fe6dd8-ba31-4d61-89e7-88639da4683d",
  "permissionName": "User.Read",
  "classification": "low"
}
```
# <a name="c"></a>[<span data-ttu-id="7760e-135">C#</span><span class="sxs-lookup"><span data-stu-id="7760e-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipal-create-delegatedpermissionclassification-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7760e-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7760e-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-create-delegatedpermissionclassification-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7760e-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7760e-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipal-create-delegatedpermissionclassification-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7760e-138">Java</span><span class="sxs-lookup"><span data-stu-id="7760e-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/serviceprincipal-create-delegatedpermissionclassification-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="7760e-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="7760e-139">Response</span></span>

<span data-ttu-id="7760e-140">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="7760e-140">The following is an example of the response.</span></span>

> <span data-ttu-id="7760e-141">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="7760e-141">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.delegatedPermissionClassification"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "2G3-4TG6YU2J54hjnaRoPQE",
  "permissionId": "e1fe6dd8-ba31-4d61-89e7-88639da4683d",
  "permissionName": "User.Read",
  "classification": "low"
}
```

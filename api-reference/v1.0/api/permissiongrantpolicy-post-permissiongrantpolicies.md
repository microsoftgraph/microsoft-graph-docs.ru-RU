---
title: Создание permissionGrantPolicy
description: Создает объект permissionGrantPolicy, описывающий условия, при которых могут быть предоставлены разрешения.
localization_priority: Normal
doc_type: apiPageType
ms.prod: identity-and-sign-in
author: psignoret
ms.openlocfilehash: a29bf42b3f9bab89e3a498aaab4154cd91b7e0e4
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52051265"
---
# <a name="create-permissiongrantpolicy"></a><span data-ttu-id="35ebd-103">Создание permissionGrantPolicy</span><span class="sxs-lookup"><span data-stu-id="35ebd-103">Create permissionGrantPolicy</span></span>

<span data-ttu-id="35ebd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="35ebd-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="35ebd-105">Создает [permissionGrantPolicy](../resources/permissiongrantpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="35ebd-105">Creates a [permissionGrantPolicy](../resources/permissiongrantpolicy.md).</span></span> <span data-ttu-id="35ebd-106">Политика предоставления разрешений используется для описания условий, при которых могут быть предоставлены разрешения (например, во время согласия приложения).</span><span class="sxs-lookup"><span data-stu-id="35ebd-106">A permission grant policy is used to describe the conditions under which permissions can be granted (for example, during application consent).</span></span>

<span data-ttu-id="35ebd-107">После создания политики предоставления разрешений можно добавить наборы условий [](permissiongrantpolicy-post-excludes.md) для добавления правил совпадения и добавить наборы исключений для добавления правил исключения. [](permissiongrantpolicy-post-includes.md)</span><span class="sxs-lookup"><span data-stu-id="35ebd-107">After creating the permission grant policy, you can [add include condition sets](permissiongrantpolicy-post-includes.md) to add matching rules, and [add exclude condition sets](permissiongrantpolicy-post-excludes.md) to add exclusion rules.</span></span>

## <a name="permissions"></a><span data-ttu-id="35ebd-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="35ebd-108">Permissions</span></span>

<span data-ttu-id="35ebd-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="35ebd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="35ebd-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="35ebd-111">Permission type</span></span>      | <span data-ttu-id="35ebd-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="35ebd-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="35ebd-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="35ebd-113">Delegated (work or school account)</span></span> | <span data-ttu-id="35ebd-114">PermissionGrantPolicy.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="35ebd-114">PermissionGrantPolicy.ReadWrite.All</span></span> |
|<span data-ttu-id="35ebd-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="35ebd-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="35ebd-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="35ebd-116">Not supported.</span></span>    |
|<span data-ttu-id="35ebd-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="35ebd-117">Application</span></span> | <span data-ttu-id="35ebd-118">PermissionGrantPolicy.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="35ebd-118">PermissionGrantPolicy.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="35ebd-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="35ebd-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /policies/permissionGrantPolicies
```

## <a name="request-headers"></a><span data-ttu-id="35ebd-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="35ebd-120">Request headers</span></span>

| <span data-ttu-id="35ebd-121">Имя</span><span class="sxs-lookup"><span data-stu-id="35ebd-121">Name</span></span>       | <span data-ttu-id="35ebd-122">Описание</span><span class="sxs-lookup"><span data-stu-id="35ebd-122">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="35ebd-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="35ebd-123">Authorization</span></span> | <span data-ttu-id="35ebd-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="35ebd-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="35ebd-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="35ebd-126">Content-type</span></span> | <span data-ttu-id="35ebd-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="35ebd-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="35ebd-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="35ebd-129">Request body</span></span>

<span data-ttu-id="35ebd-130">В теле запроса поставляем представление JSON объекта [permissionGrantPolicy.](../resources/permissiongrantpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="35ebd-130">In the request body, supply a JSON representation of an [permissionGrantPolicy](../resources/permissiongrantpolicy.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="35ebd-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="35ebd-131">Response</span></span>

<span data-ttu-id="35ebd-132">В случае успешной работы этот метод возвращает код ответа и `201 Created` [объект permissionGrantPolicy](../resources/permissiongrantpolicy.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="35ebd-132">If successful, this method returns a `201 Created` response code and a [permissionGrantPolicy](../resources/permissiongrantpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="35ebd-133">Примеры</span><span class="sxs-lookup"><span data-stu-id="35ebd-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="35ebd-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="35ebd-134">Request</span></span>

<span data-ttu-id="35ebd-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="35ebd-135">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="35ebd-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="35ebd-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "truncated": true,
  "name": "create_permissiongrantpolicy"
}-->

```http
POST https://graph.microsoft.com/v1.0/policies/permissionGrantPolicies
Content-Type: application/json

{
  "id": "my-custom-consent-policy",
  "displayName": "Custom application consent policy",
  "description": "A custom permission grant policy to customize conditions for granting consent."
}
```
# <a name="c"></a>[<span data-ttu-id="35ebd-137">C#</span><span class="sxs-lookup"><span data-stu-id="35ebd-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-permissiongrantpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="35ebd-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="35ebd-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-permissiongrantpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="35ebd-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="35ebd-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-permissiongrantpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="35ebd-140">Java</span><span class="sxs-lookup"><span data-stu-id="35ebd-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-permissiongrantpolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="35ebd-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="35ebd-141">Response</span></span>

<span data-ttu-id="35ebd-142">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="35ebd-142">The following is an example of the response.</span></span>

> <span data-ttu-id="35ebd-143">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="35ebd-143">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.permissionGrantPolicy"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "my-custom-consent-policy",
  "displayName": "Custom application consent policy",
  "description": "A custom permission grant policy to customize conditions for granting consent."
}
```

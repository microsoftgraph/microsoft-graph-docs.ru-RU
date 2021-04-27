---
title: Создание activityBasedTimeoutPolicy
description: Создайте новое действиеBasedTimeoutPolicy.
localization_priority: Normal
author: lujiangfeng666
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 18f883410957e73bab9c8c74ddb411776de9c435
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048325"
---
# <a name="create-activitybasedtimeoutpolicy"></a><span data-ttu-id="43111-103">Создание activityBasedTimeoutPolicy</span><span class="sxs-lookup"><span data-stu-id="43111-103">Create activityBasedTimeoutPolicy</span></span>

<span data-ttu-id="43111-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="43111-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="43111-105">Создайте новый [объект activityBasedTimeoutPolicy.](../resources/activitybasedtimeoutpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="43111-105">Create a new [activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="43111-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="43111-106">Permissions</span></span>

<span data-ttu-id="43111-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="43111-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="43111-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="43111-109">Permission type</span></span>                        | <span data-ttu-id="43111-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="43111-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="43111-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="43111-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="43111-112">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="43111-112">Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="43111-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="43111-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="43111-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="43111-114">Not supported.</span></span> |
| <span data-ttu-id="43111-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="43111-115">Application</span></span>                            | <span data-ttu-id="43111-116">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="43111-116">Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="43111-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="43111-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST policies/activityBasedTimeoutPolicies
```

## <a name="request-headers"></a><span data-ttu-id="43111-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="43111-118">Request headers</span></span>

| <span data-ttu-id="43111-119">Имя</span><span class="sxs-lookup"><span data-stu-id="43111-119">Name</span></span>          | <span data-ttu-id="43111-120">Описание</span><span class="sxs-lookup"><span data-stu-id="43111-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="43111-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="43111-121">Authorization</span></span> | <span data-ttu-id="43111-122">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="43111-122">Bearer {token}</span></span> |
| <span data-ttu-id="43111-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="43111-123">Content-type</span></span> | <span data-ttu-id="43111-124">application/json</span><span class="sxs-lookup"><span data-stu-id="43111-124">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="43111-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="43111-125">Request body</span></span>

<span data-ttu-id="43111-126">В теле запроса поставляем представление JSON объекта [activityBasedTimeoutPolicy.](../resources/activitybasedtimeoutpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="43111-126">In the request body, supply a JSON representation of [activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="43111-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="43111-127">Response</span></span>

<span data-ttu-id="43111-128">В случае успеха этот метод возвращает код ответа и новый `201 Created` [объект activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="43111-128">If successful, this method returns a `201 Created` response code and a new [activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="43111-129">Примеры</span><span class="sxs-lookup"><span data-stu-id="43111-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="43111-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="43111-130">Request</span></span>

<span data-ttu-id="43111-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="43111-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="43111-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="43111-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_activitybasedtimeoutpolicy_from_activitybasedtimeoutpolicies"
}-->

```http
POST https://graph.microsoft.com/beta/policies/activityBasedTimeoutPolicies
Content-type: application/json

{
  "definition": [
    "definition-value"
  ],
  "displayName": "displayName-value",
  "isOrganizationDefault": true
}
```
# <a name="javascript"></a>[<span data-ttu-id="43111-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="43111-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-activitybasedtimeoutpolicy-from-activitybasedtimeoutpolicies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="43111-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="43111-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-activitybasedtimeoutpolicy-from-activitybasedtimeoutpolicies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="43111-135">C#</span><span class="sxs-lookup"><span data-stu-id="43111-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-activitybasedtimeoutpolicy-from-activitybasedtimeoutpolicies-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="43111-136">Java</span><span class="sxs-lookup"><span data-stu-id="43111-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-activitybasedtimeoutpolicy-from-activitybasedtimeoutpolicies-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="43111-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="43111-137">Response</span></span>

<span data-ttu-id="43111-138">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="43111-138">The following is an example of the response.</span></span>

> <span data-ttu-id="43111-139">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="43111-139">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.activityBasedTimeoutPolicy"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "definition": [
    "definition-value"
  ],
  "displayName": "displayName-value",
  "isOrganizationDefault": true,
  "id": "id-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create activityBasedTimeoutPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->



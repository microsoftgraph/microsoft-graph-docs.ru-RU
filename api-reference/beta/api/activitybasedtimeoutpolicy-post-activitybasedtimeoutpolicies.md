---
title: Создание Активитибаседтимеаутполици
description: Создание нового Активитибаседтимеаутполици.
localization_priority: Normal
author: lujiangfeng666
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: be48befe6c5d5f4e63945e885b8fef89a7605164
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48952550"
---
# <a name="create-activitybasedtimeoutpolicy"></a><span data-ttu-id="b85ea-103">Создание Активитибаседтимеаутполици</span><span class="sxs-lookup"><span data-stu-id="b85ea-103">Create activityBasedTimeoutPolicy</span></span>

<span data-ttu-id="b85ea-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b85ea-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b85ea-105">Создание нового объекта [активитибаседтимеаутполици](../resources/activitybasedtimeoutpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="b85ea-105">Create a new [activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="b85ea-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b85ea-106">Permissions</span></span>

<span data-ttu-id="b85ea-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b85ea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b85ea-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b85ea-109">Permission type</span></span>                        | <span data-ttu-id="b85ea-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b85ea-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="b85ea-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b85ea-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="b85ea-112">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="b85ea-112">Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="b85ea-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b85ea-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b85ea-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b85ea-114">Not supported.</span></span> |
| <span data-ttu-id="b85ea-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b85ea-115">Application</span></span>                            | <span data-ttu-id="b85ea-116">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="b85ea-116">Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="b85ea-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b85ea-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST policies/activityBasedTimeoutPolicies
```

## <a name="request-headers"></a><span data-ttu-id="b85ea-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b85ea-118">Request headers</span></span>

| <span data-ttu-id="b85ea-119">Имя</span><span class="sxs-lookup"><span data-stu-id="b85ea-119">Name</span></span>          | <span data-ttu-id="b85ea-120">Описание</span><span class="sxs-lookup"><span data-stu-id="b85ea-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="b85ea-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="b85ea-121">Authorization</span></span> | <span data-ttu-id="b85ea-122">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="b85ea-122">Bearer {token}</span></span> |
| <span data-ttu-id="b85ea-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b85ea-123">Content-type</span></span> | <span data-ttu-id="b85ea-124">application/json</span><span class="sxs-lookup"><span data-stu-id="b85ea-124">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="b85ea-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b85ea-125">Request body</span></span>

<span data-ttu-id="b85ea-126">В тексте запроса добавьте представление объекта [активитибаседтимеаутполици](../resources/activitybasedtimeoutpolicy.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b85ea-126">In the request body, supply a JSON representation of [activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="b85ea-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="b85ea-127">Response</span></span>

<span data-ttu-id="b85ea-128">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и новый объект [активитибаседтимеаутполици](../resources/activitybasedtimeoutpolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b85ea-128">If successful, this method returns a `201 Created` response code and a new [activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b85ea-129">Примеры</span><span class="sxs-lookup"><span data-stu-id="b85ea-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b85ea-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="b85ea-130">Request</span></span>

<span data-ttu-id="b85ea-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b85ea-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b85ea-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="b85ea-132">HTTP</span></span>](#tab/http)
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
# <a name="javascript"></a>[<span data-ttu-id="b85ea-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b85ea-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-activitybasedtimeoutpolicy-from-activitybasedtimeoutpolicies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b85ea-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b85ea-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-activitybasedtimeoutpolicy-from-activitybasedtimeoutpolicies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="b85ea-135">C#</span><span class="sxs-lookup"><span data-stu-id="b85ea-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-activitybasedtimeoutpolicy-from-activitybasedtimeoutpolicies-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b85ea-136">Java</span><span class="sxs-lookup"><span data-stu-id="b85ea-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-activitybasedtimeoutpolicy-from-activitybasedtimeoutpolicies-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="b85ea-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="b85ea-137">Response</span></span>

<span data-ttu-id="b85ea-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b85ea-138">The following is an example of the response.</span></span>

> <span data-ttu-id="b85ea-p102">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b85ea-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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



---
title: Создание Активитибаседтимеаутполици
description: Создание нового Активитибаседтимеаутполици.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 82528fc95970eea2e6b9d9e01171dc54ad6f314b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42441804"
---
# <a name="create-activitybasedtimeoutpolicy"></a><span data-ttu-id="79c5f-103">Создание Активитибаседтимеаутполици</span><span class="sxs-lookup"><span data-stu-id="79c5f-103">Create activityBasedTimeoutPolicy</span></span>

<span data-ttu-id="79c5f-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="79c5f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="79c5f-105">Создание нового объекта [активитибаседтимеаутполици](../resources/activitybasedtimeoutpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="79c5f-105">Create a new [activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="79c5f-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="79c5f-106">Permissions</span></span>

<span data-ttu-id="79c5f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="79c5f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="79c5f-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="79c5f-109">Permission type</span></span>                        | <span data-ttu-id="79c5f-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="79c5f-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="79c5f-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="79c5f-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="79c5f-112">Policy. ReadWrite. Аппликатионконфигуратион</span><span class="sxs-lookup"><span data-stu-id="79c5f-112">Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="79c5f-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="79c5f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="79c5f-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="79c5f-114">Not supported.</span></span> |
| <span data-ttu-id="79c5f-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="79c5f-115">Application</span></span>                            | <span data-ttu-id="79c5f-116">Policy. ReadWrite. Аппликатионконфигуратион</span><span class="sxs-lookup"><span data-stu-id="79c5f-116">Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="79c5f-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="79c5f-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST policies/activityBasedTimeoutPolicies
```

## <a name="request-headers"></a><span data-ttu-id="79c5f-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="79c5f-118">Request headers</span></span>

| <span data-ttu-id="79c5f-119">Имя</span><span class="sxs-lookup"><span data-stu-id="79c5f-119">Name</span></span>          | <span data-ttu-id="79c5f-120">Описание</span><span class="sxs-lookup"><span data-stu-id="79c5f-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="79c5f-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="79c5f-121">Authorization</span></span> | <span data-ttu-id="79c5f-122">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="79c5f-122">Bearer {token}</span></span> |
| <span data-ttu-id="79c5f-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="79c5f-123">Content-type</span></span> | <span data-ttu-id="79c5f-124">application/json</span><span class="sxs-lookup"><span data-stu-id="79c5f-124">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="79c5f-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="79c5f-125">Request body</span></span>

<span data-ttu-id="79c5f-126">В тексте запроса добавьте представление объекта [активитибаседтимеаутполици](../resources/activitybasedtimeoutpolicy.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="79c5f-126">In the request body, supply a JSON representation of [activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="79c5f-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="79c5f-127">Response</span></span>

<span data-ttu-id="79c5f-128">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и новый объект [активитибаседтимеаутполици](../resources/activitybasedtimeoutpolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="79c5f-128">If successful, this method returns a `201 Created` response code and a new [activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="79c5f-129">Примеры</span><span class="sxs-lookup"><span data-stu-id="79c5f-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="79c5f-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="79c5f-130">Request</span></span>

<span data-ttu-id="79c5f-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="79c5f-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="79c5f-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="79c5f-132">HTTP</span></span>](#tab/http)
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
# <a name="javascript"></a>[<span data-ttu-id="79c5f-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="79c5f-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-activitybasedtimeoutpolicy-from-activitybasedtimeoutpolicies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="79c5f-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="79c5f-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-activitybasedtimeoutpolicy-from-activitybasedtimeoutpolicies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="79c5f-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="79c5f-135">Response</span></span>

<span data-ttu-id="79c5f-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="79c5f-136">The following is an example of the response.</span></span>

> <span data-ttu-id="79c5f-p102">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="79c5f-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

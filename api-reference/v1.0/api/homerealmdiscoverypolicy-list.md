---
title: Перечисление типов ресурсов homeRealmDiscoveryPolicy
description: Получите список объектов homeRealmDiscoveryPolicy.
localization_priority: Normal
author: hpsin
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: a15ebfe7941dae6365b8cbc3d2c23289cce303c6
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52051398"
---
# <a name="list-homerealmdiscoverypolicies"></a><span data-ttu-id="14dc9-103">Перечисление типов ресурсов homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="14dc9-103">List homeRealmDiscoveryPolicies</span></span>

<span data-ttu-id="14dc9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="14dc9-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="14dc9-105">Получите список объектов [homeRealmDiscoveryPolicy.](../resources/homerealmdiscoverypolicy.md)</span><span class="sxs-lookup"><span data-stu-id="14dc9-105">Get a list of [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="14dc9-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="14dc9-106">Permissions</span></span>

<span data-ttu-id="14dc9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="14dc9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="14dc9-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="14dc9-109">Permission type</span></span>                        | <span data-ttu-id="14dc9-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="14dc9-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="14dc9-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="14dc9-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="14dc9-112">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="14dc9-112">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="14dc9-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="14dc9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="14dc9-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="14dc9-114">Not supported.</span></span> |
| <span data-ttu-id="14dc9-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="14dc9-115">Application</span></span>                            | <span data-ttu-id="14dc9-116">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="14dc9-116">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="14dc9-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="14dc9-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET policies/homeRealmDiscoveryPolicies
```

## <a name="optional-query-parameters"></a><span data-ttu-id="14dc9-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="14dc9-118">Optional query parameters</span></span>

<span data-ttu-id="14dc9-119">Этот метод поддерживает `$expand` параметры `$filter` запросов , и `$select` OData, чтобы помочь `$top` настроить ответ.</span><span class="sxs-lookup"><span data-stu-id="14dc9-119">This method supports the `$expand`, `$filter`, `$select`, and `$top` OData query parameters to help customize the response.</span></span> <span data-ttu-id="14dc9-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="14dc9-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span> <span data-ttu-id="14dc9-121">При использовании `$expand` убедитесь, что ваше приложение запрашивает разрешения на чтение расширенных объектов.</span><span class="sxs-lookup"><span data-stu-id="14dc9-121">When using `$expand`, make sure that your app requests permissions to read the expanded objects.</span></span>

## <a name="request-headers"></a><span data-ttu-id="14dc9-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="14dc9-122">Request headers</span></span>

| <span data-ttu-id="14dc9-123">Имя</span><span class="sxs-lookup"><span data-stu-id="14dc9-123">Name</span></span>      |<span data-ttu-id="14dc9-124">Описание</span><span class="sxs-lookup"><span data-stu-id="14dc9-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="14dc9-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="14dc9-125">Authorization</span></span> | <span data-ttu-id="14dc9-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="14dc9-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="14dc9-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="14dc9-128">Request body</span></span>

<span data-ttu-id="14dc9-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="14dc9-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="14dc9-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="14dc9-130">Response</span></span>

<span data-ttu-id="14dc9-131">В случае успешной работы этот метод возвращает код ответа и коллекцию объектов `200 OK` [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="14dc9-131">If successful, this method returns a `200 OK` response code and a collection of [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="14dc9-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="14dc9-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="14dc9-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="14dc9-133">Request</span></span>

<span data-ttu-id="14dc9-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="14dc9-134">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="14dc9-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="14dc9-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_homerealmdiscoverypolicies"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/policies/homeRealmDiscoveryPolicies
```
# <a name="c"></a>[<span data-ttu-id="14dc9-136">C#</span><span class="sxs-lookup"><span data-stu-id="14dc9-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-homerealmdiscoverypolicies-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="14dc9-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="14dc9-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-homerealmdiscoverypolicies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="14dc9-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="14dc9-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-homerealmdiscoverypolicies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="14dc9-139">Java</span><span class="sxs-lookup"><span data-stu-id="14dc9-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-homerealmdiscoverypolicies-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="14dc9-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="14dc9-140">Response</span></span>

<span data-ttu-id="14dc9-141">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="14dc9-141">The following is an example of the response.</span></span>

> <span data-ttu-id="14dc9-142">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="14dc9-142">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.homeRealmDiscoveryPolicy",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "definition": [
        "definition-value"
      ],
      "displayName": "displayName-value",
      "isOrganizationDefault": true,
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List homeRealmDiscoveryPolicies",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


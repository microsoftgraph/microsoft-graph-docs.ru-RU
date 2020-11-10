---
title: Список назначенных ХомереалмдисковериполиЦиес
description: Список ХомереалмдисковериполиЦиес, назначенных для servicePrincipal.
localization_priority: Normal
author: sureshja
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 5d52a680ceb5c4e7a624c9b98a26a1fa75379de1
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48980566"
---
# <a name="list-assigned-homerealmdiscoverypolicy"></a><span data-ttu-id="79ddf-103">Список назначенных Хомереалмдисковериполици</span><span class="sxs-lookup"><span data-stu-id="79ddf-103">List assigned homeRealmDiscoveryPolicy</span></span>

<span data-ttu-id="79ddf-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="79ddf-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="79ddf-105">Перечисление объектов [хомереалмдисковериполици](../resources/homerealmdiscoverypolicy.md) , назначенных для [servicePrincipal](../resources/servicePrincipal.md).</span><span class="sxs-lookup"><span data-stu-id="79ddf-105">List the [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) objects that are assigned to a [servicePrincipal](../resources/servicePrincipal.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="79ddf-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="79ddf-106">Permissions</span></span>

<span data-ttu-id="79ddf-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="79ddf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="79ddf-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="79ddf-109">Permission type</span></span>                        | <span data-ttu-id="79ddf-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="79ddf-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="79ddf-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="79ddf-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="79ddf-112">Policy. Read. ALL и Application. ReadWrite. ALL, Policy. ReadWrite. Аппликатионконфигуратион и Application. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="79ddf-112">Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span>  |
| <span data-ttu-id="79ddf-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="79ddf-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="79ddf-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="79ddf-114">Not supported.</span></span> |
| <span data-ttu-id="79ddf-115">Для приложения</span><span class="sxs-lookup"><span data-stu-id="79ddf-115">Application</span></span>                            | <span data-ttu-id="79ddf-116">Policy. Read. ALL и Application. ReadWrite. Овнедби, Policy. ReadWrite. Аппликатионконфигуратион и Application. ReadWrite. Овнедби, Policy. Read. ALL и Application. ReadWrite. ALL, Policy. ReadWrite. Аппликатионконфигуратион и Application. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="79ddf-116">Policy.Read.All and Application.ReadWrite.OwnedBy, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.OwnedBy, Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="79ddf-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="79ddf-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /servicePrincipals/{id}/homeRealmDiscoveryPolicies
```

## <a name="request-headers"></a><span data-ttu-id="79ddf-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="79ddf-118">Request headers</span></span>

| <span data-ttu-id="79ddf-119">Имя</span><span class="sxs-lookup"><span data-stu-id="79ddf-119">Name</span></span>          | <span data-ttu-id="79ddf-120">Описание</span><span class="sxs-lookup"><span data-stu-id="79ddf-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="79ddf-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="79ddf-121">Authorization</span></span> | <span data-ttu-id="79ddf-122">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="79ddf-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="79ddf-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="79ddf-123">Request body</span></span>

<span data-ttu-id="79ddf-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="79ddf-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="79ddf-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="79ddf-125">Response</span></span>

<span data-ttu-id="79ddf-126">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [хомереалмдисковериполици](../resources/homeRealmDiscoveryPolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="79ddf-126">If successful, this method returns a `200 OK` response code and a collection of [homeRealmDiscoveryPolicy](../resources/homeRealmDiscoveryPolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="79ddf-127">Пример</span><span class="sxs-lookup"><span data-stu-id="79ddf-127">Example</span></span>

### <a name="request"></a><span data-ttu-id="79ddf-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="79ddf-128">Request</span></span>

<span data-ttu-id="79ddf-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="79ddf-129">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="79ddf-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="79ddf-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_homerealmdiscoverypolicies_on_serviceprincipal"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/homeRealmDiscoveryPolicies
```
# <a name="c"></a>[<span data-ttu-id="79ddf-131">C#</span><span class="sxs-lookup"><span data-stu-id="79ddf-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-homerealmdiscoverypolicies-on-serviceprincipal-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="79ddf-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="79ddf-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-homerealmdiscoverypolicies-on-serviceprincipal-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="79ddf-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="79ddf-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-homerealmdiscoverypolicies-on-serviceprincipal-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="79ddf-134">Java</span><span class="sxs-lookup"><span data-stu-id="79ddf-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-homerealmdiscoverypolicies-on-serviceprincipal-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="79ddf-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="79ddf-135">Response</span></span>

<span data-ttu-id="79ddf-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="79ddf-136">The following is an example of the response.</span></span>

> <span data-ttu-id="79ddf-p102">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="79ddf-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "description": "List assigned homeRealmDiscoveryPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->



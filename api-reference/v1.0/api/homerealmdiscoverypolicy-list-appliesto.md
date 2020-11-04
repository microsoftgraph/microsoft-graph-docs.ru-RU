---
title: Список appliesTo
description: Получение списка объектов directoryObject, к которым был применен объект Хомереалмдисковериполици.
localization_priority: Normal
author: hpsin
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 63d6af56795c3333a155df66011acc4a1dcac00d
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/04/2020
ms.locfileid: "48904772"
---
# <a name="list-appliesto"></a><span data-ttu-id="89de3-103">Список appliesTo</span><span class="sxs-lookup"><span data-stu-id="89de3-103">List appliesTo</span></span>

<span data-ttu-id="89de3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="89de3-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="89de3-105">Получение списка объектов [directoryObject](../resources/directoryObject.md) , к которым был применен объект [хомереалмдисковериполици](../resources/homerealmdiscoverypolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="89de3-105">Get a list of [directoryObject](../resources/directoryObject.md) objects that a [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) object has been applied to.</span></span>

## <a name="permissions"></a><span data-ttu-id="89de3-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="89de3-106">Permissions</span></span>

<span data-ttu-id="89de3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="89de3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="89de3-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="89de3-109">Permission type</span></span>                        | <span data-ttu-id="89de3-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="89de3-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="89de3-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="89de3-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="89de3-112">Policy. Read. ALL и Application. Read. ALL, Policy. ReadWrite. Аппликатионконфигуратион и Application. Read. ALL, Directory. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="89de3-112">Policy.Read.All and Application.Read.All, Policy.ReadWrite.ApplicationConfiguration and Application.Read.All, Directory.Read.All</span></span> |
| <span data-ttu-id="89de3-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="89de3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="89de3-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="89de3-114">Not supported.</span></span> |
| <span data-ttu-id="89de3-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="89de3-115">Application</span></span>                            | <span data-ttu-id="89de3-116">Policy. Read. ALL и Application. Read. ALL, Policy. ReadWrite. Аппликатионконфигуратион и Application. Read. ALL, Directory. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="89de3-116">Policy.Read.All and Application.Read.All, Policy.ReadWrite.ApplicationConfiguration and Application.Read.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="89de3-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="89de3-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /policies/homeRealmDiscoveryPolicies/{id}/appliesTo
```

## <a name="optional-query-parameters"></a><span data-ttu-id="89de3-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="89de3-118">Optional query parameters</span></span>

<span data-ttu-id="89de3-119">Этот метод поддерживает `$select` `$top` параметры запросов OData и для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="89de3-119">This method supports the `$select` and `$top` OData query parameters to help customize the response.</span></span> <span data-ttu-id="89de3-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="89de3-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="89de3-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="89de3-121">Request headers</span></span>

| <span data-ttu-id="89de3-122">Имя</span><span class="sxs-lookup"><span data-stu-id="89de3-122">Name</span></span>      |<span data-ttu-id="89de3-123">Описание</span><span class="sxs-lookup"><span data-stu-id="89de3-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="89de3-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="89de3-124">Authorization</span></span> | <span data-ttu-id="89de3-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="89de3-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="89de3-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="89de3-127">Request body</span></span>

<span data-ttu-id="89de3-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="89de3-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="89de3-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="89de3-129">Response</span></span>

<span data-ttu-id="89de3-130">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="89de3-130">If successful, this method returns a `200 OK` response code and a collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="89de3-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="89de3-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="89de3-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="89de3-132">Request</span></span>

<span data-ttu-id="89de3-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="89de3-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="89de3-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="89de3-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_appliesto"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/homeRealmDiscoveryPolicies/{id}/appliesTo
```
# <a name="c"></a>[<span data-ttu-id="89de3-135">C#</span><span class="sxs-lookup"><span data-stu-id="89de3-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-appliesto-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="89de3-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="89de3-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-appliesto-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="89de3-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="89de3-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-appliesto-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="89de3-138">Java</span><span class="sxs-lookup"><span data-stu-id="89de3-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-appliesto-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="89de3-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="89de3-139">Response</span></span>

<span data-ttu-id="89de3-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="89de3-140">The following is an example of the response.</span></span>

> <span data-ttu-id="89de3-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="89de3-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "id-value",
      "deletedDateTime": "datetime-value"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List appliesTo",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

---
title: Список appliesTo
description: Получение списка объектов directoryObject, к которым был применен объект Токениссуанцеполици.
localization_priority: Normal
author: luleonpla
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: a4e3193577061487b813506c868e18b9c6a8763c
ms.sourcegitcommit: 79988a42d91cc25bdd1c531b5f3261901d720a9a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/28/2020
ms.locfileid: "43917245"
---
# <a name="list-appliesto"></a><span data-ttu-id="4c7f5-103">Список appliesTo</span><span class="sxs-lookup"><span data-stu-id="4c7f5-103">List appliesTo</span></span>

<span data-ttu-id="4c7f5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4c7f5-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="4c7f5-105">Получение списка объектов [directoryObject](../resources/directoryObject.md) , к которым был применен объект [токениссуанцеполици](../resources/tokenissuancepolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="4c7f5-105">Get a list of [directoryObject](../resources/directoryObject.md) objects that a [tokenIssuancePolicy](../resources/tokenissuancepolicy.md) object has been applied to.</span></span> <span data-ttu-id="4c7f5-106">Токениссуанцеполици можно применить только к [приложению](../resources/application.md).</span><span class="sxs-lookup"><span data-stu-id="4c7f5-106">The tokenIssuancePolicy can only be applied to [application](../resources/application.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="4c7f5-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4c7f5-107">Permissions</span></span>

<span data-ttu-id="4c7f5-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4c7f5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4c7f5-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4c7f5-110">Permission type</span></span>                        | <span data-ttu-id="4c7f5-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4c7f5-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="4c7f5-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4c7f5-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="4c7f5-113">Policy. Read. ALL и Application. Read. ALL, Policy. ReadWrite. Аппликатионконфигуратион и Application. Read. ALL, Directory. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="4c7f5-113">Policy.Read.All and Application.Read.All, Policy.ReadWrite.ApplicationConfiguration and Application.Read.All, Directory.Read.All</span></span> |
| <span data-ttu-id="4c7f5-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4c7f5-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4c7f5-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4c7f5-115">Not supported.</span></span> |
| <span data-ttu-id="4c7f5-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4c7f5-116">Application</span></span>                            | <span data-ttu-id="4c7f5-117">Policy. Read. ALL и Application. Read. ALL, Policy. ReadWrite. Аппликатионконфигуратион и Application. Read. ALL, Directory. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="4c7f5-117">Policy.Read.All and Application.Read.All, Policy.ReadWrite.ApplicationConfiguration and Application.Read.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4c7f5-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4c7f5-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /policies/tokenIssuancePolicies/{id}/appliesTo
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4c7f5-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="4c7f5-119">Optional query parameters</span></span>

<span data-ttu-id="4c7f5-120">Этот метод поддерживает параметры `$expand`запроса `$select`, и `$top` OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="4c7f5-120">This method supports the `$expand`, `$select`, and `$top` OData query parameters to help customize the response.</span></span> <span data-ttu-id="4c7f5-121">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="4c7f5-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span> <span data-ttu-id="4c7f5-122">При использовании `$expand`убедитесь, что приложение запрашивает разрешения на чтение развернутых объектов.</span><span class="sxs-lookup"><span data-stu-id="4c7f5-122">When using `$expand`, make sure your app requests permissions to read the expanded objects.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4c7f5-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4c7f5-123">Request headers</span></span>

| <span data-ttu-id="4c7f5-124">Имя</span><span class="sxs-lookup"><span data-stu-id="4c7f5-124">Name</span></span>      |<span data-ttu-id="4c7f5-125">Описание</span><span class="sxs-lookup"><span data-stu-id="4c7f5-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="4c7f5-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4c7f5-126">Authorization</span></span> | <span data-ttu-id="4c7f5-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4c7f5-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4c7f5-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4c7f5-129">Request body</span></span>

<span data-ttu-id="4c7f5-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4c7f5-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4c7f5-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="4c7f5-131">Response</span></span>

<span data-ttu-id="4c7f5-132">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4c7f5-132">If successful, this method returns a `200 OK` response code and a collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4c7f5-133">Примеры</span><span class="sxs-lookup"><span data-stu-id="4c7f5-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="4c7f5-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="4c7f5-134">Request</span></span>

<span data-ttu-id="4c7f5-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4c7f5-135">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4c7f5-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="4c7f5-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_appliesto"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/policies/tokenIssuancePolicies/{id}/appliesTo
```
# <a name="c"></a>[<span data-ttu-id="4c7f5-137">C#</span><span class="sxs-lookup"><span data-stu-id="4c7f5-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-appliesto-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4c7f5-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4c7f5-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-appliesto-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4c7f5-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4c7f5-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-appliesto-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4c7f5-140">Java</span><span class="sxs-lookup"><span data-stu-id="4c7f5-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-appliesto-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="4c7f5-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="4c7f5-141">Response</span></span>

<span data-ttu-id="4c7f5-142">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4c7f5-142">The following is an example of the response.</span></span>

> <span data-ttu-id="4c7f5-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4c7f5-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

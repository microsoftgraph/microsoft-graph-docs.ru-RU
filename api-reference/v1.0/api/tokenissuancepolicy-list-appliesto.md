---
title: Список применяетсяTo
description: Получите список объектов directoryObject, к которые был применен объект tokenIssuancePolicy.
localization_priority: Normal
author: luleonpla
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 50cfc949f4e900bc91338d96b297eb3ff4577daf
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50959398"
---
# <a name="list-appliesto"></a><span data-ttu-id="0520e-103">Список применяетсяTo</span><span class="sxs-lookup"><span data-stu-id="0520e-103">List appliesTo</span></span>

<span data-ttu-id="0520e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0520e-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="0520e-105">Получите список объектов [directoryObject,](../resources/directoryObject.md) к которые был применен [объект tokenIssuancePolicy.](../resources/tokenissuancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="0520e-105">Get a list of [directoryObject](../resources/directoryObject.md) objects that a [tokenIssuancePolicy](../resources/tokenissuancepolicy.md) object has been applied to.</span></span> <span data-ttu-id="0520e-106">TokenIssuancePolicy можно применять только к [приложению.](../resources/application.md)</span><span class="sxs-lookup"><span data-stu-id="0520e-106">The tokenIssuancePolicy can only be applied to [application](../resources/application.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="0520e-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0520e-107">Permissions</span></span>

<span data-ttu-id="0520e-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0520e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0520e-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0520e-110">Permission type</span></span>                        | <span data-ttu-id="0520e-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0520e-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="0520e-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0520e-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="0520e-113">Policy.Read.All and Application.Read.All, Policy.ReadWrite.ApplicationConfiguration and Application.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="0520e-113">Policy.Read.All and Application.Read.All, Policy.ReadWrite.ApplicationConfiguration and Application.Read.All, Directory.Read.All</span></span> |
| <span data-ttu-id="0520e-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0520e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0520e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0520e-115">Not supported.</span></span> |
| <span data-ttu-id="0520e-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0520e-116">Application</span></span>                            | <span data-ttu-id="0520e-117">Policy.Read.All and Application.Read.All, Policy.ReadWrite.ApplicationConfiguration and Application.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="0520e-117">Policy.Read.All and Application.Read.All, Policy.ReadWrite.ApplicationConfiguration and Application.Read.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0520e-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0520e-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /policies/tokenIssuancePolicies/{id}/appliesTo
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0520e-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="0520e-119">Optional query parameters</span></span>

<span data-ttu-id="0520e-120">Этот метод поддерживает параметры `$expand` `$select` запроса OData и OData для настройки `$top` ответа.</span><span class="sxs-lookup"><span data-stu-id="0520e-120">This method supports the `$expand`, `$select`, and `$top` OData query parameters to help customize the response.</span></span> <span data-ttu-id="0520e-121">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="0520e-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span> <span data-ttu-id="0520e-122">При использовании убедитесь, что ваше приложение запрашивает `$expand` разрешения на чтение расширенных объектов.</span><span class="sxs-lookup"><span data-stu-id="0520e-122">When using `$expand`, make sure your app requests permissions to read the expanded objects.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0520e-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0520e-123">Request headers</span></span>

| <span data-ttu-id="0520e-124">Имя</span><span class="sxs-lookup"><span data-stu-id="0520e-124">Name</span></span>      |<span data-ttu-id="0520e-125">Описание</span><span class="sxs-lookup"><span data-stu-id="0520e-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="0520e-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0520e-126">Authorization</span></span> | <span data-ttu-id="0520e-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0520e-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0520e-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0520e-129">Request body</span></span>

<span data-ttu-id="0520e-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0520e-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0520e-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="0520e-131">Response</span></span>

<span data-ttu-id="0520e-132">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0520e-132">If successful, this method returns a `200 OK` response code and a collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0520e-133">Примеры</span><span class="sxs-lookup"><span data-stu-id="0520e-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0520e-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="0520e-134">Request</span></span>

<span data-ttu-id="0520e-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0520e-135">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="0520e-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="0520e-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_appliesto_3"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/policies/tokenIssuancePolicies/{id}/appliesTo
```
# <a name="c"></a>[<span data-ttu-id="0520e-137">C#</span><span class="sxs-lookup"><span data-stu-id="0520e-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-appliesto-3-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0520e-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0520e-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-appliesto-3-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0520e-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0520e-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-appliesto-3-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0520e-140">Java</span><span class="sxs-lookup"><span data-stu-id="0520e-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-appliesto-3-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="0520e-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="0520e-141">Response</span></span>

<span data-ttu-id="0520e-142">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="0520e-142">The following is an example of the response.</span></span>

> <span data-ttu-id="0520e-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0520e-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


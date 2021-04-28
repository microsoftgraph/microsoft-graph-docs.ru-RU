---
title: Список применяетсяTo
description: Получите список объектов directoryObject, к которые был применен объект homeRealmDiscoveryPolicy.
localization_priority: Normal
author: hpsin
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 3c30809b8dd25960dbe26275df2509d848a9063a
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52051405"
---
# <a name="list-appliesto"></a><span data-ttu-id="e021b-103">Список применяетсяTo</span><span class="sxs-lookup"><span data-stu-id="e021b-103">List appliesTo</span></span>

<span data-ttu-id="e021b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e021b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e021b-105">Получите список объектов [directoryObject,](../resources/directoryObject.md) к которые был применен [объект homeRealmDiscoveryPolicy.](../resources/homerealmdiscoverypolicy.md)</span><span class="sxs-lookup"><span data-stu-id="e021b-105">Get a list of [directoryObject](../resources/directoryObject.md) objects that a [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) object has been applied to.</span></span>

## <a name="permissions"></a><span data-ttu-id="e021b-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e021b-106">Permissions</span></span>

<span data-ttu-id="e021b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e021b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e021b-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e021b-109">Permission type</span></span>                        | <span data-ttu-id="e021b-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e021b-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="e021b-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e021b-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="e021b-112">Policy.Read.All and Application.Read.All, Policy.ReadWrite.ApplicationConfiguration and Application.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="e021b-112">Policy.Read.All and Application.Read.All, Policy.ReadWrite.ApplicationConfiguration and Application.Read.All, Directory.Read.All</span></span> |
| <span data-ttu-id="e021b-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e021b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e021b-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e021b-114">Not supported.</span></span> |
| <span data-ttu-id="e021b-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e021b-115">Application</span></span>                            | <span data-ttu-id="e021b-116">Policy.Read.All and Application.Read.All, Policy.ReadWrite.ApplicationConfiguration and Application.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="e021b-116">Policy.Read.All and Application.Read.All, Policy.ReadWrite.ApplicationConfiguration and Application.Read.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e021b-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e021b-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /policies/homeRealmDiscoveryPolicies/{id}/appliesTo
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e021b-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="e021b-118">Optional query parameters</span></span>

<span data-ttu-id="e021b-119">Этот метод поддерживает параметры `$select` `$top` запроса oData и OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="e021b-119">This method supports the `$select` and `$top` OData query parameters to help customize the response.</span></span> <span data-ttu-id="e021b-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="e021b-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="e021b-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e021b-121">Request headers</span></span>

| <span data-ttu-id="e021b-122">Имя</span><span class="sxs-lookup"><span data-stu-id="e021b-122">Name</span></span>      |<span data-ttu-id="e021b-123">Описание</span><span class="sxs-lookup"><span data-stu-id="e021b-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e021b-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e021b-124">Authorization</span></span> | <span data-ttu-id="e021b-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e021b-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e021b-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e021b-127">Request body</span></span>

<span data-ttu-id="e021b-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e021b-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e021b-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="e021b-129">Response</span></span>

<span data-ttu-id="e021b-130">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e021b-130">If successful, this method returns a `200 OK` response code and a collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e021b-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="e021b-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e021b-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="e021b-132">Request</span></span>

<span data-ttu-id="e021b-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e021b-133">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="e021b-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="e021b-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_appliesto_2"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/policies/homeRealmDiscoveryPolicies/{id}/appliesTo
```
# <a name="c"></a>[<span data-ttu-id="e021b-135">C#</span><span class="sxs-lookup"><span data-stu-id="e021b-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-appliesto-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e021b-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e021b-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-appliesto-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e021b-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e021b-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-appliesto-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e021b-138">Java</span><span class="sxs-lookup"><span data-stu-id="e021b-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-appliesto-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="e021b-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="e021b-139">Response</span></span>

<span data-ttu-id="e021b-140">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="e021b-140">The following is an example of the response.</span></span>

> <span data-ttu-id="e021b-141">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="e021b-141">**Note:** The response object shown here might be shortened for readability.</span></span>

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

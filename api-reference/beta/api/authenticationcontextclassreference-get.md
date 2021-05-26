---
title: Проверка подлинностиContextClassReference
description: Извлечение свойств и связей объекта authenticationContextClassReference.
localization_priority: Normal
author: calebb
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 38d63cf4422332502d0595b3e00fed2f305c02c6
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/26/2021
ms.locfileid: "52664526"
---
# <a name="get-authenticationcontextclassreference"></a><span data-ttu-id="9b93c-103">Проверка подлинностиContextClassReference</span><span class="sxs-lookup"><span data-stu-id="9b93c-103">Get authenticationContextClassReference</span></span>

<span data-ttu-id="9b93c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9b93c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9b93c-105">Извлечение свойств и связей объекта [authenticationContextClassReference.](../resources/authenticationcontextclassreference.md)</span><span class="sxs-lookup"><span data-stu-id="9b93c-105">Retrieve the properties and relationships of a [authenticationContextClassReference](../resources/authenticationcontextclassreference.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="9b93c-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9b93c-106">Permissions</span></span>

<span data-ttu-id="9b93c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9b93c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9b93c-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9b93c-109">Permission type</span></span>                        | <span data-ttu-id="9b93c-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9b93c-110">Permissions (from least to most privileged)</span></span>                                       |
|:--------------------------------------|:----------------------------------------------------------------------------------|
|<span data-ttu-id="9b93c-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9b93c-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="9b93c-112">Policy.Read.ConditionalAccess</span><span class="sxs-lookup"><span data-stu-id="9b93c-112">Policy.Read.ConditionalAccess</span></span> |
|<span data-ttu-id="9b93c-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9b93c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9b93c-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9b93c-114">Not supported.</span></span> |
|<span data-ttu-id="9b93c-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="9b93c-115">Application</span></span>                            | <span data-ttu-id="9b93c-116">Policy.Read.ConditionalAccess</span><span class="sxs-lookup"><span data-stu-id="9b93c-116">Policy.Read.ConditionalAccess</span></span> |

## <a name="http-request"></a><span data-ttu-id="9b93c-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9b93c-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identity/conditionalAccess/authenticationContextClassReferences/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="9b93c-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="9b93c-118">Optional query parameters</span></span>

<span data-ttu-id="9b93c-119">Этот метод не поддерживает необязательные параметры запроса для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="9b93c-119">This method does not support optional query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9b93c-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9b93c-120">Request headers</span></span>

| <span data-ttu-id="9b93c-121">Имя</span><span class="sxs-lookup"><span data-stu-id="9b93c-121">Name</span></span>      |<span data-ttu-id="9b93c-122">Описание</span><span class="sxs-lookup"><span data-stu-id="9b93c-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="9b93c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9b93c-123">Authorization</span></span> | <span data-ttu-id="9b93c-124">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="9b93c-124">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="9b93c-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="9b93c-125">Request body</span></span>

<span data-ttu-id="9b93c-126">Этот метод поддерживает параметр `$select` запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="9b93c-126">This method supports the `$select` OData query parameter to help customize the response.</span></span> <span data-ttu-id="9b93c-127">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="9b93c-127">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="response"></a><span data-ttu-id="9b93c-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="9b93c-128">Response</span></span>

<span data-ttu-id="9b93c-129">В случае успешной работы этот метод возвращает код ответа и запрашиваемую проверку `200 OK` [подлинностиContextClassReferences](../resources/\authenticationcontextclassreference.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="9b93c-129">If successful, this method returns a `200 OK` response code and the requested [authenticationContextClassReferences](../resources/\authenticationcontextclassreference.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9b93c-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="9b93c-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="9b93c-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="9b93c-131">Request</span></span>

<span data-ttu-id="9b93c-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9b93c-132">The following is an example of the request.</span></span>



# <a name="http"></a>[<span data-ttu-id="9b93c-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="9b93c-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_authenticationcontextclassreference"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identity/conditionalAccess/authenticationContextClassReferences/c1
```
# <a name="c"></a>[<span data-ttu-id="9b93c-134">C#</span><span class="sxs-lookup"><span data-stu-id="9b93c-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-authenticationcontextclassreference-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9b93c-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9b93c-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-authenticationcontextclassreference-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9b93c-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9b93c-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-authenticationcontextclassreference-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9b93c-137">Java</span><span class="sxs-lookup"><span data-stu-id="9b93c-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-authenticationcontextclassreference-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---




### <a name="response"></a><span data-ttu-id="9b93c-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="9b93c-138">Response</span></span>

<span data-ttu-id="9b93c-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="9b93c-139">The following is an example of the response.</span></span>

> <span data-ttu-id="9b93c-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9b93c-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authenticationContextClassReference"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#conditionalAccess/authenticationContextClassReferences/$entity",
    "id": "c1",
    "displayName": "Contoso medium",
    "description": "Medium protection level defined for Contoso policy",
    "isAvailable": false
}

```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get authenticationContextClassReference",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

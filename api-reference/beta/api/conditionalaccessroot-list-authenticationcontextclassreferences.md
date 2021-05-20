---
title: Проверка подлинности спискаContextClassReferences
description: Извлечение списка объектов проверки подлинностиContextClassReference.
localization_priority: Normal
author: calebb
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: c5ad949518d8371e18fc1ef10e680f618056b7f5
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/19/2021
ms.locfileid: "52547467"
---
# <a name="list-authenticationcontextclassreferences"></a><span data-ttu-id="6c67a-103">Проверка подлинности спискаContextClassReferences</span><span class="sxs-lookup"><span data-stu-id="6c67a-103">List authenticationContextClassReferences</span></span>

<span data-ttu-id="6c67a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6c67a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6c67a-105">Извлечение списка объектов [проверки подлинностиContextClassReference.](../resources/authenticationcontextclassreference.md)</span><span class="sxs-lookup"><span data-stu-id="6c67a-105">Retrieve a list of [authenticationContextClassReference](../resources/authenticationcontextclassreference.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="6c67a-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6c67a-106">Permissions</span></span>

<span data-ttu-id="6c67a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6c67a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6c67a-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6c67a-109">Permission type</span></span>                        | <span data-ttu-id="6c67a-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6c67a-110">Permissions (from least to most privileged)</span></span>                                       |
|:--------------------------------------|:----------------------------------------------------------------------------------|
|<span data-ttu-id="6c67a-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6c67a-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="6c67a-112">Policy.Read.ConditionalAccess, Policy.ReadWrite.ConditionalAccess</span><span class="sxs-lookup"><span data-stu-id="6c67a-112">Policy.Read.ConditionalAccess, Policy.ReadWrite.ConditionalAccess</span></span> |
|<span data-ttu-id="6c67a-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6c67a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6c67a-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6c67a-114">Not supported.</span></span> |
|<span data-ttu-id="6c67a-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="6c67a-115">Application</span></span>                            | <span data-ttu-id="6c67a-116">Policy.Read.ConditionalAccess, Policy.ReadWrite.ConditionalAccess</span><span class="sxs-lookup"><span data-stu-id="6c67a-116">Policy.Read.ConditionalAccess, Policy.ReadWrite.ConditionalAccess</span></span> |

## <a name="http-request"></a><span data-ttu-id="6c67a-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6c67a-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identity/conditionalAccess/authenticationContextClassReferences
```
## <a name="optional-query-parameters"></a><span data-ttu-id="6c67a-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="6c67a-118">Optional query parameters</span></span>

<span data-ttu-id="6c67a-119">Этот метод поддерживает параметры `$filter` `$select` запроса oData и OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="6c67a-119">This method supports the `$filter` and `$select` OData query parameters to help customize the response.</span></span> <span data-ttu-id="6c67a-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="6c67a-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="6c67a-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6c67a-121">Request headers</span></span>

| <span data-ttu-id="6c67a-122">Имя</span><span class="sxs-lookup"><span data-stu-id="6c67a-122">Name</span></span>      |<span data-ttu-id="6c67a-123">Описание</span><span class="sxs-lookup"><span data-stu-id="6c67a-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="6c67a-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="6c67a-124">Authorization</span></span> | <span data-ttu-id="6c67a-125">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="6c67a-125">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="6c67a-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6c67a-126">Request body</span></span>

<span data-ttu-id="6c67a-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6c67a-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6c67a-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="6c67a-128">Response</span></span>

<span data-ttu-id="6c67a-129">В случае успешной работы этот метод возвращает код ответа и коллекцию объектов `200 OK` [проверки подлинностиContextClassReference](..\resources\authenticationcontextclassreference.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="6c67a-129">If successful, this method returns a `200 OK` response code and a collection of [authenticationContextClassReference](..\resources\authenticationcontextclassreference.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6c67a-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="6c67a-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6c67a-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="6c67a-131">Request</span></span>

<span data-ttu-id="6c67a-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6c67a-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6c67a-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="6c67a-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_authenticationcontextclassreference"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identity/conditionalAccess/authenticationContextClassReferences
```



### <a name="response"></a><span data-ttu-id="6c67a-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="6c67a-134">Response</span></span>

<span data-ttu-id="6c67a-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="6c67a-135">The following is an example of the response.</span></span>

> <span data-ttu-id="6c67a-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6c67a-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.authenticationContextClassReference",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json


{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#/conditionalAccess/authenticationContextClassReferences",
  "value": [
    {
      "id": "c1",
      "displayName": "Contoso trusted locations",
      "description": "Access is only allowed from trusted locations",
      "isAvailable": true
    }
  ]
}


```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List authenticationContextClassReferences",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

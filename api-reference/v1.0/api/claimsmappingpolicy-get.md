---
title: Получение Клаимсмаппингполици
description: Получение свойств и связей объекта Клаимсмаппингполици.
localization_priority: Normal
author: paulgarn
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 10213a3112ab3b05f1e5b3dcfa4fe497dfadfc36
ms.sourcegitcommit: b083a570375252eff8054f9fe70e1e5e2becc06d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/23/2020
ms.locfileid: "44846334"
---
# <a name="get-claimsmappingpolicy"></a><span data-ttu-id="d5e50-103">Получение Клаимсмаппингполици</span><span class="sxs-lookup"><span data-stu-id="d5e50-103">Get claimsMappingPolicy</span></span>

<span data-ttu-id="d5e50-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d5e50-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d5e50-105">Получение свойств и связей объекта [клаимсмаппингполици](../resources/claimsmappingpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="d5e50-105">Retrieve the properties and relationships of a [claimsMappingPolicy](../resources/claimsmappingpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="d5e50-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d5e50-106">Permissions</span></span>

<span data-ttu-id="d5e50-107">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="d5e50-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="d5e50-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d5e50-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d5e50-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d5e50-109">Permission type</span></span>                        | <span data-ttu-id="d5e50-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d5e50-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="d5e50-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d5e50-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="d5e50-112">Policy. Read. ALL, Policy. ReadWrite. Аппликатионконфигуратион</span><span class="sxs-lookup"><span data-stu-id="d5e50-112">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="d5e50-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d5e50-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d5e50-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d5e50-114">Not supported.</span></span> |
| <span data-ttu-id="d5e50-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d5e50-115">Application</span></span>                            | <span data-ttu-id="d5e50-116">Policy. Read. ALL, Policy. ReadWrite. Аппликатионконфигуратион</span><span class="sxs-lookup"><span data-stu-id="d5e50-116">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="d5e50-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d5e50-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /policies/claimsMappingPolicies/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d5e50-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="d5e50-118">Optional query parameters</span></span>

<span data-ttu-id="d5e50-119">Этот метод поддерживает `$expand` `$select` параметры запросов OData и для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="d5e50-119">This method supports the `$expand` and `$select` OData query parameters to help customize the response.</span></span> <span data-ttu-id="d5e50-120">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="d5e50-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span> <span data-ttu-id="d5e50-121">При использовании `$expand` Убедитесь, что приложение запрашивает разрешения на чтение развернутых объектов.</span><span class="sxs-lookup"><span data-stu-id="d5e50-121">When using `$expand` make sure your app requests permissions to read the expanded objects.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d5e50-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d5e50-122">Request headers</span></span>

| <span data-ttu-id="d5e50-123">Имя</span><span class="sxs-lookup"><span data-stu-id="d5e50-123">Name</span></span>      |<span data-ttu-id="d5e50-124">Описание</span><span class="sxs-lookup"><span data-stu-id="d5e50-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d5e50-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="d5e50-125">Authorization</span></span> | <span data-ttu-id="d5e50-126">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="d5e50-126">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="d5e50-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d5e50-127">Request body</span></span>

<span data-ttu-id="d5e50-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d5e50-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d5e50-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="d5e50-129">Response</span></span>

<span data-ttu-id="d5e50-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и запрошенный объект [клаимсмаппингполици](../resources/claimsmappingpolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d5e50-130">If successful, this method returns a `200 OK` response code and the requested [claimsMappingPolicy](../resources/claimsmappingpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d5e50-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="d5e50-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d5e50-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="d5e50-132">Request</span></span>

<span data-ttu-id="d5e50-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d5e50-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d5e50-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="d5e50-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_claimsmappingpolicy"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/policies/claimsMappingPolicies/{id}
```

### <a name="response"></a><span data-ttu-id="d5e50-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="d5e50-135">Response</span></span>

<span data-ttu-id="d5e50-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d5e50-136">The following is an example of the response.</span></span>

> <span data-ttu-id="d5e50-137">**Note:** The response object shown here might be shortened for readability.</span><span class="sxs-lookup"><span data-stu-id="d5e50-137">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="d5e50-138">All the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="d5e50-138">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.claimsMappingPolicy"
} -->

```http
HTTP/1.1 200 OK
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
  "description": "Get claimsMappingPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

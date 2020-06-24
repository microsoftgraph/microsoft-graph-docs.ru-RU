---
title: Перечисление типов ресурсов claimsMappingPolicy
description: Получение списка объектов Клаимсмаппингполици.
localization_priority: Normal
author: paulgarn
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: c29332a35e9112207f3033b4e63f2b9f73ca2f9e
ms.sourcegitcommit: b083a570375252eff8054f9fe70e1e5e2becc06d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/23/2020
ms.locfileid: "44846330"
---
# <a name="list-claimsmappingpolicies"></a><span data-ttu-id="063cc-103">Перечисление типов ресурсов claimsMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="063cc-103">List claimsMappingPolicies</span></span>

<span data-ttu-id="063cc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="063cc-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="063cc-105">Получение списка объектов [клаимсмаппингполици](../resources/claimsmappingpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="063cc-105">Get a list of [claimsMappingPolicy](../resources/claimsmappingpolicy.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="063cc-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="063cc-106">Permissions</span></span>

<span data-ttu-id="063cc-107">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="063cc-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="063cc-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="063cc-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="063cc-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="063cc-109">Permission type</span></span>                        | <span data-ttu-id="063cc-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="063cc-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="063cc-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="063cc-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="063cc-112">Policy. Read. ALL, Policy. ReadWrite. Аппликатионконфигуратион</span><span class="sxs-lookup"><span data-stu-id="063cc-112">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="063cc-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="063cc-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="063cc-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="063cc-114">Not supported.</span></span> |
| <span data-ttu-id="063cc-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="063cc-115">Application</span></span>                            | <span data-ttu-id="063cc-116">Policy. Read. ALL, Policy. ReadWrite. Аппликатионконфигуратион</span><span class="sxs-lookup"><span data-stu-id="063cc-116">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="063cc-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="063cc-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET policies/claimsMappingPolicies
```

## <a name="optional-query-parameters"></a><span data-ttu-id="063cc-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="063cc-118">Optional query parameters</span></span>

<span data-ttu-id="063cc-119">Этот метод поддерживает `$expand` `$filter` `$select` Параметры запроса, и `$top` OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="063cc-119">This method supports the `$expand`, `$filter`, `$select` and `$top` OData query parameters to help customize the response.</span></span> <span data-ttu-id="063cc-120">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="063cc-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span> <span data-ttu-id="063cc-121">При использовании `$expand` Убедитесь, что приложение запрашивает разрешения на чтение развернутых объектов.</span><span class="sxs-lookup"><span data-stu-id="063cc-121">When using `$expand` make sure your app requests permissions to read the expanded objects.</span></span>

## <a name="request-headers"></a><span data-ttu-id="063cc-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="063cc-122">Request headers</span></span>

| <span data-ttu-id="063cc-123">Имя</span><span class="sxs-lookup"><span data-stu-id="063cc-123">Name</span></span>      |<span data-ttu-id="063cc-124">Описание</span><span class="sxs-lookup"><span data-stu-id="063cc-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="063cc-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="063cc-125">Authorization</span></span> | <span data-ttu-id="063cc-126">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="063cc-126">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="063cc-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="063cc-127">Request body</span></span>

<span data-ttu-id="063cc-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="063cc-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="063cc-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="063cc-129">Response</span></span>

<span data-ttu-id="063cc-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [клаимсмаппингполици](../resources/claimsmappingpolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="063cc-130">If successful, this method returns a `200 OK` response code and a collection of [claimsMappingPolicy](../resources/claimsmappingpolicy.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="063cc-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="063cc-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="063cc-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="063cc-132">Request</span></span>

<span data-ttu-id="063cc-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="063cc-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="063cc-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="063cc-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_claimsmappingpolicies"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/policies/claimsMappingPolicies
```

### <a name="response"></a><span data-ttu-id="063cc-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="063cc-135">Response</span></span>

<span data-ttu-id="063cc-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="063cc-136">The following is an example of the response.</span></span>

> <span data-ttu-id="063cc-137">**Note:** The response object shown here might be shortened for readability.</span><span class="sxs-lookup"><span data-stu-id="063cc-137">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="063cc-138">All the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="063cc-138">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.claimsMappingPolicy",
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
  "description": "List claimsMappingPolicies",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

---
title: Список АктивитибаседтимеаутполиЦиес
description: Получение списка объектов Активитибаседтимеаутполици.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 69412f5f1add1da6d14adccc2012d60c4f7c8cf7
ms.sourcegitcommit: 0536ab327c8b8bf215b726e0d4c25e8f6e8996f9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/18/2020
ms.locfileid: "41234450"
---
# <a name="list-activitybasedtimeoutpolicies"></a><span data-ttu-id="8726a-103">Список АктивитибаседтимеаутполиЦиес</span><span class="sxs-lookup"><span data-stu-id="8726a-103">List activityBasedTimeoutPolicies</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8726a-104">Получение списка объектов [активитибаседтимеаутполици](../resources/activitybasedtimeoutpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="8726a-104">Get a list of [activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="8726a-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8726a-105">Permissions</span></span>

<span data-ttu-id="8726a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8726a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8726a-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8726a-108">Permission type</span></span>                        | <span data-ttu-id="8726a-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8726a-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="8726a-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8726a-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="8726a-111">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="8726a-111">Policy.Read.All</span></span> |
| <span data-ttu-id="8726a-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8726a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8726a-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8726a-113">Not supported.</span></span> |
| <span data-ttu-id="8726a-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8726a-114">Application</span></span>                            | <span data-ttu-id="8726a-115">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="8726a-115">Policy.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8726a-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8726a-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET policies/activityBasedTimeoutPolicies
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8726a-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="8726a-117">Optional query parameters</span></span>

<span data-ttu-id="8726a-118">Этот метод поддерживает `$filter`параметры запросов `$select` OData `$top` и OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="8726a-118">This method supports the `$filter`, `$select` and `$top` OData query parameters to help customize the response.</span></span> <span data-ttu-id="8726a-119">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="8726a-119">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="8726a-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8726a-120">Request headers</span></span>

| <span data-ttu-id="8726a-121">Имя</span><span class="sxs-lookup"><span data-stu-id="8726a-121">Name</span></span>      |<span data-ttu-id="8726a-122">Описание</span><span class="sxs-lookup"><span data-stu-id="8726a-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="8726a-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8726a-123">Authorization</span></span> | <span data-ttu-id="8726a-124">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="8726a-124">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="8726a-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8726a-125">Request body</span></span>

<span data-ttu-id="8726a-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8726a-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8726a-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="8726a-127">Response</span></span>

<span data-ttu-id="8726a-128">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [активитибаседтимеаутполици](../resources/activitybasedtimeoutpolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8726a-128">If successful, this method returns a `200 OK` response code and a collection of [activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8726a-129">Примеры</span><span class="sxs-lookup"><span data-stu-id="8726a-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8726a-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="8726a-130">Request</span></span>

<span data-ttu-id="8726a-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8726a-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_activitybasedtimeoutpolicies"
}-->

```http
GET https://graph.microsoft.com/beta/policies/activityBasedTimeoutPolicies
```

### <a name="response"></a><span data-ttu-id="8726a-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="8726a-132">Response</span></span>

<span data-ttu-id="8726a-133">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="8726a-133">The following is an example of the response.</span></span>

> <span data-ttu-id="8726a-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8726a-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.activityBasedTimeoutPolicy",
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
  "description": "List activityBasedTimeoutPolicies",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
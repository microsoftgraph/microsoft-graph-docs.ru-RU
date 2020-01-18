---
title: Получение Активитибаседтимеаутполици
description: Получение свойств объекта Активитибаседтимеаутполици.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 0d982e993ce9024fcadd810f1d20a804d41c5a04
ms.sourcegitcommit: 0536ab327c8b8bf215b726e0d4c25e8f6e8996f9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/18/2020
ms.locfileid: "41234455"
---
# <a name="get-activitybasedtimeoutpolicy"></a><span data-ttu-id="a863c-103">Получение Активитибаседтимеаутполици</span><span class="sxs-lookup"><span data-stu-id="a863c-103">Get activityBasedTimeoutPolicy</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a863c-104">Получение свойств объекта [активитибаседтимеаутполици](../resources/activitybasedtimeoutpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="a863c-104">Get the properties of an [activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="a863c-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a863c-105">Permissions</span></span>

<span data-ttu-id="a863c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a863c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a863c-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a863c-108">Permission type</span></span>                        | <span data-ttu-id="a863c-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a863c-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="a863c-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a863c-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="a863c-111">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="a863c-111">Policy.Read.All</span></span> |
| <span data-ttu-id="a863c-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a863c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a863c-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a863c-113">Not supported.</span></span> |
| <span data-ttu-id="a863c-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a863c-114">Application</span></span>                            | <span data-ttu-id="a863c-115">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="a863c-115">Policy.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a863c-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a863c-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /policies/activityBasedTimeoutPolicies/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a863c-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="a863c-117">Optional query parameters</span></span>

<span data-ttu-id="a863c-118">Этот метод поддерживает параметры `$select` запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="a863c-118">This method supports the `$select` OData query parameters to help customize the response.</span></span> <span data-ttu-id="a863c-119">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="a863c-119">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="a863c-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a863c-120">Request headers</span></span>

| <span data-ttu-id="a863c-121">Имя</span><span class="sxs-lookup"><span data-stu-id="a863c-121">Name</span></span>      |<span data-ttu-id="a863c-122">Описание</span><span class="sxs-lookup"><span data-stu-id="a863c-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="a863c-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a863c-123">Authorization</span></span> | <span data-ttu-id="a863c-124">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="a863c-124">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="a863c-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a863c-125">Request body</span></span>

<span data-ttu-id="a863c-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a863c-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a863c-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="a863c-127">Response</span></span>

<span data-ttu-id="a863c-128">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и запрошенный объект [активитибаседтимеаутполици](../resources/activitybasedtimeoutpolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a863c-128">If successful, this method returns a `200 OK` response code and the requested [activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a863c-129">Примеры</span><span class="sxs-lookup"><span data-stu-id="a863c-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a863c-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="a863c-130">Request</span></span>

<span data-ttu-id="a863c-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a863c-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_activitybasedtimeoutpolicy"
}-->

```http
GET https://graph.microsoft.com/beta/policies/activityBasedTimeoutPolicies/{id}
```

### <a name="response"></a><span data-ttu-id="a863c-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="a863c-132">Response</span></span>

<span data-ttu-id="a863c-133">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="a863c-133">The following is an example of the response.</span></span>

> <span data-ttu-id="a863c-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a863c-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.activityBasedTimeoutPolicy"
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
  "description": "Get activityBasedTimeoutPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
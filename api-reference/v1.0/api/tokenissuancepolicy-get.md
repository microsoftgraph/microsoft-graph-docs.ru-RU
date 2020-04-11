---
title: Получение Токениссуанцеполици
description: Получение свойств и связей объекта Токениссуанцеполици.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 7c04068e65757faeccfcee4f75574b8494fd6fe2
ms.sourcegitcommit: 9a6ce4ddf75beead19b7c35a1949cf4d105b9b29
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2020
ms.locfileid: "43229691"
---
# <a name="get-tokenissuancepolicy"></a><span data-ttu-id="0eb03-103">Получение Токениссуанцеполици</span><span class="sxs-lookup"><span data-stu-id="0eb03-103">Get tokenIssuancePolicy</span></span>

<span data-ttu-id="0eb03-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0eb03-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="0eb03-105">Получение свойств и связей объекта [токениссуанцеполици](../resources/tokenIssuancePolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="0eb03-105">Retrieve the properties and relationships of a [tokenIssuancePolicy](../resources/tokenIssuancePolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="0eb03-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0eb03-106">Permissions</span></span>

<span data-ttu-id="0eb03-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0eb03-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0eb03-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0eb03-109">Permission type</span></span>                        | <span data-ttu-id="0eb03-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0eb03-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="0eb03-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0eb03-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="0eb03-112">Policy. Read. ALL, Policy. ReadWrite. Аппликатионконфигуратион</span><span class="sxs-lookup"><span data-stu-id="0eb03-112">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="0eb03-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0eb03-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0eb03-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0eb03-114">Not supported.</span></span> |
| <span data-ttu-id="0eb03-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="0eb03-115">Application</span></span>                            | <span data-ttu-id="0eb03-116">Policy. Read. ALL, Policy. ReadWrite. Аппликатионконфигуратион</span><span class="sxs-lookup"><span data-stu-id="0eb03-116">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="0eb03-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0eb03-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /policies/tokenIssuancePolicies/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0eb03-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="0eb03-118">Optional query parameters</span></span>

<span data-ttu-id="0eb03-119">Этот метод поддерживает параметры `$expand` запросов `$select` OData и для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="0eb03-119">This method supports the `$expand` and `$select` OData query parameters to help customize the response.</span></span> <span data-ttu-id="0eb03-120">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="0eb03-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span> <span data-ttu-id="0eb03-121">При использовании `$expand`убедитесь, что приложение запрашивает разрешения на чтение развернутых объектов.</span><span class="sxs-lookup"><span data-stu-id="0eb03-121">When using `$expand`, make sure your app requests permissions to read the expanded objects.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0eb03-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0eb03-122">Request headers</span></span>

| <span data-ttu-id="0eb03-123">Имя</span><span class="sxs-lookup"><span data-stu-id="0eb03-123">Name</span></span>      |<span data-ttu-id="0eb03-124">Описание</span><span class="sxs-lookup"><span data-stu-id="0eb03-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="0eb03-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0eb03-125">Authorization</span></span> | <span data-ttu-id="0eb03-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0eb03-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0eb03-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0eb03-128">Request body</span></span>

<span data-ttu-id="0eb03-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0eb03-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0eb03-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="0eb03-130">Response</span></span>

<span data-ttu-id="0eb03-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и запрошенный объект [токениссуанцеполици](../resources/tokenIssuancePolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0eb03-131">If successful, this method returns a `200 OK` response code and the requested [tokenIssuancePolicy](../resources/tokenIssuancePolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0eb03-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="0eb03-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0eb03-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="0eb03-133">Request</span></span>

<span data-ttu-id="0eb03-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0eb03-134">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_tokenIssuancePolicy"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/policies/tokenIssuancepolicies/{id}
```

### <a name="response"></a><span data-ttu-id="0eb03-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="0eb03-135">Response</span></span>

<span data-ttu-id="0eb03-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="0eb03-136">The following is an example of the response.</span></span>

> <span data-ttu-id="0eb03-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0eb03-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tokenIssuancePolicy"
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
  "description": "Get tokenIssuancePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

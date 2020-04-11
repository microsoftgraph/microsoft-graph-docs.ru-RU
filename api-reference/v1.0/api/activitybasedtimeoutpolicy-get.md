---
title: Получение Активитибаседтимеаутполици
description: Получение свойств объекта Активитибаседтимеаутполици.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 59a51b16b04f1d5930d13074d4f372cffee2b8d9
ms.sourcegitcommit: 9a6ce4ddf75beead19b7c35a1949cf4d105b9b29
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2020
ms.locfileid: "43227937"
---
# <a name="get-activitybasedtimeoutpolicy"></a><span data-ttu-id="b3157-103">Получение Активитибаседтимеаутполици</span><span class="sxs-lookup"><span data-stu-id="b3157-103">Get activityBasedTimeoutPolicy</span></span>

<span data-ttu-id="b3157-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b3157-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="b3157-105">Получение свойств объекта [активитибаседтимеаутполици](../resources/activitybasedtimeoutpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="b3157-105">Get the properties of an [activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="b3157-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b3157-106">Permissions</span></span>

<span data-ttu-id="b3157-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b3157-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b3157-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b3157-109">Permission type</span></span>                        | <span data-ttu-id="b3157-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b3157-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="b3157-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b3157-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="b3157-112">Policy. Read. ALL, Policy. ReadWrite. Аппликатионконфигуратион</span><span class="sxs-lookup"><span data-stu-id="b3157-112">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="b3157-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b3157-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b3157-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b3157-114">Not supported.</span></span> |
| <span data-ttu-id="b3157-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="b3157-115">Application</span></span>                            | <span data-ttu-id="b3157-116">Policy. Read. ALL, Policy. ReadWrite. Аппликатионконфигуратион</span><span class="sxs-lookup"><span data-stu-id="b3157-116">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="b3157-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b3157-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /policies/activityBasedTimeoutPolicies/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b3157-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="b3157-118">Optional query parameters</span></span>

<span data-ttu-id="b3157-119">Этот метод поддерживает параметры `$select` запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="b3157-119">This method supports the `$select` OData query parameters to help customize the response.</span></span> <span data-ttu-id="b3157-120">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="b3157-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="b3157-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b3157-121">Request headers</span></span>

| <span data-ttu-id="b3157-122">Имя</span><span class="sxs-lookup"><span data-stu-id="b3157-122">Name</span></span>      |<span data-ttu-id="b3157-123">Описание</span><span class="sxs-lookup"><span data-stu-id="b3157-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="b3157-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b3157-124">Authorization</span></span> | <span data-ttu-id="b3157-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b3157-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b3157-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b3157-127">Request body</span></span>

<span data-ttu-id="b3157-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b3157-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b3157-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="b3157-129">Response</span></span>

<span data-ttu-id="b3157-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и запрошенный объект [активитибаседтимеаутполици](../resources/activitybasedtimeoutpolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b3157-130">If successful, this method returns a `200 OK` response code and the requested [activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b3157-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="b3157-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b3157-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="b3157-132">Request</span></span>

<span data-ttu-id="b3157-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b3157-133">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_activitybasedtimeoutpolicy"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/policies/activityBasedTimeoutPolicies/{id}
```

### <a name="response"></a><span data-ttu-id="b3157-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="b3157-134">Response</span></span>

<span data-ttu-id="b3157-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b3157-135">The following is an example of the response.</span></span>

> <span data-ttu-id="b3157-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b3157-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

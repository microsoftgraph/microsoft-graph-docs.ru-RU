---
title: Список АктивитибаседтимеаутполиЦиес
description: Получение списка объектов Активитибаседтимеаутполици.
localization_priority: Normal
author: lujiangfeng666
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 9d8b8968ffcabdcc2ff67a280dafe06bdbd0f541
ms.sourcegitcommit: 79988a42d91cc25bdd1c531b5f3261901d720a9a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/28/2020
ms.locfileid: "43917098"
---
# <a name="list-activitybasedtimeoutpolicies"></a><span data-ttu-id="b43bd-103">Список АктивитибаседтимеаутполиЦиес</span><span class="sxs-lookup"><span data-stu-id="b43bd-103">List activityBasedTimeoutPolicies</span></span>

<span data-ttu-id="b43bd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b43bd-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="b43bd-105">Получение списка объектов [активитибаседтимеаутполици](../resources/activitybasedtimeoutpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="b43bd-105">Get a list of [activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="b43bd-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b43bd-106">Permissions</span></span>

<span data-ttu-id="b43bd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b43bd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b43bd-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b43bd-109">Permission type</span></span>                        | <span data-ttu-id="b43bd-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b43bd-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="b43bd-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b43bd-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="b43bd-112">Policy. Read. ALL, Policy. ReadWrite. Аппликатионконфигуратион</span><span class="sxs-lookup"><span data-stu-id="b43bd-112">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="b43bd-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b43bd-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b43bd-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b43bd-114">Not supported.</span></span> |
| <span data-ttu-id="b43bd-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b43bd-115">Application</span></span>                            | <span data-ttu-id="b43bd-116">Policy. Read. ALL, Policy. ReadWrite. Аппликатионконфигуратион</span><span class="sxs-lookup"><span data-stu-id="b43bd-116">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="b43bd-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b43bd-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET policies/activityBasedTimeoutPolicies
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b43bd-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="b43bd-118">Optional query parameters</span></span>

<span data-ttu-id="b43bd-119">Этот метод поддерживает `$filter`параметры запросов `$select` OData `$top` и OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="b43bd-119">This method supports the `$filter`, `$select` and `$top` OData query parameters to help customize the response.</span></span> <span data-ttu-id="b43bd-120">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="b43bd-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="b43bd-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b43bd-121">Request headers</span></span>

| <span data-ttu-id="b43bd-122">Имя</span><span class="sxs-lookup"><span data-stu-id="b43bd-122">Name</span></span>      |<span data-ttu-id="b43bd-123">Описание</span><span class="sxs-lookup"><span data-stu-id="b43bd-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="b43bd-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b43bd-124">Authorization</span></span> | <span data-ttu-id="b43bd-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b43bd-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b43bd-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b43bd-127">Request body</span></span>

<span data-ttu-id="b43bd-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b43bd-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b43bd-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="b43bd-129">Response</span></span>

<span data-ttu-id="b43bd-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [активитибаседтимеаутполици](../resources/activitybasedtimeoutpolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b43bd-130">If successful, this method returns a `200 OK` response code and a collection of [activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b43bd-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="b43bd-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b43bd-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="b43bd-132">Request</span></span>

<span data-ttu-id="b43bd-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b43bd-133">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="b43bd-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="b43bd-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_activitybasedtimeoutpolicies"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/policies/activityBasedTimeoutPolicies
```
# <a name="c"></a>[<span data-ttu-id="b43bd-135">C#</span><span class="sxs-lookup"><span data-stu-id="b43bd-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-activitybasedtimeoutpolicies-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b43bd-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b43bd-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-activitybasedtimeoutpolicies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b43bd-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b43bd-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-activitybasedtimeoutpolicies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b43bd-138">Java</span><span class="sxs-lookup"><span data-stu-id="b43bd-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-activitybasedtimeoutpolicies-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="b43bd-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="b43bd-139">Response</span></span>

<span data-ttu-id="b43bd-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b43bd-140">The following is an example of the response.</span></span>

> <span data-ttu-id="b43bd-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b43bd-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

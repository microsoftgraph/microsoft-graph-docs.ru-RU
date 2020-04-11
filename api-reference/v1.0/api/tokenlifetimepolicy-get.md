---
title: Получение Токенлифетимеполици
description: Получение свойств и связей объекта Токенлифетимеполици.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 8099c651470c30375b0e1118540e5b77b96e91ae
ms.sourcegitcommit: 9a6ce4ddf75beead19b7c35a1949cf4d105b9b29
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2020
ms.locfileid: "43229551"
---
# <a name="get-tokenlifetimepolicy"></a><span data-ttu-id="e699b-103">Получение Токенлифетимеполици</span><span class="sxs-lookup"><span data-stu-id="e699b-103">Get tokenLifetimePolicy</span></span>

<span data-ttu-id="e699b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e699b-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="e699b-105">Получение свойств и связей объекта [токенлифетимеполици](../resources/tokenlifetimepolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="e699b-105">Retrieve the properties and relationships of a [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="e699b-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e699b-106">Permissions</span></span>

<span data-ttu-id="e699b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e699b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e699b-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e699b-109">Permission type</span></span>                        | <span data-ttu-id="e699b-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e699b-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="e699b-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e699b-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="e699b-112">Policy. Read. ALL, Policy. ReadWrite. Аппликатионконфигуратион</span><span class="sxs-lookup"><span data-stu-id="e699b-112">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="e699b-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e699b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e699b-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e699b-114">Not supported.</span></span> |
| <span data-ttu-id="e699b-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="e699b-115">Application</span></span>                            | <span data-ttu-id="e699b-116">Policy. Read. ALL, Policy. ReadWrite. Аппликатионконфигуратион</span><span class="sxs-lookup"><span data-stu-id="e699b-116">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="e699b-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e699b-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /policies/tokenLifetimePolicies/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e699b-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="e699b-118">Optional query parameters</span></span>

<span data-ttu-id="e699b-119">Этот метод поддерживает параметры `$expand` запросов `$select` OData и для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="e699b-119">This method supports the `$expand` and `$select` OData query parameters to help customize the response.</span></span> <span data-ttu-id="e699b-120">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="e699b-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span> <span data-ttu-id="e699b-121">При использовании `$expand` убедитесь, что приложение запрашивает разрешения на чтение развернутых объектов.</span><span class="sxs-lookup"><span data-stu-id="e699b-121">When using `$expand` make sure your app requests permissions to read the expanded objects.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e699b-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e699b-122">Request headers</span></span>

| <span data-ttu-id="e699b-123">Имя</span><span class="sxs-lookup"><span data-stu-id="e699b-123">Name</span></span>      |<span data-ttu-id="e699b-124">Описание</span><span class="sxs-lookup"><span data-stu-id="e699b-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e699b-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e699b-125">Authorization</span></span> | <span data-ttu-id="e699b-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e699b-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e699b-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e699b-128">Request body</span></span>

<span data-ttu-id="e699b-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e699b-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e699b-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="e699b-130">Response</span></span>

<span data-ttu-id="e699b-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и запрошенный объект [токенлифетимеполици](../resources/tokenlifetimepolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e699b-131">If successful, this method returns a `200 OK` response code and the requested [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e699b-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="e699b-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e699b-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="e699b-133">Request</span></span>

<span data-ttu-id="e699b-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e699b-134">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_tokenlifetimepolicy"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/policies/tokenLifetimePolicies/{id}
```

### <a name="response"></a><span data-ttu-id="e699b-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="e699b-135">Response</span></span>

<span data-ttu-id="e699b-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="e699b-136">The following is an example of the response.</span></span>

> <span data-ttu-id="e699b-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e699b-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tokenLifetimePolicy"
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
  "description": "Get tokenLifetimePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

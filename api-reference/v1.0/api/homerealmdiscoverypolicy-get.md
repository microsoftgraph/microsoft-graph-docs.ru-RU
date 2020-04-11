---
title: Получение Хомереалмдисковериполици
description: Получение свойств и связей объекта Хомереалмдисковериполици.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 947c3fe0398580f3ff5deec5fe3f0b845bdcea23
ms.sourcegitcommit: 9a6ce4ddf75beead19b7c35a1949cf4d105b9b29
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2020
ms.locfileid: "43227886"
---
# <a name="get-homerealmdiscoverypolicy"></a><span data-ttu-id="03e31-103">Получение Хомереалмдисковериполици</span><span class="sxs-lookup"><span data-stu-id="03e31-103">Get homeRealmDiscoveryPolicy</span></span>

<span data-ttu-id="03e31-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="03e31-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="03e31-105">Получение свойств и связей объекта [хомереалмдисковериполици](../resources/homerealmdiscoverypolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="03e31-105">Retrieve the properties and relationships of a [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="03e31-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="03e31-106">Permissions</span></span>

<span data-ttu-id="03e31-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="03e31-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="03e31-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="03e31-109">Permission type</span></span>                        | <span data-ttu-id="03e31-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="03e31-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="03e31-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="03e31-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="03e31-112">Policy. Read. ALL, Policy. ReadWrite. Аппликатионконфигуратион</span><span class="sxs-lookup"><span data-stu-id="03e31-112">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="03e31-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="03e31-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="03e31-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="03e31-114">Not supported.</span></span> |
| <span data-ttu-id="03e31-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="03e31-115">Application</span></span>                            | <span data-ttu-id="03e31-116">Policy. Read. ALL, Policy. ReadWrite. Аппликатионконфигуратион</span><span class="sxs-lookup"><span data-stu-id="03e31-116">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="03e31-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="03e31-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /policies/homeRealmDiscoveryPolicies/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="03e31-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="03e31-118">Optional query parameters</span></span>

<span data-ttu-id="03e31-119">Этот метод поддерживает параметры `$expand` запросов `$select` OData и для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="03e31-119">This method supports the `$expand` and `$select` OData query parameters to help customize the response.</span></span> <span data-ttu-id="03e31-120">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="03e31-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span> <span data-ttu-id="03e31-121">При использовании `$expand`убедитесь, что ваше приложение запрашивает разрешение на чтение развернутых объектов.</span><span class="sxs-lookup"><span data-stu-id="03e31-121">When using `$expand`, make sure that your app requests permissions to read the expanded objects.</span></span>

## <a name="request-headers"></a><span data-ttu-id="03e31-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="03e31-122">Request headers</span></span>

| <span data-ttu-id="03e31-123">Имя</span><span class="sxs-lookup"><span data-stu-id="03e31-123">Name</span></span>      |<span data-ttu-id="03e31-124">Описание</span><span class="sxs-lookup"><span data-stu-id="03e31-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="03e31-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="03e31-125">Authorization</span></span> | <span data-ttu-id="03e31-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="03e31-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="03e31-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="03e31-128">Request body</span></span>

<span data-ttu-id="03e31-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="03e31-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="03e31-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="03e31-130">Response</span></span>

<span data-ttu-id="03e31-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и запрошенный объект [хомереалмдисковериполици](../resources/homerealmdiscoverypolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="03e31-131">If successful, this method returns a `200 OK` response code and the requested [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="03e31-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="03e31-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="03e31-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="03e31-133">Request</span></span>

<span data-ttu-id="03e31-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="03e31-134">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_homerealmdiscoverypolicy"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/policies/homeRealmDiscoveryPolicies/{id}
```

### <a name="response"></a><span data-ttu-id="03e31-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="03e31-135">Response</span></span>

<span data-ttu-id="03e31-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="03e31-136">The following is an example of the response.</span></span>

> <span data-ttu-id="03e31-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="03e31-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.homeRealmDiscoveryPolicy"
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
  "description": "Get homeRealmDiscoveryPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

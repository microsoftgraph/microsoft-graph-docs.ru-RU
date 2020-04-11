---
title: Перечисление типов ресурсов homeRealmDiscoveryPolicy
description: Получение списка объектов Хомереалмдисковериполици.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 12c2026e78b0d4915640e967b32132b9cefa4126
ms.sourcegitcommit: 9a6ce4ddf75beead19b7c35a1949cf4d105b9b29
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2020
ms.locfileid: "43227889"
---
# <a name="list-homerealmdiscoverypolicies"></a><span data-ttu-id="ace09-103">Перечисление типов ресурсов homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="ace09-103">List homeRealmDiscoveryPolicies</span></span>

<span data-ttu-id="ace09-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ace09-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="ace09-105">Получение списка объектов [хомереалмдисковериполици](../resources/homerealmdiscoverypolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="ace09-105">Get a list of [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="ace09-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ace09-106">Permissions</span></span>

<span data-ttu-id="ace09-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ace09-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ace09-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ace09-109">Permission type</span></span>                        | <span data-ttu-id="ace09-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ace09-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="ace09-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ace09-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="ace09-112">Policy. Read. ALL, Policy. ReadWrite. Аппликатионконфигуратион</span><span class="sxs-lookup"><span data-stu-id="ace09-112">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="ace09-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ace09-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ace09-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ace09-114">Not supported.</span></span> |
| <span data-ttu-id="ace09-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="ace09-115">Application</span></span>                            | <span data-ttu-id="ace09-116">Policy. Read. ALL, Policy. ReadWrite. Аппликатионконфигуратион</span><span class="sxs-lookup"><span data-stu-id="ace09-116">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="ace09-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ace09-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET policies/homeRealmDiscoveryPolicies
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ace09-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ace09-118">Optional query parameters</span></span>

<span data-ttu-id="ace09-119">Этот метод поддерживает параметры `$expand`запросов `$filter`, `$select`, и `$top` OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="ace09-119">This method supports the `$expand`, `$filter`, `$select`, and `$top` OData query parameters to help customize the response.</span></span> <span data-ttu-id="ace09-120">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="ace09-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span> <span data-ttu-id="ace09-121">При использовании `$expand`убедитесь, что ваше приложение запрашивает разрешение на чтение развернутых объектов.</span><span class="sxs-lookup"><span data-stu-id="ace09-121">When using `$expand`, make sure that your app requests permissions to read the expanded objects.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ace09-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ace09-122">Request headers</span></span>

| <span data-ttu-id="ace09-123">Имя</span><span class="sxs-lookup"><span data-stu-id="ace09-123">Name</span></span>      |<span data-ttu-id="ace09-124">Описание</span><span class="sxs-lookup"><span data-stu-id="ace09-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ace09-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ace09-125">Authorization</span></span> | <span data-ttu-id="ace09-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ace09-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ace09-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ace09-128">Request body</span></span>

<span data-ttu-id="ace09-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ace09-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ace09-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="ace09-130">Response</span></span>

<span data-ttu-id="ace09-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [хомереалмдисковериполици](../resources/homerealmdiscoverypolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ace09-131">If successful, this method returns a `200 OK` response code and a collection of [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ace09-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="ace09-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ace09-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="ace09-133">Request</span></span>

<span data-ttu-id="ace09-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ace09-134">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_homerealmdiscoverypolicies"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/policies/homeRealmDiscoveryPolicies
```

### <a name="response"></a><span data-ttu-id="ace09-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="ace09-135">Response</span></span>

<span data-ttu-id="ace09-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ace09-136">The following is an example of the response.</span></span>

> <span data-ttu-id="ace09-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ace09-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.homeRealmDiscoveryPolicy",
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
  "description": "List homeRealmDiscoveryPolicies",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

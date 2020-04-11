---
title: Перечисление типов ресурсов tokenLifetimePolicy
description: Получение списка объектов Токенлифетимеполици.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: c8ef186128a428b9bc999a14fc61a588a4eb7859
ms.sourcegitcommit: 9a6ce4ddf75beead19b7c35a1949cf4d105b9b29
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2020
ms.locfileid: "43229544"
---
# <a name="list-tokenlifetimepolicies"></a><span data-ttu-id="588bc-103">Перечисление типов ресурсов tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="588bc-103">List tokenLifetimePolicies</span></span>

<span data-ttu-id="588bc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="588bc-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="588bc-105">Получение списка объектов [токенлифетимеполици](../resources/tokenlifetimepolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="588bc-105">Get a list of [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="588bc-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="588bc-106">Permissions</span></span>

<span data-ttu-id="588bc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="588bc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="588bc-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="588bc-109">Permission type</span></span>                        | <span data-ttu-id="588bc-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="588bc-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="588bc-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="588bc-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="588bc-112">Policy. Read. ALL, Policy. ReadWrite. Аппликатионконфигуратион</span><span class="sxs-lookup"><span data-stu-id="588bc-112">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="588bc-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="588bc-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="588bc-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="588bc-114">Not supported.</span></span> |
| <span data-ttu-id="588bc-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="588bc-115">Application</span></span>                            | <span data-ttu-id="588bc-116">Policy. Read. ALL, Policy. ReadWrite. Аппликатионконфигуратион</span><span class="sxs-lookup"><span data-stu-id="588bc-116">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="588bc-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="588bc-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET policies/tokenLifetimePolicies
```

## <a name="optional-query-parameters"></a><span data-ttu-id="588bc-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="588bc-118">Optional query parameters</span></span>

<span data-ttu-id="588bc-119">Этот метод поддерживает параметры `$expand`запроса `$filter`, `$select` и `$top` OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="588bc-119">This method supports the `$expand`, `$filter`, `$select` and `$top` OData query parameters to help customize the response.</span></span> <span data-ttu-id="588bc-120">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="588bc-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span> <span data-ttu-id="588bc-121">При использовании `$expand` убедитесь, что приложение запрашивает разрешения на чтение развернутых объектов.</span><span class="sxs-lookup"><span data-stu-id="588bc-121">When using `$expand` make sure your app requests permissions to read the expanded objects.</span></span>

## <a name="request-headers"></a><span data-ttu-id="588bc-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="588bc-122">Request headers</span></span>

| <span data-ttu-id="588bc-123">Имя</span><span class="sxs-lookup"><span data-stu-id="588bc-123">Name</span></span>      |<span data-ttu-id="588bc-124">Описание</span><span class="sxs-lookup"><span data-stu-id="588bc-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="588bc-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="588bc-125">Authorization</span></span> | <span data-ttu-id="588bc-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="588bc-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="588bc-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="588bc-128">Request body</span></span>

<span data-ttu-id="588bc-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="588bc-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="588bc-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="588bc-130">Response</span></span>

<span data-ttu-id="588bc-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [токенлифетимеполици](../resources/tokenlifetimepolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="588bc-131">If successful, this method returns a `200 OK` response code and a collection of [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="588bc-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="588bc-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="588bc-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="588bc-133">Request</span></span>

<span data-ttu-id="588bc-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="588bc-134">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_tokenlifetimepolicies"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/policies/tokenLifetimePolicies
```

### <a name="response"></a><span data-ttu-id="588bc-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="588bc-135">Response</span></span>

<span data-ttu-id="588bc-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="588bc-136">The following is an example of the response.</span></span>

> <span data-ttu-id="588bc-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="588bc-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tokenLifetimePolicy",
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
  "description": "List tokenLifetimePolicies",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

---
title: Список appliesTo
description: Получение списка объектов directoryObject, к которым был применен объект Токениссуанцеполици.
localization_priority: Normal
author: luleonpla
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 44744f507131633c1c53c5922c4c068a76bf1ac8
ms.sourcegitcommit: 79988a42d91cc25bdd1c531b5f3261901d720a9a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/28/2020
ms.locfileid: "43917455"
---
# <a name="list-appliesto"></a><span data-ttu-id="e910d-103">Список appliesTo</span><span class="sxs-lookup"><span data-stu-id="e910d-103">List appliesTo</span></span>

<span data-ttu-id="e910d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e910d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e910d-105">Получение списка объектов [directoryObject](../resources/directoryObject.md) , к которым был применен объект [токениссуанцеполици](../resources/tokenissuancepolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="e910d-105">Get a list of [directoryObject](../resources/directoryObject.md) objects that a [tokenIssuancePolicy](../resources/tokenissuancepolicy.md) object has been applied to.</span></span> <span data-ttu-id="e910d-106">Токениссуанцеполици можно применять только к ресурсам [Application](../resources/application.md) и [servicePrincipal](../resources/serviceprincipal.md) .</span><span class="sxs-lookup"><span data-stu-id="e910d-106">The tokenIssuancePolicy can only be applied to [application](../resources/application.md) and [servicePrincipal](../resources/serviceprincipal.md) resources.</span></span>

## <a name="permissions"></a><span data-ttu-id="e910d-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e910d-107">Permissions</span></span>

<span data-ttu-id="e910d-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e910d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e910d-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e910d-110">Permission type</span></span>                        | <span data-ttu-id="e910d-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e910d-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="e910d-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e910d-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="e910d-113">Policy. Read. ALL и Application. Read. ALL, Policy. ReadWrite. Аппликатионконфигуратион и Application. Read. ALL, Directory. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="e910d-113">Policy.Read.All and Application.Read.All, Policy.ReadWrite.ApplicationConfiguration and Application.Read.All, Directory.Read.All</span></span> |
| <span data-ttu-id="e910d-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e910d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e910d-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e910d-115">Not supported.</span></span> |
| <span data-ttu-id="e910d-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e910d-116">Application</span></span>                            | <span data-ttu-id="e910d-117">Policy. Read. ALL и Application. Read. ALL, Policy. ReadWrite. Аппликатионконфигуратион и Application. Read. ALL, Directory. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="e910d-117">Policy.Read.All and Application.Read.All, Policy.ReadWrite.ApplicationConfiguration and Application.Read.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e910d-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e910d-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /policies/tokenIssuancePolicies/{id}/appliesTo
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e910d-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="e910d-119">Optional query parameters</span></span>

<span data-ttu-id="e910d-120">Этот метод поддерживает параметры `$expand`запроса `$select`, и `$top` OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="e910d-120">This method supports the `$expand`, `$select`, and `$top` OData query parameters to help customize the response.</span></span> <span data-ttu-id="e910d-121">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="e910d-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span> <span data-ttu-id="e910d-122">При использовании `$expand`убедитесь, что приложение запрашивает разрешения на чтение развернутых объектов.</span><span class="sxs-lookup"><span data-stu-id="e910d-122">When using `$expand`, make sure your app requests permissions to read the expanded objects.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e910d-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e910d-123">Request headers</span></span>

| <span data-ttu-id="e910d-124">Имя</span><span class="sxs-lookup"><span data-stu-id="e910d-124">Name</span></span>      |<span data-ttu-id="e910d-125">Описание</span><span class="sxs-lookup"><span data-stu-id="e910d-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e910d-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e910d-126">Authorization</span></span> | <span data-ttu-id="e910d-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e910d-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e910d-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e910d-129">Request body</span></span>

<span data-ttu-id="e910d-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e910d-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e910d-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="e910d-131">Response</span></span>

<span data-ttu-id="e910d-132">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e910d-132">If successful, this method returns a `200 OK` response code and a collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e910d-133">Примеры</span><span class="sxs-lookup"><span data-stu-id="e910d-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e910d-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="e910d-134">Request</span></span>

<span data-ttu-id="e910d-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e910d-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_appliesto"
}-->

```http
GET https://graph.microsoft.com/beta/tokenIssuancePolicies/{id}/appliesTo
```

### <a name="response"></a><span data-ttu-id="e910d-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="e910d-136">Response</span></span>

<span data-ttu-id="e910d-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="e910d-137">The following is an example of the response.</span></span>

> <span data-ttu-id="e910d-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e910d-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "id-value",
      "deletedDateTime": "datetime-value"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List appliesTo",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

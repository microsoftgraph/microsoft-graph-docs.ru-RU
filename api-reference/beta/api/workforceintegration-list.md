---
title: Список Воркфорцеинтегратионс
description: Получение списка объектов Воркфорцеинтегратион.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 7854a2bded54d8480e9423fb8e7e6d6548455430
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/13/2020
ms.locfileid: "42451287"
---
# <a name="list-workforceintegrations"></a><span data-ttu-id="f0b63-103">Список Воркфорцеинтегратионс</span><span class="sxs-lookup"><span data-stu-id="f0b63-103">List workforceIntegrations</span></span>

<span data-ttu-id="f0b63-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f0b63-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f0b63-105">Получение списка объектов [воркфорцеинтегратион](../resources/workforceintegration.md) .</span><span class="sxs-lookup"><span data-stu-id="f0b63-105">Retrieve a list of [workforceIntegration](../resources/workforceintegration.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="f0b63-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f0b63-106">Permissions</span></span>

<span data-ttu-id="f0b63-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f0b63-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f0b63-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f0b63-109">Permission type</span></span>                        | <span data-ttu-id="f0b63-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f0b63-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="f0b63-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f0b63-111">Delegated (work or school account)</span></span>     |  <span data-ttu-id="f0b63-112">Воркфорцеинтегратион. Read. ALL, Воркфорцеинтегратион. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="f0b63-112">WorkforceIntegration.Read.All, WorkforceIntegration.ReadWrite.All</span></span> |
| <span data-ttu-id="f0b63-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f0b63-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f0b63-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f0b63-114">Not supported.</span></span> |
| <span data-ttu-id="f0b63-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f0b63-115">Application</span></span>                            | <span data-ttu-id="f0b63-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f0b63-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f0b63-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f0b63-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teamwork/workforceIntegrations
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f0b63-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="f0b63-118">Optional query parameters</span></span>

<span data-ttu-id="f0b63-119">Этот метод поддерживает некоторые параметры запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="f0b63-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="f0b63-120">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="f0b63-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="f0b63-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f0b63-121">Request headers</span></span>

| <span data-ttu-id="f0b63-122">Имя</span><span class="sxs-lookup"><span data-stu-id="f0b63-122">Name</span></span>      |<span data-ttu-id="f0b63-123">Описание</span><span class="sxs-lookup"><span data-stu-id="f0b63-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f0b63-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f0b63-124">Authorization</span></span> | <span data-ttu-id="f0b63-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f0b63-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f0b63-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f0b63-127">Request body</span></span>

<span data-ttu-id="f0b63-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f0b63-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f0b63-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="f0b63-129">Response</span></span>

<span data-ttu-id="f0b63-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [воркфорцеинтегратион](../resources/workforceintegration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f0b63-130">If successful, this method returns a `200 OK` response code and a collection of [workforceIntegration](../resources/workforceintegration.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f0b63-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="f0b63-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f0b63-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="f0b63-132">Request</span></span>

<span data-ttu-id="f0b63-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f0b63-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f0b63-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="f0b63-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_workforceintegrations"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/teamwork/workforceIntegrations
```
# <a name="c"></a>[<span data-ttu-id="f0b63-135">C#</span><span class="sxs-lookup"><span data-stu-id="f0b63-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-workforceintegrations-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f0b63-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f0b63-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-workforceintegrations-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f0b63-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f0b63-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-workforceintegrations-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f0b63-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="f0b63-138">Response</span></span>

<span data-ttu-id="f0b63-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="f0b63-139">The following is an example of the response.</span></span>

> <span data-ttu-id="f0b63-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f0b63-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workforceIntegration",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "displayName": "displayName-value",
      "apiVersion": 99,
      "encryption": {
        "protocol": "protocol-value",
        "secret": "secret-value"
      },
      "isActive": true,
      "url": "url-value",
      "supports": "supports-value"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List workforceIntegrations",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

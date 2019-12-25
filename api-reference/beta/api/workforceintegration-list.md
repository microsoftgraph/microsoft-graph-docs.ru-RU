---
title: Список Воркфорцеинтегратионс
description: Получение списка объектов Воркфорцеинтегратион.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: aea3aea8181d83e1cb04be3578ef0b88d8829c15
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40870610"
---
# <a name="list-workforceintegrations"></a><span data-ttu-id="4417e-103">Список Воркфорцеинтегратионс</span><span class="sxs-lookup"><span data-stu-id="4417e-103">List workforceIntegrations</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4417e-104">Получение списка объектов [воркфорцеинтегратион](../resources/workforceintegration.md) .</span><span class="sxs-lookup"><span data-stu-id="4417e-104">Retrieve a list of [workforceIntegration](../resources/workforceintegration.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="4417e-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4417e-105">Permissions</span></span>

<span data-ttu-id="4417e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4417e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4417e-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4417e-108">Permission type</span></span>                        | <span data-ttu-id="4417e-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4417e-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="4417e-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4417e-110">Delegated (work or school account)</span></span>     |  <span data-ttu-id="4417e-111">Воркфорцеинтегратион. Read. ALL, Воркфорцеинтегратион. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="4417e-111">WorkforceIntegration.Read.All, WorkforceIntegration.ReadWrite.All</span></span> |
| <span data-ttu-id="4417e-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4417e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4417e-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4417e-113">Not supported.</span></span> |
| <span data-ttu-id="4417e-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4417e-114">Application</span></span>                            | <span data-ttu-id="4417e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4417e-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4417e-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4417e-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teamwork/workforceIntegrations
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4417e-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="4417e-117">Optional query parameters</span></span>

<span data-ttu-id="4417e-118">Этот метод поддерживает некоторые параметры запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="4417e-118">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="4417e-119">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="4417e-119">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="4417e-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4417e-120">Request headers</span></span>

| <span data-ttu-id="4417e-121">Имя</span><span class="sxs-lookup"><span data-stu-id="4417e-121">Name</span></span>      |<span data-ttu-id="4417e-122">Описание</span><span class="sxs-lookup"><span data-stu-id="4417e-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="4417e-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4417e-123">Authorization</span></span> | <span data-ttu-id="4417e-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4417e-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4417e-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4417e-126">Request body</span></span>

<span data-ttu-id="4417e-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4417e-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4417e-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="4417e-128">Response</span></span>

<span data-ttu-id="4417e-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [воркфорцеинтегратион](../resources/workforceintegration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4417e-129">If successful, this method returns a `200 OK` response code and a collection of [workforceIntegration](../resources/workforceintegration.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4417e-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="4417e-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="4417e-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="4417e-131">Request</span></span>

<span data-ttu-id="4417e-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4417e-132">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="4417e-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="4417e-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_workforceintegrations"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/teamwork/workforceIntegrations
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="4417e-134">C#</span><span class="sxs-lookup"><span data-stu-id="4417e-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-workforceintegrations-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4417e-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4417e-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-workforceintegrations-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="4417e-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4417e-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-workforceintegrations-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="4417e-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="4417e-137">Response</span></span>

<span data-ttu-id="4417e-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4417e-138">The following is an example of the response.</span></span>

> <span data-ttu-id="4417e-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4417e-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

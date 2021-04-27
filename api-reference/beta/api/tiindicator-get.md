---
title: Получить индикатор сведении об угрозах
description: Извлечение свойств и связей объекта tiindicator.
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: 7ae7d1dc59493454a3fef55948bb712a3aa1c772
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52036403"
---
# <a name="get-threat-intelligence-indicator"></a><span data-ttu-id="ec839-103">Получить индикатор сведении об угрозах</span><span class="sxs-lookup"><span data-stu-id="ec839-103">Get threat intelligence indicator</span></span>

<span data-ttu-id="ec839-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ec839-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ec839-105">Извлечение свойств и связей [объекта tiIndicator.](../resources/tiindicator.md)</span><span class="sxs-lookup"><span data-stu-id="ec839-105">Retrieve the properties and relationships of a [tiIndicator](../resources/tiindicator.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="ec839-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ec839-106">Permissions</span></span>

<span data-ttu-id="ec839-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ec839-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ec839-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ec839-109">Permission type</span></span>                        | <span data-ttu-id="ec839-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ec839-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="ec839-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ec839-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="ec839-112">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="ec839-112">ThreatIndicators.ReadWrite.OwnedBy</span></span> |
| <span data-ttu-id="ec839-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ec839-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ec839-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ec839-114">Not supported.</span></span> |
| <span data-ttu-id="ec839-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ec839-115">Application</span></span>                            | <span data-ttu-id="ec839-116">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="ec839-116">ThreatIndicators.ReadWrite.OwnedBy</span></span> |

## <a name="http-request"></a><span data-ttu-id="ec839-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ec839-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/tiIndicators/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ec839-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ec839-118">Optional query parameters</span></span>

<span data-ttu-id="ec839-119">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="ec839-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="ec839-120">Общие сведения см. в [окне Параметры запроса OData.](/graph/query-parameters)</span><span class="sxs-lookup"><span data-stu-id="ec839-120">For general information, see [OData Query Parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="ec839-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ec839-121">Request headers</span></span>

| <span data-ttu-id="ec839-122">Имя</span><span class="sxs-lookup"><span data-stu-id="ec839-122">Name</span></span>      |<span data-ttu-id="ec839-123">Описание</span><span class="sxs-lookup"><span data-stu-id="ec839-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ec839-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ec839-124">Authorization</span></span> | <span data-ttu-id="ec839-125">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="ec839-125">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="ec839-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ec839-126">Request body</span></span>

<span data-ttu-id="ec839-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ec839-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ec839-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="ec839-128">Response</span></span>

<span data-ttu-id="ec839-129">В случае успешной работы этот метод возвращает код ответа и `200 OK` [объект tiIndicator](../resources/tiindicator.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="ec839-129">If successful, this method returns a `200 OK` response code and a [tiIndicator](../resources/tiindicator.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ec839-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="ec839-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ec839-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="ec839-131">Request</span></span>

<span data-ttu-id="ec839-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ec839-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ec839-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="ec839-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_tiindicator"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/security/tiIndicators/{id}
```
# <a name="c"></a>[<span data-ttu-id="ec839-134">C#</span><span class="sxs-lookup"><span data-stu-id="ec839-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-tiindicator-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ec839-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ec839-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-tiindicator-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ec839-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ec839-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-tiindicator-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ec839-137">Java</span><span class="sxs-lookup"><span data-stu-id="ec839-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-tiindicator-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="ec839-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="ec839-138">Response</span></span>

<span data-ttu-id="ec839-139">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="ec839-139">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="ec839-140">Объект ответа, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="ec839-140">The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tiIndicator"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "action": "action-value",
  "activityGroupNames": [
    "activityGroupNames-value"
  ],
  "additionalInformation": "additionalInformation-value",
  "azureTenantId": "azureTenantId-value",
  "confidence": 99,
  "description": "description-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get tiIndicator",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->



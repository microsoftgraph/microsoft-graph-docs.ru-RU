---
title: Получение Воркфорцеинтегратион
description: Получение свойств и связей объекта воркфорцеинтегратион.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: f66479af44efcbc686ad5d3acfa7155b26447a0f
ms.sourcegitcommit: 02c16375520853d3fa2a82ff012639550f981fc8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/07/2020
ms.locfileid: "44154103"
---
# <a name="get-workforceintegration"></a><span data-ttu-id="89222-103">Получение Воркфорцеинтегратион</span><span class="sxs-lookup"><span data-stu-id="89222-103">Get workforceIntegration</span></span>

<span data-ttu-id="89222-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="89222-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="89222-105">Получение свойств и связей объекта [воркфорцеинтегратион](../resources/workforceintegration.md) .</span><span class="sxs-lookup"><span data-stu-id="89222-105">Retrieve the properties and relationships of a [workforceintegration](../resources/workforceintegration.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="89222-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="89222-106">Permissions</span></span>

<span data-ttu-id="89222-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="89222-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="89222-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="89222-109">Permission type</span></span>                        | <span data-ttu-id="89222-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="89222-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="89222-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="89222-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="89222-112">Воркфорцеинтегратион. Read. ALL, Воркфорцеинтегратион. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="89222-112">WorkforceIntegration.Read.All, WorkforceIntegration.ReadWrite.All</span></span> |
| <span data-ttu-id="89222-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="89222-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="89222-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="89222-114">Not supported.</span></span> |
| <span data-ttu-id="89222-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="89222-115">Application</span></span>                            | <span data-ttu-id="89222-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="89222-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="89222-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="89222-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teamwork/workforceIntegrations/{workforceIntegrationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="89222-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="89222-118">Optional query parameters</span></span>

<span data-ttu-id="89222-119">Этот метод поддерживает некоторые параметры запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="89222-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="89222-120">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="89222-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="89222-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="89222-121">Request headers</span></span>

| <span data-ttu-id="89222-122">Имя</span><span class="sxs-lookup"><span data-stu-id="89222-122">Name</span></span>      |<span data-ttu-id="89222-123">Описание</span><span class="sxs-lookup"><span data-stu-id="89222-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="89222-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="89222-124">Authorization</span></span> | <span data-ttu-id="89222-125">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="89222-125">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="89222-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="89222-126">Request body</span></span>

<span data-ttu-id="89222-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="89222-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="89222-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="89222-128">Response</span></span>

<span data-ttu-id="89222-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и запрошенный объект [воркфорцеинтегратион](../resources/workforceintegration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="89222-129">If successful, this method returns a `200 OK` response code and the requested [workforceIntegration](../resources/workforceintegration.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="89222-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="89222-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="89222-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="89222-131">Request</span></span>

<span data-ttu-id="89222-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="89222-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="89222-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="89222-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_workforceintegration"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/teamwork/workforceIntegrations/{workforceintegrationid}
```
# <a name="c"></a>[<span data-ttu-id="89222-134">C#</span><span class="sxs-lookup"><span data-stu-id="89222-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-workforceintegration-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="89222-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="89222-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-workforceintegration-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="89222-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="89222-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-workforceintegration-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="89222-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="89222-137">Response</span></span>

<span data-ttu-id="89222-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="89222-138">The following is an example of the response.</span></span>

> <span data-ttu-id="89222-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="89222-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workforceIntegration"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "c5d0c76b-80c4-481c-be50-923cd8d680a1",
  "displayName": "KronosWorkforceIntegration",
  "apiVersion": 1,
  "isActive": true,
  "encryption": {
    "protocol": "sharedSecret",
    "secret": null
  },
  "url": "https://contosoWorkforceIntegration.com/Contoso/",
  "supports": "shift"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get workforceIntegration",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

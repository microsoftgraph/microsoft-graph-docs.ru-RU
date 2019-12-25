---
title: Получение Воркфорцеинтегратион
description: Получение свойств и связей объекта воркфорцеинтегратион.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 92da94aa2b2b58bbea3af0ed47582d1532793349
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40870557"
---
# <a name="get-workforceintegration"></a><span data-ttu-id="9023f-103">Получение Воркфорцеинтегратион</span><span class="sxs-lookup"><span data-stu-id="9023f-103">Get workforceIntegration</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9023f-104">Получение свойств и связей объекта [воркфорцеинтегратион](../resources/workforceintegration.md) .</span><span class="sxs-lookup"><span data-stu-id="9023f-104">Retrieve the properties and relationships of a [workforceintegration](../resources/workforceintegration.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="9023f-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9023f-105">Permissions</span></span>

<span data-ttu-id="9023f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9023f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9023f-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9023f-108">Permission type</span></span>                        | <span data-ttu-id="9023f-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9023f-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="9023f-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9023f-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="9023f-111">Воркфорцеинтегратион. Read. ALL, Воркфорцеинтегратион. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="9023f-111">WorkforceIntegration.Read.All, WorkforceIntegration.ReadWrite.All</span></span> |
| <span data-ttu-id="9023f-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9023f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9023f-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9023f-113">Not supported.</span></span> |
| <span data-ttu-id="9023f-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9023f-114">Application</span></span>                            | <span data-ttu-id="9023f-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9023f-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9023f-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9023f-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teamwork/workforceIntegrations
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9023f-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="9023f-117">Optional query parameters</span></span>

<span data-ttu-id="9023f-118">Этот метод поддерживает некоторые параметры запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="9023f-118">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="9023f-119">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="9023f-119">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="9023f-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9023f-120">Request headers</span></span>

| <span data-ttu-id="9023f-121">Имя</span><span class="sxs-lookup"><span data-stu-id="9023f-121">Name</span></span>      |<span data-ttu-id="9023f-122">Описание</span><span class="sxs-lookup"><span data-stu-id="9023f-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="9023f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9023f-123">Authorization</span></span> | <span data-ttu-id="9023f-124">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="9023f-124">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="9023f-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="9023f-125">Request body</span></span>

<span data-ttu-id="9023f-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9023f-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9023f-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="9023f-127">Response</span></span>

<span data-ttu-id="9023f-128">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и запрошенный объект [воркфорцеинтегратион](../resources/workforceintegration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9023f-128">If successful, this method returns a `200 OK` response code and the requested [workforceIntegration](../resources/workforceintegration.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9023f-129">Примеры</span><span class="sxs-lookup"><span data-stu-id="9023f-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="9023f-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="9023f-130">Request</span></span>

<span data-ttu-id="9023f-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9023f-131">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="9023f-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="9023f-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_workforceintegration"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/teamwork/workforceIntegrations/{workforceintegrationid}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="9023f-133">C#</span><span class="sxs-lookup"><span data-stu-id="9023f-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-workforceintegration-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9023f-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9023f-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-workforceintegration-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="9023f-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9023f-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-workforceintegration-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="9023f-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="9023f-136">Response</span></span>

<span data-ttu-id="9023f-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="9023f-137">The following is an example of the response.</span></span>

> <span data-ttu-id="9023f-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9023f-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

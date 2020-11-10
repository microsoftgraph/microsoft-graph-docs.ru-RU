---
title: Получение Аппликатионтемплате
description: Получение свойств и связей объекта аппликатионтемплате.
localization_priority: Normal
author: luleonpla
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 596ae1ecbf8c3a2fd98272e2f03b413d7841c08f
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48961751"
---
# <a name="get-applicationtemplate"></a><span data-ttu-id="1ff9c-103">Получение Аппликатионтемплате</span><span class="sxs-lookup"><span data-stu-id="1ff9c-103">Get applicationTemplate</span></span>

<span data-ttu-id="1ff9c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1ff9c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1ff9c-105">Получение свойств объекта [аппликатионтемплате](../resources/applicationtemplate.md) .</span><span class="sxs-lookup"><span data-stu-id="1ff9c-105">Retrieve the properties of an [applicationTemplate](../resources/applicationtemplate.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="1ff9c-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1ff9c-106">Permissions</span></span>

<span data-ttu-id="1ff9c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1ff9c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1ff9c-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1ff9c-109">Permission type</span></span>                        | <span data-ttu-id="1ff9c-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1ff9c-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="1ff9c-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1ff9c-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="1ff9c-112">Нет.</span><span class="sxs-lookup"><span data-stu-id="1ff9c-112">None.</span></span> |
| <span data-ttu-id="1ff9c-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1ff9c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1ff9c-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1ff9c-114">Not supported.</span></span> |
| <span data-ttu-id="1ff9c-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1ff9c-115">Application</span></span>                            | <span data-ttu-id="1ff9c-116">Нет.</span><span class="sxs-lookup"><span data-stu-id="1ff9c-116">None.</span></span> |

<span data-ttu-id="1ff9c-117">Дополнительные разрешения не являются обязательными для вызова этого API, если ваше приложение имеет действительный маркер доступа для вызова Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="1ff9c-117">Additional permissions are not required to call this API, as long as your application has a valid access token to call Microsoft Graph.</span></span>

## <a name="http-request"></a><span data-ttu-id="1ff9c-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1ff9c-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /applicationTemplates/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1ff9c-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="1ff9c-119">Optional query parameters</span></span>

<span data-ttu-id="1ff9c-120">`$select`С помощью параметра запроса можно указать только те свойства, которые необходимы для достижения максимальной производительности.</span><span class="sxs-lookup"><span data-stu-id="1ff9c-120">You can use a `$select` query parameter to specify only the properties you need for best performance.</span></span> <span data-ttu-id="1ff9c-121">Свойство **id** возвращается всегда.</span><span class="sxs-lookup"><span data-stu-id="1ff9c-121">The **id** property is always returned.</span></span> 

<span data-ttu-id="1ff9c-122">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="1ff9c-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="1ff9c-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1ff9c-123">Request headers</span></span>

| <span data-ttu-id="1ff9c-124">Имя</span><span class="sxs-lookup"><span data-stu-id="1ff9c-124">Name</span></span>      |<span data-ttu-id="1ff9c-125">Описание</span><span class="sxs-lookup"><span data-stu-id="1ff9c-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="1ff9c-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1ff9c-126">Authorization</span></span> | <span data-ttu-id="1ff9c-127">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="1ff9c-127">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="1ff9c-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1ff9c-128">Request body</span></span>

<span data-ttu-id="1ff9c-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1ff9c-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1ff9c-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="1ff9c-130">Response</span></span>

<span data-ttu-id="1ff9c-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и запрошенный объект [аппликатионтемплате](../resources/applicationtemplate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1ff9c-131">If successful, this method returns a `200 OK` response code and the requested [applicationTemplate](../resources/applicationtemplate.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1ff9c-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="1ff9c-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1ff9c-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="1ff9c-133">Request</span></span>

<span data-ttu-id="1ff9c-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1ff9c-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1ff9c-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="1ff9c-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_applicationtemplate"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/applicationTemplates/{id}
```
# <a name="c"></a>[<span data-ttu-id="1ff9c-136">C#</span><span class="sxs-lookup"><span data-stu-id="1ff9c-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-applicationtemplate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1ff9c-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1ff9c-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-applicationtemplate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1ff9c-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1ff9c-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-applicationtemplate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1ff9c-139">Java</span><span class="sxs-lookup"><span data-stu-id="1ff9c-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-applicationtemplate-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="1ff9c-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="1ff9c-140">Response</span></span>

<span data-ttu-id="1ff9c-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="1ff9c-141">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="1ff9c-142">Объект Response, показанный здесь, может быть укорочен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="1ff9c-142">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="1ff9c-143">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1ff9c-143">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.applicationTemplate"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id" : "id-value",
    "displayName" : "displayName-value",
    "homePageUrl" : "homePageUrl-value",
    "supportedSingleSignOnModes" : ["supportedSingleSignOnModes-value"],
    "logoUrl" : "logoUrl-value",
    "categories" : ["categories-value"],
    "publisher" : "publisher-value",
    "description" : "description-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get applicationTemplate",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->



---
title: Получение Аппликатионтемплате
description: Получение свойств и связей объекта аппликатионтемплате.
localization_priority: Normal
author: luleonpla
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: fbf38412fc6442ffcc0a7037e2a1dcde30a35469
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42441405"
---
# <a name="get-applicationtemplate"></a><span data-ttu-id="329c8-103">Получение Аппликатионтемплате</span><span class="sxs-lookup"><span data-stu-id="329c8-103">Get applicationTemplate</span></span>

<span data-ttu-id="329c8-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="329c8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="329c8-105">Получение свойств объекта [аппликатионтемплате](../resources/applicationtemplate.md) .</span><span class="sxs-lookup"><span data-stu-id="329c8-105">Retrieve the properties of an [applicationTemplate](../resources/applicationtemplate.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="329c8-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="329c8-106">Permissions</span></span>

<span data-ttu-id="329c8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="329c8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="329c8-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="329c8-109">Permission type</span></span>                        | <span data-ttu-id="329c8-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="329c8-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="329c8-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="329c8-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="329c8-112">Нет.</span><span class="sxs-lookup"><span data-stu-id="329c8-112">None.</span></span> |
| <span data-ttu-id="329c8-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="329c8-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="329c8-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="329c8-114">Not supported.</span></span> |
| <span data-ttu-id="329c8-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="329c8-115">Application</span></span>                            | <span data-ttu-id="329c8-116">Нет.</span><span class="sxs-lookup"><span data-stu-id="329c8-116">None.</span></span> |

<span data-ttu-id="329c8-117">Дополнительные разрешения не являются обязательными для вызова этого API, если ваше приложение имеет действительный маркер доступа для вызова Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="329c8-117">Additional permissions are not required to call this API, as long as your application has a valid access token to call Microsoft Graph.</span></span>

## <a name="http-request"></a><span data-ttu-id="329c8-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="329c8-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /applicationTemplates/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="329c8-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="329c8-119">Optional query parameters</span></span>

<span data-ttu-id="329c8-120">С помощью параметра `$select` запроса можно указать только те свойства, которые необходимы для достижения максимальной производительности.</span><span class="sxs-lookup"><span data-stu-id="329c8-120">You can use a `$select` query parameter to specify only the properties you need for best performance.</span></span> <span data-ttu-id="329c8-121">Свойство **id** возвращается всегда.</span><span class="sxs-lookup"><span data-stu-id="329c8-121">The **id** property is always returned.</span></span> 

<span data-ttu-id="329c8-122">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="329c8-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="329c8-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="329c8-123">Request headers</span></span>

| <span data-ttu-id="329c8-124">Имя</span><span class="sxs-lookup"><span data-stu-id="329c8-124">Name</span></span>      |<span data-ttu-id="329c8-125">Описание</span><span class="sxs-lookup"><span data-stu-id="329c8-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="329c8-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="329c8-126">Authorization</span></span> | <span data-ttu-id="329c8-127">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="329c8-127">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="329c8-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="329c8-128">Request body</span></span>

<span data-ttu-id="329c8-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="329c8-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="329c8-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="329c8-130">Response</span></span>

<span data-ttu-id="329c8-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и запрошенный объект [аппликатионтемплате](../resources/applicationtemplate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="329c8-131">If successful, this method returns a `200 OK` response code and the requested [applicationTemplate](../resources/applicationtemplate.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="329c8-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="329c8-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="329c8-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="329c8-133">Request</span></span>

<span data-ttu-id="329c8-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="329c8-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="329c8-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="329c8-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_applicationtemplate"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/applicationTemplates/{id}
```
# <a name="c"></a>[<span data-ttu-id="329c8-136">C#</span><span class="sxs-lookup"><span data-stu-id="329c8-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-applicationtemplate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="329c8-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="329c8-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-applicationtemplate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="329c8-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="329c8-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-applicationtemplate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="329c8-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="329c8-139">Response</span></span>

<span data-ttu-id="329c8-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="329c8-140">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="329c8-141">Объект Response, показанный здесь, может быть укорочен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="329c8-141">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="329c8-142">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="329c8-142">All the properties will be returned from an actual call.</span></span>

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

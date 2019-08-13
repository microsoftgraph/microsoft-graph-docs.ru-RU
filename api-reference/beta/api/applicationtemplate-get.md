---
title: Получение Аппликатионтемплате
description: Получение свойств и связей объекта аппликатионтемплате.
localization_priority: Normal
author: luleonpla
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: e32439d98961a95ef98113f86833eec2c38dc869
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36318644"
---
# <a name="get-applicationtemplate"></a><span data-ttu-id="c9e6f-103">Получение Аппликатионтемплате</span><span class="sxs-lookup"><span data-stu-id="c9e6f-103">Get applicationTemplate</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c9e6f-104">Получение свойств объекта [аппликатионтемплате](../resources/applicationtemplate.md) .</span><span class="sxs-lookup"><span data-stu-id="c9e6f-104">Retrieve the properties of an [applicationTemplate](../resources/applicationtemplate.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="c9e6f-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c9e6f-105">Permissions</span></span>

<span data-ttu-id="c9e6f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c9e6f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c9e6f-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c9e6f-108">Permission type</span></span>                        | <span data-ttu-id="c9e6f-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c9e6f-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="c9e6f-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c9e6f-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="c9e6f-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="c9e6f-111">None.</span></span> |
| <span data-ttu-id="c9e6f-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c9e6f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c9e6f-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c9e6f-113">Not supported.</span></span> |
| <span data-ttu-id="c9e6f-114">Приложение</span><span class="sxs-lookup"><span data-stu-id="c9e6f-114">Application</span></span>                            | <span data-ttu-id="c9e6f-115">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="c9e6f-115">None.</span></span> |

<span data-ttu-id="c9e6f-116">Дополнительные разрешения не являются обязательными для вызова этого API, если ваше приложение имеет действительный маркер доступа для вызова Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="c9e6f-116">Additional permissions are not required to call this API, as long as your application has a valid access token to call Microsoft Graph.</span></span>

## <a name="http-request"></a><span data-ttu-id="c9e6f-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c9e6f-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /applicationTemplates/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c9e6f-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="c9e6f-118">Optional query parameters</span></span>

<span data-ttu-id="c9e6f-119">С помощью параметра `$select` запроса можно указать только те свойства, которые необходимы для достижения максимальной производительности.</span><span class="sxs-lookup"><span data-stu-id="c9e6f-119">You can use a `$select` query parameter to specify only the properties you need for best performance.</span></span> <span data-ttu-id="c9e6f-120">Свойство **id** возвращается всегда.</span><span class="sxs-lookup"><span data-stu-id="c9e6f-120">The **id** property is always returned.</span></span> 

<span data-ttu-id="c9e6f-121">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="c9e6f-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="c9e6f-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c9e6f-122">Request headers</span></span>

| <span data-ttu-id="c9e6f-123">Имя</span><span class="sxs-lookup"><span data-stu-id="c9e6f-123">Name</span></span>      |<span data-ttu-id="c9e6f-124">Описание</span><span class="sxs-lookup"><span data-stu-id="c9e6f-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c9e6f-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c9e6f-125">Authorization</span></span> | <span data-ttu-id="c9e6f-126">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="c9e6f-126">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="c9e6f-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c9e6f-127">Request body</span></span>

<span data-ttu-id="c9e6f-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c9e6f-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c9e6f-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="c9e6f-129">Response</span></span>

<span data-ttu-id="c9e6f-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и запрошенный объект [аппликатионтемплате](../resources/applicationtemplate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c9e6f-130">If successful, this method returns a `200 OK` response code and the requested [applicationTemplate](../resources/applicationtemplate.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c9e6f-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="c9e6f-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c9e6f-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="c9e6f-132">Request</span></span>

<span data-ttu-id="c9e6f-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c9e6f-133">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="c9e6f-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="c9e6f-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_applicationtemplate"
}-->

```http
GET https://graph.microsoft.com/beta/applicationTemplates/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c9e6f-135">C#</span><span class="sxs-lookup"><span data-stu-id="c9e6f-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-applicationtemplate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c9e6f-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c9e6f-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-applicationtemplate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c9e6f-137">Цель — C</span><span class="sxs-lookup"><span data-stu-id="c9e6f-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-applicationtemplate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="c9e6f-138">Java</span><span class="sxs-lookup"><span data-stu-id="c9e6f-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-applicationtemplate-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="c9e6f-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="c9e6f-139">Response</span></span>

<span data-ttu-id="c9e6f-140">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="c9e6f-140">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="c9e6f-141">Объект Response, показанный здесь, может быть укорочен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="c9e6f-141">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="c9e6f-142">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c9e6f-142">All the properties will be returned from an actual call.</span></span>

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

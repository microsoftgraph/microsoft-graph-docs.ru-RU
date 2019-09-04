---
title: Получение Аппликатионтемплате
description: Получение свойств и связей объекта аппликатионтемплате.
localization_priority: Normal
author: luleonpla
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 3433d4a5c112a4474942cdad0b0543653c79e4e2
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/04/2019
ms.locfileid: "36719005"
---
# <a name="get-applicationtemplate"></a><span data-ttu-id="53529-103">Получение Аппликатионтемплате</span><span class="sxs-lookup"><span data-stu-id="53529-103">Get applicationTemplate</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="53529-104">Получение свойств объекта [аппликатионтемплате](../resources/applicationtemplate.md) .</span><span class="sxs-lookup"><span data-stu-id="53529-104">Retrieve the properties of an [applicationTemplate](../resources/applicationtemplate.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="53529-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="53529-105">Permissions</span></span>

<span data-ttu-id="53529-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="53529-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="53529-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="53529-108">Permission type</span></span>                        | <span data-ttu-id="53529-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="53529-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="53529-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="53529-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="53529-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="53529-111">None.</span></span> |
| <span data-ttu-id="53529-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="53529-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="53529-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="53529-113">Not supported.</span></span> |
| <span data-ttu-id="53529-114">Приложение</span><span class="sxs-lookup"><span data-stu-id="53529-114">Application</span></span>                            | <span data-ttu-id="53529-115">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="53529-115">None.</span></span> |

<span data-ttu-id="53529-116">Дополнительные разрешения не являются обязательными для вызова этого API, если ваше приложение имеет действительный маркер доступа для вызова Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="53529-116">Additional permissions are not required to call this API, as long as your application has a valid access token to call Microsoft Graph.</span></span>

## <a name="http-request"></a><span data-ttu-id="53529-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="53529-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /applicationTemplates/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="53529-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="53529-118">Optional query parameters</span></span>

<span data-ttu-id="53529-119">С помощью параметра `$select` запроса можно указать только те свойства, которые необходимы для достижения максимальной производительности.</span><span class="sxs-lookup"><span data-stu-id="53529-119">You can use a `$select` query parameter to specify only the properties you need for best performance.</span></span> <span data-ttu-id="53529-120">Свойство **id** возвращается всегда.</span><span class="sxs-lookup"><span data-stu-id="53529-120">The **id** property is always returned.</span></span> 

<span data-ttu-id="53529-121">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="53529-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="53529-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="53529-122">Request headers</span></span>

| <span data-ttu-id="53529-123">Имя</span><span class="sxs-lookup"><span data-stu-id="53529-123">Name</span></span>      |<span data-ttu-id="53529-124">Описание</span><span class="sxs-lookup"><span data-stu-id="53529-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="53529-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="53529-125">Authorization</span></span> | <span data-ttu-id="53529-126">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="53529-126">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="53529-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="53529-127">Request body</span></span>

<span data-ttu-id="53529-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="53529-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="53529-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="53529-129">Response</span></span>

<span data-ttu-id="53529-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и запрошенный объект [аппликатионтемплате](../resources/applicationtemplate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="53529-130">If successful, this method returns a `200 OK` response code and the requested [applicationTemplate](../resources/applicationtemplate.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="53529-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="53529-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="53529-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="53529-132">Request</span></span>

<span data-ttu-id="53529-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="53529-133">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="53529-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="53529-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_applicationtemplate"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/applicationTemplates/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="53529-135">C#</span><span class="sxs-lookup"><span data-stu-id="53529-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-applicationtemplate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="53529-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="53529-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-applicationtemplate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="53529-137">Цель — C</span><span class="sxs-lookup"><span data-stu-id="53529-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-applicationtemplate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="53529-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="53529-138">Response</span></span>

<span data-ttu-id="53529-139">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="53529-139">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="53529-140">Объект Response, показанный здесь, может быть укорочен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="53529-140">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="53529-141">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="53529-141">All the properties will be returned from an actual call.</span></span>

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

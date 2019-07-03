---
title: Получение Аппликатионтемплате
description: Получение свойств и связей объекта аппликатионтемплате.
localization_priority: Normal
author: luleonpla
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 498eaf8b33916cbaa493f211dab8b99889e14a59
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35439541"
---
# <a name="get-applicationtemplate"></a><span data-ttu-id="982b0-103">Получение Аппликатионтемплате</span><span class="sxs-lookup"><span data-stu-id="982b0-103">Get applicationTemplate</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="982b0-104">Получение свойств объекта [аппликатионтемплате](../resources/applicationtemplate.md) .</span><span class="sxs-lookup"><span data-stu-id="982b0-104">Retrieve the properties of an [applicationTemplate](../resources/applicationtemplate.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="982b0-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="982b0-105">Permissions</span></span>

<span data-ttu-id="982b0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="982b0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="982b0-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="982b0-108">Permission type</span></span>                        | <span data-ttu-id="982b0-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="982b0-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="982b0-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="982b0-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="982b0-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="982b0-111">None.</span></span> |
| <span data-ttu-id="982b0-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="982b0-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="982b0-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="982b0-113">Not supported.</span></span> |
| <span data-ttu-id="982b0-114">Приложение</span><span class="sxs-lookup"><span data-stu-id="982b0-114">Application</span></span>                            | <span data-ttu-id="982b0-115">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="982b0-115">None.</span></span> |

<span data-ttu-id="982b0-116">Дополнительные разрешения не являются обязательными для вызова этого API, если ваше приложение имеет действительный маркер доступа для вызова Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="982b0-116">Additional permissions are not required to call this API, as long as your application has a valid access token to call Microsoft Graph.</span></span>

## <a name="http-request"></a><span data-ttu-id="982b0-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="982b0-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /applicationTemplates/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="982b0-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="982b0-118">Optional query parameters</span></span>

<span data-ttu-id="982b0-119">С помощью параметра `$select` запроса можно указать только те свойства, которые необходимы для достижения максимальной производительности.</span><span class="sxs-lookup"><span data-stu-id="982b0-119">You can use a `$select` query parameter to specify only the properties you need for best performance.</span></span> <span data-ttu-id="982b0-120">Свойство **id** возвращается всегда.</span><span class="sxs-lookup"><span data-stu-id="982b0-120">The **id** property is always returned.</span></span> 

<span data-ttu-id="982b0-121">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="982b0-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="982b0-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="982b0-122">Request headers</span></span>

| <span data-ttu-id="982b0-123">Имя</span><span class="sxs-lookup"><span data-stu-id="982b0-123">Name</span></span>      |<span data-ttu-id="982b0-124">Описание</span><span class="sxs-lookup"><span data-stu-id="982b0-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="982b0-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="982b0-125">Authorization</span></span> | <span data-ttu-id="982b0-126">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="982b0-126">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="982b0-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="982b0-127">Request body</span></span>

<span data-ttu-id="982b0-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="982b0-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="982b0-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="982b0-129">Response</span></span>

<span data-ttu-id="982b0-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и запрошенный объект [аппликатионтемплате](../resources/applicationtemplate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="982b0-130">If successful, this method returns a `200 OK` response code and the requested [applicationTemplate](../resources/applicationtemplate.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="982b0-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="982b0-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="982b0-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="982b0-132">Request</span></span>

<span data-ttu-id="982b0-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="982b0-133">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="982b0-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="982b0-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_applicationtemplate"
}-->

```http
GET https://graph.microsoft.com/beta/applicationTemplates/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="982b0-135">C#</span><span class="sxs-lookup"><span data-stu-id="982b0-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-applicationtemplate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="982b0-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="982b0-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-applicationtemplate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="982b0-137">Цель — C</span><span class="sxs-lookup"><span data-stu-id="982b0-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-applicationtemplate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="982b0-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="982b0-138">Response</span></span>

<span data-ttu-id="982b0-139">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="982b0-139">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="982b0-140">Объект Response, показанный здесь, может быть укорочен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="982b0-140">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="982b0-141">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="982b0-141">All the properties will be returned from an actual call.</span></span>

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

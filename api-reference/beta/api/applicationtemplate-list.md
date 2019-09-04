---
title: Список Аппликатионтемплатес
description: Получение списка объектов аппликатионтемплате.
localization_priority: Normal
author: luleonpla
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: ca603ac58cd5136d8ef4f5da77727380cd27c609
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/04/2019
ms.locfileid: "36718984"
---
# <a name="list-applicationtemplates"></a><span data-ttu-id="86929-103">Список Аппликатионтемплатес</span><span class="sxs-lookup"><span data-stu-id="86929-103">List applicationTemplates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="86929-104">Получение списка объектов [аппликатионтемплате](../resources/applicationtemplate.md) из коллекции приложений Azure AD.</span><span class="sxs-lookup"><span data-stu-id="86929-104">Retrieve a list of [applicationTemplate](../resources/applicationtemplate.md) objects from the Azure AD application gallery.</span></span>

## <a name="permissions"></a><span data-ttu-id="86929-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="86929-105">Permissions</span></span>

<span data-ttu-id="86929-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="86929-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="86929-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="86929-108">Permission type</span></span>                        | <span data-ttu-id="86929-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="86929-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="86929-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="86929-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="86929-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="86929-111">None.</span></span> |
| <span data-ttu-id="86929-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="86929-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="86929-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="86929-113">Not supported.</span></span> |
| <span data-ttu-id="86929-114">Приложение</span><span class="sxs-lookup"><span data-stu-id="86929-114">Application</span></span>                            | <span data-ttu-id="86929-115">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="86929-115">None.</span></span> |

<span data-ttu-id="86929-116">Дополнительные разрешения не являются обязательными для вызова этого API, если ваше приложение имеет действительный маркер доступа для вызова Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="86929-116">Additional permissions are not required to call this API, as long as your application has a valid access token to call Microsoft Graph.</span></span>

## <a name="http-request"></a><span data-ttu-id="86929-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="86929-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /applicationTemplates
```

## <a name="optional-query-parameters"></a><span data-ttu-id="86929-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="86929-118">Optional query parameters</span></span>

<span data-ttu-id="86929-119">Этот метод поддерживает некоторые параметры запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="86929-119">This method supports some of the OData query parameters to help customize the response.</span></span> 

- <span data-ttu-id="86929-120">Вы можете использовать этот `$filter` параметр ограниченное количеством способов.</span><span class="sxs-lookup"><span data-stu-id="86929-120">You can use the `$filter` parameter in a limited way.</span></span> <span data-ttu-id="86929-121">Фильтровать можно только по **DisplayName** или **категориям**.</span><span class="sxs-lookup"><span data-stu-id="86929-121">You can only filter by **displayName** or **categories**.</span></span> <span data-ttu-id="86929-122">Пример:  `$filter=contains(displayName, 'salesf')` или `$filter=categories/any(c:contains(c, 'myCategory'))`.</span><span class="sxs-lookup"><span data-stu-id="86929-122">For example,  `$filter=contains(displayName, 'salesf')` or `$filter=categories/any(c:contains(c, 'myCategory'))`.</span></span>
- <span data-ttu-id="86929-123">Вы можете использовать `$orderby` `$top,` и `$skip` запрос параметров в любом запросе GET.</span><span class="sxs-lookup"><span data-stu-id="86929-123">You can use `$orderby`, `$top,` and `$skip` query parameters in any GET request.</span></span>

<span data-ttu-id="86929-124">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="86929-124">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="86929-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="86929-125">Request headers</span></span>

| <span data-ttu-id="86929-126">Имя</span><span class="sxs-lookup"><span data-stu-id="86929-126">Name</span></span>      |<span data-ttu-id="86929-127">Описание</span><span class="sxs-lookup"><span data-stu-id="86929-127">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="86929-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="86929-128">Authorization</span></span> | <span data-ttu-id="86929-129">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="86929-129">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="86929-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="86929-130">Request body</span></span>

<span data-ttu-id="86929-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="86929-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="86929-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="86929-132">Response</span></span>

<span data-ttu-id="86929-133">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [аппликатионтемплате](../resources/applicationtemplate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="86929-133">If successful, this method returns a `200 OK` response code and a collection of [applicationTemplate](../resources/applicationtemplate.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="86929-134">Примеры</span><span class="sxs-lookup"><span data-stu-id="86929-134">Examples</span></span>

### <a name="request"></a><span data-ttu-id="86929-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="86929-135">Request</span></span>

<span data-ttu-id="86929-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="86929-136">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="86929-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="86929-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_applicationtemplates"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/applicationTemplates
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="86929-138">C#</span><span class="sxs-lookup"><span data-stu-id="86929-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-applicationtemplates-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="86929-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="86929-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-applicationtemplates-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="86929-140">Цель — C</span><span class="sxs-lookup"><span data-stu-id="86929-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-applicationtemplates-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="86929-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="86929-141">Response</span></span>

<span data-ttu-id="86929-142">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="86929-142">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="86929-143">Объект Response, показанный здесь, может быть укорочен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="86929-143">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="86929-144">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="86929-144">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.applicationTemplate",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
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
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List applicationTemplates",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

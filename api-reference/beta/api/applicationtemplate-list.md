---
title: Список Аппликатионтемплатес
description: Получение списка объектов аппликатионтемплате.
localization_priority: Normal
author: luleonpla
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 5df0ee457464e766fd2581bcb9440039029fc58a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47996656"
---
# <a name="list-applicationtemplates"></a><span data-ttu-id="aedfa-103">Список Аппликатионтемплатес</span><span class="sxs-lookup"><span data-stu-id="aedfa-103">List applicationTemplates</span></span>

<span data-ttu-id="aedfa-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aedfa-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aedfa-105">Получение списка объектов [аппликатионтемплате](../resources/applicationtemplate.md) из коллекции приложений Azure AD.</span><span class="sxs-lookup"><span data-stu-id="aedfa-105">Retrieve a list of [applicationTemplate](../resources/applicationtemplate.md) objects from the Azure AD application gallery.</span></span>

## <a name="permissions"></a><span data-ttu-id="aedfa-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="aedfa-106">Permissions</span></span>

<span data-ttu-id="aedfa-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aedfa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="aedfa-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="aedfa-109">Permission type</span></span>                        | <span data-ttu-id="aedfa-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="aedfa-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="aedfa-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="aedfa-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="aedfa-112">Нет.</span><span class="sxs-lookup"><span data-stu-id="aedfa-112">None.</span></span> |
| <span data-ttu-id="aedfa-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="aedfa-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="aedfa-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aedfa-114">Not supported.</span></span> |
| <span data-ttu-id="aedfa-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="aedfa-115">Application</span></span>                            | <span data-ttu-id="aedfa-116">Нет.</span><span class="sxs-lookup"><span data-stu-id="aedfa-116">None.</span></span> |

<span data-ttu-id="aedfa-117">Дополнительные разрешения не являются обязательными для вызова этого API, если ваше приложение имеет действительный маркер доступа для вызова Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="aedfa-117">Additional permissions are not required to call this API, as long as your application has a valid access token to call Microsoft Graph.</span></span>

## <a name="http-request"></a><span data-ttu-id="aedfa-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="aedfa-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /applicationTemplates
```

## <a name="optional-query-parameters"></a><span data-ttu-id="aedfa-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="aedfa-119">Optional query parameters</span></span>

<span data-ttu-id="aedfa-120">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="aedfa-120">This method supports some of the OData query parameters to help customize the response.</span></span> 

- <span data-ttu-id="aedfa-121">Вы можете использовать этот `$filter` параметр ограниченное количеством способов.</span><span class="sxs-lookup"><span data-stu-id="aedfa-121">You can use the `$filter` parameter in a limited way.</span></span> <span data-ttu-id="aedfa-122">Фильтровать можно только по **DisplayName** или **категориям**.</span><span class="sxs-lookup"><span data-stu-id="aedfa-122">You can only filter by **displayName** or **categories**.</span></span> <span data-ttu-id="aedfa-123">Пример:  `$filter=contains(displayName, 'salesf')` или `$filter=categories/any(c:contains(c, 'myCategory'))`.</span><span class="sxs-lookup"><span data-stu-id="aedfa-123">For example,  `$filter=contains(displayName, 'salesf')` or `$filter=categories/any(c:contains(c, 'myCategory'))`.</span></span>
- <span data-ttu-id="aedfa-124">Вы можете использовать `$orderby` `$top,` и `$skip` запрос параметров в любом запросе GET.</span><span class="sxs-lookup"><span data-stu-id="aedfa-124">You can use `$orderby`, `$top,` and `$skip` query parameters in any GET request.</span></span>

<span data-ttu-id="aedfa-125">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="aedfa-125">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="aedfa-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="aedfa-126">Request headers</span></span>

| <span data-ttu-id="aedfa-127">Имя</span><span class="sxs-lookup"><span data-stu-id="aedfa-127">Name</span></span>      |<span data-ttu-id="aedfa-128">Описание</span><span class="sxs-lookup"><span data-stu-id="aedfa-128">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="aedfa-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="aedfa-129">Authorization</span></span> | <span data-ttu-id="aedfa-130">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="aedfa-130">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="aedfa-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="aedfa-131">Request body</span></span>

<span data-ttu-id="aedfa-132">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="aedfa-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="aedfa-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="aedfa-133">Response</span></span>

<span data-ttu-id="aedfa-134">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [аппликатионтемплате](../resources/applicationtemplate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="aedfa-134">If successful, this method returns a `200 OK` response code and a collection of [applicationTemplate](../resources/applicationtemplate.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="aedfa-135">Примеры</span><span class="sxs-lookup"><span data-stu-id="aedfa-135">Examples</span></span>

### <a name="request"></a><span data-ttu-id="aedfa-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="aedfa-136">Request</span></span>

<span data-ttu-id="aedfa-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="aedfa-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="aedfa-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="aedfa-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_applicationtemplates"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/applicationTemplates
```
# <a name="c"></a>[<span data-ttu-id="aedfa-139">C#</span><span class="sxs-lookup"><span data-stu-id="aedfa-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-applicationtemplates-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="aedfa-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="aedfa-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-applicationtemplates-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="aedfa-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="aedfa-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-applicationtemplates-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="aedfa-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="aedfa-142">Response</span></span>

<span data-ttu-id="aedfa-143">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="aedfa-143">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="aedfa-144">Объект Response, показанный здесь, может быть укорочен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="aedfa-144">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="aedfa-145">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="aedfa-145">All the properties will be returned from an actual call.</span></span>

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



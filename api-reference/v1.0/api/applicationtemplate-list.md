---
title: List applicationTemplates
description: Получение списка объектов applicationtemplate.
localization_priority: Normal
author: luleonpla
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 7d8a80b6f2cee8726f50cf32a7c5c6efa5e947c6
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50775146"
---
# <a name="list-applicationtemplates"></a><span data-ttu-id="d11be-103">List applicationTemplates</span><span class="sxs-lookup"><span data-stu-id="d11be-103">List applicationTemplates</span></span>

<span data-ttu-id="d11be-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d11be-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d11be-105">Получение списка объектов [applicationTemplate](../resources/applicationtemplate.md) из галереи приложений Azure AD.</span><span class="sxs-lookup"><span data-stu-id="d11be-105">Retrieve a list of [applicationTemplate](../resources/applicationtemplate.md) objects from the Azure AD application gallery.</span></span>

## <a name="permissions"></a><span data-ttu-id="d11be-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d11be-106">Permissions</span></span>

<span data-ttu-id="d11be-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d11be-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d11be-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d11be-109">Permission type</span></span>                        | <span data-ttu-id="d11be-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d11be-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="d11be-111">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d11be-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="d11be-112">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="d11be-112">None.</span></span>                                       |
| <span data-ttu-id="d11be-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d11be-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d11be-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d11be-114">Not supported.</span></span>                              |
| <span data-ttu-id="d11be-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="d11be-115">Application</span></span>                            | <span data-ttu-id="d11be-116">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="d11be-116">None.</span></span>                                       |

<span data-ttu-id="d11be-117">Дополнительные разрешения не требуются для вызова этого API, если приложение имеет допустимый маркер доступа для вызова Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="d11be-117">Additional permissions are not required to call this API, as long as your application has a valid access token to call Microsoft Graph.</span></span>

## <a name="http-request"></a><span data-ttu-id="d11be-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d11be-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /applicationTemplates
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d11be-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="d11be-119">Optional query parameters</span></span>

<span data-ttu-id="d11be-120">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="d11be-120">This method supports some of the OData query parameters to help customize the response.</span></span>

- <span data-ttu-id="d11be-121">Параметр можно `$filter` использовать ограниченным способом.</span><span class="sxs-lookup"><span data-stu-id="d11be-121">You can use the `$filter` parameter in a limited way.</span></span> <span data-ttu-id="d11be-122">Фильтровать можно только **по displayName** или **категориям.**</span><span class="sxs-lookup"><span data-stu-id="d11be-122">You can only filter by **displayName** or **categories**.</span></span> <span data-ttu-id="d11be-123">Например, `$filter=contains(displayName, 'salesf')` или `$filter=categories/any(c:contains(c, 'myCategory'))`.</span><span class="sxs-lookup"><span data-stu-id="d11be-123">For example, `$filter=contains(displayName, 'salesf')` or `$filter=categories/any(c:contains(c, 'myCategory'))`.</span></span>
- <span data-ttu-id="d11be-124">Параметры `$orderby` запроса и `$top,` `$skip` запроса можно использовать в любом запросе GET.</span><span class="sxs-lookup"><span data-stu-id="d11be-124">You can use `$orderby`, `$top,` and `$skip` query parameters in any GET request.</span></span>

<span data-ttu-id="d11be-125">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="d11be-125">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="d11be-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d11be-126">Request headers</span></span>

| <span data-ttu-id="d11be-127">Имя</span><span class="sxs-lookup"><span data-stu-id="d11be-127">Name</span></span>          | <span data-ttu-id="d11be-128">Описание</span><span class="sxs-lookup"><span data-stu-id="d11be-128">Description</span></span>   |
| :------------ | :------------ |
| <span data-ttu-id="d11be-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d11be-129">Authorization</span></span> | <span data-ttu-id="d11be-130">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="d11be-130">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="d11be-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d11be-131">Request body</span></span>

<span data-ttu-id="d11be-132">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d11be-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d11be-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="d11be-133">Response</span></span>

<span data-ttu-id="d11be-134">В случае успешного применения этот метод возвращает код отклика и коллекцию `200 OK` [объектов applicationTemplate](../resources/applicationtemplate.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="d11be-134">If successful, this method returns a `200 OK` response code and a collection of [applicationTemplate](../resources/applicationtemplate.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d11be-135">Примеры</span><span class="sxs-lookup"><span data-stu-id="d11be-135">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d11be-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="d11be-136">Request</span></span>

<span data-ttu-id="d11be-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d11be-137">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="d11be-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="d11be-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_applicationtemplates"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/applicationTemplates
```
# <a name="c"></a>[<span data-ttu-id="d11be-139">C#</span><span class="sxs-lookup"><span data-stu-id="d11be-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-applicationtemplates-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d11be-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d11be-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-applicationtemplates-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d11be-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d11be-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-applicationtemplates-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d11be-142">Java</span><span class="sxs-lookup"><span data-stu-id="d11be-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-applicationtemplates-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d11be-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="d11be-143">Response</span></span>

<span data-ttu-id="d11be-144">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="d11be-144">The following is an example of the response.</span></span>

> <span data-ttu-id="d11be-145">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="d11be-145">**Note:** The response object shown here might be shortened for readability.</span></span>

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

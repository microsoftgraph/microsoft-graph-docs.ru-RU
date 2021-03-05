---
title: List applicationTemplates
description: Получение списка объектов applicationtemplate.
localization_priority: Normal
author: luleonpla
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: ebd1b178ad1a6ea0e178ab582439ace433951ffb
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50471539"
---
# <a name="list-applicationtemplates"></a><span data-ttu-id="9c146-103">List applicationTemplates</span><span class="sxs-lookup"><span data-stu-id="9c146-103">List applicationTemplates</span></span>

<span data-ttu-id="9c146-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9c146-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9c146-105">Получение списка объектов [applicationTemplate](../resources/applicationtemplate.md) из галереи приложений Azure AD.</span><span class="sxs-lookup"><span data-stu-id="9c146-105">Retrieve a list of [applicationTemplate](../resources/applicationtemplate.md) objects from the Azure AD application gallery.</span></span>

## <a name="permissions"></a><span data-ttu-id="9c146-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9c146-106">Permissions</span></span>

<span data-ttu-id="9c146-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9c146-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9c146-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9c146-109">Permission type</span></span>                        | <span data-ttu-id="9c146-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9c146-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="9c146-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9c146-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="9c146-112">Нет.</span><span class="sxs-lookup"><span data-stu-id="9c146-112">None.</span></span> |
| <span data-ttu-id="9c146-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9c146-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9c146-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9c146-114">Not supported.</span></span> |
| <span data-ttu-id="9c146-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9c146-115">Application</span></span>                            | <span data-ttu-id="9c146-116">Нет.</span><span class="sxs-lookup"><span data-stu-id="9c146-116">None.</span></span> |

<span data-ttu-id="9c146-117">Дополнительные разрешения не требуются для вызова этого API, если приложение имеет допустимый маркер доступа для вызова Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="9c146-117">Additional permissions are not required to call this API, as long as your application has a valid access token to call Microsoft Graph.</span></span>

## <a name="http-request"></a><span data-ttu-id="9c146-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9c146-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /applicationTemplates
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9c146-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="9c146-119">Optional query parameters</span></span>

<span data-ttu-id="9c146-120">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="9c146-120">This method supports some of the OData query parameters to help customize the response.</span></span> 

- <span data-ttu-id="9c146-121">Параметр можно `$filter` использовать ограниченным способом.</span><span class="sxs-lookup"><span data-stu-id="9c146-121">You can use the `$filter` parameter in a limited way.</span></span> <span data-ttu-id="9c146-122">Фильтровать можно только **по displayName** или **категориям.**</span><span class="sxs-lookup"><span data-stu-id="9c146-122">You can only filter by **displayName** or **categories**.</span></span> <span data-ttu-id="9c146-123">Пример:  `$filter=contains(displayName, 'salesf')` или `$filter=categories/any(c:contains(c, 'myCategory'))`.</span><span class="sxs-lookup"><span data-stu-id="9c146-123">For example,  `$filter=contains(displayName, 'salesf')` or `$filter=categories/any(c:contains(c, 'myCategory'))`.</span></span>
- <span data-ttu-id="9c146-124">Параметры `$orderby` запроса и `$top,` `$skip` запроса можно использовать в любом запросе GET.</span><span class="sxs-lookup"><span data-stu-id="9c146-124">You can use `$orderby`, `$top,` and `$skip` query parameters in any GET request.</span></span>

<span data-ttu-id="9c146-125">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="9c146-125">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="9c146-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9c146-126">Request headers</span></span>

| <span data-ttu-id="9c146-127">Имя</span><span class="sxs-lookup"><span data-stu-id="9c146-127">Name</span></span>      |<span data-ttu-id="9c146-128">Описание</span><span class="sxs-lookup"><span data-stu-id="9c146-128">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="9c146-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9c146-129">Authorization</span></span> | <span data-ttu-id="9c146-130">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="9c146-130">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="9c146-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9c146-131">Request body</span></span>

<span data-ttu-id="9c146-132">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9c146-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9c146-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="9c146-133">Response</span></span>

<span data-ttu-id="9c146-134">В случае успешного применения этот метод возвращает код отклика и коллекцию `200 OK` [объектов applicationTemplate](../resources/applicationtemplate.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="9c146-134">If successful, this method returns a `200 OK` response code and a collection of [applicationTemplate](../resources/applicationtemplate.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9c146-135">Примеры</span><span class="sxs-lookup"><span data-stu-id="9c146-135">Examples</span></span>

### <a name="request"></a><span data-ttu-id="9c146-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="9c146-136">Request</span></span>

<span data-ttu-id="9c146-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9c146-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9c146-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="9c146-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_applicationtemplates"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/applicationTemplates
```
# <a name="c"></a>[<span data-ttu-id="9c146-139">C#</span><span class="sxs-lookup"><span data-stu-id="9c146-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-applicationtemplates-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9c146-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9c146-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-applicationtemplates-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9c146-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9c146-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-applicationtemplates-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9c146-142">Java</span><span class="sxs-lookup"><span data-stu-id="9c146-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-applicationtemplates-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="9c146-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="9c146-143">Response</span></span>

<span data-ttu-id="9c146-144">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="9c146-144">The following is an example of the response.</span></span>

> <span data-ttu-id="9c146-145">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="9c146-145">**Note:** The response object shown here might be shortened for readability.</span></span>

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




---
title: Получение applicationTemplate
description: Получение свойств и связей объекта applicationtemplate.
localization_priority: Normal
author: luleonpla
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 4ae3d9f451785ef44f36df75667968bc271065dc
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50471595"
---
# <a name="get-applicationtemplate"></a><span data-ttu-id="f10eb-103">Получение applicationTemplate</span><span class="sxs-lookup"><span data-stu-id="f10eb-103">Get applicationTemplate</span></span>

<span data-ttu-id="f10eb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f10eb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f10eb-105">Получение свойств объекта [applicationTemplate.](../resources/applicationtemplate.md)</span><span class="sxs-lookup"><span data-stu-id="f10eb-105">Retrieve the properties of an [applicationTemplate](../resources/applicationtemplate.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f10eb-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f10eb-106">Permissions</span></span>

<span data-ttu-id="f10eb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f10eb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f10eb-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f10eb-109">Permission type</span></span>                        | <span data-ttu-id="f10eb-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f10eb-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="f10eb-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f10eb-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="f10eb-112">Нет.</span><span class="sxs-lookup"><span data-stu-id="f10eb-112">None.</span></span> |
| <span data-ttu-id="f10eb-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f10eb-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f10eb-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f10eb-114">Not supported.</span></span> |
| <span data-ttu-id="f10eb-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f10eb-115">Application</span></span>                            | <span data-ttu-id="f10eb-116">Нет.</span><span class="sxs-lookup"><span data-stu-id="f10eb-116">None.</span></span> |

<span data-ttu-id="f10eb-117">Дополнительные разрешения не требуются для вызова этого API, если приложение имеет допустимый маркер доступа для вызова Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="f10eb-117">Additional permissions are not required to call this API, as long as your application has a valid access token to call Microsoft Graph.</span></span>

## <a name="http-request"></a><span data-ttu-id="f10eb-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f10eb-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /applicationTemplates/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f10eb-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="f10eb-119">Optional query parameters</span></span>

<span data-ttu-id="f10eb-120">Параметр запроса можно указать только свойства, необходимые `$select` для лучшей производительности.</span><span class="sxs-lookup"><span data-stu-id="f10eb-120">You can use a `$select` query parameter to specify only the properties you need for best performance.</span></span> <span data-ttu-id="f10eb-121">Свойство **id** возвращается всегда.</span><span class="sxs-lookup"><span data-stu-id="f10eb-121">The **id** property is always returned.</span></span> 

<span data-ttu-id="f10eb-122">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="f10eb-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="f10eb-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f10eb-123">Request headers</span></span>

| <span data-ttu-id="f10eb-124">Имя</span><span class="sxs-lookup"><span data-stu-id="f10eb-124">Name</span></span>      |<span data-ttu-id="f10eb-125">Описание</span><span class="sxs-lookup"><span data-stu-id="f10eb-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f10eb-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f10eb-126">Authorization</span></span> | <span data-ttu-id="f10eb-127">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="f10eb-127">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="f10eb-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f10eb-128">Request body</span></span>

<span data-ttu-id="f10eb-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f10eb-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f10eb-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="f10eb-130">Response</span></span>

<span data-ttu-id="f10eb-131">В случае успешного применения этот метод возвращает код ответа и запрашиваемого объекта `200 OK` [applicationTemplate](../resources/applicationtemplate.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="f10eb-131">If successful, this method returns a `200 OK` response code and the requested [applicationTemplate](../resources/applicationtemplate.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f10eb-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="f10eb-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f10eb-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="f10eb-133">Request</span></span>

<span data-ttu-id="f10eb-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f10eb-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f10eb-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="f10eb-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_applicationtemplate"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/applicationTemplates/{id}
```
# <a name="c"></a>[<span data-ttu-id="f10eb-136">C#</span><span class="sxs-lookup"><span data-stu-id="f10eb-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-applicationtemplate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f10eb-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f10eb-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-applicationtemplate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f10eb-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f10eb-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-applicationtemplate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f10eb-139">Java</span><span class="sxs-lookup"><span data-stu-id="f10eb-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-applicationtemplate-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f10eb-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="f10eb-140">Response</span></span>

<span data-ttu-id="f10eb-141">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="f10eb-141">The following is an example of the response.</span></span>

> <span data-ttu-id="f10eb-142">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="f10eb-142">**Note:** The response object shown here might be shortened for readability.</span></span> 

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




---
title: Получить термин
description: Ознакомьтесь с свойствами и отношениями объекта терминов.
author: mohitpcad
localization_priority: Normal
ms.prod: Sharepoint
doc_type: apiPageType
ms.openlocfilehash: d4f989b9ef5b1481c5e889a2cf1ea5fe41bc4ab0
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50958861"
---
# <a name="get-term"></a><span data-ttu-id="f6379-103">Получить термин</span><span class="sxs-lookup"><span data-stu-id="f6379-103">Get term</span></span>
<span data-ttu-id="f6379-104">Пространство имен: microsoft.graph.termStore</span><span class="sxs-lookup"><span data-stu-id="f6379-104">Namespace: microsoft.graph.termStore</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f6379-105">Ознакомьтесь с свойствами и отношениями объекта [терминов.](../resources/termstore-term.md)</span><span class="sxs-lookup"><span data-stu-id="f6379-105">Read the properties and relationships of a [term](../resources/termstore-term.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f6379-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f6379-106">Permissions</span></span>
<span data-ttu-id="f6379-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f6379-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f6379-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f6379-109">Permission type</span></span>|<span data-ttu-id="f6379-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f6379-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f6379-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f6379-111">Delegated (work or school account)</span></span> | <span data-ttu-id="f6379-112">TermStore.Read.All, TermStore.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f6379-112">TermStore.Read.All, TermStore.ReadWrite.All</span></span> |
|<span data-ttu-id="f6379-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f6379-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f6379-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f6379-114">Not supported.</span></span>    |
|<span data-ttu-id="f6379-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f6379-115">Application</span></span> | <span data-ttu-id="f6379-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f6379-116">Not supported.</span></span> |


## <a name="http-request"></a><span data-ttu-id="f6379-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f6379-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
} -->

``` http
GET /termStore/groups/{groupId}/sets/{setId}/terms/{termId}
GET /termStore/sets/{setId}/terms/{termId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f6379-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="f6379-118">Optional query parameters</span></span>
<span data-ttu-id="f6379-119">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="f6379-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="f6379-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="f6379-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="f6379-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f6379-121">Request headers</span></span>
|<span data-ttu-id="f6379-122">Имя</span><span class="sxs-lookup"><span data-stu-id="f6379-122">Name</span></span>|<span data-ttu-id="f6379-123">Описание</span><span class="sxs-lookup"><span data-stu-id="f6379-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="f6379-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f6379-124">Authorization</span></span>|<span data-ttu-id="f6379-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f6379-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f6379-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f6379-127">Request body</span></span>
<span data-ttu-id="f6379-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f6379-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f6379-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="f6379-129">Response</span></span>

<span data-ttu-id="f6379-130">В случае успешной работы этот метод возвращает код ответа и объект `200 OK` [терминов](../resources/termstore-term.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="f6379-130">If successful, this method returns a `200 OK` response code and a [term](../resources/termstore-term.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f6379-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="f6379-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f6379-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="f6379-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="f6379-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="f6379-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_term_1"
} -->

``` http
GET https://graph.microsoft.com/beta/termStore/groups/{groupId}/sets/{setId}/terms/{termId}
```
# <a name="c"></a>[<span data-ttu-id="f6379-134">C#</span><span class="sxs-lookup"><span data-stu-id="f6379-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-term-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f6379-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f6379-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-term-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f6379-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f6379-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-term-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f6379-137">Java</span><span class="sxs-lookup"><span data-stu-id="f6379-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-term-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="f6379-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="f6379-138">Response</span></span>
<span data-ttu-id="f6379-139">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="f6379-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.termStore.term"
} -->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "id": "81be9856-9856-81be-5698-be815698be81",
  "createdDateTime": "2019-06-21T20:01:37Z",
  "labels" : [
    {
        "name" : "Copy of myTerm",
        "languageTag" : "en-US",
        "isDefault" : true
    }
  ],
  "lastModifiedDateTime": "2019-06-21T20:01:37Z"
}
```

[microsoft.graph.termStore.term]: ../resources/termstore-term.md

<!--
{
  "type": "#page.annotation",
  "description": "Get term entity in termStore",
  "keywords": "term,termStore",
  "section": "documentation",
  "tocPath": "termStore/Get term",
  "suppressions": [
  ]
}
-->




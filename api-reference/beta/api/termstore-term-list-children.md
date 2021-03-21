---
title: Список дочерних элементов
description: Получите условия из свойства навигации для детей.
author: mohitpcad
ms.prod: Sharepoint
localization_priority: Normal
doc_type: apiPageType
ms.openlocfilehash: 6bc2ba250498d6d7ac51914e2f0c072a34fc9bfe
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50955393"
---
# <a name="list-children"></a><span data-ttu-id="238ea-103">Список дочерних элементов</span><span class="sxs-lookup"><span data-stu-id="238ea-103">List children</span></span>
<span data-ttu-id="238ea-104">Пространство имен: microsoft.graph.termStore</span><span class="sxs-lookup"><span data-stu-id="238ea-104">Namespace: microsoft.graph.termStore</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="238ea-105">Получите детей первого уровня набора [или] ресурса [терминов] с помощью свойства навигации для детей.</span><span class="sxs-lookup"><span data-stu-id="238ea-105">Get the first level children of a [set] or [term] resource using the children navigation property.</span></span>

## <a name="permissions"></a><span data-ttu-id="238ea-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="238ea-106">Permissions</span></span>
<span data-ttu-id="238ea-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="238ea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="238ea-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="238ea-109">Permission type</span></span>|<span data-ttu-id="238ea-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="238ea-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="238ea-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="238ea-111">Delegated (work or school account)</span></span> | <span data-ttu-id="238ea-112">TermStore.Read.All, TermStore.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="238ea-112">TermStore.Read.All, TermStore.ReadWrite.All</span></span> |
|<span data-ttu-id="238ea-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="238ea-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="238ea-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="238ea-114">Not supported.</span></span>    |
|<span data-ttu-id="238ea-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="238ea-115">Application</span></span> | <span data-ttu-id="238ea-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="238ea-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="238ea-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="238ea-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /termStore/sets/{setId}/children
GET /termStore/sets/{setId}/terms/{termId}/children
```

## <a name="optional-query-parameters"></a><span data-ttu-id="238ea-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="238ea-118">Optional query parameters</span></span>
<span data-ttu-id="238ea-119">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="238ea-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="238ea-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="238ea-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="238ea-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="238ea-121">Request headers</span></span>
|<span data-ttu-id="238ea-122">Имя</span><span class="sxs-lookup"><span data-stu-id="238ea-122">Name</span></span>|<span data-ttu-id="238ea-123">Описание</span><span class="sxs-lookup"><span data-stu-id="238ea-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="238ea-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="238ea-124">Authorization</span></span>|<span data-ttu-id="238ea-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="238ea-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="238ea-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="238ea-127">Request body</span></span>
<span data-ttu-id="238ea-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="238ea-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="238ea-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="238ea-129">Response</span></span>

<span data-ttu-id="238ea-130">В случае успешной работы этот метод возвращает код отклика и `200 OK` набор терминов в тексте ответа. [](../resources/termstore-term.md)</span><span class="sxs-lookup"><span data-stu-id="238ea-130">If successful, this method returns a `200 OK` response code and a collection of [term](../resources/termstore-term.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="238ea-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="238ea-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="238ea-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="238ea-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="238ea-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="238ea-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_term_2"
}-->

``` http
GET https://graph.microsoft.com/beta/termStore/sets/{setId}/children
```
# <a name="c"></a>[<span data-ttu-id="238ea-134">C#</span><span class="sxs-lookup"><span data-stu-id="238ea-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-term-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="238ea-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="238ea-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-term-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="238ea-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="238ea-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-term-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="238ea-137">Java</span><span class="sxs-lookup"><span data-stu-id="238ea-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-term-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="238ea-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="238ea-138">Response</span></span>
<span data-ttu-id="238ea-139">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="238ea-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.termStore.term)"
}-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {      
      "id": "81be9856-9856-81be-5698-be815698be81",
      "labels" : [
        {
          "name" : "Car",
          "languageTag" : "en-US",
          "isDefault" : true
        }
      ],
      "lastModifiedDateTime": "2019-06-21T20:01:37Z"
   }  
 ]
}
```

[термин]: ../resources/termstore-term.md
[term]: ../resources/termstore-term.md
[set]: ../resources/termstore-set.md

<!--
{
  "type": "#page.annotation",
  "description": "Get children of a term or termSet in termStore",
  "keywords": "term,termStore",
  "section": "documentation",
  "tocPath": "termStore/Get termchildren",
  "suppressions": []
}
-->



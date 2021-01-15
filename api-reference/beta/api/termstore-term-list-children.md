---
title: Список дочерних элементов
description: Получите термины из свойства навигации children.
author: mohitpcad
ms.prod: Sharepoint
localization_priority: Normal
doc_type: apiPageType
ms.openlocfilehash: ddf7a7ba3419437b300d90ed33f3841e46bae5a0
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/15/2021
ms.locfileid: "49874454"
---
# <a name="list-children"></a><span data-ttu-id="473a2-103">Список дочерних элементов</span><span class="sxs-lookup"><span data-stu-id="473a2-103">List children</span></span>
<span data-ttu-id="473a2-104">Пространство имен: microsoft.graph.termStore</span><span class="sxs-lookup"><span data-stu-id="473a2-104">Namespace: microsoft.graph.termStore</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="473a2-105">Получите детей первого уровня набора [или] ресурса [терминов] с помощью свойства навигации children.</span><span class="sxs-lookup"><span data-stu-id="473a2-105">Get the first level children of a [set] or [term] resource using the children navigation property.</span></span>

## <a name="permissions"></a><span data-ttu-id="473a2-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="473a2-106">Permissions</span></span>
<span data-ttu-id="473a2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="473a2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="473a2-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="473a2-109">Permission type</span></span>|<span data-ttu-id="473a2-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="473a2-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="473a2-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="473a2-111">Delegated (work or school account)</span></span> | <span data-ttu-id="473a2-112">TermStore.Read.All, TermStore.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="473a2-112">TermStore.Read.All, TermStore.ReadWrite.All</span></span> |
|<span data-ttu-id="473a2-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="473a2-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="473a2-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="473a2-114">Not supported.</span></span>    |
|<span data-ttu-id="473a2-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="473a2-115">Application</span></span> | <span data-ttu-id="473a2-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="473a2-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="473a2-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="473a2-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /termStore/sets/{setId}/children
GET /termStore/sets/{setId}/terms/{termId}/children
```

## <a name="optional-query-parameters"></a><span data-ttu-id="473a2-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="473a2-118">Optional query parameters</span></span>
<span data-ttu-id="473a2-119">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="473a2-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="473a2-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="473a2-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="473a2-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="473a2-121">Request headers</span></span>
|<span data-ttu-id="473a2-122">Имя</span><span class="sxs-lookup"><span data-stu-id="473a2-122">Name</span></span>|<span data-ttu-id="473a2-123">Описание</span><span class="sxs-lookup"><span data-stu-id="473a2-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="473a2-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="473a2-124">Authorization</span></span>|<span data-ttu-id="473a2-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="473a2-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="473a2-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="473a2-127">Request body</span></span>
<span data-ttu-id="473a2-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="473a2-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="473a2-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="473a2-129">Response</span></span>

<span data-ttu-id="473a2-130">В случае успеха этот метод возвращает код отклика и коллекцию объектов `200 OK` [терминов](../resources/termstore-term.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="473a2-130">If successful, this method returns a `200 OK` response code and a collection of [term](../resources/termstore-term.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="473a2-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="473a2-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="473a2-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="473a2-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="473a2-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="473a2-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_term"
}-->

``` http
GET https://graph.microsoft.com/beta/termStore/sets/{setId}/children
```
# <a name="c"></a>[<span data-ttu-id="473a2-134">C#</span><span class="sxs-lookup"><span data-stu-id="473a2-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-term-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="473a2-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="473a2-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-term-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="473a2-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="473a2-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-term-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="473a2-137">Java</span><span class="sxs-lookup"><span data-stu-id="473a2-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-term-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="473a2-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="473a2-138">Response</span></span>
<span data-ttu-id="473a2-139">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="473a2-139">**Note:** The response object shown here might be shortened for readability.</span></span>
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



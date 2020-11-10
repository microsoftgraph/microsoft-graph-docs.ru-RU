---
title: Список отношений
description: Получение связей из свойства навигации "отношения".
author: mohitpcad
localization_priority: Normal
ms.prod: Sharepoint
doc_type: apiPageType
ms.openlocfilehash: ac82d8c83bb4494d8ccbc80602dac833baffc7f2
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48972249"
---
# <a name="list-relations"></a><span data-ttu-id="8d3e0-103">Список отношений</span><span class="sxs-lookup"><span data-stu-id="8d3e0-103">List relations</span></span>
<span data-ttu-id="8d3e0-104">Пространство имен: Microsoft. Graph. банка</span><span class="sxs-lookup"><span data-stu-id="8d3e0-104">Namespace: microsoft.graph.termStore</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8d3e0-105">Получение другого отношения [термина] или [набора] из свойства навигации отношений.</span><span class="sxs-lookup"><span data-stu-id="8d3e0-105">Get the different relation of a [term] or [set] from the relations navigation property.</span></span>

## <a name="permissions"></a><span data-ttu-id="8d3e0-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8d3e0-106">Permissions</span></span>
<span data-ttu-id="8d3e0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8d3e0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8d3e0-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8d3e0-109">Permission type</span></span>|<span data-ttu-id="8d3e0-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8d3e0-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8d3e0-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8d3e0-111">Delegated (work or school account)</span></span> |<span data-ttu-id="8d3e0-112">Банк. чтение. ALL, банк. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="8d3e0-112">TermStore.Read.All, TermStore.ReadWrite.All</span></span> |
|<span data-ttu-id="8d3e0-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8d3e0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8d3e0-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8d3e0-114">Not supported.</span></span>    |
|<span data-ttu-id="8d3e0-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8d3e0-115">Application</span></span> | <span data-ttu-id="8d3e0-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8d3e0-116">Not supported.</span></span> |


## <a name="http-request"></a><span data-ttu-id="8d3e0-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8d3e0-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /termStore/sets/{setId}/relations
GET /termStore/sets/{setId}/terms/{termId}/relations
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8d3e0-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="8d3e0-118">Optional query parameters</span></span>
<span data-ttu-id="8d3e0-119">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="8d3e0-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="8d3e0-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="8d3e0-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="8d3e0-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8d3e0-121">Request headers</span></span>
|<span data-ttu-id="8d3e0-122">Имя</span><span class="sxs-lookup"><span data-stu-id="8d3e0-122">Name</span></span>|<span data-ttu-id="8d3e0-123">Описание</span><span class="sxs-lookup"><span data-stu-id="8d3e0-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="8d3e0-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8d3e0-124">Authorization</span></span>|<span data-ttu-id="8d3e0-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8d3e0-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8d3e0-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8d3e0-127">Request body</span></span>
<span data-ttu-id="8d3e0-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8d3e0-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8d3e0-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="8d3e0-129">Response</span></span>

<span data-ttu-id="8d3e0-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [relation](../resources/termstore-relation.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8d3e0-130">If successful, this method returns a `200 OK` response code and a collection of [relation](../resources/termstore-relation.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8d3e0-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="8d3e0-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8d3e0-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="8d3e0-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="8d3e0-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="8d3e0-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_relation"
}-->

``` http
GET https://graph.microsoft.com/beta/termStore/sets/{setId}/relations
```
# <a name="c"></a>[<span data-ttu-id="8d3e0-134">C#</span><span class="sxs-lookup"><span data-stu-id="8d3e0-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-relation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8d3e0-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8d3e0-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-relation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8d3e0-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8d3e0-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-relation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8d3e0-137">Java</span><span class="sxs-lookup"><span data-stu-id="8d3e0-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-relation-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="8d3e0-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="8d3e0-138">Response</span></span>
<span data-ttu-id="8d3e0-139">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="8d3e0-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.termStore.relation)"
}-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "052c749c-749c-052c-9c74-2c059c742c05",
      "relationship": "pin"
    }
  ]
}
```


[set]: ../resources/termstore-set.md
[банком]: ../resources/termstore-term.md
[term]: ../resources/termstore-term.md
[microsoft.graph.termStore.relation]: ../resources/termstore-relation.md


<!--
{
  "type": "#page.annotation",
  "description": "Create a pinned term entity in termStore",
  "keywords": "term,termStore",
  "section": "documentation",
  "tocPath": "termStore/term list relations",
  "suppressions": [
  ]
}
-->



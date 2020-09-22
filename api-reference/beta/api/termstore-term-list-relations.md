---
title: Список отношений
description: Получение связей из свойства навигации "отношения".
author: mohitpcad
localization_priority: Normal
ms.prod: Sharepoint
doc_type: apiPageType
ms.openlocfilehash: ba593b7d5be184d5a53c0dd2af98dc655a3712bc
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48042866"
---
# <a name="list-relations"></a><span data-ttu-id="a2c5b-103">Список отношений</span><span class="sxs-lookup"><span data-stu-id="a2c5b-103">List relations</span></span>
<span data-ttu-id="a2c5b-104">Пространство имен: Microsoft. Graph. банка</span><span class="sxs-lookup"><span data-stu-id="a2c5b-104">Namespace: microsoft.graph.termStore</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a2c5b-105">Получение другого отношения [термина] или [набора] из свойства навигации отношений.</span><span class="sxs-lookup"><span data-stu-id="a2c5b-105">Get the different relation of a [term] or [set] from the relations navigation property.</span></span>

## <a name="permissions"></a><span data-ttu-id="a2c5b-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a2c5b-106">Permissions</span></span>
<span data-ttu-id="a2c5b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a2c5b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a2c5b-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a2c5b-109">Permission type</span></span>|<span data-ttu-id="a2c5b-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a2c5b-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a2c5b-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a2c5b-111">Delegated (work or school account)</span></span> |<span data-ttu-id="a2c5b-112">Банк. чтение. ALL, банк. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="a2c5b-112">TermStore.Read.All, TermStore.ReadWrite.All</span></span> |
|<span data-ttu-id="a2c5b-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a2c5b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a2c5b-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a2c5b-114">Not supported.</span></span>    |
|<span data-ttu-id="a2c5b-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a2c5b-115">Application</span></span> | <span data-ttu-id="a2c5b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a2c5b-116">Not supported.</span></span> |


## <a name="http-request"></a><span data-ttu-id="a2c5b-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a2c5b-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /termStore/sets/{setId}/relations
GET /termStore/sets/{setId}/terms/{termId}/relations
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a2c5b-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="a2c5b-118">Optional query parameters</span></span>
<span data-ttu-id="a2c5b-119">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="a2c5b-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="a2c5b-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="a2c5b-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="a2c5b-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a2c5b-121">Request headers</span></span>
|<span data-ttu-id="a2c5b-122">Имя</span><span class="sxs-lookup"><span data-stu-id="a2c5b-122">Name</span></span>|<span data-ttu-id="a2c5b-123">Описание</span><span class="sxs-lookup"><span data-stu-id="a2c5b-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="a2c5b-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a2c5b-124">Authorization</span></span>|<span data-ttu-id="a2c5b-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a2c5b-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a2c5b-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a2c5b-127">Request body</span></span>
<span data-ttu-id="a2c5b-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a2c5b-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a2c5b-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="a2c5b-129">Response</span></span>

<span data-ttu-id="a2c5b-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [relation](../resources/termstore-relation.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a2c5b-130">If successful, this method returns a `200 OK` response code and a collection of [relation](../resources/termstore-relation.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a2c5b-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="a2c5b-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a2c5b-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="a2c5b-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="a2c5b-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="a2c5b-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_relation"
}-->

``` http
GET https://graph.microsoft.com/beta/termStore/sets/{setId}/relations
```
# <a name="c"></a>[<span data-ttu-id="a2c5b-134">C#</span><span class="sxs-lookup"><span data-stu-id="a2c5b-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-relation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a2c5b-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a2c5b-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-relation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a2c5b-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a2c5b-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-relation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="a2c5b-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="a2c5b-137">Response</span></span>
<span data-ttu-id="a2c5b-138">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="a2c5b-138">**Note:** The response object shown here might be shortened for readability.</span></span>
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



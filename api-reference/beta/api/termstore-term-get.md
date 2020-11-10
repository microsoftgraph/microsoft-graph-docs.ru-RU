---
title: Получение термина
description: Чтение свойств и связей объекта Term.
author: mohitpcad
localization_priority: Normal
ms.prod: Sharepoint
doc_type: apiPageType
ms.openlocfilehash: 993b09b6ba9fbff261a92fa2263807f1ef4d77f4
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48972272"
---
# <a name="get-term"></a><span data-ttu-id="abdb5-103">Получение термина</span><span class="sxs-lookup"><span data-stu-id="abdb5-103">Get term</span></span>
<span data-ttu-id="abdb5-104">Пространство имен: Microsoft. Graph. банка</span><span class="sxs-lookup"><span data-stu-id="abdb5-104">Namespace: microsoft.graph.termStore</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="abdb5-105">Чтение свойств и связей объекта [Term](../resources/termstore-term.md) .</span><span class="sxs-lookup"><span data-stu-id="abdb5-105">Read the properties and relationships of a [term](../resources/termstore-term.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="abdb5-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="abdb5-106">Permissions</span></span>
<span data-ttu-id="abdb5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="abdb5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="abdb5-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="abdb5-109">Permission type</span></span>|<span data-ttu-id="abdb5-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="abdb5-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="abdb5-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="abdb5-111">Delegated (work or school account)</span></span> | <span data-ttu-id="abdb5-112">Банк. чтение. ALL, банк. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="abdb5-112">TermStore.Read.All, TermStore.ReadWrite.All</span></span> |
|<span data-ttu-id="abdb5-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="abdb5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="abdb5-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="abdb5-114">Not supported.</span></span>    |
|<span data-ttu-id="abdb5-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="abdb5-115">Application</span></span> | <span data-ttu-id="abdb5-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="abdb5-116">Not supported.</span></span> |


## <a name="http-request"></a><span data-ttu-id="abdb5-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="abdb5-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
} -->

``` http
GET /termStore/groups/{groupId}/sets/{setId}/terms/{termId}
GET /termStore/sets/{setId}/terms/{termId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="abdb5-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="abdb5-118">Optional query parameters</span></span>
<span data-ttu-id="abdb5-119">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="abdb5-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="abdb5-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="abdb5-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="abdb5-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="abdb5-121">Request headers</span></span>
|<span data-ttu-id="abdb5-122">Имя</span><span class="sxs-lookup"><span data-stu-id="abdb5-122">Name</span></span>|<span data-ttu-id="abdb5-123">Описание</span><span class="sxs-lookup"><span data-stu-id="abdb5-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="abdb5-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="abdb5-124">Authorization</span></span>|<span data-ttu-id="abdb5-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="abdb5-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="abdb5-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="abdb5-127">Request body</span></span>
<span data-ttu-id="abdb5-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="abdb5-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="abdb5-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="abdb5-129">Response</span></span>

<span data-ttu-id="abdb5-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [Term](../resources/termstore-term.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="abdb5-130">If successful, this method returns a `200 OK` response code and a [term](../resources/termstore-term.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="abdb5-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="abdb5-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="abdb5-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="abdb5-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="abdb5-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="abdb5-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_term"
} -->

``` http
GET https://graph.microsoft.com/beta/termStore/groups/{groupId}/sets/{setId}/terms/{termId}
```
# <a name="c"></a>[<span data-ttu-id="abdb5-134">C#</span><span class="sxs-lookup"><span data-stu-id="abdb5-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-term-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="abdb5-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="abdb5-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-term-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="abdb5-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="abdb5-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-term-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="abdb5-137">Java</span><span class="sxs-lookup"><span data-stu-id="abdb5-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-term-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="abdb5-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="abdb5-138">Response</span></span>
<span data-ttu-id="abdb5-139">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="abdb5-139">**Note:** The response object shown here might be shortened for readability.</span></span>
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




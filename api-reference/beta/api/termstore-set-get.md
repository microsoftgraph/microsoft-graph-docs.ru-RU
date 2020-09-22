---
title: Получение набора
description: Считывание свойств и связей объекта Set.
author: mohitpcad
localization_priority: Normal
ms.prod: Sharepoint
doc_type: apiPageType
ms.openlocfilehash: a10a6214c3920290d1a2bb33b17e3fc739b47da1
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48064628"
---
# <a name="get-set"></a><span data-ttu-id="b3878-103">Получение набора</span><span class="sxs-lookup"><span data-stu-id="b3878-103">Get set</span></span>
<span data-ttu-id="b3878-104">Пространство имен: Microsoft. Graph. банка [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span><span class="sxs-lookup"><span data-stu-id="b3878-104">Namespace: microsoft.graph.termStore [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span></span>

<span data-ttu-id="b3878-105">Считывание свойств и связей объекта [Set](../resources/termstore-set.md) .</span><span class="sxs-lookup"><span data-stu-id="b3878-105">Read the properties and relationships of a [set](../resources/termstore-set.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="b3878-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b3878-106">Permissions</span></span>
<span data-ttu-id="b3878-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b3878-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b3878-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b3878-109">Permission type</span></span>|<span data-ttu-id="b3878-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b3878-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b3878-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b3878-111">Delegated (work or school account)</span></span> |<span data-ttu-id="b3878-112">Банк. чтение. ALL, банк. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="b3878-112">TermStore.Read.All, TermStore.ReadWrite.All</span></span> |
|<span data-ttu-id="b3878-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b3878-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b3878-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b3878-114">Not supported.</span></span>    |
|<span data-ttu-id="b3878-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b3878-115">Application</span></span> | <span data-ttu-id="b3878-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b3878-116">Not supported.</span></span> |


## <a name="http-request"></a><span data-ttu-id="b3878-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b3878-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /termStore/sets/{setId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b3878-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="b3878-118">Optional query parameters</span></span>
<span data-ttu-id="b3878-119">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="b3878-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="b3878-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="b3878-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="b3878-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b3878-121">Request headers</span></span>
|<span data-ttu-id="b3878-122">Имя</span><span class="sxs-lookup"><span data-stu-id="b3878-122">Name</span></span>|<span data-ttu-id="b3878-123">Описание</span><span class="sxs-lookup"><span data-stu-id="b3878-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="b3878-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b3878-124">Authorization</span></span>|<span data-ttu-id="b3878-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b3878-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b3878-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b3878-127">Request body</span></span>
<span data-ttu-id="b3878-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b3878-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b3878-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="b3878-129">Response</span></span>

<span data-ttu-id="b3878-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [Set](../resources/termstore-set.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b3878-130">If successful, this method returns a `200 OK` response code and a [set](../resources/termstore-set.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b3878-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="b3878-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b3878-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="b3878-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="b3878-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="b3878-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_set"
}-->

``` http
GET https://graph.microsoft.com/beta/termStore/sets/{setId}
```
# <a name="c"></a>[<span data-ttu-id="b3878-134">C#</span><span class="sxs-lookup"><span data-stu-id="b3878-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-set-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b3878-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b3878-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-set-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b3878-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b3878-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-set-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="b3878-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="b3878-137">Response</span></span>
<span data-ttu-id="b3878-138">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="b3878-138">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.termStore.set"
} -->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{

  "createdDateTime": "2019-06-21T20:01:37Z",  
  "description": "Starting term Set",
  "id": "8ed8c9ea-7052-4c1d-a4d7-b9c10bffea6f",
  "localizedNames" : [
    {
      "languageTag" : "en-US",
      "name" : "Department"
    }
  ]
}
```

[microsoft.graph.termStore.group]: ../resources/termstore-group.md
[microsoft.graph.termStore.set]: ../resources/termstore-set.md
[microsoft.graph.termStore.store]: ../resources/termstore-store.md

<!--
{
  "type": "#page.annotation",
  "description": "Get termSet entity in termStore",
  "keywords": "term,termStore",
  "section": "documentation",
  "tocPath": "termStore/Get termSet",
  "suppressions": [
  ]
}
-->



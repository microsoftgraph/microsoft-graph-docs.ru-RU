---
title: Получить термин
description: Ознакомьтесь с свойствами и отношениями объекта терминов.
author: mohitpcad
localization_priority: Normal
ms.prod: taxonomy
doc_type: apiPageType
ms.openlocfilehash: b26b1bc5da13bd8edabe3f381f950c47894800d2
ms.sourcegitcommit: 73bbf84e6f5dbc8c3db8ed2c48cc5ab9ae3cff78
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/16/2021
ms.locfileid: "53456480"
---
# <a name="get-term"></a><span data-ttu-id="43666-103">Получить термин</span><span class="sxs-lookup"><span data-stu-id="43666-103">Get term</span></span>
<span data-ttu-id="43666-104">Пространство имен: microsoft.graph.termStore</span><span class="sxs-lookup"><span data-stu-id="43666-104">Namespace: microsoft.graph.termStore</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="43666-105">Ознакомьтесь с свойствами и отношениями объекта [терминов.](../resources/termstore-term.md)</span><span class="sxs-lookup"><span data-stu-id="43666-105">Read the properties and relationships of a [term](../resources/termstore-term.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="43666-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="43666-106">Permissions</span></span>
<span data-ttu-id="43666-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="43666-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="43666-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="43666-109">Permission type</span></span>|<span data-ttu-id="43666-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="43666-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="43666-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="43666-111">Delegated (work or school account)</span></span> | <span data-ttu-id="43666-112">TermStore.Read.All, TermStore.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="43666-112">TermStore.Read.All, TermStore.ReadWrite.All</span></span> |
|<span data-ttu-id="43666-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="43666-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="43666-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="43666-114">Not supported.</span></span>    |
|<span data-ttu-id="43666-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="43666-115">Application</span></span> | <span data-ttu-id="43666-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="43666-116">Not supported.</span></span> |


## <a name="http-request"></a><span data-ttu-id="43666-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="43666-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
} -->

``` http
GET /termStore/groups/{group-id}/sets/{set-id}/terms/{term-id}
GET /termStore/sets/{set-id}/terms/{term-id}
GET /sites/{site-id}/termStore/groups/{group-id}/sets/{set-id}/terms/{term-id}
GET /sites/{site-id}/termStore/sets/{set-id}/terms/{term-id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="43666-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="43666-118">Optional query parameters</span></span>
<span data-ttu-id="43666-119">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="43666-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="43666-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="43666-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="43666-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="43666-121">Request headers</span></span>
|<span data-ttu-id="43666-122">Имя</span><span class="sxs-lookup"><span data-stu-id="43666-122">Name</span></span>|<span data-ttu-id="43666-123">Описание</span><span class="sxs-lookup"><span data-stu-id="43666-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="43666-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="43666-124">Authorization</span></span>|<span data-ttu-id="43666-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="43666-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="43666-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="43666-127">Request body</span></span>
<span data-ttu-id="43666-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="43666-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="43666-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="43666-129">Response</span></span>

<span data-ttu-id="43666-130">В случае успешной работы этот метод возвращает код ответа и объект `200 OK` [терминов](../resources/termstore-term.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="43666-130">If successful, this method returns a `200 OK` response code and a [term](../resources/termstore-term.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="43666-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="43666-131">Examples</span></span>

### <a name="example-1-get-a-termstore-term"></a><span data-ttu-id="43666-132">Пример 1. Получить термин TermStore</span><span class="sxs-lookup"><span data-stu-id="43666-132">Example 1: Get a termStore term</span></span>

#### <a name="request"></a><span data-ttu-id="43666-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="43666-133">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="43666-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="43666-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_term_1"
} -->

``` http
GET https://graph.microsoft.com/beta/termStore/groups/1FFD3F87-9464-488A-A0EC-8FB90911182C/sets/8ed8c9ea-7052-4c1d-a4d7-b9c10bffea6f/terms/81be9856-9856-81be-5698-be815698be81
```
# <a name="c"></a>[<span data-ttu-id="43666-135">C#</span><span class="sxs-lookup"><span data-stu-id="43666-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-term-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="43666-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="43666-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-term-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="43666-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="43666-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-term-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="43666-138">Java</span><span class="sxs-lookup"><span data-stu-id="43666-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-term-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="43666-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="43666-139">Response</span></span>
><span data-ttu-id="43666-140">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="43666-140">**Note:** The response object shown here might be shortened for readability.</span></span>
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
### <a name="example-2--get-a-site-collection-termstore-term"></a><span data-ttu-id="43666-141">Пример 2. Получить термин termStore для коллекции сайтов</span><span class="sxs-lookup"><span data-stu-id="43666-141">Example 2 : Get a site collection termStore term</span></span>

#### <a name="request"></a><span data-ttu-id="43666-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="43666-142">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_term_1"
} -->

``` http
GET https://graph.microsoft.com/beta/sites/microsoft.sharepoint.com,c6482504-4a85-4b21-858a-7e88dafc8232,d90ca07d-25c0-4ce7-864b-d68b607e697f/termStore/groups/1FFD3F87-9464-488A-A0EC-8FB90911182C/sets/8ed8c9ea-7052-4c1d-a4d7-b9c10bffea6f/terms/81be9856-9856-81be-5698-be815698be81
```

#### <a name="response"></a><span data-ttu-id="43666-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="43666-143">Response</span></span>
><span data-ttu-id="43666-144">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="43666-144">**Note:** The response object shown here might be shortened for readability.</span></span>
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




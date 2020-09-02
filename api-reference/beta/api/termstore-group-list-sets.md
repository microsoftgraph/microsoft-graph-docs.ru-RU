---
title: Наборы списков
description: Получение списка объектов Set и их свойств.
author: mohitpcad
localization_priority: Normal
ms.prod: Sharepoint
doc_type: apiPageType
ms.openlocfilehash: f4d35decdae3303576565e2844206c7bfe16cf23
ms.sourcegitcommit: 726f20403323be7d267b67c2764ed7c244e02ee1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/02/2020
ms.locfileid: "47330296"
---
# <a name="list-sets"></a><span data-ttu-id="d1f7a-103">Наборы списков</span><span class="sxs-lookup"><span data-stu-id="d1f7a-103">List sets</span></span>
<span data-ttu-id="d1f7a-104">Пространство имен: Microsoft. Graph. банка</span><span class="sxs-lookup"><span data-stu-id="d1f7a-104">Namespace: microsoft.graph.termStore</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d1f7a-105">Получение списка объектов [Set](../resources/termstore-set.md) и их свойств.</span><span class="sxs-lookup"><span data-stu-id="d1f7a-105">Get a list of the [set](../resources/termstore-set.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="d1f7a-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d1f7a-106">Permissions</span></span>
<span data-ttu-id="d1f7a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d1f7a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d1f7a-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d1f7a-109">Permission type</span></span>|<span data-ttu-id="d1f7a-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d1f7a-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d1f7a-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d1f7a-111">Delegated (work or school account)</span></span> |<span data-ttu-id="d1f7a-112">Банк. чтение. ALL, банк. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="d1f7a-112">TermStore.Read.All, TermStore.ReadWrite.All</span></span> |
|<span data-ttu-id="d1f7a-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d1f7a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d1f7a-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d1f7a-114">Not supported.</span></span>    |
|<span data-ttu-id="d1f7a-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d1f7a-115">Application</span></span> | <span data-ttu-id="d1f7a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d1f7a-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d1f7a-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d1f7a-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /termStore/groups/{groupId}/sets
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d1f7a-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="d1f7a-118">Optional query parameters</span></span>
<span data-ttu-id="d1f7a-119">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="d1f7a-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="d1f7a-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="d1f7a-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="d1f7a-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d1f7a-121">Request headers</span></span>
|<span data-ttu-id="d1f7a-122">Имя</span><span class="sxs-lookup"><span data-stu-id="d1f7a-122">Name</span></span>|<span data-ttu-id="d1f7a-123">Описание</span><span class="sxs-lookup"><span data-stu-id="d1f7a-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="d1f7a-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d1f7a-124">Authorization</span></span>|<span data-ttu-id="d1f7a-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d1f7a-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d1f7a-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d1f7a-127">Request body</span></span>
<span data-ttu-id="d1f7a-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d1f7a-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d1f7a-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="d1f7a-129">Response</span></span>

<span data-ttu-id="d1f7a-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [Set](../resources/termstore-set.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d1f7a-130">If successful, this method returns a `200 OK` response code and a collection of [set](../resources/termstore-set.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d1f7a-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="d1f7a-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d1f7a-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="d1f7a-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="d1f7a-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="d1f7a-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_set"
}-->

``` http
GET https://graph.microsoft.com/beta/termStore/groups/{groupId}/sets
```
# <a name="c"></a>[<span data-ttu-id="d1f7a-134">C#</span><span class="sxs-lookup"><span data-stu-id="d1f7a-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-set-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d1f7a-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d1f7a-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-set-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d1f7a-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d1f7a-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-set-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="d1f7a-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="d1f7a-137">Response</span></span>

<span data-ttu-id="d1f7a-138">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="d1f7a-138">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.termStore.set)"
} -->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "3607e9f9-e9f9-3607-f9e9-0736f9e90736",
      "description": "Starting term Set",    
      "localizedNames" : [
        {
          "languageTag" : "en-US",
          "name" : "Department"
        }
      ]
    }
  ]
}
```

[microsoft.graph.termStore.set]: ../resources/termstore-set.md

<!--
{
  "type": "#page.annotation",
  "description": "Get termSet entity in termStore",
  "keywords": "term,termStore",
  "section": "documentation",
  "tocPath": "termStore/List termstore-set",
  "suppressions": [
  ]
}
-->

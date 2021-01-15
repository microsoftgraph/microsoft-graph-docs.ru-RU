---
title: Наборы списков
description: Получите список объектов набора и их свойств.
author: mohitpcad
localization_priority: Normal
ms.prod: Sharepoint
doc_type: apiPageType
ms.openlocfilehash: 4d358769f7d4a73c2f01f84e0237747c456307a5
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/15/2021
ms.locfileid: "49873943"
---
# <a name="list-sets"></a><span data-ttu-id="cdc95-103">Наборы списков</span><span class="sxs-lookup"><span data-stu-id="cdc95-103">List sets</span></span>
<span data-ttu-id="cdc95-104">Пространство имен: microsoft.graph.termStore</span><span class="sxs-lookup"><span data-stu-id="cdc95-104">Namespace: microsoft.graph.termStore</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cdc95-105">Получите список объектов [набора и](../resources/termstore-set.md) их свойств.</span><span class="sxs-lookup"><span data-stu-id="cdc95-105">Get a list of the [set](../resources/termstore-set.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="cdc95-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cdc95-106">Permissions</span></span>
<span data-ttu-id="cdc95-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cdc95-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cdc95-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cdc95-109">Permission type</span></span>|<span data-ttu-id="cdc95-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cdc95-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cdc95-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cdc95-111">Delegated (work or school account)</span></span> |<span data-ttu-id="cdc95-112">TermStore.Read.All, TermStore.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cdc95-112">TermStore.Read.All, TermStore.ReadWrite.All</span></span> |
|<span data-ttu-id="cdc95-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cdc95-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cdc95-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cdc95-114">Not supported.</span></span>    |
|<span data-ttu-id="cdc95-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cdc95-115">Application</span></span> | <span data-ttu-id="cdc95-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cdc95-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="cdc95-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cdc95-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /termStore/groups/{groupId}/sets
```

## <a name="optional-query-parameters"></a><span data-ttu-id="cdc95-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="cdc95-118">Optional query parameters</span></span>
<span data-ttu-id="cdc95-119">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="cdc95-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="cdc95-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="cdc95-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="cdc95-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cdc95-121">Request headers</span></span>
|<span data-ttu-id="cdc95-122">Имя</span><span class="sxs-lookup"><span data-stu-id="cdc95-122">Name</span></span>|<span data-ttu-id="cdc95-123">Описание</span><span class="sxs-lookup"><span data-stu-id="cdc95-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="cdc95-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cdc95-124">Authorization</span></span>|<span data-ttu-id="cdc95-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cdc95-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="cdc95-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cdc95-127">Request body</span></span>
<span data-ttu-id="cdc95-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="cdc95-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cdc95-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="cdc95-129">Response</span></span>

<span data-ttu-id="cdc95-130">В случае успеха этот метод возвращает код отклика и коллекцию установленных `200 OK` объектов в тексте отклика. [](../resources/termstore-set.md)</span><span class="sxs-lookup"><span data-stu-id="cdc95-130">If successful, this method returns a `200 OK` response code and a collection of [set](../resources/termstore-set.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="cdc95-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="cdc95-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="cdc95-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="cdc95-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="cdc95-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="cdc95-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_set"
}-->

``` http
GET https://graph.microsoft.com/beta/termStore/groups/{groupId}/sets
```
# <a name="c"></a>[<span data-ttu-id="cdc95-134">C#</span><span class="sxs-lookup"><span data-stu-id="cdc95-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-set-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cdc95-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cdc95-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-set-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cdc95-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cdc95-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-set-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="cdc95-137">Java</span><span class="sxs-lookup"><span data-stu-id="cdc95-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-set-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="cdc95-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="cdc95-138">Response</span></span>

<span data-ttu-id="cdc95-139">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="cdc95-139">**Note:** The response object shown here might be shortened for readability.</span></span>

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



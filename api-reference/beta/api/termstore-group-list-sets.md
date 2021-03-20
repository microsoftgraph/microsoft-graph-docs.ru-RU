---
title: Наборы списков
description: Получите список установленных объектов и их свойств.
author: mohitpcad
localization_priority: Normal
ms.prod: Sharepoint
doc_type: apiPageType
ms.openlocfilehash: 32c929f5156304e2a36aa64a5fcc8d97cee8468d
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50950454"
---
# <a name="list-sets"></a><span data-ttu-id="eb5cd-103">Наборы списков</span><span class="sxs-lookup"><span data-stu-id="eb5cd-103">List sets</span></span>
<span data-ttu-id="eb5cd-104">Пространство имен: microsoft.graph.termStore</span><span class="sxs-lookup"><span data-stu-id="eb5cd-104">Namespace: microsoft.graph.termStore</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eb5cd-105">Получите список [установленных объектов](../resources/termstore-set.md) и их свойств.</span><span class="sxs-lookup"><span data-stu-id="eb5cd-105">Get a list of the [set](../resources/termstore-set.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="eb5cd-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="eb5cd-106">Permissions</span></span>
<span data-ttu-id="eb5cd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eb5cd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eb5cd-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="eb5cd-109">Permission type</span></span>|<span data-ttu-id="eb5cd-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="eb5cd-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="eb5cd-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="eb5cd-111">Delegated (work or school account)</span></span> |<span data-ttu-id="eb5cd-112">TermStore.Read.All, TermStore.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eb5cd-112">TermStore.Read.All, TermStore.ReadWrite.All</span></span> |
|<span data-ttu-id="eb5cd-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="eb5cd-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eb5cd-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eb5cd-114">Not supported.</span></span>    |
|<span data-ttu-id="eb5cd-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="eb5cd-115">Application</span></span> | <span data-ttu-id="eb5cd-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eb5cd-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="eb5cd-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="eb5cd-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /termStore/groups/{groupId}/sets
```

## <a name="optional-query-parameters"></a><span data-ttu-id="eb5cd-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="eb5cd-118">Optional query parameters</span></span>
<span data-ttu-id="eb5cd-119">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="eb5cd-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="eb5cd-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="eb5cd-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="eb5cd-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="eb5cd-121">Request headers</span></span>
|<span data-ttu-id="eb5cd-122">Имя</span><span class="sxs-lookup"><span data-stu-id="eb5cd-122">Name</span></span>|<span data-ttu-id="eb5cd-123">Описание</span><span class="sxs-lookup"><span data-stu-id="eb5cd-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="eb5cd-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="eb5cd-124">Authorization</span></span>|<span data-ttu-id="eb5cd-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="eb5cd-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="eb5cd-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="eb5cd-127">Request body</span></span>
<span data-ttu-id="eb5cd-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="eb5cd-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="eb5cd-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="eb5cd-129">Response</span></span>

<span data-ttu-id="eb5cd-130">В случае успешной работы этот метод возвращает код отклика и коллекцию заданной `200 OK` объекты в [](../resources/termstore-set.md) тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="eb5cd-130">If successful, this method returns a `200 OK` response code and a collection of [set](../resources/termstore-set.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="eb5cd-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="eb5cd-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="eb5cd-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="eb5cd-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="eb5cd-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="eb5cd-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_set_1"
}-->

``` http
GET https://graph.microsoft.com/beta/termStore/groups/{groupId}/sets
```
# <a name="c"></a>[<span data-ttu-id="eb5cd-134">C#</span><span class="sxs-lookup"><span data-stu-id="eb5cd-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-set-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="eb5cd-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="eb5cd-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-set-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="eb5cd-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="eb5cd-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-set-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="eb5cd-137">Java</span><span class="sxs-lookup"><span data-stu-id="eb5cd-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-set-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="eb5cd-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="eb5cd-138">Response</span></span>

<span data-ttu-id="eb5cd-139">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="eb5cd-139">**Note:** The response object shown here might be shortened for readability.</span></span>

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



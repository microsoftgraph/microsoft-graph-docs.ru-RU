---
title: Get store
description: Ознакомьтесь с свойствами и отношениями объекта магазина.
author: mohitpcad
localization_priority: Normal
ms.prod: taxonomy
doc_type: apiPageType
ms.openlocfilehash: 71f23420196bab347cfe74068602b128eada36f4
ms.sourcegitcommit: 73bbf84e6f5dbc8c3db8ed2c48cc5ab9ae3cff78
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/16/2021
ms.locfileid: "53456487"
---
# <a name="get-store"></a><span data-ttu-id="b3bbd-103">Get store</span><span class="sxs-lookup"><span data-stu-id="b3bbd-103">Get store</span></span>
<span data-ttu-id="b3bbd-104">Пространство имен: microsoft.graph.termStore</span><span class="sxs-lookup"><span data-stu-id="b3bbd-104">Namespace: microsoft.graph.termStore</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b3bbd-105">Ознакомьтесь с свойствами и отношениями объекта [магазина.](../resources/termstore-store.md)</span><span class="sxs-lookup"><span data-stu-id="b3bbd-105">Read the properties and relationships of a [store](../resources/termstore-store.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="b3bbd-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b3bbd-106">Permissions</span></span>
<span data-ttu-id="b3bbd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b3bbd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b3bbd-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b3bbd-109">Permission type</span></span>|<span data-ttu-id="b3bbd-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b3bbd-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b3bbd-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b3bbd-111">Delegated (work or school account)</span></span> | <span data-ttu-id="b3bbd-112">TermStore.Read.All, TermStore.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b3bbd-112">TermStore.Read.All, TermStore.ReadWrite.All</span></span> |
|<span data-ttu-id="b3bbd-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b3bbd-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b3bbd-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b3bbd-114">Not supported.</span></span>    |
|<span data-ttu-id="b3bbd-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b3bbd-115">Application</span></span> | <span data-ttu-id="b3bbd-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b3bbd-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b3bbd-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b3bbd-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /termStore
GET /sites/{site-id}/termStore
```

## <a name="request-headers"></a><span data-ttu-id="b3bbd-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b3bbd-118">Request headers</span></span>
|<span data-ttu-id="b3bbd-119">Имя</span><span class="sxs-lookup"><span data-stu-id="b3bbd-119">Name</span></span>|<span data-ttu-id="b3bbd-120">Описание</span><span class="sxs-lookup"><span data-stu-id="b3bbd-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="b3bbd-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b3bbd-121">Authorization</span></span>|<span data-ttu-id="b3bbd-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b3bbd-p102">Bearer {token}. Required.</span></span>|

## <a name="response"></a><span data-ttu-id="b3bbd-124">Отклик</span><span class="sxs-lookup"><span data-stu-id="b3bbd-124">Response</span></span>

<span data-ttu-id="b3bbd-125">В случае успешной работы этот метод возвращает код отклика и `200 OK` объект [магазина](../resources/termstore-store.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="b3bbd-125">If successful, this method returns a `200 OK` response code and a [store](../resources/termstore-store.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b3bbd-126">Примеры</span><span class="sxs-lookup"><span data-stu-id="b3bbd-126">Examples</span></span>

### <a name="example-1-get-a-termstore"></a><span data-ttu-id="b3bbd-127">Пример 1. Получить терминStore</span><span class="sxs-lookup"><span data-stu-id="b3bbd-127">Example 1: Get a termStore</span></span>

#### <a name="request"></a><span data-ttu-id="b3bbd-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="b3bbd-128">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="b3bbd-129">HTTP</span><span class="sxs-lookup"><span data-stu-id="b3bbd-129">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_store"
}-->

``` http
GET https://graph.microsoft.com/beta/termStore
```
# <a name="c"></a>[<span data-ttu-id="b3bbd-130">C#</span><span class="sxs-lookup"><span data-stu-id="b3bbd-130">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-store-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b3bbd-131">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b3bbd-131">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-store-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b3bbd-132">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b3bbd-132">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-store-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b3bbd-133">Java</span><span class="sxs-lookup"><span data-stu-id="b3bbd-133">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-store-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a><span data-ttu-id="b3bbd-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="b3bbd-134">Response</span></span>
><span data-ttu-id="b3bbd-135">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="b3bbd-135">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.termStore.store"
} -->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{  
  "id": "dad13b4b-3b4b-dad1-4b3b-d1da4b3bd1da",
  "defaultLanguageTag" : "en-US",
  "languageTags" : ["en-US", "de-DE", "fr-FR"]
}
```

### <a name="example-2-get-a-site-collection-termstore"></a><span data-ttu-id="b3bbd-136">Пример 2. Получить термин коллекция сайтовStore</span><span class="sxs-lookup"><span data-stu-id="b3bbd-136">Example 2: Get a site collection termStore</span></span>

#### <a name="request"></a><span data-ttu-id="b3bbd-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="b3bbd-137">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_store"
}-->

``` http
GET https://graph.microsoft.com/beta/sites/microsoft.sharepoint.com,c6482504-4a85-4b21-858a-7e88dafc8232,d90ca07d-25c0-4ce7-864b-d68b607e697f/termStore
```

#### <a name="response"></a><span data-ttu-id="b3bbd-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="b3bbd-138">Response</span></span>
><span data-ttu-id="b3bbd-139">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="b3bbd-139">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.termStore.store"
} -->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{  
  "id": "dad13b4b-3b4b-dad1-4b3b-d1da4b3bd1da",
  "defaultLanguageTag" : "en-US",
  "languageTags" : ["en-US", "de-DE", "fr-FR"]
}
```

<!--
{
  "type": "#page.annotation",
  "description": "Get termStore entity in termStore",
  "keywords": "term,termStore",
  "section": "documentation",
  "tocPath": "termStore/Get termStore",
  "suppressions": []
}
-->



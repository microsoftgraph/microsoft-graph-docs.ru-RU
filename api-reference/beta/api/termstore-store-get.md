---
title: Получить магазин
description: Чтение свойств и связей объекта store.
author: mohitpcad
localization_priority: Normal
ms.prod: Sharepoint
doc_type: apiPageType
ms.openlocfilehash: fb94dd40644fc1c8ad3f1727fa41b9143f2b1e13
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/15/2021
ms.locfileid: "49874419"
---
# <a name="get-store"></a><span data-ttu-id="d4ded-103">Получить магазин</span><span class="sxs-lookup"><span data-stu-id="d4ded-103">Get store</span></span>
<span data-ttu-id="d4ded-104">Пространство имен: microsoft.graph.termStore</span><span class="sxs-lookup"><span data-stu-id="d4ded-104">Namespace: microsoft.graph.termStore</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d4ded-105">Чтение свойств и связей [объекта](../resources/termstore-store.md) store.</span><span class="sxs-lookup"><span data-stu-id="d4ded-105">Read the properties and relationships of a [store](../resources/termstore-store.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="d4ded-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d4ded-106">Permissions</span></span>
<span data-ttu-id="d4ded-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d4ded-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d4ded-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d4ded-109">Permission type</span></span>|<span data-ttu-id="d4ded-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d4ded-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d4ded-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d4ded-111">Delegated (work or school account)</span></span> | <span data-ttu-id="d4ded-112">TermStore.Read.All, TermStore.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d4ded-112">TermStore.Read.All, TermStore.ReadWrite.All</span></span> |
|<span data-ttu-id="d4ded-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d4ded-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d4ded-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d4ded-114">Not supported.</span></span>    |
|<span data-ttu-id="d4ded-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d4ded-115">Application</span></span> | <span data-ttu-id="d4ded-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d4ded-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d4ded-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d4ded-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /termStore
```

## <a name="request-headers"></a><span data-ttu-id="d4ded-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d4ded-118">Request headers</span></span>
|<span data-ttu-id="d4ded-119">Имя</span><span class="sxs-lookup"><span data-stu-id="d4ded-119">Name</span></span>|<span data-ttu-id="d4ded-120">Описание</span><span class="sxs-lookup"><span data-stu-id="d4ded-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="d4ded-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d4ded-121">Authorization</span></span>|<span data-ttu-id="d4ded-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d4ded-p102">Bearer {token}. Required.</span></span>|

## <a name="response"></a><span data-ttu-id="d4ded-124">Отклик</span><span class="sxs-lookup"><span data-stu-id="d4ded-124">Response</span></span>

<span data-ttu-id="d4ded-125">В случае успеха этот метод возвращает код отклика и `200 OK` объект [store](../resources/termstore-store.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d4ded-125">If successful, this method returns a `200 OK` response code and a [store](../resources/termstore-store.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d4ded-126">Примеры</span><span class="sxs-lookup"><span data-stu-id="d4ded-126">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d4ded-127">Запрос</span><span class="sxs-lookup"><span data-stu-id="d4ded-127">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="d4ded-128">HTTP</span><span class="sxs-lookup"><span data-stu-id="d4ded-128">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_store"
}-->

``` http
GET https://graph.microsoft.com/beta/termStore
```
# <a name="c"></a>[<span data-ttu-id="d4ded-129">C#</span><span class="sxs-lookup"><span data-stu-id="d4ded-129">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-store-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d4ded-130">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d4ded-130">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-store-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d4ded-131">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d4ded-131">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-store-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d4ded-132">Java</span><span class="sxs-lookup"><span data-stu-id="d4ded-132">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-store-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="d4ded-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="d4ded-133">Response</span></span>
<span data-ttu-id="d4ded-134">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="d4ded-134">**Note:** The response object shown here might be shortened for readability.</span></span>

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



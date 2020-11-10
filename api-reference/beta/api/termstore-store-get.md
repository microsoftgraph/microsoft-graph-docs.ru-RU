---
title: Получение хранилища
description: Считывание свойств и связей объекта Store.
author: mohitpcad
localization_priority: Normal
ms.prod: Sharepoint
doc_type: apiPageType
ms.openlocfilehash: 05175c566aa3c9ea516b9c5126754c0dce348571
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48972352"
---
# <a name="get-store"></a><span data-ttu-id="ae0fe-103">Получение хранилища</span><span class="sxs-lookup"><span data-stu-id="ae0fe-103">Get store</span></span>
<span data-ttu-id="ae0fe-104">Пространство имен: Microsoft. Graph. банка</span><span class="sxs-lookup"><span data-stu-id="ae0fe-104">Namespace: microsoft.graph.termStore</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ae0fe-105">Считывание свойств и связей объекта [Store](../resources/termstore-store.md) .</span><span class="sxs-lookup"><span data-stu-id="ae0fe-105">Read the properties and relationships of a [store](../resources/termstore-store.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="ae0fe-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ae0fe-106">Permissions</span></span>
<span data-ttu-id="ae0fe-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ae0fe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ae0fe-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ae0fe-109">Permission type</span></span>|<span data-ttu-id="ae0fe-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ae0fe-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ae0fe-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ae0fe-111">Delegated (work or school account)</span></span> | <span data-ttu-id="ae0fe-112">Банк. чтение. ALL, банк. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="ae0fe-112">TermStore.Read.All, TermStore.ReadWrite.All</span></span> |
|<span data-ttu-id="ae0fe-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ae0fe-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ae0fe-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ae0fe-114">Not supported.</span></span>    |
|<span data-ttu-id="ae0fe-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ae0fe-115">Application</span></span> | <span data-ttu-id="ae0fe-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ae0fe-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ae0fe-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ae0fe-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /termStore
```

## <a name="request-headers"></a><span data-ttu-id="ae0fe-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ae0fe-118">Request headers</span></span>
|<span data-ttu-id="ae0fe-119">Имя</span><span class="sxs-lookup"><span data-stu-id="ae0fe-119">Name</span></span>|<span data-ttu-id="ae0fe-120">Описание</span><span class="sxs-lookup"><span data-stu-id="ae0fe-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="ae0fe-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ae0fe-121">Authorization</span></span>|<span data-ttu-id="ae0fe-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ae0fe-p102">Bearer {token}. Required.</span></span>|

## <a name="response"></a><span data-ttu-id="ae0fe-124">Отклик</span><span class="sxs-lookup"><span data-stu-id="ae0fe-124">Response</span></span>

<span data-ttu-id="ae0fe-125">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [Store](../resources/termstore-store.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ae0fe-125">If successful, this method returns a `200 OK` response code and a [store](../resources/termstore-store.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ae0fe-126">Примеры</span><span class="sxs-lookup"><span data-stu-id="ae0fe-126">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ae0fe-127">Запрос</span><span class="sxs-lookup"><span data-stu-id="ae0fe-127">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="ae0fe-128">HTTP</span><span class="sxs-lookup"><span data-stu-id="ae0fe-128">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_store"
}-->

``` http
GET https://graph.microsoft.com/beta/termStore
```
# <a name="c"></a>[<span data-ttu-id="ae0fe-129">C#</span><span class="sxs-lookup"><span data-stu-id="ae0fe-129">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-store-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ae0fe-130">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ae0fe-130">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-store-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ae0fe-131">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ae0fe-131">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-store-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ae0fe-132">Java</span><span class="sxs-lookup"><span data-stu-id="ae0fe-132">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-store-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="ae0fe-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="ae0fe-133">Response</span></span>
<span data-ttu-id="ae0fe-134">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="ae0fe-134">**Note:** The response object shown here might be shortened for readability.</span></span>

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



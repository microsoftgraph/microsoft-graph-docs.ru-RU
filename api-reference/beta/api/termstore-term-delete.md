---
title: Удаление термина
description: Удаление объекта термина.
author: mohitpcad
localization_priority: Normal
ms.prod: Sharepoint
doc_type: apiPageType
ms.openlocfilehash: 706ad5b9457014de236485f526db994dd8a29866
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/15/2021
ms.locfileid: "49874377"
---
# <a name="delete-term"></a><span data-ttu-id="23fa5-103">Удаление термина</span><span class="sxs-lookup"><span data-stu-id="23fa5-103">Delete term</span></span>
<span data-ttu-id="23fa5-104">Пространство имен: microsoft.graph.termStore</span><span class="sxs-lookup"><span data-stu-id="23fa5-104">Namespace: microsoft.graph.termStore</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="23fa5-105">Удаление объекта [термина.](../resources/termstore-term.md)</span><span class="sxs-lookup"><span data-stu-id="23fa5-105">Delete a [term](../resources/termstore-term.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="23fa5-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="23fa5-106">Permissions</span></span>
<span data-ttu-id="23fa5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="23fa5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="23fa5-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="23fa5-109">Permission type</span></span>|<span data-ttu-id="23fa5-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="23fa5-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="23fa5-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="23fa5-111">Delegated (work or school account)</span></span> |<span data-ttu-id="23fa5-112">TermStore.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="23fa5-112">TermStore.ReadWrite.All</span></span> |
|<span data-ttu-id="23fa5-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="23fa5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="23fa5-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="23fa5-114">Not supported.</span></span>    |
|<span data-ttu-id="23fa5-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="23fa5-115">Application</span></span> | <span data-ttu-id="23fa5-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="23fa5-116">Not supported.</span></span> |


## <a name="http-request"></a><span data-ttu-id="23fa5-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="23fa5-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /termStore/sets/{setId}/terms/{termId}
```

## <a name="request-headers"></a><span data-ttu-id="23fa5-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="23fa5-118">Request headers</span></span>
|<span data-ttu-id="23fa5-119">Имя</span><span class="sxs-lookup"><span data-stu-id="23fa5-119">Name</span></span>|<span data-ttu-id="23fa5-120">Описание</span><span class="sxs-lookup"><span data-stu-id="23fa5-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="23fa5-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="23fa5-121">Authorization</span></span>|<span data-ttu-id="23fa5-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="23fa5-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="23fa5-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="23fa5-124">Request body</span></span>
<span data-ttu-id="23fa5-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="23fa5-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="23fa5-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="23fa5-126">Response</span></span>

<span data-ttu-id="23fa5-127">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="23fa5-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="23fa5-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="23fa5-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="23fa5-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="23fa5-129">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="23fa5-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="23fa5-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_term"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/termStore/sets/{setId}/terms/{termId}
```
# <a name="c"></a>[<span data-ttu-id="23fa5-131">C#</span><span class="sxs-lookup"><span data-stu-id="23fa5-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-term-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="23fa5-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="23fa5-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-term-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="23fa5-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="23fa5-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-term-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="23fa5-134">Java</span><span class="sxs-lookup"><span data-stu-id="23fa5-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-term-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="23fa5-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="23fa5-135">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

[microsoft.graph.termStore.term]: ../resources/termstore-term.md

<!--
{
  "type": "#page.annotation",
  "description": "Delete a term entity in termStore",
  "keywords": "term,termStore",
  "section": "documentation",
  "tocPath": "termStore/Delete term",
  "suppressions": [
  ]
}
-->



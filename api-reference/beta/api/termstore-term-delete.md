---
title: Удаление термина
description: Удаление объекта Term.
author: mohitpcad
localization_priority: Normal
ms.prod: Sharepoint
doc_type: apiPageType
ms.openlocfilehash: 9fe4d60e81a6124fbb7745c40864ef66ac5de40a
ms.sourcegitcommit: 726f20403323be7d267b67c2764ed7c244e02ee1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/02/2020
ms.locfileid: "47330032"
---
# <a name="delete-term"></a><span data-ttu-id="27311-103">Удаление термина</span><span class="sxs-lookup"><span data-stu-id="27311-103">Delete term</span></span>
<span data-ttu-id="27311-104">Пространство имен: Microsoft. Graph. банка</span><span class="sxs-lookup"><span data-stu-id="27311-104">Namespace: microsoft.graph.termStore</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="27311-105">Удаление объекта [Term](../resources/termstore-term.md) .</span><span class="sxs-lookup"><span data-stu-id="27311-105">Delete a [term](../resources/termstore-term.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="27311-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="27311-106">Permissions</span></span>
<span data-ttu-id="27311-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="27311-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="27311-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="27311-109">Permission type</span></span>|<span data-ttu-id="27311-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="27311-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="27311-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="27311-111">Delegated (work or school account)</span></span> |<span data-ttu-id="27311-112">TermStore.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="27311-112">TermStore.ReadWrite.All</span></span> |
|<span data-ttu-id="27311-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="27311-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="27311-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="27311-114">Not supported.</span></span>    |
|<span data-ttu-id="27311-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="27311-115">Application</span></span> | <span data-ttu-id="27311-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="27311-116">Not supported.</span></span> |


## <a name="http-request"></a><span data-ttu-id="27311-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="27311-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /termStore/sets/{setId}/terms/{termId}
```

## <a name="request-headers"></a><span data-ttu-id="27311-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="27311-118">Request headers</span></span>
|<span data-ttu-id="27311-119">Имя</span><span class="sxs-lookup"><span data-stu-id="27311-119">Name</span></span>|<span data-ttu-id="27311-120">Описание</span><span class="sxs-lookup"><span data-stu-id="27311-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="27311-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="27311-121">Authorization</span></span>|<span data-ttu-id="27311-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="27311-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="27311-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="27311-124">Request body</span></span>
<span data-ttu-id="27311-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="27311-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="27311-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="27311-126">Response</span></span>

<span data-ttu-id="27311-127">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="27311-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="27311-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="27311-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="27311-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="27311-129">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="27311-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="27311-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_term"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/termStore/sets/{setId}/terms/{termId}
```
# <a name="c"></a>[<span data-ttu-id="27311-131">C#</span><span class="sxs-lookup"><span data-stu-id="27311-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-term-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="27311-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="27311-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-term-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="27311-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="27311-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-term-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="27311-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="27311-134">Response</span></span>
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

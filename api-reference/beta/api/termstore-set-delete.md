---
title: Удаление набора
description: Удаление объекта Set.
author: mohitpcad
localization_priority: Normal
ms.prod: Sharepoint
doc_type: apiPageType
ms.openlocfilehash: 725cc8e44b47007a8f039f1855ef3cfdf0039d27
ms.sourcegitcommit: 726f20403323be7d267b67c2764ed7c244e02ee1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/02/2020
ms.locfileid: "47330442"
---
# <a name="delete-set"></a><span data-ttu-id="9b702-103">Удаление набора</span><span class="sxs-lookup"><span data-stu-id="9b702-103">Delete set</span></span>
<span data-ttu-id="9b702-104">Пространство имен: Microsoft. Graph. банка</span><span class="sxs-lookup"><span data-stu-id="9b702-104">Namespace: microsoft.graph.termStore</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9b702-105">Удаление объекта [Set](../resources/termstore-set.md) .</span><span class="sxs-lookup"><span data-stu-id="9b702-105">Delete a [set](../resources/termstore-set.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="9b702-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9b702-106">Permissions</span></span>
<span data-ttu-id="9b702-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9b702-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9b702-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9b702-109">Permission type</span></span>|<span data-ttu-id="9b702-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9b702-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9b702-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9b702-111">Delegated (work or school account)</span></span> |<span data-ttu-id="9b702-112">TermStore.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9b702-112">TermStore.ReadWrite.All</span></span> |
|<span data-ttu-id="9b702-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9b702-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9b702-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9b702-114">Not supported.</span></span>    |
|<span data-ttu-id="9b702-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9b702-115">Application</span></span> | <span data-ttu-id="9b702-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9b702-116">Not supported.</span></span> |


## <a name="http-request"></a><span data-ttu-id="9b702-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9b702-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /termStore/sets/{setId}
```

## <a name="request-headers"></a><span data-ttu-id="9b702-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9b702-118">Request headers</span></span>
|<span data-ttu-id="9b702-119">Имя</span><span class="sxs-lookup"><span data-stu-id="9b702-119">Name</span></span>|<span data-ttu-id="9b702-120">Описание</span><span class="sxs-lookup"><span data-stu-id="9b702-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="9b702-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9b702-121">Authorization</span></span>|<span data-ttu-id="9b702-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9b702-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9b702-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9b702-124">Request body</span></span>
<span data-ttu-id="9b702-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9b702-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9b702-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="9b702-126">Response</span></span>

<span data-ttu-id="9b702-127">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="9b702-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="9b702-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="9b702-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="9b702-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="9b702-129">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="9b702-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="9b702-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_set"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/termStore/sets/{setId}
```
# <a name="c"></a>[<span data-ttu-id="9b702-131">C#</span><span class="sxs-lookup"><span data-stu-id="9b702-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-set-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9b702-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9b702-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-set-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9b702-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9b702-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-set-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="9b702-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="9b702-134">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

[microsoft.graph.termStore.group]: ../resources/termstore-group.md
[microsoft.graph.termStore.set]: ../resources/termstore-set.md

<!--
{
  "type": "#page.annotation",
  "description": "Delete a termSet entity in termStore",
  "keywords": "term,termStore",
  "section": "documentation",
  "tocPath": "termStore/Delete termSet",
  "suppressions": [
  ]
}
-->

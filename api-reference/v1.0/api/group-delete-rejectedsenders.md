---
title: Удаление объекта rejectedSender
description: Удаление пользователя или группы из списка отклоненных отправителей.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: dd73afd18dc7112e4506580ade0a664f3730df52
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42517182"
---
# <a name="remove-rejectedsender"></a><span data-ttu-id="eec13-103">Удаление объекта rejectedSender</span><span class="sxs-lookup"><span data-stu-id="eec13-103">Remove rejectedSender</span></span>

<span data-ttu-id="eec13-104">Пространство имен: Microsoft. Graph удаление пользователя или группы из списка отклоненных отправителей.</span><span class="sxs-lookup"><span data-stu-id="eec13-104">Namespace: microsoft.graph Remove a user or group from the rejected-senders list.</span></span>

## <a name="permissions"></a><span data-ttu-id="eec13-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="eec13-105">Permissions</span></span>
<span data-ttu-id="eec13-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eec13-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="eec13-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="eec13-108">Permission type</span></span>                        | <span data-ttu-id="eec13-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="eec13-109">Permissions (from least to most privileged)</span></span>  |
|:---------------------------------------|:-------------------------------------------- |
| <span data-ttu-id="eec13-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="eec13-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="eec13-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eec13-111">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="eec13-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="eec13-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eec13-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eec13-113">Not supported.</span></span> |
| <span data-ttu-id="eec13-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="eec13-114">Application</span></span>                            | <span data-ttu-id="eec13-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eec13-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="eec13-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="eec13-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/rejectedSenders/$ref?$id=https://graph.microsoft.com/v1.0/users/{user-id}
DELETE /groups/{id}/rejectedSenders/$ref?$id=https://graph.microsoft.com/v1.0/groups/{other-group-id}
```

## <a name="request-headers"></a><span data-ttu-id="eec13-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="eec13-117">Request headers</span></span>

| <span data-ttu-id="eec13-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="eec13-118">Header</span></span>         | <span data-ttu-id="eec13-119">Значение</span><span class="sxs-lookup"><span data-stu-id="eec13-119">Value</span></span>                      |
|:---------------|:---------------------------|
| <span data-ttu-id="eec13-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="eec13-120">Authorization</span></span>  | <span data-ttu-id="eec13-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="eec13-p102">Bearer {token}. Required.</span></span> 

## <a name="request-body"></a><span data-ttu-id="eec13-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="eec13-123">Request body</span></span>
<span data-ttu-id="eec13-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="eec13-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="eec13-125">Ответ</span><span class="sxs-lookup"><span data-stu-id="eec13-125">Response</span></span>
<span data-ttu-id="eec13-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="eec13-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eec13-128">Пример</span><span class="sxs-lookup"><span data-stu-id="eec13-128">Example</span></span>
#### <a name="request"></a><span data-ttu-id="eec13-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="eec13-129">Request</span></span>
<span data-ttu-id="eec13-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="eec13-130">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="eec13-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="eec13-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "remove_rejectedSender_from_group"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groups/{id}/rejectedSenders/$ref?$id=https://graph.microsoft.com/v1.0/users/{user-id}
```
# <a name="c"></a>[<span data-ttu-id="eec13-132">C#</span><span class="sxs-lookup"><span data-stu-id="eec13-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/remove-rejectedsender-from-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="eec13-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="eec13-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/remove-rejectedsender-from-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="eec13-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="eec13-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/remove-rejectedsender-from-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="eec13-135">Java</span><span class="sxs-lookup"><span data-stu-id="eec13-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/remove-rejectedsender-from-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="eec13-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="eec13-136">Response</span></span>
<span data-ttu-id="eec13-137">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="eec13-137">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Remove rejectedSender",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

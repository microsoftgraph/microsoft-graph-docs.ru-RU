---
title: Удаление messageRule
description: Удаление указанного объекта messageRule.
author: svpsiva
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: cef718dc2f9ef23cc006ba61a3cde71c38d2b1c8
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48019049"
---
# <a name="delete-messagerule"></a><span data-ttu-id="a7366-103">Удаление messageRule</span><span class="sxs-lookup"><span data-stu-id="a7366-103">Delete messageRule</span></span>

<span data-ttu-id="a7366-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a7366-104">Namespace: microsoft.graph</span></span>


<span data-ttu-id="a7366-105">Удаление указанного объекта [messageRule](../resources/messagerule.md).</span><span class="sxs-lookup"><span data-stu-id="a7366-105">Delete the specified [messageRule](../resources/messagerule.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="a7366-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a7366-106">Permissions</span></span>
<span data-ttu-id="a7366-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a7366-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a7366-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a7366-109">Permission type</span></span>      | <span data-ttu-id="a7366-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a7366-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a7366-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a7366-111">Delegated (work or school account)</span></span> | <span data-ttu-id="a7366-112">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a7366-112">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="a7366-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a7366-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a7366-114">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a7366-114">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="a7366-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a7366-115">Application</span></span> | <span data-ttu-id="a7366-116">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a7366-116">MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="a7366-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a7366-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/mailFolders/inbox/messageRules/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/inbox/messageRules/{id}
```
## <a name="request-headers"></a><span data-ttu-id="a7366-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a7366-118">Request headers</span></span>
| <span data-ttu-id="a7366-119">Имя</span><span class="sxs-lookup"><span data-stu-id="a7366-119">Name</span></span>       | <span data-ttu-id="a7366-120">Описание</span><span class="sxs-lookup"><span data-stu-id="a7366-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="a7366-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a7366-121">Authorization</span></span>  | <span data-ttu-id="a7366-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a7366-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="a7366-124">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a7366-124">Request body</span></span>
<span data-ttu-id="a7366-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a7366-125">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="a7366-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="a7366-126">Response</span></span>
<span data-ttu-id="a7366-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="a7366-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a7366-129">Пример</span><span class="sxs-lookup"><span data-stu-id="a7366-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a7366-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="a7366-130">Request</span></span>
<span data-ttu-id="a7366-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a7366-131">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a7366-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="a7366-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["inbox", "AQAAAJ5dZp8="],
  "name": "delete_messagerule"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/mailFolders/inbox/messageRules/AQAAAJ5dZp8=

```
# <a name="c"></a>[<span data-ttu-id="a7366-133">C#</span><span class="sxs-lookup"><span data-stu-id="a7366-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-messagerule-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a7366-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a7366-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-messagerule-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a7366-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a7366-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-messagerule-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a7366-136">Java</span><span class="sxs-lookup"><span data-stu-id="a7366-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-messagerule-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="a7366-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="a7366-137">Response</span></span>
<span data-ttu-id="a7366-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="a7366-138">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "isEmpty": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete rule",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->


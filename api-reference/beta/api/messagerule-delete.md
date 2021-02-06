---
title: Удаление messageRule
description: Удаление указанного объекта messageRule.
author: abheek-das
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 6b8486fcfafaf971261dd56b5639ac37c7cc8e80
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50131084"
---
# <a name="delete-messagerule"></a><span data-ttu-id="4b21d-103">Удаление messageRule</span><span class="sxs-lookup"><span data-stu-id="4b21d-103">Delete messageRule</span></span>

<span data-ttu-id="4b21d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4b21d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4b21d-105">Удаление указанного объекта [messageRule](../resources/messagerule.md).</span><span class="sxs-lookup"><span data-stu-id="4b21d-105">Delete the specified [messageRule](../resources/messagerule.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="4b21d-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4b21d-106">Permissions</span></span>
<span data-ttu-id="4b21d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4b21d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4b21d-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4b21d-109">Permission type</span></span>      | <span data-ttu-id="4b21d-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4b21d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4b21d-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4b21d-111">Delegated (work or school account)</span></span> | <span data-ttu-id="4b21d-112">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4b21d-112">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="4b21d-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4b21d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4b21d-114">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4b21d-114">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="4b21d-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4b21d-115">Application</span></span> | <span data-ttu-id="4b21d-116">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4b21d-116">MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="4b21d-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4b21d-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/mailFolders/inbox/messagerules/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/inbox/messagerules/{id}
```
## <a name="request-headers"></a><span data-ttu-id="4b21d-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4b21d-118">Request headers</span></span>
| <span data-ttu-id="4b21d-119">Имя</span><span class="sxs-lookup"><span data-stu-id="4b21d-119">Name</span></span>       | <span data-ttu-id="4b21d-120">Описание</span><span class="sxs-lookup"><span data-stu-id="4b21d-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="4b21d-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4b21d-121">Authorization</span></span>  | <span data-ttu-id="4b21d-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4b21d-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="4b21d-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4b21d-124">Request body</span></span>
<span data-ttu-id="4b21d-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4b21d-125">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="4b21d-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="4b21d-126">Response</span></span>
<span data-ttu-id="4b21d-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="4b21d-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4b21d-129">Пример</span><span class="sxs-lookup"><span data-stu-id="4b21d-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4b21d-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="4b21d-130">Request</span></span>
<span data-ttu-id="4b21d-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4b21d-131">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4b21d-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="4b21d-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_messagerule"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/mailfolders/inbox/messagerules('AQAAAJ5dZp8=')

```
# <a name="c"></a>[<span data-ttu-id="4b21d-133">C#</span><span class="sxs-lookup"><span data-stu-id="4b21d-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-messagerule-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4b21d-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4b21d-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-messagerule-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4b21d-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4b21d-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-messagerule-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4b21d-136">Java</span><span class="sxs-lookup"><span data-stu-id="4b21d-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-messagerule-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="4b21d-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="4b21d-137">Response</span></span>
<span data-ttu-id="4b21d-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4b21d-138">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "isEmpty": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete rule",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->



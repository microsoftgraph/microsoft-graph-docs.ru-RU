---
title: Удаление messageRule
description: Удаление указанного объекта messageRule.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 177b66649bae0ed78ffde2b689e20aee21dcf68b
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36342791"
---
# <a name="delete-messagerule"></a><span data-ttu-id="db81b-103">Удаление messageRule</span><span class="sxs-lookup"><span data-stu-id="db81b-103">Delete messageRule</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="db81b-104">Удаление указанного объекта [messageRule](../resources/messagerule.md).</span><span class="sxs-lookup"><span data-stu-id="db81b-104">Delete the specified [messageRule](../resources/messagerule.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="db81b-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="db81b-105">Permissions</span></span>
<span data-ttu-id="db81b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="db81b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="db81b-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="db81b-108">Permission type</span></span>      | <span data-ttu-id="db81b-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="db81b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="db81b-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="db81b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="db81b-111">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="db81b-111">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="db81b-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="db81b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="db81b-113">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="db81b-113">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="db81b-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="db81b-114">Application</span></span> | <span data-ttu-id="db81b-115">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="db81b-115">MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="db81b-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="db81b-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/mailFolders/inbox/messagerules/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/inbox/messagerules/{id}
```
## <a name="request-headers"></a><span data-ttu-id="db81b-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="db81b-117">Request headers</span></span>
| <span data-ttu-id="db81b-118">Имя</span><span class="sxs-lookup"><span data-stu-id="db81b-118">Name</span></span>       | <span data-ttu-id="db81b-119">Описание</span><span class="sxs-lookup"><span data-stu-id="db81b-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="db81b-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="db81b-120">Authorization</span></span>  | <span data-ttu-id="db81b-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="db81b-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="db81b-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="db81b-123">Request body</span></span>
<span data-ttu-id="db81b-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="db81b-124">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="db81b-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="db81b-125">Response</span></span>
<span data-ttu-id="db81b-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="db81b-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="db81b-128">Пример</span><span class="sxs-lookup"><span data-stu-id="db81b-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="db81b-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="db81b-129">Request</span></span>
<span data-ttu-id="db81b-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="db81b-130">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="db81b-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="db81b-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_messagerule"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/mailfolders/inbox/messagerules('AQAAAJ5dZp8=')

```
# <a name="ctabcsharp"></a>[<span data-ttu-id="db81b-132">C#</span><span class="sxs-lookup"><span data-stu-id="db81b-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-messagerule-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="db81b-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="db81b-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-messagerule-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="db81b-134">Цель — C</span><span class="sxs-lookup"><span data-stu-id="db81b-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-messagerule-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="db81b-135">Java</span><span class="sxs-lookup"><span data-stu-id="db81b-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-messagerule-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="db81b-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="db81b-136">Response</span></span>
<span data-ttu-id="db81b-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="db81b-137">Here is an example of the response.</span></span> 
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

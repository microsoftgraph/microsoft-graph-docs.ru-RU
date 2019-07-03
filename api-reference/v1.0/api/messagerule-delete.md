---
title: Удаление messageRule
description: Удаление указанного объекта messageRule.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 169ea8adbfeb976b1ec10b2ed3b00e4a5b4fbddb
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35449325"
---
# <a name="delete-messagerule"></a><span data-ttu-id="614d3-103">Удаление messageRule</span><span class="sxs-lookup"><span data-stu-id="614d3-103">Delete messageRule</span></span>


<span data-ttu-id="614d3-104">Удаление указанного объекта [messageRule](../resources/messagerule.md).</span><span class="sxs-lookup"><span data-stu-id="614d3-104">Delete the specified [messageRule](../resources/messagerule.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="614d3-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="614d3-105">Permissions</span></span>
<span data-ttu-id="614d3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="614d3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="614d3-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="614d3-108">Permission type</span></span>      | <span data-ttu-id="614d3-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="614d3-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="614d3-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="614d3-110">Delegated (work or school account)</span></span> | <span data-ttu-id="614d3-111">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="614d3-111">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="614d3-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="614d3-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="614d3-113">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="614d3-113">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="614d3-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="614d3-114">Application</span></span> | <span data-ttu-id="614d3-115">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="614d3-115">MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="614d3-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="614d3-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/mailFolders/inbox/messageRules/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/inbox/messageRules/{id}
```
## <a name="request-headers"></a><span data-ttu-id="614d3-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="614d3-117">Request headers</span></span>
| <span data-ttu-id="614d3-118">Имя</span><span class="sxs-lookup"><span data-stu-id="614d3-118">Name</span></span>       | <span data-ttu-id="614d3-119">Описание</span><span class="sxs-lookup"><span data-stu-id="614d3-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="614d3-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="614d3-120">Authorization</span></span>  | <span data-ttu-id="614d3-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="614d3-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="614d3-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="614d3-123">Request body</span></span>
<span data-ttu-id="614d3-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="614d3-124">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="614d3-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="614d3-125">Response</span></span>
<span data-ttu-id="614d3-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="614d3-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="614d3-128">Пример</span><span class="sxs-lookup"><span data-stu-id="614d3-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="614d3-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="614d3-129">Request</span></span>
<span data-ttu-id="614d3-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="614d3-130">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="614d3-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="614d3-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["inbox", "AQAAAJ5dZp8="],
  "name": "delete_messagerule"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/mailFolders/inbox/messageRules/AQAAAJ5dZp8=

```
# <a name="ctabcsharp"></a>[<span data-ttu-id="614d3-132">C#</span><span class="sxs-lookup"><span data-stu-id="614d3-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-messagerule-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="614d3-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="614d3-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-messagerule-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="614d3-134">Цель — C</span><span class="sxs-lookup"><span data-stu-id="614d3-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-messagerule-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="614d3-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="614d3-135">Response</span></span>
<span data-ttu-id="614d3-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="614d3-136">Here is an example of the response.</span></span> 
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

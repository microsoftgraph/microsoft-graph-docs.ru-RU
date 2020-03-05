---
title: Удаление messageRule
description: Удаление указанного объекта messageRule.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 1406b7b453b909109177ea7912028ea55bfa567c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42456861"
---
# <a name="delete-messagerule"></a><span data-ttu-id="31cc0-103">Удаление messageRule</span><span class="sxs-lookup"><span data-stu-id="31cc0-103">Delete messageRule</span></span>

<span data-ttu-id="31cc0-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="31cc0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="31cc0-105">Удаление указанного объекта [messageRule](../resources/messagerule.md).</span><span class="sxs-lookup"><span data-stu-id="31cc0-105">Delete the specified [messageRule](../resources/messagerule.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="31cc0-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="31cc0-106">Permissions</span></span>
<span data-ttu-id="31cc0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="31cc0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="31cc0-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="31cc0-109">Permission type</span></span>      | <span data-ttu-id="31cc0-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="31cc0-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="31cc0-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="31cc0-111">Delegated (work or school account)</span></span> | <span data-ttu-id="31cc0-112">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="31cc0-112">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="31cc0-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="31cc0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="31cc0-114">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="31cc0-114">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="31cc0-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="31cc0-115">Application</span></span> | <span data-ttu-id="31cc0-116">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="31cc0-116">MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="31cc0-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="31cc0-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/mailFolders/inbox/messagerules/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/inbox/messagerules/{id}
```
## <a name="request-headers"></a><span data-ttu-id="31cc0-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="31cc0-118">Request headers</span></span>
| <span data-ttu-id="31cc0-119">Имя</span><span class="sxs-lookup"><span data-stu-id="31cc0-119">Name</span></span>       | <span data-ttu-id="31cc0-120">Описание</span><span class="sxs-lookup"><span data-stu-id="31cc0-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="31cc0-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="31cc0-121">Authorization</span></span>  | <span data-ttu-id="31cc0-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="31cc0-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="31cc0-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="31cc0-124">Request body</span></span>
<span data-ttu-id="31cc0-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="31cc0-125">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="31cc0-126">Ответ</span><span class="sxs-lookup"><span data-stu-id="31cc0-126">Response</span></span>
<span data-ttu-id="31cc0-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="31cc0-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="31cc0-129">Пример</span><span class="sxs-lookup"><span data-stu-id="31cc0-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="31cc0-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="31cc0-130">Request</span></span>
<span data-ttu-id="31cc0-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="31cc0-131">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="31cc0-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="31cc0-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_messagerule"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/mailfolders/inbox/messagerules('AQAAAJ5dZp8=')

```
# <a name="c"></a>[<span data-ttu-id="31cc0-133">C#</span><span class="sxs-lookup"><span data-stu-id="31cc0-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-messagerule-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="31cc0-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="31cc0-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-messagerule-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="31cc0-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="31cc0-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-messagerule-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="31cc0-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="31cc0-136">Response</span></span>
<span data-ttu-id="31cc0-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="31cc0-137">Here is an example of the response.</span></span> 
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

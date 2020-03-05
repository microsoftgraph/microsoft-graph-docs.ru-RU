---
title: Удаление категории Outlook
description: Удаление указанного объекта outlookCategory.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 394d81154a5fde4ef2bb3e271772892ae0a8d90f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42456252"
---
# <a name="delete-outlook-category"></a><span data-ttu-id="646ce-103">Удаление категории Outlook</span><span class="sxs-lookup"><span data-stu-id="646ce-103">Delete Outlook category</span></span>

<span data-ttu-id="646ce-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="646ce-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="646ce-105">Удаление указанного объекта [outlookCategory](../resources/outlookcategory.md).</span><span class="sxs-lookup"><span data-stu-id="646ce-105">Delete the specified [outlookCategory](../resources/outlookcategory.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="646ce-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="646ce-106">Permissions</span></span>
<span data-ttu-id="646ce-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="646ce-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="646ce-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="646ce-109">Permission type</span></span>      | <span data-ttu-id="646ce-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="646ce-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="646ce-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="646ce-111">Delegated (work or school account)</span></span> | <span data-ttu-id="646ce-112">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="646ce-112">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="646ce-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="646ce-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="646ce-114">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="646ce-114">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="646ce-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="646ce-115">Application</span></span> | <span data-ttu-id="646ce-116">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="646ce-116">MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="646ce-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="646ce-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/outlook/masterCategories/{id}
DELETE /users/{id|userPrincipalName}/outlook/masterCategories/{id}
```

## <a name="request-headers"></a><span data-ttu-id="646ce-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="646ce-118">Request headers</span></span>
| <span data-ttu-id="646ce-119">Имя</span><span class="sxs-lookup"><span data-stu-id="646ce-119">Name</span></span>      |<span data-ttu-id="646ce-120">Описание</span><span class="sxs-lookup"><span data-stu-id="646ce-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="646ce-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="646ce-121">Authorization</span></span>  | <span data-ttu-id="646ce-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="646ce-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="646ce-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="646ce-124">Request body</span></span>
<span data-ttu-id="646ce-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="646ce-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="646ce-126">Ответ</span><span class="sxs-lookup"><span data-stu-id="646ce-126">Response</span></span>

<span data-ttu-id="646ce-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="646ce-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="646ce-129">Пример</span><span class="sxs-lookup"><span data-stu-id="646ce-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="646ce-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="646ce-130">Request</span></span>
<span data-ttu-id="646ce-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="646ce-131">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="646ce-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="646ce-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_outlookcategory"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/outlook/masterCategories/4b1c2495-54c9-4a5e-90a2-0ab0b31987d8
```
# <a name="c"></a>[<span data-ttu-id="646ce-133">C#</span><span class="sxs-lookup"><span data-stu-id="646ce-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-outlookcategory-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="646ce-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="646ce-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-outlookcategory-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="646ce-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="646ce-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-outlookcategory-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="646ce-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="646ce-136">Response</span></span>
<span data-ttu-id="646ce-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="646ce-137">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "name": "delete_outlookcategory",
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
  "description": "Delete outlookCategory",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

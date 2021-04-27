---
title: Удаление программы
description: В функции обзоров доступа Azure AD удалите объект программы.
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: markwahl-msft
ms.openlocfilehash: be26ef2876f5aecc171bd262d41a711a0d0b0f3e
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52049844"
---
# <a name="delete-program"></a><span data-ttu-id="85c8c-103">Удаление программы</span><span class="sxs-lookup"><span data-stu-id="85c8c-103">Delete program</span></span>

<span data-ttu-id="85c8c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="85c8c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="85c8c-105">В функции обзоров доступа Azure [AD](../resources/accessreviews-root.md) удалите [объект](../resources/program.md) программы.</span><span class="sxs-lookup"><span data-stu-id="85c8c-105">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, delete a [program](../resources/program.md) object.</span></span>

<span data-ttu-id="85c8c-106">Не удаляйте программу, которая по-прежнему связана с ней, эти обзоры доступа сначала должны быть удалены или отвязаны из программы и связаны `programControl` с другой программой.</span><span class="sxs-lookup"><span data-stu-id="85c8c-106">Do not delete a program which still has `programControl` linked to it, those access reviews should first be deleted or unlinked from the program and linked to a different program.</span></span>  <span data-ttu-id="85c8c-107">Кроме того, обратите внимание, что встроенная программа по умолчанию не может быть удалена.</span><span class="sxs-lookup"><span data-stu-id="85c8c-107">Also, please note that the built-in default program cannot be deleted.</span></span>


## <a name="permissions"></a><span data-ttu-id="85c8c-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="85c8c-108">Permissions</span></span>
<span data-ttu-id="85c8c-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="85c8c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="85c8c-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="85c8c-111">Permission type</span></span>                        | <span data-ttu-id="85c8c-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="85c8c-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="85c8c-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="85c8c-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="85c8c-114">ProgramControl.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="85c8c-114">ProgramControl.ReadWrite.All</span></span>   |
|<span data-ttu-id="85c8c-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="85c8c-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="85c8c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="85c8c-116">Not supported.</span></span> |
|<span data-ttu-id="85c8c-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="85c8c-117">Application</span></span>                            | <span data-ttu-id="85c8c-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="85c8c-118">Not supported.</span></span> |

<span data-ttu-id="85c8c-119">Подписанный пользователь также должен быть в роли каталога, что позволяет им создавать программу.</span><span class="sxs-lookup"><span data-stu-id="85c8c-119">The signed in user must also be in a directory role that permits them to create a program.</span></span>

## <a name="http-request"></a><span data-ttu-id="85c8c-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="85c8c-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /programs/{id}
```
## <a name="request-headers"></a><span data-ttu-id="85c8c-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="85c8c-121">Request headers</span></span>
| <span data-ttu-id="85c8c-122">Имя</span><span class="sxs-lookup"><span data-stu-id="85c8c-122">Name</span></span>         | <span data-ttu-id="85c8c-123">Тип</span><span class="sxs-lookup"><span data-stu-id="85c8c-123">Type</span></span>        | <span data-ttu-id="85c8c-124">Описание</span><span class="sxs-lookup"><span data-stu-id="85c8c-124">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="85c8c-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="85c8c-125">Authorization</span></span> | <span data-ttu-id="85c8c-126">string</span><span class="sxs-lookup"><span data-stu-id="85c8c-126">string</span></span> | <span data-ttu-id="85c8c-p103">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="85c8c-p103">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="85c8c-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="85c8c-129">Request body</span></span>
<span data-ttu-id="85c8c-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="85c8c-130">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="85c8c-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="85c8c-131">Response</span></span>
<span data-ttu-id="85c8c-p104">При успешном выполнении этот метод возвращает код отклика `204, No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="85c8c-p104">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="85c8c-134">Пример</span><span class="sxs-lookup"><span data-stu-id="85c8c-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="85c8c-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="85c8c-135">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="85c8c-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="85c8c-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_program"
}-->
```http
DELETE https://graph.microsoft.com/beta/programs/7e59d237-2fb0-4e5d-b7bb-d4f9f9129213
```
# <a name="c"></a>[<span data-ttu-id="85c8c-137">C#</span><span class="sxs-lookup"><span data-stu-id="85c8c-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-program-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="85c8c-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="85c8c-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-program-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="85c8c-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="85c8c-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-program-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="85c8c-140">Java</span><span class="sxs-lookup"><span data-stu-id="85c8c-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-program-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="85c8c-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="85c8c-141">Response</span></span>
><span data-ttu-id="85c8c-142">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="85c8c-142">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-25 00:00:01 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete program",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->



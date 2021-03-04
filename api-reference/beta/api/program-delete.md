---
title: Удаление программы
description: В функции обзоров доступа Azure AD удалите объект программы.
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: markwahl-msft
ms.openlocfilehash: a80b84aa0835fe0c8fa3e21cf1f8da37e851b394
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50440992"
---
# <a name="delete-program"></a><span data-ttu-id="17581-103">Удаление программы</span><span class="sxs-lookup"><span data-stu-id="17581-103">Delete program</span></span>

<span data-ttu-id="17581-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="17581-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="17581-105">В функции обзоров доступа Azure [AD](../resources/accessreviews-root.md) удалите [объект](../resources/program.md) программы.</span><span class="sxs-lookup"><span data-stu-id="17581-105">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, delete a [program](../resources/program.md) object.</span></span>

<span data-ttu-id="17581-106">Не удаляйте программу, которая по-прежнему связана с ней, эти обзоры доступа сначала должны быть удалены или отвязаны из программы и связаны `programControl` с другой программой.</span><span class="sxs-lookup"><span data-stu-id="17581-106">Do not delete a program which still has `programControl` linked to it, those access reviews should first be deleted or unlinked from the program and linked to a different program.</span></span>  <span data-ttu-id="17581-107">Кроме того, обратите внимание, что встроенная программа по умолчанию не может быть удалена.</span><span class="sxs-lookup"><span data-stu-id="17581-107">Also, please note that the built-in default program cannot be deleted.</span></span>


## <a name="permissions"></a><span data-ttu-id="17581-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="17581-108">Permissions</span></span>
<span data-ttu-id="17581-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="17581-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="17581-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="17581-111">Permission type</span></span>                        | <span data-ttu-id="17581-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="17581-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="17581-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="17581-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="17581-114">ProgramControl.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="17581-114">ProgramControl.ReadWrite.All</span></span>   |
|<span data-ttu-id="17581-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="17581-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="17581-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="17581-116">Not supported.</span></span> |
|<span data-ttu-id="17581-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="17581-117">Application</span></span>                            | <span data-ttu-id="17581-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="17581-118">Not supported.</span></span> |

<span data-ttu-id="17581-119">Подписанный пользователь также должен быть в роли каталога, что позволяет им создавать программу.</span><span class="sxs-lookup"><span data-stu-id="17581-119">The signed in user must also be in a directory role that permits them to create a program.</span></span>

## <a name="http-request"></a><span data-ttu-id="17581-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="17581-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /programs/{id}
```
## <a name="request-headers"></a><span data-ttu-id="17581-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="17581-121">Request headers</span></span>
| <span data-ttu-id="17581-122">Имя</span><span class="sxs-lookup"><span data-stu-id="17581-122">Name</span></span>         | <span data-ttu-id="17581-123">Тип</span><span class="sxs-lookup"><span data-stu-id="17581-123">Type</span></span>        | <span data-ttu-id="17581-124">Описание</span><span class="sxs-lookup"><span data-stu-id="17581-124">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="17581-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="17581-125">Authorization</span></span> | <span data-ttu-id="17581-126">string</span><span class="sxs-lookup"><span data-stu-id="17581-126">string</span></span> | <span data-ttu-id="17581-p103">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="17581-p103">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="17581-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="17581-129">Request body</span></span>
<span data-ttu-id="17581-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="17581-130">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="17581-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="17581-131">Response</span></span>
<span data-ttu-id="17581-p104">При успешном выполнении этот метод возвращает код отклика `204, No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="17581-p104">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="17581-134">Пример</span><span class="sxs-lookup"><span data-stu-id="17581-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="17581-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="17581-135">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="17581-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="17581-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_program"
}-->
```http
DELETE https://graph.microsoft.com/beta/programs/7e59d237-2fb0-4e5d-b7bb-d4f9f9129213
```
# <a name="c"></a>[<span data-ttu-id="17581-137">C#</span><span class="sxs-lookup"><span data-stu-id="17581-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-program-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="17581-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="17581-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-program-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="17581-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="17581-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-program-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="17581-140">Java</span><span class="sxs-lookup"><span data-stu-id="17581-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-program-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="17581-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="17581-141">Response</span></span>
><span data-ttu-id="17581-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="17581-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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



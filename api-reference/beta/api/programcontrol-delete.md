---
title: Удаление Програмконтрол
description: В функции рецензирования Access Azure AD удалите объект Програмконтрол.  Это отменяет связь с проверкой доступа из программы.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: markwahl-msft
ms.openlocfilehash: a6b6d52e7699517555db22dee92a116af1f37c58
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48969454"
---
# <a name="delete-programcontrol"></a><span data-ttu-id="da1c4-104">Удаление Програмконтрол</span><span class="sxs-lookup"><span data-stu-id="da1c4-104">Delete programControl</span></span>

<span data-ttu-id="da1c4-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="da1c4-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="da1c4-106">В функции [рецензирования Access](../resources/accessreviews-root.md) Azure AD удалите объект [програмконтрол](../resources/programcontrol.md) .</span><span class="sxs-lookup"><span data-stu-id="da1c4-106">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, delete a [programControl](../resources/programcontrol.md) object.</span></span>  <span data-ttu-id="da1c4-107">Это отменяет связь с проверкой доступа из программы.</span><span class="sxs-lookup"><span data-stu-id="da1c4-107">This unlinks an access review from a program.</span></span>
## <a name="permissions"></a><span data-ttu-id="da1c4-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="da1c4-108">Permissions</span></span>
<span data-ttu-id="da1c4-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="da1c4-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="da1c4-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="da1c4-111">Permission type</span></span>                        | <span data-ttu-id="da1c4-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="da1c4-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="da1c4-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="da1c4-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="da1c4-114">ProgramControl.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="da1c4-114">ProgramControl.ReadWrite.All</span></span>   |
|<span data-ttu-id="da1c4-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="da1c4-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="da1c4-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="da1c4-116">Not supported.</span></span> |
|<span data-ttu-id="da1c4-117">Для приложения</span><span class="sxs-lookup"><span data-stu-id="da1c4-117">Application</span></span>                            | <span data-ttu-id="da1c4-118">ProgramControl.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="da1c4-118">ProgramControl.ReadWrite.All</span></span>  |

<span data-ttu-id="da1c4-119">Пользователь, вошедшего в систему, также должен находиться в роли каталога, который разрешает им удалять `programControl` .</span><span class="sxs-lookup"><span data-stu-id="da1c4-119">The signed in user must also be in a directory role that permits them to delete a `programControl`.</span></span>

## <a name="http-request"></a><span data-ttu-id="da1c4-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="da1c4-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /programControls/{id}
```
## <a name="request-headers"></a><span data-ttu-id="da1c4-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="da1c4-121">Request headers</span></span>
| <span data-ttu-id="da1c4-122">Имя</span><span class="sxs-lookup"><span data-stu-id="da1c4-122">Name</span></span>         | <span data-ttu-id="da1c4-123">Тип</span><span class="sxs-lookup"><span data-stu-id="da1c4-123">Type</span></span>        | <span data-ttu-id="da1c4-124">Описание</span><span class="sxs-lookup"><span data-stu-id="da1c4-124">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="da1c4-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="da1c4-125">Authorization</span></span> | <span data-ttu-id="da1c4-126">string</span><span class="sxs-lookup"><span data-stu-id="da1c4-126">string</span></span> | <span data-ttu-id="da1c4-p104">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="da1c4-p104">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="da1c4-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="da1c4-129">Request body</span></span>
<span data-ttu-id="da1c4-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="da1c4-130">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="da1c4-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="da1c4-131">Response</span></span>
<span data-ttu-id="da1c4-p105">При успешном выполнении этот метод возвращает код отклика `204, No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="da1c4-p105">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="da1c4-134">Пример</span><span class="sxs-lookup"><span data-stu-id="da1c4-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="da1c4-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="da1c4-135">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="da1c4-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="da1c4-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_programControl"
}-->
```http
DELETE https://graph.microsoft.com/beta/programControls/7e59d237-2fb0-4e5d-b7bb-d4f9f9129213
```
# <a name="c"></a>[<span data-ttu-id="da1c4-137">C#</span><span class="sxs-lookup"><span data-stu-id="da1c4-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-programcontrol-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="da1c4-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="da1c4-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-programcontrol-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="da1c4-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="da1c4-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-programcontrol-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="da1c4-140">Java</span><span class="sxs-lookup"><span data-stu-id="da1c4-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-programcontrol-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="da1c4-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="da1c4-141">Response</span></span>
><span data-ttu-id="da1c4-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="da1c4-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "description": "Delete programControl",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->



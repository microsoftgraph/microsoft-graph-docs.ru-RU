---
title: Удаление программы
description: В функции рецензирования Access Azure AD удалите объект Program.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: bf91890b5e339bebc73242172d64f6e710e41b02
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/15/2019
ms.locfileid: "36412539"
---
# <a name="delete-program"></a><span data-ttu-id="f80c2-103">Удаление программы</span><span class="sxs-lookup"><span data-stu-id="f80c2-103">Delete program</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f80c2-104">В функции рецензирования [Access](../resources/accessreviews-root.md) Azure AD удалите объект [Program](../resources/program.md) .</span><span class="sxs-lookup"><span data-stu-id="f80c2-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, delete a [program](../resources/program.md) object.</span></span>

<span data-ttu-id="f80c2-105">Не удаляйте программу, с которой все `programControl` еще связаны, эти проверки доступа сначала необходимо удалить или удалить из программы, а затем связать с другой программой.</span><span class="sxs-lookup"><span data-stu-id="f80c2-105">Do not delete a program which still has `programControl` linked to it, those access reviews should first be deleted or unlinked from the program and linked to a different program.</span></span>  <span data-ttu-id="f80c2-106">Кроме того, обратите внимание на то, что встроенная программа по умолчанию не может быть удалена.</span><span class="sxs-lookup"><span data-stu-id="f80c2-106">Also, please note that the built-in default program cannot be deleted.</span></span>


## <a name="permissions"></a><span data-ttu-id="f80c2-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f80c2-107">Permissions</span></span>
<span data-ttu-id="f80c2-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f80c2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f80c2-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f80c2-110">Permission type</span></span>                        | <span data-ttu-id="f80c2-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f80c2-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="f80c2-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f80c2-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="f80c2-113">ProgramControl.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f80c2-113">ProgramControl.ReadWrite.All</span></span>   |
|<span data-ttu-id="f80c2-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f80c2-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f80c2-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f80c2-115">Not supported.</span></span> |
|<span data-ttu-id="f80c2-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f80c2-116">Application</span></span>                            | <span data-ttu-id="f80c2-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f80c2-117">Not supported.</span></span> |

<span data-ttu-id="f80c2-118">Пользователь, вошедшего в систему, также должен находиться в роли каталога, который позволяет им создавать программы.</span><span class="sxs-lookup"><span data-stu-id="f80c2-118">The signed in user must also be in a directory role that permits them to create a program.</span></span>

## <a name="http-request"></a><span data-ttu-id="f80c2-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f80c2-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /programs('{id}')
```
## <a name="request-headers"></a><span data-ttu-id="f80c2-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f80c2-120">Request headers</span></span>
| <span data-ttu-id="f80c2-121">Имя</span><span class="sxs-lookup"><span data-stu-id="f80c2-121">Name</span></span>         | <span data-ttu-id="f80c2-122">Тип</span><span class="sxs-lookup"><span data-stu-id="f80c2-122">Type</span></span>        | <span data-ttu-id="f80c2-123">Описание</span><span class="sxs-lookup"><span data-stu-id="f80c2-123">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="f80c2-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="f80c2-124">Authorization</span></span> | <span data-ttu-id="f80c2-125">string</span><span class="sxs-lookup"><span data-stu-id="f80c2-125">string</span></span> | <span data-ttu-id="f80c2-p103">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f80c2-p103">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f80c2-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f80c2-128">Request body</span></span>
<span data-ttu-id="f80c2-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f80c2-129">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="f80c2-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="f80c2-130">Response</span></span>
<span data-ttu-id="f80c2-p104">При успешном выполнении этот метод возвращает код отклика `204, No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="f80c2-p104">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f80c2-133">Пример</span><span class="sxs-lookup"><span data-stu-id="f80c2-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f80c2-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="f80c2-134">Request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="f80c2-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="f80c2-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_program"
}-->
```http
DELETE https://graph.microsoft.com/beta/programs/7e59d237-2fb0-4e5d-b7bb-d4f9f9129213
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="f80c2-136">C#</span><span class="sxs-lookup"><span data-stu-id="f80c2-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-program-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f80c2-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f80c2-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-program-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f80c2-138">Цель — C</span><span class="sxs-lookup"><span data-stu-id="f80c2-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-program-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="f80c2-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="f80c2-139">Response</span></span>
><span data-ttu-id="f80c2-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f80c2-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

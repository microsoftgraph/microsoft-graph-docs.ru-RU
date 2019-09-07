---
title: Удаление программы
description: В функции рецензирования Access Azure AD удалите объект Program.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: d2451ba6ef8ae993b2ee6be5784bed98fd5f0ea9
ms.sourcegitcommit: c68a83d28fa4bfca6e0618467934813a9ae17b12
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/07/2019
ms.locfileid: "36792806"
---
# <a name="delete-program"></a><span data-ttu-id="3c861-103">Удаление программы</span><span class="sxs-lookup"><span data-stu-id="3c861-103">Delete program</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3c861-104">В функции [рецензирования Access](../resources/accessreviews-root.md) Azure AD удалите объект [Program](../resources/program.md) .</span><span class="sxs-lookup"><span data-stu-id="3c861-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, delete a [program](../resources/program.md) object.</span></span>

<span data-ttu-id="3c861-105">Не удаляйте программу, с которой все `programControl` еще связаны, эти проверки доступа сначала необходимо удалить или удалить из программы, а затем связать с другой программой.</span><span class="sxs-lookup"><span data-stu-id="3c861-105">Do not delete a program which still has `programControl` linked to it, those access reviews should first be deleted or unlinked from the program and linked to a different program.</span></span>  <span data-ttu-id="3c861-106">Кроме того, обратите внимание на то, что встроенная программа по умолчанию не может быть удалена.</span><span class="sxs-lookup"><span data-stu-id="3c861-106">Also, please note that the built-in default program cannot be deleted.</span></span>


## <a name="permissions"></a><span data-ttu-id="3c861-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3c861-107">Permissions</span></span>
<span data-ttu-id="3c861-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3c861-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3c861-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3c861-110">Permission type</span></span>                        | <span data-ttu-id="3c861-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3c861-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="3c861-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3c861-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="3c861-113">ProgramControl.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3c861-113">ProgramControl.ReadWrite.All</span></span>   |
|<span data-ttu-id="3c861-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3c861-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3c861-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3c861-115">Not supported.</span></span> |
|<span data-ttu-id="3c861-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3c861-116">Application</span></span>                            | <span data-ttu-id="3c861-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3c861-117">Not supported.</span></span> |

<span data-ttu-id="3c861-118">Пользователь, вошедшего в систему, также должен находиться в роли каталога, который позволяет им создавать программы.</span><span class="sxs-lookup"><span data-stu-id="3c861-118">The signed in user must also be in a directory role that permits them to create a program.</span></span>

## <a name="http-request"></a><span data-ttu-id="3c861-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3c861-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /programs/{id}
```
## <a name="request-headers"></a><span data-ttu-id="3c861-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3c861-120">Request headers</span></span>
| <span data-ttu-id="3c861-121">Имя</span><span class="sxs-lookup"><span data-stu-id="3c861-121">Name</span></span>         | <span data-ttu-id="3c861-122">Тип</span><span class="sxs-lookup"><span data-stu-id="3c861-122">Type</span></span>        | <span data-ttu-id="3c861-123">Описание</span><span class="sxs-lookup"><span data-stu-id="3c861-123">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="3c861-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="3c861-124">Authorization</span></span> | <span data-ttu-id="3c861-125">string</span><span class="sxs-lookup"><span data-stu-id="3c861-125">string</span></span> | <span data-ttu-id="3c861-p103">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3c861-p103">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3c861-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="3c861-128">Request body</span></span>
<span data-ttu-id="3c861-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3c861-129">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="3c861-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="3c861-130">Response</span></span>
<span data-ttu-id="3c861-p104">При успешном выполнении этот метод возвращает код отклика `204, No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="3c861-p104">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3c861-133">Пример</span><span class="sxs-lookup"><span data-stu-id="3c861-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3c861-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="3c861-134">Request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="3c861-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="3c861-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_program"
}-->
```http
DELETE https://graph.microsoft.com/beta/programs/7e59d237-2fb0-4e5d-b7bb-d4f9f9129213
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="3c861-136">C#</span><span class="sxs-lookup"><span data-stu-id="3c861-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-program-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3c861-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3c861-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-program-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="3c861-138">Цель — C</span><span class="sxs-lookup"><span data-stu-id="3c861-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-program-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="3c861-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="3c861-139">Response</span></span>
><span data-ttu-id="3c861-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3c861-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

---
title: Удаление программы
description: В функции рецензирования Access Azure AD удалите объект Program.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: markwahl-msft
ms.openlocfilehash: 205384fea42dd1b6b5bb77f82320082c4d14ae29
ms.sourcegitcommit: bd40e302ce04b686e86989246ab7c4cc9ad3f320
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/03/2020
ms.locfileid: "43123176"
---
# <a name="delete-program"></a><span data-ttu-id="cbee5-103">Удаление программы</span><span class="sxs-lookup"><span data-stu-id="cbee5-103">Delete program</span></span>

<span data-ttu-id="cbee5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cbee5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cbee5-105">В функции [рецензирования Access](../resources/accessreviews-root.md) Azure AD удалите объект [Program](../resources/program.md) .</span><span class="sxs-lookup"><span data-stu-id="cbee5-105">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, delete a [program](../resources/program.md) object.</span></span>

<span data-ttu-id="cbee5-106">Не удаляйте программу, с которой все `programControl` еще связаны, эти проверки доступа сначала необходимо удалить или удалить из программы, а затем связать с другой программой.</span><span class="sxs-lookup"><span data-stu-id="cbee5-106">Do not delete a program which still has `programControl` linked to it, those access reviews should first be deleted or unlinked from the program and linked to a different program.</span></span>  <span data-ttu-id="cbee5-107">Кроме того, обратите внимание на то, что встроенная программа по умолчанию не может быть удалена.</span><span class="sxs-lookup"><span data-stu-id="cbee5-107">Also, please note that the built-in default program cannot be deleted.</span></span>


## <a name="permissions"></a><span data-ttu-id="cbee5-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cbee5-108">Permissions</span></span>
<span data-ttu-id="cbee5-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cbee5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cbee5-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cbee5-111">Permission type</span></span>                        | <span data-ttu-id="cbee5-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cbee5-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="cbee5-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cbee5-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="cbee5-114">ProgramControl.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cbee5-114">ProgramControl.ReadWrite.All</span></span>   |
|<span data-ttu-id="cbee5-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cbee5-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cbee5-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cbee5-116">Not supported.</span></span> |
|<span data-ttu-id="cbee5-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cbee5-117">Application</span></span>                            | <span data-ttu-id="cbee5-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cbee5-118">Not supported.</span></span> |

<span data-ttu-id="cbee5-119">Пользователь, вошедшего в систему, также должен находиться в роли каталога, который позволяет им создавать программы.</span><span class="sxs-lookup"><span data-stu-id="cbee5-119">The signed in user must also be in a directory role that permits them to create a program.</span></span>

## <a name="http-request"></a><span data-ttu-id="cbee5-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cbee5-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /programs/{id}
```
## <a name="request-headers"></a><span data-ttu-id="cbee5-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cbee5-121">Request headers</span></span>
| <span data-ttu-id="cbee5-122">Имя</span><span class="sxs-lookup"><span data-stu-id="cbee5-122">Name</span></span>         | <span data-ttu-id="cbee5-123">Тип</span><span class="sxs-lookup"><span data-stu-id="cbee5-123">Type</span></span>        | <span data-ttu-id="cbee5-124">Описание</span><span class="sxs-lookup"><span data-stu-id="cbee5-124">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="cbee5-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="cbee5-125">Authorization</span></span> | <span data-ttu-id="cbee5-126">string</span><span class="sxs-lookup"><span data-stu-id="cbee5-126">string</span></span> | <span data-ttu-id="cbee5-p103">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cbee5-p103">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cbee5-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cbee5-129">Request body</span></span>
<span data-ttu-id="cbee5-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="cbee5-130">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="cbee5-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="cbee5-131">Response</span></span>
<span data-ttu-id="cbee5-p104">При успешном выполнении этот метод возвращает код отклика `204, No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="cbee5-p104">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cbee5-134">Пример</span><span class="sxs-lookup"><span data-stu-id="cbee5-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="cbee5-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="cbee5-135">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="cbee5-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="cbee5-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_program"
}-->
```http
DELETE https://graph.microsoft.com/beta/programs/7e59d237-2fb0-4e5d-b7bb-d4f9f9129213
```
# <a name="c"></a>[<span data-ttu-id="cbee5-137">C#</span><span class="sxs-lookup"><span data-stu-id="cbee5-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-program-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cbee5-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cbee5-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-program-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cbee5-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cbee5-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-program-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="cbee5-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="cbee5-140">Response</span></span>
><span data-ttu-id="cbee5-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="cbee5-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

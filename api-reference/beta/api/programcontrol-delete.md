---
title: Удаление Програмконтрол
description: В функции рецензирования Access Azure AD удалите объект Програмконтрол.  Это отменяет связь с проверкой доступа из программы.
localization_priority: Normal
ms.openlocfilehash: 59c533e2cacfd612b46b7e1afafdf12be7553b58
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/25/2019
ms.locfileid: "35875345"
---
# <a name="delete-programcontrol"></a><span data-ttu-id="37b14-104">Удаление Програмконтрол</span><span class="sxs-lookup"><span data-stu-id="37b14-104">Delete programControl</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="37b14-105">В функции рецензирования [Access](../resources/accessreviews-root.md) Azure AD удалите объект [програмконтрол](../resources/programcontrol.md) .</span><span class="sxs-lookup"><span data-stu-id="37b14-105">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, delete a [programControl](../resources/programcontrol.md) object.</span></span>  <span data-ttu-id="37b14-106">Это отменяет связь с проверкой доступа из программы.</span><span class="sxs-lookup"><span data-stu-id="37b14-106">This unlinks an access review from a program.</span></span>
## <a name="permissions"></a><span data-ttu-id="37b14-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="37b14-107">Permissions</span></span>
<span data-ttu-id="37b14-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="37b14-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="37b14-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="37b14-110">Permission type</span></span>                        | <span data-ttu-id="37b14-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="37b14-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="37b14-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="37b14-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="37b14-113">ProgramControl.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="37b14-113">ProgramControl.ReadWrite.All</span></span>   |
|<span data-ttu-id="37b14-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="37b14-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="37b14-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="37b14-115">Not supported.</span></span> |
|<span data-ttu-id="37b14-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="37b14-116">Application</span></span>                            | <span data-ttu-id="37b14-117">ProgramControl.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="37b14-117">ProgramControl.ReadWrite.All</span></span>  |

<span data-ttu-id="37b14-118">Пользователь, вошедшего в систему, также должен находиться в роли каталога, который разрешает им `programControl`удалять.</span><span class="sxs-lookup"><span data-stu-id="37b14-118">The signed in user must also be in a directory role that permits them to delete a `programControl`.</span></span>

## <a name="http-request"></a><span data-ttu-id="37b14-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="37b14-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /programControls('<id>')
```
## <a name="request-headers"></a><span data-ttu-id="37b14-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="37b14-120">Request headers</span></span>
| <span data-ttu-id="37b14-121">Имя</span><span class="sxs-lookup"><span data-stu-id="37b14-121">Name</span></span>         | <span data-ttu-id="37b14-122">Тип</span><span class="sxs-lookup"><span data-stu-id="37b14-122">Type</span></span>        | <span data-ttu-id="37b14-123">Описание</span><span class="sxs-lookup"><span data-stu-id="37b14-123">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="37b14-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="37b14-124">Authorization</span></span> | <span data-ttu-id="37b14-125">string</span><span class="sxs-lookup"><span data-stu-id="37b14-125">string</span></span> | <span data-ttu-id="37b14-p104">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="37b14-p104">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="37b14-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="37b14-128">Request body</span></span>
<span data-ttu-id="37b14-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="37b14-129">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="37b14-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="37b14-130">Response</span></span>
<span data-ttu-id="37b14-p105">При успешном выполнении этот метод возвращает код отклика `204, No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="37b14-p105">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="37b14-133">Пример</span><span class="sxs-lookup"><span data-stu-id="37b14-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="37b14-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="37b14-134">Request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="37b14-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="37b14-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_programControl"
}-->
```http
DELETE https://graph.microsoft.com/beta/programControls/7e59d237-2fb0-4e5d-b7bb-d4f9f9129213
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="37b14-136">C#</span><span class="sxs-lookup"><span data-stu-id="37b14-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-programcontrol-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="37b14-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="37b14-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-programcontrol-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="37b14-138">Цель — C</span><span class="sxs-lookup"><span data-stu-id="37b14-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-programcontrol-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="37b14-139">Java</span><span class="sxs-lookup"><span data-stu-id="37b14-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-programcontrol-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="37b14-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="37b14-140">Response</span></span>
><span data-ttu-id="37b14-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="37b14-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

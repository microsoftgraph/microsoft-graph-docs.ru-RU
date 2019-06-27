---
title: Удаление Програмконтрол
description: В функции рецензирования Access Azure AD удалите объект Програмконтрол.  Это отменяет связь с проверкой доступа из программы.
localization_priority: Normal
ms.openlocfilehash: ddbd040d05d6e2c236a024e3d5eb8710562cebe9
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35264094"
---
# <a name="delete-programcontrol"></a><span data-ttu-id="3e3b8-104">Удаление Програмконтрол</span><span class="sxs-lookup"><span data-stu-id="3e3b8-104">Delete programControl</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3e3b8-105">В функции рецензирования [Access](../resources/accessreviews-root.md) Azure AD удалите объект [програмконтрол](../resources/programcontrol.md) .</span><span class="sxs-lookup"><span data-stu-id="3e3b8-105">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, delete a [programControl](../resources/programcontrol.md) object.</span></span>  <span data-ttu-id="3e3b8-106">Это отменяет связь с проверкой доступа из программы.</span><span class="sxs-lookup"><span data-stu-id="3e3b8-106">This unlinks an access review from a program.</span></span>
## <a name="permissions"></a><span data-ttu-id="3e3b8-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3e3b8-107">Permissions</span></span>
<span data-ttu-id="3e3b8-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3e3b8-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3e3b8-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3e3b8-110">Permission type</span></span>                        | <span data-ttu-id="3e3b8-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3e3b8-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="3e3b8-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3e3b8-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="3e3b8-113">ProgramControl.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3e3b8-113">ProgramControl.ReadWrite.All</span></span>   |
|<span data-ttu-id="3e3b8-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3e3b8-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3e3b8-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3e3b8-115">Not supported.</span></span> |
|<span data-ttu-id="3e3b8-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3e3b8-116">Application</span></span>                            | <span data-ttu-id="3e3b8-117">ProgramControl.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3e3b8-117">ProgramControl.ReadWrite.All</span></span>  |

<span data-ttu-id="3e3b8-118">Пользователь, вошедшего в систему, также должен находиться в роли каталога, который разрешает им `programControl`удалять.</span><span class="sxs-lookup"><span data-stu-id="3e3b8-118">The signed in user must also be in a directory role that permits them to delete a `programControl`.</span></span>

## <a name="http-request"></a><span data-ttu-id="3e3b8-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3e3b8-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /programControls('<id>')
```
## <a name="request-headers"></a><span data-ttu-id="3e3b8-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3e3b8-120">Request headers</span></span>
| <span data-ttu-id="3e3b8-121">Имя</span><span class="sxs-lookup"><span data-stu-id="3e3b8-121">Name</span></span>         | <span data-ttu-id="3e3b8-122">Тип</span><span class="sxs-lookup"><span data-stu-id="3e3b8-122">Type</span></span>        | <span data-ttu-id="3e3b8-123">Описание</span><span class="sxs-lookup"><span data-stu-id="3e3b8-123">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="3e3b8-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="3e3b8-124">Authorization</span></span> | <span data-ttu-id="3e3b8-125">string</span><span class="sxs-lookup"><span data-stu-id="3e3b8-125">string</span></span> | <span data-ttu-id="3e3b8-p104">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3e3b8-p104">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3e3b8-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="3e3b8-128">Request body</span></span>
<span data-ttu-id="3e3b8-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3e3b8-129">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="3e3b8-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="3e3b8-130">Response</span></span>
<span data-ttu-id="3e3b8-p105">При успешном выполнении этот метод возвращает код отклика `204, No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="3e3b8-p105">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3e3b8-133">Пример</span><span class="sxs-lookup"><span data-stu-id="3e3b8-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3e3b8-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="3e3b8-134">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_programControl"
}-->
```http
DELETE https://graph.microsoft.com/beta/programControls/7e59d237-2fb0-4e5d-b7bb-d4f9f9129213
```
##### <a name="response"></a><span data-ttu-id="3e3b8-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="3e3b8-135">Response</span></span>
><span data-ttu-id="3e3b8-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3e3b8-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="3e3b8-138">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="3e3b8-138">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="3e3b8-139">C#</span><span class="sxs-lookup"><span data-stu-id="3e3b8-139">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_programControl-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3e3b8-140">Javascript</span><span class="sxs-lookup"><span data-stu-id="3e3b8-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_programControl-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="3e3b8-141">Цель — C</span><span class="sxs-lookup"><span data-stu-id="3e3b8-141">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/delete_programControl-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/programcontrol-delete.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/programcontrol-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/programcontrol-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->

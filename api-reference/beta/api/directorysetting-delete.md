---
title: Удаление параметра каталога
description: Удаление параметра каталога.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 8351d3611f60cc8f4a3422d9b45f2ba22db9980b
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35260594"
---
# <a name="delete-a-directory-setting"></a><span data-ttu-id="588b2-103">Удаление параметра каталога</span><span class="sxs-lookup"><span data-stu-id="588b2-103">Delete a directory setting</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="588b2-104">Удаление параметра каталога.</span><span class="sxs-lookup"><span data-stu-id="588b2-104">Delete a directory setting.</span></span>

> <span data-ttu-id="588b2-105">**Note**: версия/Beta этого API применяется только к группам.</span><span class="sxs-lookup"><span data-stu-id="588b2-105">**Note**: The /beta version of this API is only applies to groups.</span></span> <span data-ttu-id="588b2-106">Версия/v1.0 этого API была переименована, чтобы *Удалить граупсеттингс*.</span><span class="sxs-lookup"><span data-stu-id="588b2-106">The /v1.0 version of this API has been renamed to *Delete groupSettings*.</span></span>

## <a name="permissions"></a><span data-ttu-id="588b2-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="588b2-107">Permissions</span></span>
<span data-ttu-id="588b2-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="588b2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="588b2-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="588b2-110">Permission type</span></span>      | <span data-ttu-id="588b2-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="588b2-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="588b2-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="588b2-112">Delegated (work or school account)</span></span> | <span data-ttu-id="588b2-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="588b2-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="588b2-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="588b2-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="588b2-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="588b2-115">Not supported.</span></span>    |
|<span data-ttu-id="588b2-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="588b2-116">Application</span></span> | <span data-ttu-id="588b2-117">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="588b2-117">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="588b2-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="588b2-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="588b2-119">Удаление определенного параметра на уровне клиента или группы</span><span class="sxs-lookup"><span data-stu-id="588b2-119">Delete a specific tenant-wide or group setting</span></span>
```http
DELETE /settings/{id}
DELETE /groups/{id}/settings/{id}

```
## <a name="request-headers"></a><span data-ttu-id="588b2-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="588b2-120">Request headers</span></span>
| <span data-ttu-id="588b2-121">Имя</span><span class="sxs-lookup"><span data-stu-id="588b2-121">Name</span></span>       | <span data-ttu-id="588b2-122">Описание</span><span class="sxs-lookup"><span data-stu-id="588b2-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="588b2-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="588b2-123">Authorization</span></span>  | <span data-ttu-id="588b2-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="588b2-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="588b2-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="588b2-126">Request body</span></span>
<span data-ttu-id="588b2-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="588b2-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="588b2-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="588b2-128">Response</span></span>

<span data-ttu-id="588b2-p104">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="588b2-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="588b2-131">Пример</span><span class="sxs-lookup"><span data-stu-id="588b2-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="588b2-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="588b2-132">Request</span></span>
<span data-ttu-id="588b2-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="588b2-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_directorysetting"
}-->
```http
DELETE https://graph.microsoft.com/beta/settings/{id}
```
##### <a name="response"></a><span data-ttu-id="588b2-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="588b2-134">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="588b2-135">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="588b2-135">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="588b2-136">C#</span><span class="sxs-lookup"><span data-stu-id="588b2-136">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_directorysetting-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="588b2-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="588b2-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_directorysetting-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="588b2-138">Цель — C</span><span class="sxs-lookup"><span data-stu-id="588b2-138">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/delete_directorysetting-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete directorySetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/directorysetting-delete.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/directorysetting-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/directorysetting-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->

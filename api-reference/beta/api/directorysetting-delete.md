---
title: Удаление параметра каталога
description: Удаление параметра каталога.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 35f67790bb634fd2b45a3e67db6412c40f7972d3
ms.sourcegitcommit: ed03445225e98cf0881de08273c36be8d0e576ea
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/07/2020
ms.locfileid: "40951684"
---
# <a name="delete-a-directory-setting"></a><span data-ttu-id="574b0-103">Удаление параметра каталога</span><span class="sxs-lookup"><span data-stu-id="574b0-103">Delete a directory setting</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="574b0-104">Удаление параметра каталога.</span><span class="sxs-lookup"><span data-stu-id="574b0-104">Delete a directory setting.</span></span>

> <span data-ttu-id="574b0-105">**Note**: версия/Beta этого API применяется только к группам.</span><span class="sxs-lookup"><span data-stu-id="574b0-105">**Note**: The /beta version of this API only applies to groups.</span></span> <span data-ttu-id="574b0-106">Версия/v1.0 этого API была переименована, чтобы *Удалить граупсеттингс*.</span><span class="sxs-lookup"><span data-stu-id="574b0-106">The /v1.0 version of this API has been renamed to *Delete groupSettings*.</span></span>

## <a name="permissions"></a><span data-ttu-id="574b0-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="574b0-107">Permissions</span></span>
<span data-ttu-id="574b0-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="574b0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="574b0-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="574b0-110">Permission type</span></span>      | <span data-ttu-id="574b0-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="574b0-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="574b0-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="574b0-112">Delegated (work or school account)</span></span> | <span data-ttu-id="574b0-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="574b0-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="574b0-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="574b0-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="574b0-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="574b0-115">Not supported.</span></span>    |
|<span data-ttu-id="574b0-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="574b0-116">Application</span></span> | <span data-ttu-id="574b0-117">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="574b0-117">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="574b0-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="574b0-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="574b0-119">Удаление определенного параметра на уровне клиента или группы</span><span class="sxs-lookup"><span data-stu-id="574b0-119">Delete a specific tenant-wide or group setting</span></span>
```http
DELETE /settings/{id}
DELETE /groups/{id}/settings/{id}

```
## <a name="request-headers"></a><span data-ttu-id="574b0-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="574b0-120">Request headers</span></span>
| <span data-ttu-id="574b0-121">Имя</span><span class="sxs-lookup"><span data-stu-id="574b0-121">Name</span></span>       | <span data-ttu-id="574b0-122">Описание</span><span class="sxs-lookup"><span data-stu-id="574b0-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="574b0-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="574b0-123">Authorization</span></span>  | <span data-ttu-id="574b0-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="574b0-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="574b0-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="574b0-126">Request body</span></span>
<span data-ttu-id="574b0-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="574b0-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="574b0-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="574b0-128">Response</span></span>

<span data-ttu-id="574b0-p104">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="574b0-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="574b0-131">Пример</span><span class="sxs-lookup"><span data-stu-id="574b0-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="574b0-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="574b0-132">Request</span></span>
<span data-ttu-id="574b0-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="574b0-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="574b0-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="574b0-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_directorysetting"
}-->
```http
DELETE https://graph.microsoft.com/beta/settings/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="574b0-135">C#</span><span class="sxs-lookup"><span data-stu-id="574b0-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-directorysetting-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="574b0-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="574b0-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-directorysetting-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="574b0-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="574b0-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-directorysetting-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="574b0-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="574b0-138">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

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
  ]
}
-->

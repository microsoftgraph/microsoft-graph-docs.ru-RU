---
title: Удаление параметра каталога
description: Удаление параметра каталога.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 16add1a6545740a068895c3af8c8a0afd3c66beb
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42434100"
---
# <a name="delete-a-directory-setting"></a><span data-ttu-id="14e10-103">Удаление параметра каталога</span><span class="sxs-lookup"><span data-stu-id="14e10-103">Delete a directory setting</span></span>

<span data-ttu-id="14e10-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="14e10-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="14e10-105">Удаление параметра каталога.</span><span class="sxs-lookup"><span data-stu-id="14e10-105">Delete a directory setting.</span></span>

> <span data-ttu-id="14e10-106">**Note**: версия/Beta этого API применяется только к группам.</span><span class="sxs-lookup"><span data-stu-id="14e10-106">**Note**: The /beta version of this API only applies to groups.</span></span> <span data-ttu-id="14e10-107">Версия/v1.0 этого API была переименована, чтобы *Удалить граупсеттингс*.</span><span class="sxs-lookup"><span data-stu-id="14e10-107">The /v1.0 version of this API has been renamed to *Delete groupSettings*.</span></span>

## <a name="permissions"></a><span data-ttu-id="14e10-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="14e10-108">Permissions</span></span>
<span data-ttu-id="14e10-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="14e10-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="14e10-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="14e10-111">Permission type</span></span>      | <span data-ttu-id="14e10-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="14e10-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="14e10-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="14e10-113">Delegated (work or school account)</span></span> | <span data-ttu-id="14e10-114">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="14e10-114">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="14e10-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="14e10-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="14e10-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="14e10-116">Not supported.</span></span>    |
|<span data-ttu-id="14e10-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="14e10-117">Application</span></span> | <span data-ttu-id="14e10-118">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="14e10-118">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="14e10-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="14e10-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="14e10-120">Удаление определенного параметра на уровне клиента или группы</span><span class="sxs-lookup"><span data-stu-id="14e10-120">Delete a specific tenant-wide or group setting</span></span>
```http
DELETE /settings/{id}
DELETE /groups/{id}/settings/{id}

```
## <a name="request-headers"></a><span data-ttu-id="14e10-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="14e10-121">Request headers</span></span>
| <span data-ttu-id="14e10-122">Имя</span><span class="sxs-lookup"><span data-stu-id="14e10-122">Name</span></span>       | <span data-ttu-id="14e10-123">Описание</span><span class="sxs-lookup"><span data-stu-id="14e10-123">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="14e10-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="14e10-124">Authorization</span></span>  | <span data-ttu-id="14e10-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="14e10-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="14e10-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="14e10-127">Request body</span></span>
<span data-ttu-id="14e10-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="14e10-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="14e10-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="14e10-129">Response</span></span>

<span data-ttu-id="14e10-p104">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="14e10-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="14e10-132">Пример</span><span class="sxs-lookup"><span data-stu-id="14e10-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="14e10-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="14e10-133">Request</span></span>
<span data-ttu-id="14e10-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="14e10-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="14e10-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="14e10-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_directorysetting"
}-->
```http
DELETE https://graph.microsoft.com/beta/settings/{id}
```
# <a name="c"></a>[<span data-ttu-id="14e10-136">C#</span><span class="sxs-lookup"><span data-stu-id="14e10-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-directorysetting-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="14e10-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="14e10-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-directorysetting-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="14e10-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="14e10-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-directorysetting-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="14e10-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="14e10-139">Response</span></span>
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

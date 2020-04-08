---
title: Удаление параметра каталога
description: Удаление параметра каталога.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 27eb77aebf0dac6eac352f370088d8729952ff96
ms.sourcegitcommit: 11503211a31ea17f4e577c21ec36d364184c0580
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/08/2020
ms.locfileid: "43180846"
---
# <a name="delete-a-directory-setting"></a><span data-ttu-id="a997e-103">Удаление параметра каталога</span><span class="sxs-lookup"><span data-stu-id="a997e-103">Delete a directory setting</span></span>

<span data-ttu-id="a997e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a997e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a997e-105">Удаление параметра каталога.</span><span class="sxs-lookup"><span data-stu-id="a997e-105">Delete a directory setting.</span></span>

> <span data-ttu-id="a997e-106">**Note**: версия/Beta этого API применяется только к группам.</span><span class="sxs-lookup"><span data-stu-id="a997e-106">**Note**: The /beta version of this API only applies to groups.</span></span> <span data-ttu-id="a997e-107">Версия/v1.0 этого API была переименована, чтобы *Удалить граупсеттингс*.</span><span class="sxs-lookup"><span data-stu-id="a997e-107">The /v1.0 version of this API has been renamed to *Delete groupSettings*.</span></span>

## <a name="permissions"></a><span data-ttu-id="a997e-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a997e-108">Permissions</span></span>
<span data-ttu-id="a997e-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a997e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a997e-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a997e-111">Permission type</span></span>      | <span data-ttu-id="a997e-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a997e-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a997e-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a997e-113">Delegated (work or school account)</span></span> | <span data-ttu-id="a997e-114">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a997e-114">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="a997e-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a997e-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a997e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a997e-116">Not supported.</span></span>    |
|<span data-ttu-id="a997e-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a997e-117">Application</span></span> | <span data-ttu-id="a997e-118">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a997e-118">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a997e-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a997e-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="a997e-120">Удаление определенного параметра на уровне клиента или группы</span><span class="sxs-lookup"><span data-stu-id="a997e-120">Delete a specific tenant-wide or group setting</span></span>
```http
DELETE /settings/{id}
DELETE /groups/{id}/settings/{id}

```
## <a name="request-headers"></a><span data-ttu-id="a997e-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a997e-121">Request headers</span></span>
| <span data-ttu-id="a997e-122">Имя</span><span class="sxs-lookup"><span data-stu-id="a997e-122">Name</span></span>       | <span data-ttu-id="a997e-123">Описание</span><span class="sxs-lookup"><span data-stu-id="a997e-123">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="a997e-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a997e-124">Authorization</span></span>  | <span data-ttu-id="a997e-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a997e-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a997e-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a997e-127">Request body</span></span>
<span data-ttu-id="a997e-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a997e-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a997e-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="a997e-129">Response</span></span>

<span data-ttu-id="a997e-p104">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="a997e-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a997e-132">Пример</span><span class="sxs-lookup"><span data-stu-id="a997e-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a997e-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="a997e-133">Request</span></span>
<span data-ttu-id="a997e-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a997e-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a997e-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="a997e-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_directorysetting"
}-->
```http
DELETE https://graph.microsoft.com/beta/settings/{id}
```
# <a name="c"></a>[<span data-ttu-id="a997e-136">C#</span><span class="sxs-lookup"><span data-stu-id="a997e-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-directorysetting-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a997e-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a997e-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-directorysetting-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a997e-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a997e-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-directorysetting-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="a997e-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="a997e-139">Response</span></span>
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

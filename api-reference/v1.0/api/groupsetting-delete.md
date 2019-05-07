---
title: Удаление параметра группы
description: Удаление параметра группы.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 7fdce32ee8091fccf0324360a30e484d54163990
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33614023"
---
# <a name="delete-a-group-setting"></a><span data-ttu-id="32fc4-103">Удаление параметра группы</span><span class="sxs-lookup"><span data-stu-id="32fc4-103">Delete a group setting</span></span>

<span data-ttu-id="32fc4-104">Удаление параметра группы.</span><span class="sxs-lookup"><span data-stu-id="32fc4-104">Delete a group setting.</span></span>

## <a name="permissions"></a><span data-ttu-id="32fc4-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="32fc4-105">Permissions</span></span>

<span data-ttu-id="32fc4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="32fc4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="32fc4-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="32fc4-108">Permission type</span></span>      | <span data-ttu-id="32fc4-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="32fc4-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="32fc4-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="32fc4-110">Delegated (work or school account)</span></span> | <span data-ttu-id="32fc4-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="32fc4-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="32fc4-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="32fc4-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="32fc4-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="32fc4-113">Not supported.</span></span>    |
|<span data-ttu-id="32fc4-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="32fc4-114">Application</span></span> | <span data-ttu-id="32fc4-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="32fc4-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="32fc4-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="32fc4-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groupSettings/{id}
DELETE /groups/{id}/settings/{id}

```

## <a name="request-headers"></a><span data-ttu-id="32fc4-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="32fc4-117">Request headers</span></span>

| <span data-ttu-id="32fc4-118">Имя</span><span class="sxs-lookup"><span data-stu-id="32fc4-118">Name</span></span> | <span data-ttu-id="32fc4-119">Описание</span><span class="sxs-lookup"><span data-stu-id="32fc4-119">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="32fc4-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="32fc4-120">Authorization</span></span>  | <span data-ttu-id="32fc4-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="32fc4-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="32fc4-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="32fc4-123">Content-Type</span></span>  | <span data-ttu-id="32fc4-124">application/json</span><span class="sxs-lookup"><span data-stu-id="32fc4-124">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="32fc4-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="32fc4-125">Request body</span></span>
<span data-ttu-id="32fc4-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="32fc4-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="32fc4-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="32fc4-127">Response</span></span>

<span data-ttu-id="32fc4-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="32fc4-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="32fc4-130">Пример</span><span class="sxs-lookup"><span data-stu-id="32fc4-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="32fc4-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="32fc4-131">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_groupsetting"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groupSettings/{id}
```
##### <a name="response"></a><span data-ttu-id="32fc4-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="32fc4-132">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="32fc4-133">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="32fc4-133">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="32fc4-134">Языках</span><span class="sxs-lookup"><span data-stu-id="32fc4-134">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_groupsetting-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="32fc4-135">Язык</span><span class="sxs-lookup"><span data-stu-id="32fc4-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_groupsetting-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete groupSetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/groupsetting-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/groupsetting-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->

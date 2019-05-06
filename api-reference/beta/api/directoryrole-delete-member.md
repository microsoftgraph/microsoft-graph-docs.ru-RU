---
title: Удаление элемента роли каталога
description: Удаление элемента из объекта directoryRole.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 9dd2e47b4471184c23d9f219fb1cc3c0dfa5e72c
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33590558"
---
# <a name="remove-directory-role-member"></a><span data-ttu-id="427e5-103">Удаление элемента роли каталога</span><span class="sxs-lookup"><span data-stu-id="427e5-103">Remove directory role member</span></span>

<span data-ttu-id="427e5-104">Удаление элемента из объекта directoryRole.</span><span class="sxs-lookup"><span data-stu-id="427e5-104">Remove a member from a directoryRole.</span></span>

## <a name="permissions"></a><span data-ttu-id="427e5-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="427e5-105">Permissions</span></span>

<span data-ttu-id="427e5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="427e5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="427e5-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="427e5-108">Permission type</span></span>      | <span data-ttu-id="427e5-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="427e5-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="427e5-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="427e5-110">Delegated (work or school account)</span></span> | <span data-ttu-id="427e5-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="427e5-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="427e5-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="427e5-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="427e5-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="427e5-113">Not supported.</span></span>    |
|<span data-ttu-id="427e5-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="427e5-114">Application</span></span> | <span data-ttu-id="427e5-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="427e5-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="427e5-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="427e5-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /directoryRoles/{id}/members/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="427e5-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="427e5-117">Request headers</span></span>

| <span data-ttu-id="427e5-118">Имя</span><span class="sxs-lookup"><span data-stu-id="427e5-118">Name</span></span>       | <span data-ttu-id="427e5-119">Тип</span><span class="sxs-lookup"><span data-stu-id="427e5-119">Type</span></span> | <span data-ttu-id="427e5-120">Описание</span><span class="sxs-lookup"><span data-stu-id="427e5-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="427e5-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="427e5-121">Authorization</span></span>  | <span data-ttu-id="427e5-122">string</span><span class="sxs-lookup"><span data-stu-id="427e5-122">string</span></span>  | <span data-ttu-id="427e5-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="427e5-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="427e5-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="427e5-125">Request body</span></span>

<span data-ttu-id="427e5-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="427e5-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="427e5-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="427e5-127">Response</span></span>

<span data-ttu-id="427e5-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="427e5-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="427e5-130">Пример</span><span class="sxs-lookup"><span data-stu-id="427e5-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="427e5-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="427e5-131">Request</span></span>

<span data-ttu-id="427e5-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="427e5-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_directoryobject_from_directoryrole"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/directoryRoles/{id}/members/{id}/$ref
```

##### <a name="response"></a><span data-ttu-id="427e5-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="427e5-133">Response</span></span>

<span data-ttu-id="427e5-134">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="427e5-134">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="427e5-135">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="427e5-135">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="427e5-136">Языках</span><span class="sxs-lookup"><span data-stu-id="427e5-136">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_directoryobject_from_directoryrole-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="427e5-137">Язык</span><span class="sxs-lookup"><span data-stu-id="427e5-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_directoryobject_from_directoryrole-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete a member",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/directoryrole-delete-member.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/directoryrole-delete-member.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->

---
title: Удаление элемента роли каталога
description: Удаление элемента из объекта directoryRole.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 2f19162726a1b99de054332313982b741546237b
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35459344"
---
# <a name="remove-directory-role-member"></a><span data-ttu-id="c0e7b-103">Удаление элемента роли каталога</span><span class="sxs-lookup"><span data-stu-id="c0e7b-103">Remove directory role member</span></span>

<span data-ttu-id="c0e7b-104">Удаление элемента из объекта directoryRole.</span><span class="sxs-lookup"><span data-stu-id="c0e7b-104">Remove a member from a directoryRole.</span></span>

## <a name="permissions"></a><span data-ttu-id="c0e7b-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c0e7b-105">Permissions</span></span>

<span data-ttu-id="c0e7b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c0e7b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="c0e7b-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c0e7b-108">Permission type</span></span>      | <span data-ttu-id="c0e7b-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c0e7b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c0e7b-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c0e7b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c0e7b-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c0e7b-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c0e7b-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c0e7b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c0e7b-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c0e7b-113">Not supported.</span></span>    |
|<span data-ttu-id="c0e7b-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c0e7b-114">Application</span></span> | <span data-ttu-id="c0e7b-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c0e7b-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c0e7b-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c0e7b-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /directoryRoles/{id}/members/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="c0e7b-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c0e7b-117">Request headers</span></span>

| <span data-ttu-id="c0e7b-118">Имя</span><span class="sxs-lookup"><span data-stu-id="c0e7b-118">Name</span></span>       | <span data-ttu-id="c0e7b-119">Тип</span><span class="sxs-lookup"><span data-stu-id="c0e7b-119">Type</span></span> | <span data-ttu-id="c0e7b-120">Описание</span><span class="sxs-lookup"><span data-stu-id="c0e7b-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="c0e7b-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="c0e7b-121">Authorization</span></span>  | <span data-ttu-id="c0e7b-122">string</span><span class="sxs-lookup"><span data-stu-id="c0e7b-122">string</span></span>  | <span data-ttu-id="c0e7b-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c0e7b-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c0e7b-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c0e7b-125">Request body</span></span>

<span data-ttu-id="c0e7b-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c0e7b-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c0e7b-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="c0e7b-127">Response</span></span>

<span data-ttu-id="c0e7b-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="c0e7b-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c0e7b-130">Пример</span><span class="sxs-lookup"><span data-stu-id="c0e7b-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="c0e7b-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="c0e7b-131">Request</span></span>

<span data-ttu-id="c0e7b-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c0e7b-132">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="c0e7b-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="c0e7b-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_directoryobject_from_directoryrole"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/directoryRoles/{id}/members/{id}/$ref
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c0e7b-134">C#</span><span class="sxs-lookup"><span data-stu-id="c0e7b-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-directoryobject-from-directoryrole-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c0e7b-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="c0e7b-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-directoryobject-from-directoryrole-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c0e7b-136">Цель — C</span><span class="sxs-lookup"><span data-stu-id="c0e7b-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-directoryobject-from-directoryrole-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="c0e7b-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="c0e7b-137">Response</span></span>

<span data-ttu-id="c0e7b-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c0e7b-138">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete a member",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

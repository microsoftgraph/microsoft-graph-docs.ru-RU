---
title: Удаление объекта directoryObject
description: Удаление directoryObject.
author: keylimesoda
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 62a4d9f6d83df0eaa80be7262a9d3057fe28d724
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50769991"
---
# <a name="delete-directoryobject"></a><span data-ttu-id="9f4cc-103">Удаление объекта directoryObject</span><span class="sxs-lookup"><span data-stu-id="9f4cc-103">Delete directoryObject</span></span>

<span data-ttu-id="9f4cc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9f4cc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9f4cc-105">Удаление directoryObject.</span><span class="sxs-lookup"><span data-stu-id="9f4cc-105">Delete directoryObject.</span></span>
## <a name="permissions"></a><span data-ttu-id="9f4cc-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9f4cc-106">Permissions</span></span>
<span data-ttu-id="9f4cc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9f4cc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="9f4cc-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9f4cc-109">Permission type</span></span>      | <span data-ttu-id="9f4cc-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9f4cc-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9f4cc-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9f4cc-111">Delegated (work or school account)</span></span> | <span data-ttu-id="9f4cc-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="9f4cc-112">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="9f4cc-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9f4cc-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9f4cc-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9f4cc-114">Not supported.</span></span>    |
|<span data-ttu-id="9f4cc-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9f4cc-115">Application</span></span> | <span data-ttu-id="9f4cc-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9f4cc-116">Not supported.</span></span> |

<span data-ttu-id="9f4cc-117">**ПРИМЕЧАНИЕ:** Пользователи, группы и контакты — это типы объекта каталога.</span><span class="sxs-lookup"><span data-stu-id="9f4cc-117">**NOTE:** Users, groups, and contacts are types of directory object.</span></span> <span data-ttu-id="9f4cc-118">В результате, если требуется удалить пользователей, можно и нужно использовать следующее разрешение: User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9f4cc-118">As a result,if you need to delete users, the following permission can and should be used: User.ReadWrite.All</span></span>
## <a name="http-request"></a><span data-ttu-id="9f4cc-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9f4cc-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /directoryObjects/{id}

```
## <a name="request-headers"></a><span data-ttu-id="9f4cc-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9f4cc-120">Request headers</span></span>
| <span data-ttu-id="9f4cc-121">Имя</span><span class="sxs-lookup"><span data-stu-id="9f4cc-121">Name</span></span>       | <span data-ttu-id="9f4cc-122">Тип</span><span class="sxs-lookup"><span data-stu-id="9f4cc-122">Type</span></span> | <span data-ttu-id="9f4cc-123">Описание</span><span class="sxs-lookup"><span data-stu-id="9f4cc-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="9f4cc-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="9f4cc-124">Authorization</span></span>  | <span data-ttu-id="9f4cc-125">string</span><span class="sxs-lookup"><span data-stu-id="9f4cc-125">string</span></span>  | <span data-ttu-id="9f4cc-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9f4cc-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9f4cc-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9f4cc-128">Request body</span></span>
<span data-ttu-id="9f4cc-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9f4cc-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9f4cc-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="9f4cc-130">Response</span></span>

<span data-ttu-id="9f4cc-p104">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="9f4cc-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9f4cc-133">Пример</span><span class="sxs-lookup"><span data-stu-id="9f4cc-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9f4cc-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="9f4cc-134">Request</span></span>
<span data-ttu-id="9f4cc-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9f4cc-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9f4cc-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="9f4cc-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_directoryobject"
}-->
```http
DELETE https://graph.microsoft.com/beta/directoryObjects/ffab4dce-9b82-49a6-b7c7-1a143106598c
```
# <a name="c"></a>[<span data-ttu-id="9f4cc-137">C#</span><span class="sxs-lookup"><span data-stu-id="9f4cc-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-directoryobject-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9f4cc-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9f4cc-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-directoryobject-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9f4cc-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9f4cc-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-directoryobject-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9f4cc-140">Java</span><span class="sxs-lookup"><span data-stu-id="9f4cc-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-directoryobject-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="9f4cc-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="9f4cc-141">Response</span></span>
<span data-ttu-id="9f4cc-142">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="9f4cc-142">Here is an example of the response.</span></span> 
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
  "description": "Delete directoryObject",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->



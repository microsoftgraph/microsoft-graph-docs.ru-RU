---
title: Удаление владельца
description: Используйте этот API, чтобы удалить владельца из группы Microsoft 365, группы безопасности или группы безопасности с поддержкой почты через свойство навигации владельцев.
localization_priority: Normal
author: Jordanndahl
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 34a7dcd31642f56d34aacc05082ef57c801e5e6a
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/27/2021
ms.locfileid: "52680985"
---
# <a name="remove-owner"></a><span data-ttu-id="946ce-103">Удаление владельца</span><span class="sxs-lookup"><span data-stu-id="946ce-103">Remove owner</span></span>

<span data-ttu-id="946ce-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="946ce-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="946ce-105">Используйте этот API, чтобы удалить владельца из группы Microsoft 365, группы безопасности или группы безопасности с поддержкой почты через свойство навигации владельцев.</span><span class="sxs-lookup"><span data-stu-id="946ce-105">Use this API to remove an owner from a Microsoft 365 group, a security group, or a mail-enabled security group through the owners navigation property.</span></span> <span data-ttu-id="946ce-106">После того как владельцы назначены группе, последний владелец группы не может быть удален.</span><span class="sxs-lookup"><span data-stu-id="946ce-106">Once owners are assigned to a group, the last owner of the group cannot be removed.</span></span> 

## <a name="permissions"></a><span data-ttu-id="946ce-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="946ce-107">Permissions</span></span>
<span data-ttu-id="946ce-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="946ce-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="946ce-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="946ce-110">Permission type</span></span>      | <span data-ttu-id="946ce-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="946ce-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="946ce-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="946ce-112">Delegated (work or school account)</span></span> | <span data-ttu-id="946ce-113">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="946ce-113">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="946ce-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="946ce-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="946ce-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="946ce-115">Not supported.</span></span>    |
|<span data-ttu-id="946ce-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="946ce-116">Application</span></span> | <span data-ttu-id="946ce-117">Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="946ce-117">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="946ce-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="946ce-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/owners/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="946ce-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="946ce-119">Request headers</span></span>
| <span data-ttu-id="946ce-120">Имя</span><span class="sxs-lookup"><span data-stu-id="946ce-120">Name</span></span>       | <span data-ttu-id="946ce-121">Тип</span><span class="sxs-lookup"><span data-stu-id="946ce-121">Type</span></span> | <span data-ttu-id="946ce-122">Описание</span><span class="sxs-lookup"><span data-stu-id="946ce-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="946ce-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="946ce-123">Authorization</span></span>  | <span data-ttu-id="946ce-124">string</span><span class="sxs-lookup"><span data-stu-id="946ce-124">string</span></span>  | <span data-ttu-id="946ce-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="946ce-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="946ce-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="946ce-127">Request body</span></span>
<span data-ttu-id="946ce-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="946ce-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="946ce-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="946ce-129">Response</span></span>
<span data-ttu-id="946ce-p104">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="946ce-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="946ce-132">Пример</span><span class="sxs-lookup"><span data-stu-id="946ce-132">Example</span></span>
#### <a name="request"></a><span data-ttu-id="946ce-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="946ce-133">Request</span></span>
<span data-ttu-id="946ce-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="946ce-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="946ce-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="946ce-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_owner_from_group"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groups/{id}/owners/{id}/$ref
```
# <a name="c"></a>[<span data-ttu-id="946ce-136">C#</span><span class="sxs-lookup"><span data-stu-id="946ce-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-owner-from-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="946ce-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="946ce-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-owner-from-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="946ce-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="946ce-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-owner-from-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="946ce-139">Java</span><span class="sxs-lookup"><span data-stu-id="946ce-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-owner-from-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="946ce-140">Укажите в запросе свойство `id` удаляемого объекта каталога после сегмента $ref.</span><span class="sxs-lookup"><span data-stu-id="946ce-140">In the request, specify the `id` of the directory object you want to remove after the $ref segment.</span></span>

#### <a name="response"></a><span data-ttu-id="946ce-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="946ce-141">Response</span></span>
<span data-ttu-id="946ce-142">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="946ce-142">The following is an example of the response.</span></span>
><span data-ttu-id="946ce-143">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="946ce-143">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete owner",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->


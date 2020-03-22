---
title: Удаление владельца
description: С помощью этого API можно удалить владельца из группы Office 365 или группы безопасности (обычной или с поддержкой почты) через свойство навигации owners.
localization_priority: Normal
author: dkershaw10
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 87880e417af00695b3644fac87d47db5d91f8047
ms.sourcegitcommit: 7baf4847486885edf08ead533c76503cd31a98a4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/21/2020
ms.locfileid: "42892641"
---
# <a name="remove-owner"></a><span data-ttu-id="8eeb2-103">Удаление владельца</span><span class="sxs-lookup"><span data-stu-id="8eeb2-103">Remove owner</span></span>

<span data-ttu-id="8eeb2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8eeb2-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8eeb2-105">С помощью этого API можно удалить владельца из группы Office 365 или группы безопасности (обычной или с поддержкой почты) через свойство навигации owners.</span><span class="sxs-lookup"><span data-stu-id="8eeb2-105">Use this API to remove an owner from an Office 365 group, a security group, or a mail-enabled security group through the owners navigation property.</span></span>

## <a name="permissions"></a><span data-ttu-id="8eeb2-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8eeb2-106">Permissions</span></span>
<span data-ttu-id="8eeb2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8eeb2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8eeb2-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8eeb2-109">Permission type</span></span>      | <span data-ttu-id="8eeb2-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8eeb2-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8eeb2-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8eeb2-111">Delegated (work or school account)</span></span> | <span data-ttu-id="8eeb2-112">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="8eeb2-112">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="8eeb2-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8eeb2-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8eeb2-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8eeb2-114">Not supported.</span></span>    |
|<span data-ttu-id="8eeb2-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8eeb2-115">Application</span></span> | <span data-ttu-id="8eeb2-116">Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8eeb2-116">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8eeb2-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8eeb2-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/owners/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="8eeb2-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8eeb2-118">Request headers</span></span>
| <span data-ttu-id="8eeb2-119">Имя</span><span class="sxs-lookup"><span data-stu-id="8eeb2-119">Name</span></span>       | <span data-ttu-id="8eeb2-120">Тип</span><span class="sxs-lookup"><span data-stu-id="8eeb2-120">Type</span></span> | <span data-ttu-id="8eeb2-121">Описание</span><span class="sxs-lookup"><span data-stu-id="8eeb2-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="8eeb2-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="8eeb2-122">Authorization</span></span>  | <span data-ttu-id="8eeb2-123">string</span><span class="sxs-lookup"><span data-stu-id="8eeb2-123">string</span></span>  | <span data-ttu-id="8eeb2-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8eeb2-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8eeb2-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="8eeb2-126">Request body</span></span>
<span data-ttu-id="8eeb2-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8eeb2-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8eeb2-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="8eeb2-128">Response</span></span>
<span data-ttu-id="8eeb2-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="8eeb2-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8eeb2-131">Пример</span><span class="sxs-lookup"><span data-stu-id="8eeb2-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="8eeb2-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="8eeb2-132">Request</span></span>
<span data-ttu-id="8eeb2-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8eeb2-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="8eeb2-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="8eeb2-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_owner_from_group"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groups/{id}/owners/{id}/$ref
```
# <a name="c"></a>[<span data-ttu-id="8eeb2-135">C#</span><span class="sxs-lookup"><span data-stu-id="8eeb2-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-owner-from-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8eeb2-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8eeb2-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-owner-from-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8eeb2-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8eeb2-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-owner-from-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8eeb2-138">Java</span><span class="sxs-lookup"><span data-stu-id="8eeb2-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-owner-from-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="8eeb2-139">Укажите в запросе свойство `id` удаляемого объекта каталога после сегмента $ref.</span><span class="sxs-lookup"><span data-stu-id="8eeb2-139">In the request, specify the `id` of the directory object you want to remove after the $ref segment.</span></span>

#### <a name="response"></a><span data-ttu-id="8eeb2-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="8eeb2-140">Response</span></span>
<span data-ttu-id="8eeb2-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="8eeb2-141">The following is an example of the response.</span></span>
><span data-ttu-id="8eeb2-142">**Примечание.**  Объект ответа, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="8eeb2-142">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="8eeb2-143">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8eeb2-143">All the properties will be returned from an actual call.</span></span>
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

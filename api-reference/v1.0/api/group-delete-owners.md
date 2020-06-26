---
title: Удаление владельца
description: Используйте этот API, чтобы удалить владельца из группы Microsoft 365, группы безопасности или группы безопасности с включенной поддержкой почты с помощью свойства навигации Owners.
localization_priority: Normal
author: yyuank
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 133edd14f1ac71cd2f3f24d3f45c435072be247d
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/26/2020
ms.locfileid: "44895596"
---
# <a name="remove-owner"></a><span data-ttu-id="f56df-103">Удаление владельца</span><span class="sxs-lookup"><span data-stu-id="f56df-103">Remove owner</span></span>

<span data-ttu-id="f56df-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f56df-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f56df-105">Используйте этот API, чтобы удалить владельца из группы Microsoft 365, группы безопасности или группы безопасности с включенной поддержкой почты с помощью свойства навигации Owners.</span><span class="sxs-lookup"><span data-stu-id="f56df-105">Use this API to remove an owner from a Microsoft 365 group, a security group, or a mail-enabled security group through the owners navigation property.</span></span>

## <a name="permissions"></a><span data-ttu-id="f56df-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f56df-106">Permissions</span></span>
<span data-ttu-id="f56df-107">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="f56df-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="f56df-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f56df-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f56df-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f56df-109">Permission type</span></span>      | <span data-ttu-id="f56df-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f56df-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f56df-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f56df-111">Delegated (work or school account)</span></span> | <span data-ttu-id="f56df-112">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f56df-112">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="f56df-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f56df-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f56df-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f56df-114">Not supported.</span></span>    |
|<span data-ttu-id="f56df-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f56df-115">Application</span></span> | <span data-ttu-id="f56df-116">Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f56df-116">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f56df-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f56df-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/owners/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="f56df-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f56df-118">Request headers</span></span>
| <span data-ttu-id="f56df-119">Имя</span><span class="sxs-lookup"><span data-stu-id="f56df-119">Name</span></span>       | <span data-ttu-id="f56df-120">Тип</span><span class="sxs-lookup"><span data-stu-id="f56df-120">Type</span></span> | <span data-ttu-id="f56df-121">Описание</span><span class="sxs-lookup"><span data-stu-id="f56df-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="f56df-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f56df-122">Authorization</span></span>  | <span data-ttu-id="f56df-123">string</span><span class="sxs-lookup"><span data-stu-id="f56df-123">string</span></span>  | <span data-ttu-id="f56df-124">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="f56df-124">Bearer {token}.</span></span> <span data-ttu-id="f56df-125">Required.</span><span class="sxs-lookup"><span data-stu-id="f56df-125">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f56df-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f56df-126">Request body</span></span>
<span data-ttu-id="f56df-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f56df-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f56df-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="f56df-128">Response</span></span>
<span data-ttu-id="f56df-129">If successful, this method returns `204 No Content` response code.</span><span class="sxs-lookup"><span data-stu-id="f56df-129">If successful, this method returns `204 No Content` response code.</span></span> <span data-ttu-id="f56df-130">It does not return anything in the response body.</span><span class="sxs-lookup"><span data-stu-id="f56df-130">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f56df-131">Пример</span><span class="sxs-lookup"><span data-stu-id="f56df-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="f56df-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="f56df-132">Request</span></span>
<span data-ttu-id="f56df-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f56df-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f56df-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="f56df-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_owner_from_group"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groups/{id}/owners/{id}/$ref
```
# <a name="c"></a>[<span data-ttu-id="f56df-135">C#</span><span class="sxs-lookup"><span data-stu-id="f56df-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-owner-from-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f56df-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f56df-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-owner-from-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f56df-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f56df-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-owner-from-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f56df-138">Java</span><span class="sxs-lookup"><span data-stu-id="f56df-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-owner-from-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="f56df-139">Укажите в запросе свойство `id` удаляемого объекта каталога после сегмента $ref.</span><span class="sxs-lookup"><span data-stu-id="f56df-139">In the request, specify the `id` of the directory object you want to remove after the $ref segment.</span></span>

#### <a name="response"></a><span data-ttu-id="f56df-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="f56df-140">Response</span></span>
<span data-ttu-id="f56df-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="f56df-141">The following is an example of the response.</span></span>
><span data-ttu-id="f56df-142">**Примечание.**  Объект ответа, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="f56df-142">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="f56df-143">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f56df-143">All the properties will be returned from an actual call.</span></span>
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

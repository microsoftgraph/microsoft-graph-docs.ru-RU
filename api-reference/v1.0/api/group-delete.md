---
title: Delete Group — API Microsoft Graph
description: Описывает метод Delete ресурса Group (Entity) API Microsoft Graph (REST).
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 916b3db0e3e4df24f1e0dc53bd1f17a10b8365c2
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42517168"
---
# <a name="delete-group"></a><span data-ttu-id="45c0f-103">Delete group</span><span class="sxs-lookup"><span data-stu-id="45c0f-103">Delete group</span></span>

<span data-ttu-id="45c0f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="45c0f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="45c0f-105">Удаление группы.</span><span class="sxs-lookup"><span data-stu-id="45c0f-105">Delete group.</span></span>  

<span data-ttu-id="45c0f-106">После удаления группы Office 365 перемещаются во временный контейнер и могут быть восстановлены в течение 30 дней.</span><span class="sxs-lookup"><span data-stu-id="45c0f-106">When deleted, Office 365 groups are moved to a temporary container and can be restored within 30 days.</span></span>  <span data-ttu-id="45c0f-107">По истечении этого периода они удаляются без возможности восстановления.</span><span class="sxs-lookup"><span data-stu-id="45c0f-107">After that time, they are permanently deleted.</span></span>  <span data-ttu-id="45c0f-108">Дополнительные сведения см. в статье [deletedItems](../resources/directory.md).</span><span class="sxs-lookup"><span data-stu-id="45c0f-108">To learn more, see [deletedItems](../resources/directory.md).</span></span>  <span data-ttu-id="45c0f-109">Это применимо только к группам Office 365.</span><span class="sxs-lookup"><span data-stu-id="45c0f-109">This applies only to Office 365 groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="45c0f-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="45c0f-110">Permissions</span></span>

<span data-ttu-id="45c0f-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="45c0f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="45c0f-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="45c0f-113">Permission type</span></span>      | <span data-ttu-id="45c0f-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="45c0f-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="45c0f-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="45c0f-115">Delegated (work or school account)</span></span> | <span data-ttu-id="45c0f-116">Group.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="45c0f-116">Group.ReadWrite.All, Directory.AccessAsUser.All</span></span>   |
|<span data-ttu-id="45c0f-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="45c0f-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="45c0f-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="45c0f-118">Not supported.</span></span>    |
|<span data-ttu-id="45c0f-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="45c0f-119">Application</span></span> | <span data-ttu-id="45c0f-120">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="45c0f-120">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="45c0f-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="45c0f-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}
```

## <a name="request-headers"></a><span data-ttu-id="45c0f-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="45c0f-122">Request headers</span></span>

| <span data-ttu-id="45c0f-123">Имя</span><span class="sxs-lookup"><span data-stu-id="45c0f-123">Name</span></span>       | <span data-ttu-id="45c0f-124">Тип</span><span class="sxs-lookup"><span data-stu-id="45c0f-124">Type</span></span> | <span data-ttu-id="45c0f-125">Описание</span><span class="sxs-lookup"><span data-stu-id="45c0f-125">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="45c0f-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="45c0f-126">Authorization</span></span>  | <span data-ttu-id="45c0f-127">string</span><span class="sxs-lookup"><span data-stu-id="45c0f-127">string</span></span>  | <span data-ttu-id="45c0f-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="45c0f-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="45c0f-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="45c0f-130">Request body</span></span>

<span data-ttu-id="45c0f-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="45c0f-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="45c0f-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="45c0f-132">Response</span></span>

<span data-ttu-id="45c0f-p104">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="45c0f-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="45c0f-135">Пример</span><span class="sxs-lookup"><span data-stu-id="45c0f-135">Example</span></span>

### <a name="request"></a><span data-ttu-id="45c0f-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="45c0f-136">Request</span></span>

<span data-ttu-id="45c0f-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="45c0f-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="45c0f-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="45c0f-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_group"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groups/{id}
```
# <a name="c"></a>[<span data-ttu-id="45c0f-139">C#</span><span class="sxs-lookup"><span data-stu-id="45c0f-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="45c0f-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="45c0f-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="45c0f-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="45c0f-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="45c0f-142">Java</span><span class="sxs-lookup"><span data-stu-id="45c0f-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="45c0f-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="45c0f-143">Response</span></span>

<span data-ttu-id="45c0f-144">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="45c0f-144">The following is an example of the response.</span></span> 
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
  "description": "Delete group",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

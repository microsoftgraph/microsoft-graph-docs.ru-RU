---
title: Delete Group — API Microsoft Graph
description: Описывает метод Delete ресурса Group (Entity) API Microsoft Graph (REST).
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 95638630fd95220760cce6766edbef5dc84cb544
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36014972"
---
# <a name="delete-group"></a><span data-ttu-id="c0c2e-103">Удаление группы</span><span class="sxs-lookup"><span data-stu-id="c0c2e-103">Delete group</span></span>

<span data-ttu-id="c0c2e-104">Удаление группы.</span><span class="sxs-lookup"><span data-stu-id="c0c2e-104">Delete group.</span></span>  

<span data-ttu-id="c0c2e-105">После удаления группы Office 365 перемещаются во временный контейнер и могут быть восстановлены в течение 30 дней.</span><span class="sxs-lookup"><span data-stu-id="c0c2e-105">When deleted, Office 365 groups are moved to a temporary container and can be restored within 30 days.</span></span>  <span data-ttu-id="c0c2e-106">По истечении этого периода они удаляются без возможности восстановления.</span><span class="sxs-lookup"><span data-stu-id="c0c2e-106">After that time, they are permanently deleted.</span></span>  <span data-ttu-id="c0c2e-107">Дополнительные сведения см. в статье [deletedItems](../resources/directory.md).</span><span class="sxs-lookup"><span data-stu-id="c0c2e-107">To learn more, see [deletedItems](../resources/directory.md).</span></span>  <span data-ttu-id="c0c2e-108">Это применимо только к группам Office 365.</span><span class="sxs-lookup"><span data-stu-id="c0c2e-108">This applies only to Office 365 groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="c0c2e-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c0c2e-109">Permissions</span></span>

<span data-ttu-id="c0c2e-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c0c2e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c0c2e-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c0c2e-112">Permission type</span></span>      | <span data-ttu-id="c0c2e-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c0c2e-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c0c2e-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c0c2e-114">Delegated (work or school account)</span></span> | <span data-ttu-id="c0c2e-115">Group.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c0c2e-115">Group.ReadWrite.All, Directory.AccessAsUser.All</span></span>   |
|<span data-ttu-id="c0c2e-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c0c2e-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c0c2e-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c0c2e-117">Not supported.</span></span>    |
|<span data-ttu-id="c0c2e-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c0c2e-118">Application</span></span> | <span data-ttu-id="c0c2e-119">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c0c2e-119">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c0c2e-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c0c2e-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}
```

## <a name="request-headers"></a><span data-ttu-id="c0c2e-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c0c2e-121">Request headers</span></span>

| <span data-ttu-id="c0c2e-122">Имя</span><span class="sxs-lookup"><span data-stu-id="c0c2e-122">Name</span></span>       | <span data-ttu-id="c0c2e-123">Тип</span><span class="sxs-lookup"><span data-stu-id="c0c2e-123">Type</span></span> | <span data-ttu-id="c0c2e-124">Описание</span><span class="sxs-lookup"><span data-stu-id="c0c2e-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="c0c2e-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="c0c2e-125">Authorization</span></span>  | <span data-ttu-id="c0c2e-126">string</span><span class="sxs-lookup"><span data-stu-id="c0c2e-126">string</span></span>  | <span data-ttu-id="c0c2e-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c0c2e-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c0c2e-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c0c2e-129">Request body</span></span>

<span data-ttu-id="c0c2e-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c0c2e-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c0c2e-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="c0c2e-131">Response</span></span>

<span data-ttu-id="c0c2e-p104">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="c0c2e-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c0c2e-134">Пример</span><span class="sxs-lookup"><span data-stu-id="c0c2e-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="c0c2e-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="c0c2e-135">Request</span></span>

<span data-ttu-id="c0c2e-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c0c2e-136">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="c0c2e-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="c0c2e-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_group"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groups/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c0c2e-138">C#</span><span class="sxs-lookup"><span data-stu-id="c0c2e-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c0c2e-139">Javascript</span><span class="sxs-lookup"><span data-stu-id="c0c2e-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c0c2e-140">Цель — C</span><span class="sxs-lookup"><span data-stu-id="c0c2e-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="c0c2e-141">Java</span><span class="sxs-lookup"><span data-stu-id="c0c2e-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="c0c2e-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="c0c2e-142">Response</span></span>

<span data-ttu-id="c0c2e-143">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="c0c2e-143">The following is an example of the response.</span></span> 
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

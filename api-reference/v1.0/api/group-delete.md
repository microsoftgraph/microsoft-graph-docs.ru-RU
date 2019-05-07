---
title: Delete Group — API Microsoft Graph
description: Описывает метод Delete ресурса Group (Entity) API Microsoft Graph (REST).
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 86e32d83bd30a66405a61c767c46f34f0dd3614c
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33614671"
---
# <a name="delete-group"></a><span data-ttu-id="60e1f-103">Удаление группы</span><span class="sxs-lookup"><span data-stu-id="60e1f-103">Delete group</span></span>

<span data-ttu-id="60e1f-104">Удаление группы.</span><span class="sxs-lookup"><span data-stu-id="60e1f-104">Delete group.</span></span>  

<span data-ttu-id="60e1f-105">После удаления группы Office 365 перемещаются во временный контейнер и могут быть восстановлены в течение 30 дней.</span><span class="sxs-lookup"><span data-stu-id="60e1f-105">When deleted, Office 365 groups are moved to a temporary container and can be restored within 30 days.</span></span>  <span data-ttu-id="60e1f-106">По истечении этого периода они удаляются без возможности восстановления.</span><span class="sxs-lookup"><span data-stu-id="60e1f-106">After that time, they are permanently deleted.</span></span>  <span data-ttu-id="60e1f-107">Дополнительные сведения см. в статье [deletedItems](../resources/directory.md).</span><span class="sxs-lookup"><span data-stu-id="60e1f-107">To learn more, see [deletedItems](../resources/directory.md).</span></span>  <span data-ttu-id="60e1f-108">Это применимо только к группам Office 365.</span><span class="sxs-lookup"><span data-stu-id="60e1f-108">This applies only to Office 365 groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="60e1f-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="60e1f-109">Permissions</span></span>

<span data-ttu-id="60e1f-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="60e1f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="60e1f-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="60e1f-112">Permission type</span></span>      | <span data-ttu-id="60e1f-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="60e1f-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="60e1f-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="60e1f-114">Delegated (work or school account)</span></span> | <span data-ttu-id="60e1f-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="60e1f-115">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="60e1f-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="60e1f-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="60e1f-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="60e1f-117">Not supported.</span></span>    |
|<span data-ttu-id="60e1f-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="60e1f-118">Application</span></span> | <span data-ttu-id="60e1f-119">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="60e1f-119">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="60e1f-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="60e1f-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}
```

## <a name="request-headers"></a><span data-ttu-id="60e1f-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="60e1f-121">Request headers</span></span>

| <span data-ttu-id="60e1f-122">Имя</span><span class="sxs-lookup"><span data-stu-id="60e1f-122">Name</span></span>       | <span data-ttu-id="60e1f-123">Тип</span><span class="sxs-lookup"><span data-stu-id="60e1f-123">Type</span></span> | <span data-ttu-id="60e1f-124">Описание</span><span class="sxs-lookup"><span data-stu-id="60e1f-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="60e1f-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="60e1f-125">Authorization</span></span>  | <span data-ttu-id="60e1f-126">string</span><span class="sxs-lookup"><span data-stu-id="60e1f-126">string</span></span>  | <span data-ttu-id="60e1f-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="60e1f-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="60e1f-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="60e1f-129">Request body</span></span>

<span data-ttu-id="60e1f-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="60e1f-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="60e1f-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="60e1f-131">Response</span></span>

<span data-ttu-id="60e1f-p104">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="60e1f-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="60e1f-134">Пример</span><span class="sxs-lookup"><span data-stu-id="60e1f-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="60e1f-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="60e1f-135">Request</span></span>

<span data-ttu-id="60e1f-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="60e1f-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_group"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groups/{id}
```

### <a name="response"></a><span data-ttu-id="60e1f-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="60e1f-137">Response</span></span>

<span data-ttu-id="60e1f-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="60e1f-138">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="60e1f-139">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="60e1f-139">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="60e1f-140">Языках</span><span class="sxs-lookup"><span data-stu-id="60e1f-140">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_group-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="60e1f-141">Язык</span><span class="sxs-lookup"><span data-stu-id="60e1f-141">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_group-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete group",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/group-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/group-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->

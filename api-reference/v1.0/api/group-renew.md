---
title: 'group: renew'
description: Обновление, продлевающее срок действия группы. Когда группа обновляется, срок ее действия продляется на количество дней, определенное политикой.
localization_priority: Normal
author: Jordanndahl
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 05fde82e6ae9bc3e3d7662e140605391ab08abdb
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/06/2021
ms.locfileid: "52787767"
---
# <a name="group-renew"></a><span data-ttu-id="0f4e2-104">group: renew</span><span class="sxs-lookup"><span data-stu-id="0f4e2-104">group: renew</span></span>

<span data-ttu-id="0f4e2-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0f4e2-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0f4e2-p102">Обновление, продлевающее срок действия группы. Когда группа обновляется, срок ее действия продляется на количество дней, определенное политикой.</span><span class="sxs-lookup"><span data-stu-id="0f4e2-p102">Renews a group's expiration. When a group is renewed, the group expiration is extended by the number of days defined in the policy.</span></span>

## <a name="permissions"></a><span data-ttu-id="0f4e2-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0f4e2-108">Permissions</span></span>

<span data-ttu-id="0f4e2-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0f4e2-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>
 

|<span data-ttu-id="0f4e2-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0f4e2-111">Permission type</span></span>      | <span data-ttu-id="0f4e2-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0f4e2-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0f4e2-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0f4e2-113">Delegated (work or school account)</span></span> | <span data-ttu-id="0f4e2-114">Group.ReadWrite.All или Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0f4e2-114">Group.ReadWrite.All or Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="0f4e2-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0f4e2-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0f4e2-116">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="0f4e2-116">Not supported</span></span> |
|<span data-ttu-id="0f4e2-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0f4e2-117">Application</span></span> | <span data-ttu-id="0f4e2-118">Group.ReadWrite.All или Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0f4e2-118">Group.ReadWrite.All or Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0f4e2-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0f4e2-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/renew
```

## <a name="request-headers"></a><span data-ttu-id="0f4e2-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0f4e2-120">Request headers</span></span>
| <span data-ttu-id="0f4e2-121">Имя</span><span class="sxs-lookup"><span data-stu-id="0f4e2-121">Name</span></span>       | <span data-ttu-id="0f4e2-122">Описание</span><span class="sxs-lookup"><span data-stu-id="0f4e2-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="0f4e2-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0f4e2-123">Authorization</span></span>  | <span data-ttu-id="0f4e2-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0f4e2-p104">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="0f4e2-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="0f4e2-126">Request body</span></span>

<span data-ttu-id="0f4e2-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0f4e2-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0f4e2-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="0f4e2-128">Response</span></span>

<span data-ttu-id="0f4e2-p105">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="0f4e2-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0f4e2-131">Пример</span><span class="sxs-lookup"><span data-stu-id="0f4e2-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="0f4e2-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="0f4e2-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="0f4e2-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="0f4e2-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_renew"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/renew
```
# <a name="c"></a>[<span data-ttu-id="0f4e2-134">C#</span><span class="sxs-lookup"><span data-stu-id="0f4e2-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-renew-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0f4e2-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0f4e2-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-renew-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0f4e2-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0f4e2-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-renew-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0f4e2-137">Java</span><span class="sxs-lookup"><span data-stu-id="0f4e2-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-renew-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="0f4e2-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="0f4e2-138">Response</span></span>
<span data-ttu-id="0f4e2-139">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="0f4e2-139">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "group: renew",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->


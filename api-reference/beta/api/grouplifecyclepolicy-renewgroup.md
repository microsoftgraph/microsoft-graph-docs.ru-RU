---
title: 'groupLifecyclePolicy: Реневграуп'
description: Обновляет срок действия группы. Когда группа обновляется, срок ее действия продляется на количество дней, определенное политикой.
localization_priority: Normal
author: dkershaw10
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 57179bdc1d542e58cbf5ffa8411dcf3b1eed4ce4
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36322998"
---
# <a name="grouplifecyclepolicy-renewgroup"></a><span data-ttu-id="51ad8-104">groupLifecyclePolicy: Реневграуп</span><span class="sxs-lookup"><span data-stu-id="51ad8-104">groupLifecyclePolicy: renewGroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="51ad8-105">Обновляет срок действия группы.</span><span class="sxs-lookup"><span data-stu-id="51ad8-105">Renews a group's expiration.</span></span> <span data-ttu-id="51ad8-106">Когда группа обновляется, срок ее действия продляется на количество дней, определенное политикой.</span><span class="sxs-lookup"><span data-stu-id="51ad8-106">When a group is renewed, the group expiration is extended by the number of days defined in the policy.</span></span>

> <span data-ttu-id="51ad8-107">**Примечание:** В версии 1.0 [Используйте ресурс Group, чтобы выполнить обновление запросов](/graph/api/group-renew?view=graph-rest-1.0).</span><span class="sxs-lookup"><span data-stu-id="51ad8-107">**Note:** In V1.0, [use the group resource to make renew requests](/graph/api/group-renew?view=graph-rest-1.0).</span></span>

## <a name="permissions"></a><span data-ttu-id="51ad8-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="51ad8-108">Permissions</span></span>

<span data-ttu-id="51ad8-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="51ad8-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>
 

|<span data-ttu-id="51ad8-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="51ad8-111">Permission type</span></span>      | <span data-ttu-id="51ad8-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="51ad8-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="51ad8-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="51ad8-113">Delegated (work or school account)</span></span> | <span data-ttu-id="51ad8-114">Group.ReadWrite.All или Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="51ad8-114">Group.ReadWrite.All or Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="51ad8-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="51ad8-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="51ad8-116">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="51ad8-116">Not supported</span></span> |
|<span data-ttu-id="51ad8-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="51ad8-117">Application</span></span> | <span data-ttu-id="51ad8-118">Group.ReadWrite.All или Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="51ad8-118">Group.ReadWrite.All or Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="51ad8-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="51ad8-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groupLifecyclePolicies/renewGroup

```

## <a name="request-headers"></a><span data-ttu-id="51ad8-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="51ad8-120">Request headers</span></span>

| <span data-ttu-id="51ad8-121">Имя</span><span class="sxs-lookup"><span data-stu-id="51ad8-121">Name</span></span> | <span data-ttu-id="51ad8-122">Описание</span><span class="sxs-lookup"><span data-stu-id="51ad8-122">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="51ad8-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="51ad8-123">Authorization</span></span> | <span data-ttu-id="51ad8-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="51ad8-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="51ad8-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="51ad8-126">Content-Type</span></span>  | <span data-ttu-id="51ad8-127">application/json</span><span class="sxs-lookup"><span data-stu-id="51ad8-127">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="51ad8-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="51ad8-128">Request body</span></span>
<span data-ttu-id="51ad8-129">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="51ad8-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="51ad8-130">Параметр</span><span class="sxs-lookup"><span data-stu-id="51ad8-130">Parameter</span></span> | <span data-ttu-id="51ad8-131">Тип</span><span class="sxs-lookup"><span data-stu-id="51ad8-131">Type</span></span> | <span data-ttu-id="51ad8-132">Описание</span><span class="sxs-lookup"><span data-stu-id="51ad8-132">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="51ad8-133">groupId</span><span class="sxs-lookup"><span data-stu-id="51ad8-133">groupId</span></span>|<span data-ttu-id="51ad8-134">GUID</span><span class="sxs-lookup"><span data-stu-id="51ad8-134">Guid</span></span>| <span data-ttu-id="51ad8-135">Идентификатор группы, которую требуется обновить.</span><span class="sxs-lookup"><span data-stu-id="51ad8-135">The id of the group to renew.</span></span> |

## <a name="response"></a><span data-ttu-id="51ad8-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="51ad8-136">Response</span></span>

<span data-ttu-id="51ad8-p105">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="51ad8-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="51ad8-139">Пример</span><span class="sxs-lookup"><span data-stu-id="51ad8-139">Example</span></span>

##### <a name="request"></a><span data-ttu-id="51ad8-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="51ad8-140">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="51ad8-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="51ad8-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "grouplifecyclepolicy_renewgroup"
}-->
```http
POST https://graph.microsoft.com/beta/groupLifecyclePolicies/renewGroup
Content-type: application/json
Content-length: 57

{
  "groupId": "ffffffff-ffff-ffff-ffff-ffffffffffff"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="51ad8-142">C#</span><span class="sxs-lookup"><span data-stu-id="51ad8-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/grouplifecyclepolicy-renewgroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="51ad8-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="51ad8-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/grouplifecyclepolicy-renewgroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="51ad8-144">Цель — C</span><span class="sxs-lookup"><span data-stu-id="51ad8-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/grouplifecyclepolicy-renewgroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="51ad8-145">Java</span><span class="sxs-lookup"><span data-stu-id="51ad8-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/grouplifecyclepolicy-renewgroup-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="51ad8-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="51ad8-146">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "groupLifecyclePolicy: renewgroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

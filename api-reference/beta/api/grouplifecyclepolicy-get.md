---
title: Получение groupLifecyclePolicy
description: Получение свойств и связей, принадлежащих объекту groupLifecyclePolicies.
author: Jordanndahl
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: cb3698fef265028afefea0ee4011f96628c6acc3
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/27/2021
ms.locfileid: "52681146"
---
# <a name="get-grouplifecyclepolicy"></a><span data-ttu-id="95db5-103">Получение groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="95db5-103">Get groupLifecyclePolicy</span></span>

<span data-ttu-id="95db5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="95db5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="95db5-105">Получение свойств и связей, принадлежащих объекту [groupLifecyclePolicies](../resources/grouplifecyclepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="95db5-105">Retrieve the properties and relationships of a [groupLifecyclePolicies](../resources/grouplifecyclepolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="95db5-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="95db5-106">Permissions</span></span>

<span data-ttu-id="95db5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="95db5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="95db5-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="95db5-109">Permission type</span></span>      | <span data-ttu-id="95db5-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="95db5-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="95db5-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="95db5-111">Delegated (work or school account)</span></span> | <span data-ttu-id="95db5-112">Directory.Read.All или Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="95db5-112">Directory.Read.All or Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="95db5-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="95db5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="95db5-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="95db5-114">Not supported</span></span> |
|<span data-ttu-id="95db5-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="95db5-115">Application</span></span> | <span data-ttu-id="95db5-116">Directory.Read.All или Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="95db5-116">Directory.Read.All or Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="95db5-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="95db5-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groupLifecyclePolicies/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="95db5-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="95db5-118">Optional query parameters</span></span>
<span data-ttu-id="95db5-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="95db5-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="95db5-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="95db5-120">Request headers</span></span>
| <span data-ttu-id="95db5-121">Имя</span><span class="sxs-lookup"><span data-stu-id="95db5-121">Name</span></span> | <span data-ttu-id="95db5-122">Описание</span><span class="sxs-lookup"><span data-stu-id="95db5-122">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="95db5-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="95db5-123">Authorization</span></span> | <span data-ttu-id="95db5-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="95db5-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="95db5-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="95db5-126">Request body</span></span>
<span data-ttu-id="95db5-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="95db5-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="95db5-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="95db5-128">Response</span></span>
<span data-ttu-id="95db5-129">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="95db5-129">If successful, this method returns a `200 OK` response code and [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="95db5-130">Пример</span><span class="sxs-lookup"><span data-stu-id="95db5-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="95db5-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="95db5-131">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="95db5-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="95db5-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_grouplifecyclepolicy_1"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groupLifecyclePolicies/{id}
```
# <a name="c"></a>[<span data-ttu-id="95db5-133">C#</span><span class="sxs-lookup"><span data-stu-id="95db5-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-grouplifecyclepolicy-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="95db5-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="95db5-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-grouplifecyclepolicy-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="95db5-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="95db5-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-grouplifecyclepolicy-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="95db5-136">Java</span><span class="sxs-lookup"><span data-stu-id="95db5-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-grouplifecyclepolicy-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="95db5-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="95db5-137">Response</span></span>

<span data-ttu-id="95db5-138">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="95db5-138">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.groupLifecyclePolicy"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 174

{
  "id": "ffffffff-ffff-ffff-ffff-ffffffffffff",
  "groupLifetimeInDays": 100,
  "managedGroupTypes": "Selected",
  "alternateNotificationEmails": "admin@contoso.com"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get groupLifecyclePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

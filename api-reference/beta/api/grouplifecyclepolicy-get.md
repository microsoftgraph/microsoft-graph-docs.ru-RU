---
title: Получение groupLifecyclePolicy
description: Получение свойств и связей, принадлежащих объекту groupLifecyclePolicies.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 66d7084000ca659c6938189b136c6777e762f1e0
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/15/2019
ms.locfileid: "36420002"
---
# <a name="get-grouplifecyclepolicy"></a><span data-ttu-id="356fb-103">Получение groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="356fb-103">Get groupLifecyclePolicy</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="356fb-104">Получение свойств и связей, принадлежащих объекту [groupLifecyclePolicies](../resources/grouplifecyclepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="356fb-104">Retrieve the properties and relationships of a [groupLifecyclePolicies](../resources/grouplifecyclepolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="356fb-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="356fb-105">Permissions</span></span>

<span data-ttu-id="356fb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="356fb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="356fb-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="356fb-108">Permission type</span></span>      | <span data-ttu-id="356fb-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="356fb-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="356fb-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="356fb-110">Delegated (work or school account)</span></span> | <span data-ttu-id="356fb-111">Directory.Read.All или Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="356fb-111">Directory.Read.All or Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="356fb-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="356fb-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="356fb-113">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="356fb-113">Not supported</span></span> |
|<span data-ttu-id="356fb-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="356fb-114">Application</span></span> | <span data-ttu-id="356fb-115">Directory.Read.All или Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="356fb-115">Directory.Read.All or Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="356fb-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="356fb-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groupLifecyclePolicies/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="356fb-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="356fb-117">Optional query parameters</span></span>
<span data-ttu-id="356fb-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="356fb-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="356fb-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="356fb-119">Request headers</span></span>
| <span data-ttu-id="356fb-120">Имя</span><span class="sxs-lookup"><span data-stu-id="356fb-120">Name</span></span> | <span data-ttu-id="356fb-121">Описание</span><span class="sxs-lookup"><span data-stu-id="356fb-121">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="356fb-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="356fb-122">Authorization</span></span> | <span data-ttu-id="356fb-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="356fb-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="356fb-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="356fb-125">Request body</span></span>
<span data-ttu-id="356fb-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="356fb-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="356fb-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="356fb-127">Response</span></span>
<span data-ttu-id="356fb-128">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="356fb-128">If successful, this method returns a `200 OK` response code and [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="356fb-129">Пример</span><span class="sxs-lookup"><span data-stu-id="356fb-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="356fb-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="356fb-130">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="356fb-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="356fb-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_grouplifecyclepolicy"
}-->
```http
GET https://graph.microsoft.com/beta/groupLifecyclePolicies/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="356fb-132">C#</span><span class="sxs-lookup"><span data-stu-id="356fb-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-grouplifecyclepolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="356fb-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="356fb-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-grouplifecyclepolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="356fb-134">Цель — C</span><span class="sxs-lookup"><span data-stu-id="356fb-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-grouplifecyclepolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="356fb-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="356fb-135">Response</span></span>

<span data-ttu-id="356fb-p103">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="356fb-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

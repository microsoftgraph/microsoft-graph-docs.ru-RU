---
title: Получение groupLifecyclePolicy
description: Получение свойств и связей, принадлежащих объекту groupLifecyclePolicies.
author: yyuank
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 43d4f6b11df2ca40af24b808b584802489963089
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/14/2020
ms.locfileid: "48459664"
---
# <a name="get-grouplifecyclepolicy"></a><span data-ttu-id="b9835-103">Получение groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="b9835-103">Get groupLifecyclePolicy</span></span>

<span data-ttu-id="b9835-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b9835-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b9835-105">Получение свойств и связей, принадлежащих объекту [groupLifecyclePolicies](../resources/grouplifecyclepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="b9835-105">Retrieve the properties and relationships of a [groupLifecyclePolicies](../resources/grouplifecyclepolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="b9835-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b9835-106">Permissions</span></span>

<span data-ttu-id="b9835-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b9835-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="b9835-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b9835-109">Permission type</span></span>      | <span data-ttu-id="b9835-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b9835-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b9835-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b9835-111">Delegated (work or school account)</span></span> | <span data-ttu-id="b9835-112">Directory.Read.All или Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b9835-112">Directory.Read.All or Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="b9835-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b9835-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b9835-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="b9835-114">Not supported</span></span> |
|<span data-ttu-id="b9835-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b9835-115">Application</span></span> | <span data-ttu-id="b9835-116">Directory.Read.All или Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b9835-116">Directory.Read.All or Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b9835-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b9835-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groupLifecyclePolicies/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="b9835-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="b9835-118">Optional query parameters</span></span>
<span data-ttu-id="b9835-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="b9835-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b9835-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b9835-120">Request headers</span></span>
| <span data-ttu-id="b9835-121">Имя</span><span class="sxs-lookup"><span data-stu-id="b9835-121">Name</span></span> | <span data-ttu-id="b9835-122">Описание</span><span class="sxs-lookup"><span data-stu-id="b9835-122">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="b9835-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b9835-123">Authorization</span></span> | <span data-ttu-id="b9835-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b9835-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b9835-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b9835-126">Request body</span></span>
<span data-ttu-id="b9835-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b9835-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="b9835-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="b9835-128">Response</span></span>
<span data-ttu-id="b9835-129">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="b9835-129">If successful, this method returns a `200 OK` response code and [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b9835-130">Пример</span><span class="sxs-lookup"><span data-stu-id="b9835-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="b9835-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="b9835-131">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="b9835-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="b9835-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_grouplifecyclepolicy"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groupLifecyclePolicies/{id}
```
# <a name="c"></a>[<span data-ttu-id="b9835-133">C#</span><span class="sxs-lookup"><span data-stu-id="b9835-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-grouplifecyclepolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b9835-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b9835-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-grouplifecyclepolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b9835-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b9835-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-grouplifecyclepolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="b9835-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="b9835-136">Response</span></span>

<span data-ttu-id="b9835-p103">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b9835-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

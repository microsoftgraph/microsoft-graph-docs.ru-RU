---
title: Перечисление groupLifecyclePolicies
description: Перечисление всех объектов groupLifecyclePolicy.
author: yyuank
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 08555aeb58212279966752da6b61867efefbe359
ms.sourcegitcommit: bd40e302ce04b686e86989246ab7c4cc9ad3f320
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/03/2020
ms.locfileid: "43124639"
---
# <a name="list-grouplifecyclepolicies"></a><span data-ttu-id="b5f34-103">Перечисление groupLifecyclePolicies</span><span class="sxs-lookup"><span data-stu-id="b5f34-103">List groupLifecyclePolicies</span></span>

<span data-ttu-id="b5f34-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b5f34-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b5f34-105">Список всех объектов [groupLifecyclePolicies](../resources/grouplifecyclepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="b5f34-105">List all the [groupLifecyclePolicies](../resources/grouplifecyclepolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="b5f34-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b5f34-106">Permissions</span></span>

<span data-ttu-id="b5f34-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b5f34-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="b5f34-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b5f34-109">Permission type</span></span>      | <span data-ttu-id="b5f34-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b5f34-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b5f34-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b5f34-111">Delegated (work or school account)</span></span> | <span data-ttu-id="b5f34-112">Directory.Read.All или Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b5f34-112">Directory.Read.All or Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="b5f34-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b5f34-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b5f34-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b5f34-114">Not supported.</span></span>    |
|<span data-ttu-id="b5f34-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b5f34-115">Application</span></span> | <span data-ttu-id="b5f34-116">Directory.Read.All или Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b5f34-116">Directory.Read.All or Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b5f34-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b5f34-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groupLifecyclePolicies
```
## <a name="optional-query-parameters"></a><span data-ttu-id="b5f34-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="b5f34-118">Optional query parameters</span></span>
<span data-ttu-id="b5f34-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="b5f34-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b5f34-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b5f34-120">Request headers</span></span>
| <span data-ttu-id="b5f34-121">Имя</span><span class="sxs-lookup"><span data-stu-id="b5f34-121">Name</span></span> | <span data-ttu-id="b5f34-122">Описание</span><span class="sxs-lookup"><span data-stu-id="b5f34-122">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="b5f34-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b5f34-123">Authorization</span></span> | <span data-ttu-id="b5f34-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b5f34-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b5f34-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b5f34-126">Request body</span></span>
<span data-ttu-id="b5f34-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b5f34-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b5f34-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="b5f34-128">Response</span></span>

<span data-ttu-id="b5f34-129">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="b5f34-129">If successful, this method returns a `200 OK` response code and a collection of [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b5f34-130">Пример</span><span class="sxs-lookup"><span data-stu-id="b5f34-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="b5f34-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="b5f34-131">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="b5f34-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="b5f34-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_grouplifecyclepolicy"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groupLifecyclePolicies
```
# <a name="c"></a>[<span data-ttu-id="b5f34-133">C#</span><span class="sxs-lookup"><span data-stu-id="b5f34-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-grouplifecyclepolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b5f34-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b5f34-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-grouplifecyclepolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b5f34-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b5f34-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-grouplifecyclepolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b5f34-136">Java</span><span class="sxs-lookup"><span data-stu-id="b5f34-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-grouplifecyclepolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="b5f34-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="b5f34-137">Response</span></span>

<span data-ttu-id="b5f34-p103">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b5f34-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.groupLifecyclePolicy",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 223

{
  "value": [
    {
      "id": "ffffffff-ffff-ffff-ffff-ffffffffffff",
      "groupLifetimeInDays": 100,
      "managedGroupTypes": "Selected",
      "alternateNotificationEmails": "admin@contoso.com"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List groupLifecyclePolicies",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

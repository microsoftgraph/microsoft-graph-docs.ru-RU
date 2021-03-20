---
title: Перечисление groupLifecyclePolicies
description: Перечисление всех объектов groupLifecyclePolicy.
author: yyuank
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: ed1f2098dc67ca65a81671b49073d2fcc0764ff9
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50949905"
---
# <a name="list-grouplifecyclepolicies"></a><span data-ttu-id="58e23-103">Перечисление groupLifecyclePolicies</span><span class="sxs-lookup"><span data-stu-id="58e23-103">List groupLifecyclePolicies</span></span>

<span data-ttu-id="58e23-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="58e23-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="58e23-105">Список всех объектов [groupLifecyclePolicies](../resources/grouplifecyclepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="58e23-105">List all the [groupLifecyclePolicies](../resources/grouplifecyclepolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="58e23-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="58e23-106">Permissions</span></span>

<span data-ttu-id="58e23-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="58e23-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="58e23-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="58e23-109">Permission type</span></span>      | <span data-ttu-id="58e23-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="58e23-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="58e23-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="58e23-111">Delegated (work or school account)</span></span> | <span data-ttu-id="58e23-112">Directory.Read.All или Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="58e23-112">Directory.Read.All or Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="58e23-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="58e23-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="58e23-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="58e23-114">Not supported.</span></span>    |
|<span data-ttu-id="58e23-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="58e23-115">Application</span></span> | <span data-ttu-id="58e23-116">Directory.Read.All или Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="58e23-116">Directory.Read.All or Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="58e23-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="58e23-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groupLifecyclePolicies
```
## <a name="optional-query-parameters"></a><span data-ttu-id="58e23-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="58e23-118">Optional query parameters</span></span>
<span data-ttu-id="58e23-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="58e23-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="58e23-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="58e23-120">Request headers</span></span>
| <span data-ttu-id="58e23-121">Имя</span><span class="sxs-lookup"><span data-stu-id="58e23-121">Name</span></span> | <span data-ttu-id="58e23-122">Описание</span><span class="sxs-lookup"><span data-stu-id="58e23-122">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="58e23-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="58e23-123">Authorization</span></span> | <span data-ttu-id="58e23-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="58e23-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="58e23-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="58e23-126">Request body</span></span>
<span data-ttu-id="58e23-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="58e23-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="58e23-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="58e23-128">Response</span></span>

<span data-ttu-id="58e23-129">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="58e23-129">If successful, this method returns a `200 OK` response code and a collection of [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="58e23-130">Пример</span><span class="sxs-lookup"><span data-stu-id="58e23-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="58e23-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="58e23-131">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="58e23-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="58e23-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_grouplifecyclepolicy_2"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groupLifecyclePolicies
```
# <a name="c"></a>[<span data-ttu-id="58e23-133">C#</span><span class="sxs-lookup"><span data-stu-id="58e23-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-grouplifecyclepolicy-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="58e23-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="58e23-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-grouplifecyclepolicy-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="58e23-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="58e23-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-grouplifecyclepolicy-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="58e23-136">Java</span><span class="sxs-lookup"><span data-stu-id="58e23-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-grouplifecyclepolicy-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="58e23-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="58e23-137">Response</span></span>

<span data-ttu-id="58e23-p103">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="58e23-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
